# Comparing `tmp/cloud-api-signer-0.1.0.tar.gz` & `tmp/cloud-api-signer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-api-signer-0.1.0.tar", max compression
+gzip compressed data, was "cloud-api-signer-0.2.0.tar", max compression
```

## Comparing `cloud-api-signer-0.1.0.tar` & `cloud-api-signer-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-07-07 06:24:40.964525 cloud-api-signer-0.1.0/LICENSE
--rw-r--r--   0        0        0       24 2023-07-12 11:21:37.224643 cloud-api-signer-0.1.0/cloud_api_signer/__init__.py
--rw-r--r--   0        0        0     3360 2023-07-12 08:27:54.175728 cloud-api-signer-0.1.0/cloud_api_signer/bce.py
--rw-r--r--   0        0        0      365 2023-07-12 08:11:52.756879 cloud-api-signer-0.1.0/cloud_api_signer/models.py
--rw-r--r--   0        0        0      633 2023-07-12 07:20:17.304093 cloud-api-signer-0.1.0/cloud_api_signer/utils.py
--rw-r--r--   0        0        0     4588 2023-07-12 08:28:32.719797 cloud-api-signer-0.1.0/cloud_api_signer/volc.py
--rw-r--r--   0        0        0     2254 2023-07-12 11:21:49.062023 cloud-api-signer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      608 2023-07-13 03:22:18.742000 cloud-api-signer-0.1.0/setup.py
--rw-r--r--   0        0        0      448 2023-07-13 03:22:18.742203 cloud-api-signer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-07 06:24:40.964525 cloud-api-signer-0.2.0/LICENSE
+-rw-r--r--   0        0        0       24 2023-07-12 11:21:37.224643 cloud-api-signer-0.2.0/cloud_api_signer/__init__.py
+-rw-r--r--   0        0        0     3653 2023-07-13 09:01:49.781679 cloud-api-signer-0.2.0/cloud_api_signer/bce.py
+-rw-r--r--   0        0        0      365 2023-07-12 08:11:52.756879 cloud-api-signer-0.2.0/cloud_api_signer/models.py
+-rw-r--r--   0        0        0      633 2023-07-12 07:20:17.304093 cloud-api-signer-0.2.0/cloud_api_signer/utils.py
+-rw-r--r--   0        0        0     4653 2023-07-14 00:02:33.851497 cloud-api-signer-0.2.0/cloud_api_signer/volc.py
+-rw-r--r--   0        0        0     2254 2023-07-13 08:38:32.144650 cloud-api-signer-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      608 2023-07-14 00:08:26.272226 cloud-api-signer-0.2.0/setup.py
+-rw-r--r--   0        0        0      448 2023-07-14 00:08:26.272537 cloud-api-signer-0.2.0/PKG-INFO
```

### Comparing `cloud-api-signer-0.1.0/LICENSE` & `cloud-api-signer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-api-signer-0.1.0/cloud_api_signer/bce.py` & `cloud-api-signer-0.2.0/cloud_api_signer/bce.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,97 +4,104 @@
 https://cloud.baidu.com/doc/Reference/s/njwvz1yfu
 
 """
 
 import hashlib
 import hmac
 from datetime import datetime
-from typing import Dict, List, Optional, Set, Tuple
+from typing import Dict, List, Set, Tuple
 
 from pydantic import BaseModel
 from typing_extensions import Final
 
 from cloud_api_signer import utils
-from cloud_api_signer.models import AkSk, HttpHeaders, HttpParams
-
-BCE_PREFIX: Final = 'x-bce-'
+from cloud_api_signer.models import AkSk, HttpHeaders, HttpMethod, HttpParams
 
 # 签名有效期限，硬编码以简化调用者的代码
 EXPIRATION_PERIOD_IN_SECONDS: Final = 1800
 
 
 class AuthResult(BaseModel):
     """ 存放签名计算的结果和重要的中间值，以便验证 """
 
-    # 包含 Authorization 和其他必要的 header。可以作为 http 请求的 headers 参数
-    # 对于百度智能云，它包含1个 header：Authorization
+    # 包含 Authorization 和其他签名过程中自动生成的 header。可以作为 http 请求的 headers 参数
+    # 对于百度智能云，它包含3个 header：Authorization、Host 和 x-bce-date
     sign_result: Dict[str, str]
 
     # 下面的值是中间结果，用于验证
     canonical_request: str
     auth_string_prefix: str
     signing_key: str
     signature: str
 
 
+class ApiInfo(BaseModel):
+    host: str
+    path: str
+    http_request_method: HttpMethod
+
+
 def make_auth(
     aksk: AkSk,
-    method: str,
-    path: str,
+    api_info: ApiInfo,
     params: HttpParams,
-    headers: HttpHeaders,
-    headers_to_sign: Set[str] = None,
 ) -> AuthResult:
-    canonical_uri = utils.uri_encode_except_slash(path)
+    """ 实现签名算法，返回签名结果 """
+    canonical_uri = utils.uri_encode_except_slash(api_info.path)
     canonical_query_string = utils.make_canonical_query_string(params)
-    canonical_headers, signed_headers = _to_canonical_headers(headers, headers_to_sign)
-    canonical_request = f'{method}\n{canonical_uri}\n{canonical_query_string}\n{canonical_headers}'
 
     # 文档中将“生成签名的 UTC 时间”称为 timestamp
     # 但它其实是一个 rfc3339 格式的字符串。这里沿用 timestamp 的命名，以便和文档一致
     timestamp = _to_timestamp()
 
+    headers_to_sign = {
+        # 百度智能云只强制要求编码 "Host" header
+        # 百度智能云提供的签名工具总是使用小写的 host，为了便于校验，这里也使用小写
+        'host': api_info.host,
+        # 再加上 x-bce-date，更好地防御重放攻击。同时，它也是部分 API 的必选项
+        'x-bce-date': timestamp,
+        # 其他 header 都是可选的，我们的选择是不将它们纳入签名，简化实现
+    }
+    canonical_headers, signed_headers = _to_canonical_headers(headers_to_sign)
+    canonical_request = '\n'.join(
+        [
+            api_info.http_request_method,
+            canonical_uri,
+            canonical_query_string,
+            canonical_headers,
+        ]
+    )
+
     auth_string_prefix = f'bce-auth-v1/{aksk.ak}/{timestamp}/{EXPIRATION_PERIOD_IN_SECONDS}'
 
     signing_key = hmac.new(aksk.sk.encode(), auth_string_prefix.encode(), hashlib.sha256).hexdigest()
 
     signature = hmac.new(signing_key.encode(), canonical_request.encode(), hashlib.sha256).hexdigest()
 
     return AuthResult(
         canonical_request=canonical_request,
         auth_string_prefix=auth_string_prefix,
         signing_key=signing_key,
         signature=signature,
         sign_result={
             'Authorization': f'{auth_string_prefix}/{signed_headers}/{signature}',
+            **headers_to_sign,
         },
     )
 
 
-def _to_canonical_headers(headers: HttpHeaders, headers_to_sign: Optional[Set[str]] = None) -> Tuple[str, str]:
-    headers = headers or {}
-
-    if headers_to_sign is None or len(headers_to_sign) == 0:
-        headers_to_sign = {
-            # 百度云只强制要求编码 "host" header
-            'host',
-        }
-    else:
-        headers_to_sign = {h.strip().lower() for h in headers_to_sign}
-
+def _to_canonical_headers(headers: HttpHeaders) -> Tuple[str, str]:
     result: List[str] = []
     signed_headers: Set[str] = set()
     for k, v in headers.items():
-        k_lower = k.strip().lower()
-
-        if k_lower.startswith(BCE_PREFIX) or k_lower in headers_to_sign:
-            new_k = utils.uri_encode(k_lower)
-            new_v = utils.uri_encode(str(v).strip())
-            result.append(f'{new_k}:{new_v}')
-            signed_headers.add(new_k)
+        # 百度智能云要求 key 和 value 都要进行 uri 编码
+        new_k = utils.uri_encode(k)
+        new_v = utils.uri_encode(v.strip())
+        result.append(f'{new_k}:{new_v}')
+        signed_headers.add(new_k)
 
     return '\n'.join(sorted(result)), ';'.join(sorted(signed_headers))
 
 
 def _to_timestamp() -> str:
     # 百度智能云的时间戳，按照 rfc3339 格式，精确到秒
     # 如：2015-04-27T08:23:49Z
```

### Comparing `cloud-api-signer-0.1.0/cloud_api_signer/utils.py` & `cloud-api-signer-0.2.0/cloud_api_signer/utils.py`

 * *Files identical despite different names*

### Comparing `cloud-api-signer-0.1.0/cloud_api_signer/volc.py` & `cloud-api-signer-0.2.0/cloud_api_signer/volc.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # 官方文档约定：算法固定为 HMAC-SHA256
 ALGORITHM: Final = 'HMAC-SHA256'
 
 
 class AuthResult(BaseModel):
     """ 存放签名计算的结果和重要的中间值，以便验证 """
 
-    # 包含 Authorization 和其他必要的 header。可以作为 http 请求的 headers 参数
+    # 包含 Authorization 和其他签名过程中自动生成的 header。可以作为 http 请求的 headers 参数
     # 对于火山引擎，它包含5个 header：Authorization X-Date X-Content-Sha256 Host Content-Type
     sign_result: Dict[str, str]
 
     # 下面的值是中间结果，用于验证
     canonical_query_string: str
     canonical_headers: str
     signed_headers: str
@@ -49,27 +49,28 @@
 def make_auth(
     aksk: AkSk,
     api_info: ApiInfo,
     params: HttpParams,
     content_type: str,
     body_str: Optional[str] = None,
 ) -> AuthResult:
-    """ 生成 Authorization header 的内容 """
-    x_date, x_date_short = _to_x_date()
-    x_content_sha256 = _hash_sha256(body_str or '')
+    """ 实现签名算法，返回签名结果 """
     canonical_uri = api_info.path
     canonical_query_string = utils.make_canonical_query_string(params)
 
-    headers: HttpHeaders = {
+    x_date, x_date_short = _to_x_date()
+    x_content_sha256 = _hash_sha256(body_str or '')
+
+    headers_to_sign: HttpHeaders = {
         'X-Date': x_date,
         'X-Content-Sha256': x_content_sha256,
         'Host': api_info.host,
         'Content-Type': content_type,
     }
-    ordered_headers = _make_oredered_headers(headers)
+    ordered_headers = _make_oredered_headers(headers_to_sign)
     signed_headers = ';'.join([k for k, _ in ordered_headers])
     # 每一个 canonical_header 都要以 \n 结尾，包括最后一个
     canonical_headers = ''.join([f'{k}:{v}\n' for k, v in ordered_headers])
     canonical_request = '\n'.join(
         [
             api_info.http_request_method,
             canonical_uri,
@@ -92,28 +93,28 @@
         credential_scope=credential_scope,
         string_to_sign=string_to_sign,
         sign_result={
             'Authorization': (
                 f'{ALGORITHM} Credential={aksk.ak}/{credential_scope}, '
                 f'SignedHeaders={signed_headers}, Signature={signature}'
             ),
-            **headers
+            **headers_to_sign,
         },
     )
 
 
 def _to_x_date() -> Tuple[str, str]:
     # 火山引擎的 x-data 格式是 ISO8601
     # 如：20201230T081805Z
     t = datetime.utcnow().strftime('%Y%m%dT%H%M%SZ')
     return t, t[:8]
 
 
 def _make_oredered_headers(headers: HttpHeaders) -> List[Tuple[str, str]]:
-    lowercase_headers = [(k.lower(), v) for k, v in headers.items()]
+    lowercase_headers = [(k.strip().lower(), v.strip()) for k, v in headers.items()]
     return sorted(lowercase_headers, key=lambda x: x[0])
 
 
 def _make_string_to_sign(x_date: str, credential_scope: str, canonical_request: str) -> str:
     request_date = x_date
     hashed_canonical_request = _hash_sha256(canonical_request)
     return '\n'.join([ALGORITHM, request_date, credential_scope, hashed_canonical_request])
```

### Comparing `cloud-api-signer-0.1.0/pyproject.toml` & `cloud-api-signer-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cloud-api-signer"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Huang Shaoyan <huangshaoyan1982@gmail.com>"]
 
 [[tool.poetry.source]]
 name = "aliyun"
 url = "https://mirrors.aliyun.com/pypi/simple/"
 default = true
```

### Comparing `cloud-api-signer-0.1.0/setup.py` & `cloud-api-signer-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.9.2']
 
 setup_kwargs = {
     'name': 'cloud-api-signer',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': '',
     'long_description': None,
     'author': 'Huang Shaoyan',
     'author_email': 'huangshaoyan1982@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

