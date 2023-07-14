# Comparing `tmp/fastapi_nextauth_jwt-1.0.1.tar.gz` & `tmp/fastapi_nextauth_jwt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_nextauth_jwt-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fastapi_nextauth_jwt-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fastapi_nextauth_jwt-1.0.1.tar` & `fastapi_nextauth_jwt-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      985 2023-07-13 19:58:45.841817 fastapi_nextauth_jwt-1.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      741 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     3089 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/LICENSE
--rw-r--r--   0        0        0     1484 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/README.md
--rw-r--r--   0        0        0      563 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      222 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/__init__.py
--rw-r--r--   0        0        0      974 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/cookies.py
--rw-r--r--   0        0        0      938 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/csrf.py
--rw-r--r--   0        0        0      696 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/exceptions.py
--rw-r--r--   0        0        0     5412 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/fastapi_nextauth_jwt.py
--rw-r--r--   0        0        0      312 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/operations.py
--rw-r--r--   0        0        0      646 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/tests/fastapi/main.py
--rw-r--r--   0        0        0    17406 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/tests/fastapi/test_main.py
--rw-r--r--   0        0        0     1021 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/tests/unit/test_cookies.py
--rw-r--r--   0        0        0     1654 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/tests/unit/test_csrf.py
--rw-r--r--   0        0        0      503 2023-07-13 19:58:45.845817 fastapi_nextauth_jwt-1.0.1/tests/unit/test_operations.py
--rw-r--r--   0        0        0     2054 1970-01-01 00:00:00.000000 fastapi_nextauth_jwt-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      985 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      741 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3089 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1069 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1541 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/README.md
+-rw-r--r--   0        0        0      563 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      222 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/__init__.py
+-rw-r--r--   0        0        0      974 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/cookies.py
+-rw-r--r--   0        0        0      938 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/csrf.py
+-rw-r--r--   0        0        0      873 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/exceptions.py
+-rw-r--r--   0        0        0     5850 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/fastapi_nextauth_jwt.py
+-rw-r--r--   0        0        0      580 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/operations.py
+-rw-r--r--   0        0        0      646 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/tests/fastapi/main.py
+-rw-r--r--   0        0        0    18051 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/tests/fastapi/test_main.py
+-rw-r--r--   0        0        0     1021 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/tests/unit/test_cookies.py
+-rw-r--r--   0        0        0     1654 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/tests/unit/test_csrf.py
+-rw-r--r--   0        0        0      503 2023-07-14 13:12:22.819178 fastapi_nextauth_jwt-1.1.0/tests/unit/test_operations.py
+-rw-r--r--   0        0        0     2111 1970-01-01 00:00:00.000000 fastapi_nextauth_jwt-1.1.0/PKG-INFO
```

### Comparing `fastapi_nextauth_jwt-1.0.1/.github/workflows/publish.yml` & `fastapi_nextauth_jwt-1.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.1/.github/workflows/test.yml` & `fastapi_nextauth_jwt-1.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.1/.gitignore` & `fastapi_nextauth_jwt-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.1/LICENSE` & `fastapi_nextauth_jwt-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.1/README.md` & `fastapi_nextauth_jwt-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # fastapi-nextauth-jwt
+[![PyPI version](https://badge.fury.io/py/fastapi-nextauth-jwt.svg)](https://badge.fury.io/py/fastapi-nextauth-jwt)
 
 This project contains a FastAPI dependency that can be used to decrypt and validate JWTs generated by NextAuth.
 The purpose of this project is to make it easy to use a FastAPI backend in projects that use Next.js and NextAuth 
 in the frontend. 
 
 Besides JWT decryption and validation, NextAuth compatible cross-site request forgery (CSRF) protection is also implemented.
 
@@ -38,11 +39,7 @@
 which should be equivalent to `NEXTAUTH_SECRET` on the Next.js side. 
 
 It is also possible to enable or disable CSRF protection using `csrf_prevention_enabled`. 
 If this is not set, this will looks at the ENV environment variable. If this is `dev` then CSRF protection will be disabled.
 
 You should also set the `NEXTAUTH_URL` environment variable, as it is used to determine
 whether or not secure cookies are being used. Or you can set the cookie names manually.
-
-# TODO
-
-- [ ] Add check to see if token has expired or not
```

### Comparing `fastapi_nextauth_jwt-1.0.1/pyproject.toml` & `fastapi_nextauth_jwt-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/cookies.py` & `fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/cookies.py`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/csrf.py` & `fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/csrf.py`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/exceptions.py` & `fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,7 +19,12 @@
 
 
 class CSRFMismatchError(NextAuthJWTException):
     def __init__(self, status_code: int, message: str):
         self.status_code = status_code
         self.message = message
 
+
+class TokenExpiredException(NextAuthJWTException):
+    def __init__(self, status_code: int, message: str):
+        self.status_code = status_code
+        self.message = message
```

### Comparing `fastapi_nextauth_jwt-1.0.1/src/fastapi_nextauth_jwt/fastapi_nextauth_jwt.py` & `fastapi_nextauth_jwt-1.1.0/src/fastapi_nextauth_jwt/fastapi_nextauth_jwt.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from starlette.requests import Request
 
 from jose import jwe
 from jose.exceptions import JWEError
 from cryptography.hazmat.primitives import hashes
 
-from fastapi_nextauth_jwt.operations import derive_key
+from fastapi_nextauth_jwt.operations import derive_key, check_expiry
 from fastapi_nextauth_jwt.cookies import extract_token
 from fastapi_nextauth_jwt.csrf import extract_csrf_info, validate_csrf_info
 from fastapi_nextauth_jwt.exceptions import InvalidTokenError, MissingTokenError, CSRFMismatchError
 
 
 class NextAuthJWT:
     def __init__(self,
@@ -23,15 +23,16 @@
                  secure_cookie: bool = None,
                  csrf_cookie_name: str = None,
                  csrf_header_name: str = "X-XSRF-Token",
                  info: bytes = b"NextAuth.js Generated Encryption Key",
                  salt: bytes = b"",
                  hash_algorithm: Any = hashes.SHA256(),
                  csrf_prevention_enabled: bool = None,
-                 csrf_methods: Set[str] = None):
+                 csrf_methods: Set[str] = None,
+                 check_expiry: bool = True):
         """
         Initializes a new instance of the NextAuthJWT class.
 
         Args:
             secret (str): The secret used for key derivation.
 
             cookie_name (str, optional): The name of the session cookie. Defaults to "__Secure-next-auth.session-token"
@@ -50,14 +51,16 @@
 
             csrf_prevention_enabled (bool, optional): Indicates if CSRF prevention is enabled.
              Defaults to True if ENV == "dev, else False.
 
             csrf_methods (Set[str], optional): The HTTP methods that require CSRF protection.
              Defaults to {'POST', 'PUT', 'PATCH', 'DELETE'}.
 
+             check_expiry (bool, optional): Whether or not to check the token for expiry. Defaults to True
+
         Example:
             >>> auth = NextAuthJWT(secret=os.getenv("NEXTAUTH_SECRET"))
         """
 
         self.secret = secret
 
         if secure_cookie is None:
@@ -89,27 +92,36 @@
             self.csrf_prevention_enabled = csrf_prevention_enabled
 
         if csrf_methods is None:
             self.csrf_methods = {'POST', 'PUT', 'PATCH', 'DELETE'}
         else:
             self.csrf_methods = csrf_methods
 
+        self.check_expiry = check_expiry
+
     def __call__(self, req: Request = None):
         encrypted_token = extract_token(req.cookies, self.cookie_name)
 
         if self.csrf_prevention_enabled:
             self.check_csrf_token(req)
 
         try:
             decrypted_token_string = jwe.decrypt(encrypted_token, self.key)
-            return json.loads(decrypted_token_string)
+            token = json.loads(decrypted_token_string)
         except (JWEError, JSONDecodeError) as e:
             print(e)
             raise InvalidTokenError(status_code=401, message="Invalid JWT format")
 
+        if self.check_expiry:
+            if "exp" not in token:
+                raise InvalidTokenError(status_code=401, message="Invalid JWT format, missing exp")
+            check_expiry(token['exp'])
+
+        return token
+
     def check_csrf_token(self, req: Request):
         if req.method not in self.csrf_methods:
             return
 
         if self.csrf_cookie_name not in req.cookies:
             raise MissingTokenError(status_code=401, message=f"Missing CSRF token: {self.csrf_cookie_name}")
         if self.csrf_header_name not in req.headers:
@@ -122,8 +134,9 @@
         # for info on how the CSRF cookie is created
         validate_csrf_info(self.secret, csrf_cookie_token, csrf_cookie_hash)
 
         # Check if the CSRF token in the headers matches the one in the cookie
         csrf_header_token = req.headers[self.csrf_header_name]
 
         if csrf_header_token != csrf_cookie_token:
-            raise CSRFMismatchError(status_code=401, message="CSRF Token mismatch")
+            raise CSRFMismatchError(status_code=401, message="CSRF Token mismatch")
+
```

### Comparing `fastapi_nextauth_jwt-1.0.1/tests/fastapi/main.py` & `fastapi_nextauth_jwt-1.1.0/tests/fastapi/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.1/tests/fastapi/test_main.py` & `fastapi_nextauth_jwt-1.1.0/tests/fastapi/test_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 from fastapi.testclient import TestClient
 
-from fastapi_nextauth_jwt.exceptions import MissingTokenError, InvalidTokenError
+from fastapi_nextauth_jwt.exceptions import MissingTokenError, InvalidTokenError, TokenExpiredException
 from main import app
 
 client = TestClient(app)
 
 cookies = {
     "next-auth.session-token.0": "eyJhbGciOiJkaXIiLCJlbmMiOiJBMjU2R0NNIn0..95CNrOPTvSJ7jhfv.xIqTgbOdms-gLkyDoOfhkdEaTVnqDkQiXPXcf6hhxHsdbYZIiQysxQBEA76SmPy5h6pk_bHKXqkFBjtLHmb2Pj-Ed4UEErI2csSxSvayy0SiunIA9H-bTkGuAp2ae6Z3vHHEPISOtVVU44Xlp3EvllRosIIkhWjMaSIfWhsv_agzSumU6dwA253xiI5pEoO4JyNd83vkdGC9RR7XPSNkJV2RZ-TUedJiqekd3Laacq8ZwkY3aHODOhvaRYnvvC5TGJqRNoHfo8_XzqNme5lw-jlidIjkF0q-5vXFp9E5ZnHmClql6lDS5xWLqyNNmaG_HvBKh8IfpCJJdweYY9nH_Dl8K89CIQACi9wvlVBw72_28wv6IjvIEOoZUX0yjGOY1bgULlJdfDIIZJ01dbPxoTpm1yI-5pu_1DkL_vdUA_pH3wqoRakKfNBJvdrRDG0AK7ZnnJ12SGOP0kymWuOc9D1rOxO3ac53IQ4XxN0AyZwF9VgfDtT3jW_oO69mn-dKzbq80mFk8bZo4Nd0WxlZm53SWsPTMaNZaJ5pR1IEd5Yxws8l6A1iR8WFYF9st2rYLV1euTx4ahpDFaNPn9IeosZWNodfy6644rXh-K5OLo57_YG9I-I8RQGz0sVs6m3gEUxtL7URCPQWcY_NAkdo5YTJZ3LI_zqDNqoMMpavqkls6nPfM6Rnb8qw2N-0krfEuvGithp2zhghuKpG2BPBOJAXCk9lU4WyYOJ3RcPk4hl0L_Hfp_5jjliRP0217HIKfduAEgG-qrhY_UG-e49ntXjrkFNwqYEi_hH7x8yq7d_1Y7Fg7hdJAPGZcaLuWPNc8ZNGQGnQrpVYDooM7YnCAMlqZVvkZjE631xrlvgJfhDd8ILs11Rylju22r1Jw7eNcnodBjRCSk7LVDsiqg6YU0I8tM2nTKMW9KL30lDKY0AI_0IsHzfR3wwlsiZVrjm7AuZ3rLoAhF5pua51q-RCI9yAsFTWa0_r3sylEK2Rms-9NjkOVzBZQWYKqnXX7ZGpboMrKwy1mfTNxo0M7Gdr1_Rw93UWAXfdFJzqj8foVr3JncLRrbMCCYiCJgYWUkbWFJCcef-KjF1gIJ8_fIR83HSDvQq-UrBCSXWYh8iL6zvkcpDvUUT6ECtaeR2c3Boe1XqsqcAjeu8TVtAC-QbXd91LglhHy32cn9rbqnEcrBhHa7f_MevfyVtEsyQbfwT6jsV8GJbH8Q92oQ_EhxVtLwXv8vuaGdINFQ0I0-1MUUpu6rRd7LOBp9C7-vfQYuqybmH75YycNXzTIT6DXa5c66gXUWrfnGgAteqIRWG9dPn2TUNBcPv8IDkHEoutgP7IiCigFw6QyvpGSZ2YrMuFiDLJMG1qnDFgFjbWOEC173ZGACv4z4NJr6dwlUJaisx4_At42SsDxQN5lwUekDGSARCOwyO7KkezM2UIPcvexdYhTVazH3Piut3Ih1wmP2ruujZRdVaQSp1-i-JigE0yplmxBVJXZFgNaiHMmnnLmod3N2sq8Gs9gSXN2bNgdZx8MT0wPrh0NlBjAWSOyPCd9ZU5EeWwd1CahgMly9AqHDHhHyAigfzgMAvMNhqv01hOJu6D_j46QA6xYqzTobOg_pHIdcnjpjkZHamLlk60GUwLkIugqsn0glQiUWPi0VjLPYmoaL2n8bZ_DGqrJZQyyoz6VvI2zhCXBj0GoebTVBQAT7djeFPoESo8Mp-ae-yqnusbZGdpcC68HWDeK1JmIunigG0DQqaatIg4JZqYOPKhKX-utQKujt1jAe_7UBiWgWAPgLkgU07sYEEhEqKkTNfzrY5_5AStww5d9pSdFsRHKRrtOsElcuII0WuAbbnzI7j7ISZS34aAfIuOBkrvJeoTun12amonBxtaifYXcPWydNwlsz0R0giZQ3VdqLAwqU-v1OcTbTsLaJO8G0RHcsrxRGNpcKl45pN8rMwvOR1NyAHVCRvH-cnWIQeFrO3qimRI5CWhmMZy7LBI-Jmk6SiF7ze8x1IOwEFZuQ8IMoP8ZmipwiEZAYk88J-zAe2tTA5lazi7JensWlLe3uRwhCVg0-OKGexYz_MKxvLe4QeJDIHEyyLFjXJVzUn1xQO4h6F1Z6W9G6eWygjgQA3dpVf5Xg2_5akVmhCeQ9HcFOFx8DoT6wxb1DNb1x26thPp5Cj7ScagvVeL_Z0dpFM6Py5N8qiHu8WCzHhOgdWIWpY_Vlrn0m3g5mQzt6i26qGW5MMDpsneUpe--_M21YzbHfhYqIWbKsjfVFDspWHUA-6uKgJLNn3UpE2U9uUY54HsEEeUxTSutzSFmZpl-YOzZYToKRKGgKoyoLKaFIju-XUlrPcSL7324z0U-0g7Zfe5axO9TFQIyoa-yG2Iub8-CujPqfg5NaKa853ESkmqeFf929XFD0I4LX6j2-I-8n0357X6qjwnx9EQQ1P5KTxWGJ3v5Hxajj4bqV8NhwJmCV4jiDYGAGjl6KRWNcDHfhb9nSAQd6w12FFWkxVQCEujkFh6ZlVR0a8wfdEMqio-UldCTgx51sAn00_n8TmAv8ovc_6DCBcXiOxZuBqOnqkGFH9LEkE4TDOkUOpRLvAex9qMxKKodNZWRWF4Mmp_g4yQmY5A10Xtpe33ofdoSQWQ0YSHcyjX1WHyJ-bQ_B_kUu5ttpkCa7r4YG_zNK7dQQszi1EgfmuLKYdJ26wRuTvasynybBgA_RTNVVAQQeGTgaVvnhX0dSOtIsounIpPtydujZwAux1sxcYDK9ocfGr7rmWuz4xmtw-_DvgFQg5eM2g9s921L0c_8TDiZuIyiDk72XydTz_2R_4zeo-w133BITMRK1hH9IcjHqLYV1qx8HsUqN85fdSzhQWcv7jeQt_emXOb8A5JlYqO4aVP8q3RxCupiA0NvBNS8mJI3qVvmutFpfIR00DkhbJlK9zc63TILSdtYk3ljIph5s6bV1tTHwuHX4fdHZ4ny-Tx2wPkjIiqn_EX9znG5luDXc8LPmAG_J4UsiBrLfktjBZSIWErO8dDF3JoGkR71GZNJi_7wYphVP9e7cB4_YB3royTnS3o1qUXUma3eRVZztLkQDMbGrj9QiDAPsGGpAW005Fmvs4w5cZECGgxbbhTQ9GLBuXyI9ba4cLB5hcL1wf3krowAAjGI9vXr4vlakTuiTmbo0OflEblWq2D996CALd9UC5viyP3zFlc25U4cYRn97HKcxaeFa6noODigtnF3rMEjzQdVi2IZKoKHI1AG0F84tF_05Mbzm1R1cvEvUD7NfQPAt2J0OsmcK6oqWBNBlS06jC_BAG2eoZ78LZOsXo1zvjimez-fKun0w_u7TR-SVg2RqRCVICPpN7l8UtO4JTWy86Wnu5JynyKGyRVaLHCvChEF4mS2ohIcGeymB-pVpnH6jHMGgUJ9JEGU2uD9yxJc4CiDP6aBOEmwu4kVcGFbWbNQTXga7e6AuqtWBjmDuopKuYX_3cGYYYq_y8iMI6f1VoQPc6r0l_cs6E2PfHGhVZfrKRN3tFvELHqXBMGuiI7dfpOuWUxDvGuD4qa5sFiUXZSdDvns2LDX6tmuquFPXnhZZJnQhdjfLegBwbdj1J07UMUXDXlz5PzFyT43_yG8ZthP_dzgKYVi5lHSal_2UFPAtvICxa0uVNAiDorEjiUphTp1u_kSvJVzeFnaDWbdk6AtLByH0p6Bf-A-luibzqMQWC7UdiMZFaDVsypSBiRVO1znr1p9HBHEkvi1fs60gIYcbeum4qWsIF1dlQFqGZQNj5r9tze-r1Cwy7KGoPeRCzr3Pxh9nw8nrO13NmRg8YW7_wJctrVw3CV31VTCuUtBCMXvlqOw0f8wW8XLx3zpMe81fvvL7WPxkZ",
     "next-auth.session-token.1": "Wbm5RpcYwdLRwd6CdfaKBR4n_bYW_fIIXWrsOfwnqBhWOC7DwALBOlO4MD9Ms6yqf_7HnRlrtnpy9WZVbZlGxvKbQF3wjJ7jTUTqo6dRsQJVUiJrfGFAUkJvv6_gTUd-K-id1.wdD2KVszoMv3uvO1RK_X9A",
@@ -27,14 +27,20 @@
                 'accessToken': 'eyJraWQiOiJ6ZnVyQ2prWk50OUs0SzYwdGQ3cDhnVEloNG40OXZWN0IyNzhFNlFHUjRJPSIsImFsZyI6IlJTMjU2In0.eyJzdWIiOiI4NGM4YjNhMS03MzU4LTQyMTEtYTBmOC1kNTQyODM3NWIzYWUiLCJpc3MiOiJodHRwczpcL1wvY29nbml0by1pZHAuZXUtd2VzdC0xLmFtYXpvbmF3cy5jb21cL2V1LXdlc3QtMV90bUJnUUxITkMiLCJ2ZXJzaW9uIjoyLCJjbGllbnRfaWQiOiI0ZGI1NmJkOWFsZGRycmpibG45NTV0bzFzOCIsIm9yaWdpbl9qdGkiOiI0MGJjNjYyNS1mMjk4LTQwODUtOTEzOS05MmI1YmQ3Zjk3YTUiLCJldmVudF9pZCI6ImYyNjc0MDc2LTc1MGMtNDIyNC1iMjNkLTJkZjc4YjExODVmZCIsInRva2VuX3VzZSI6ImFjY2VzcyIsInNjb3BlIjoib3BlbmlkIiwiYXV0aF90aW1lIjoxNjg5MjczMzA3LCJleHAiOjE2ODkyNzY5MDcsImlhdCI6MTY4OTI3MzMwNywianRpIjoiZTM2YTFkNTItNGI1YS00NjJmLWJmODctY2NjZDk0NTBmY2ZjIiwidXNlcm5hbWUiOiI4NGM4YjNhMS03MzU4LTQyMTEtYTBmOC1kNTQyODM3NWIzYWUifQ.I8rXQOMgz2hdQRb1vIiTjXig6kQX1ItntqW9wPr-Dr19wf_lU2zW_9TkzasP1_n6-Sl4nYfwixbcbhtez2XNPyNlF_oUZ3TccI6X2mp7-6c4hPUzuWeqrGGGBM0zoN5HJXXf-M2WKBZ5VF5TDQv4-Cl-BfbuYVbdS7zNdHhoAagCTRjCNg3d3p2ubZFWdzAI8cwl1qosYxKd8zy1qFmHBCuOjPz_HhAz-70gk4L4bcuU5BJkOIXy3GiHjiTloXkEmkF0uPPj3wjGDTab_h5yT8u0Cgh3Nrbaa1-f7xeTNhrUWd-eze50cTGC-rrl6nLF9K34eZso9o1jtfiwz_yUXQ',
                 'refreshToken': 'eyJjdHkiOiJKV1QiLCJlbmMiOiJBMjU2R0NNIiwiYWxnIjoiUlNBLU9BRVAifQ.jTJoyxspsiO93uKWyI03nEumiyc_X4o0_n-gZpDBpWeaQXXayHrOk3UwzMoDD9PvZOgD1F77lJ9tQ38T_f0XyhTscLWBuolicxwHUfhWQNHhngVKGs9zFQgbyxipgJih_eoioRnFv9u_UQ7NshBkf1AG72goYaHYMgaOTlnSD0aR96ysfyedSCEZTIB4nPwKEvOc_cRZFeUnT5Any-LJyEZbTiO1hcdA8WWtuI18mDmaJP_5rI3jTMxoMtnIwapo2kP2fkqDDBukJAoTOU1BzXsmSOvw3s-ztT95qUN_Ni8Wlcv0YpceupCXPnGbHkPbgMQKCzny9dO6WEiCS7r7Wg.FGYQIB7zvKzRm9GG.rdQi4z18GY-e5we2Qz9l2EChKatT8uSpn_LvSJVm6kcvfORukZrT8Ox-KVVSdK0J9mh0NWnW5AdN2q2O5luSqJZyti-_hj73CqfBgKMrThvMW45cu6N7gKP3HlkFQIx4y0vherAxP3imCC66Lo-c-vCNPJJBZjgfQ_-VmIJ49AGk3Im39_B7_y5xwPHi42-VPST6AYBtQeAcAmOcZGzXStWl8-iKatWNjBw16QHtWoawI9UCydLrV4dn-WbtkiO7-MQwADKM0Ql8O9S7Fm9qx_DItBkayTJGrabDRMrbc9QsYttvRyXuWaFwxPqRK1zJsSQ8WFkXYSZTcMZ74u9axbIkqZtQvqK24nhUFTfdz2XVkIyNPhaV_JmL8SRV7dXhKrcdK-5B4tBSNcw1d5AkhoK75JmeBQOlHUBbAQGga1oeFxZTKNrXKrgsVNaCYi3KomhQcvjCNvzpCyn36EXwQkNId2a7Rd_Jvh4gxfVZGlHDmQ-ONDnlPs9EsILhD87nFRIhR900X7-VUK_MG1GoWwFRKaWG_N6npBNVg8tLVFB-7d-n8CDJJuI0sWh3jNqlfek12FWZerh5TEyUOAN6Wcl8ov-ocLfkrnOgKBjCz2_-POJhWUIPwr2_nunqO-sgZ-vPitU8R-7OB6sdgG7ZQNYLboyC2NrB7TPY4CpDrM-Vx7xEiWOVWG0biS30dE9xK8E5DhddC5aUs6yt-P3lsrHeZ-ttIyOwJ-asrZRSe3uU7t4ItPqDeqCjXU5ib8YyOSk8OJwhyKTddvhCs0m4PdjKj9uA4uWRmg7VdMNS6g-BX0uGDP5sLdV0WzADyqJ0NEkyCybTiCebSi_4vqHm4ZsAcnkgtMgd5xp--0v0f4lOc5W_6HqDWCkoqxmIKgAve4cV3LoqkmIret1MnuZQoZt3Z-BXr4z4jk8oXGHzL292567zG5eKJVVWvm-V_Pch3pl4wEnbeiOzf01h9C4Yym9OSjXZd3Xjc26UtMoAyW2ERD8TUQy5ZOuboknjy2eH-hJRUOB-C28IzW3_MavRjhv8_jyI3InzPnzqmuBB8grkEprQ5-_bnOYGcBQpB1F1tWOSNzmfEH0ksVMDCktP5ph4XyBIdAz2O662Vxub5ouZDp5GPCWCXZMLOC3yrVLkCiG0AD5vepXIN6U6tFBIk--d6YOZZRAo9zuDKFTgC65KQE8xMZzq9zzrqVY-igaZZ8NqlY_8M7Xfxdlch-X4tx5zHY_Ku9zYmx14drB1Vuj98wP7m-p0KRqwJDYcpDhjc_XYRuG8uunjgHEJ3C_s0LJlDQcEalvJfQzcPsX0.sj7jXlqlX0lm4AJzId1EDw',
                 'iat': 1689273309,
                 'exp': 1691865309,
                 'jti': '2b8540dd-4d7c-400f-ad65-7d112ac5a07a'}
 
 
+@pytest.fixture(autouse=True)
+def patch_current_time(monkeypatch):
+    # Monkeypatch the deadline so the tests don't rely on the current time
+    monkeypatch.setattr("fastapi_nextauth_jwt.operations.check_expiry.__defaults__", (1691865310,))
+
+
 def test_no_csrf():
     client.cookies = cookies
     response = client.get("/")
 
     assert response.status_code == 200
     assert response.json() == expected_jwt
 
@@ -73,7 +79,17 @@
 
 
 def test_invalid_jwt():
     with pytest.raises(InvalidTokenError) as exc_info:
         client.cookies = cookies_invalid
         client.get("/")
         assert exc_info.value.message == "Invalid JWT format"
+
+
+def test_expiry(monkeypatch):
+    # In this case, we patch the deadline to be before token expiration
+    monkeypatch.setattr("fastapi_nextauth_jwt.operations.check_expiry.__defaults__", (1691865300,))
+
+    with pytest.raises(TokenExpiredException) as exc_info:
+        client.cookies = cookies
+        client.get("/")
+        assert exc_info.value.message == "Token Expired"
```

### Comparing `fastapi_nextauth_jwt-1.0.1/tests/unit/test_cookies.py` & `fastapi_nextauth_jwt-1.1.0/tests/unit/test_cookies.py`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.1/tests/unit/test_csrf.py` & `fastapi_nextauth_jwt-1.1.0/tests/unit/test_csrf.py`

 * *Files identical despite different names*

### Comparing `fastapi_nextauth_jwt-1.0.1/PKG-INFO` & `fastapi_nextauth_jwt-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: fastapi_nextauth_jwt
-Version: 1.0.1
+Version: 1.1.0
 Summary: A fastapi dependency used to decode jwt tokens generated by nextauth,
 Author: Tom Catshoek
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: fastapi
 Requires-Dist: cryptography
 Requires-Dist: python-jose[cryptography]
 Requires-Dist: pytest >=2.7.3 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: httpx ; extra == "test"
 Project-URL: Home, https://github.com/TCatshoek/fastapi-nextauth-jwt
 Provides-Extra: test
 
 # fastapi-nextauth-jwt
+[![PyPI version](https://badge.fury.io/py/fastapi-nextauth-jwt.svg)](https://badge.fury.io/py/fastapi-nextauth-jwt)
 
 This project contains a FastAPI dependency that can be used to decrypt and validate JWTs generated by NextAuth.
 The purpose of this project is to make it easy to use a FastAPI backend in projects that use Next.js and NextAuth 
 in the frontend. 
 
 Besides JWT decryption and validation, NextAuth compatible cross-site request forgery (CSRF) protection is also implemented.
 
@@ -55,10 +56,7 @@
 
 It is also possible to enable or disable CSRF protection using `csrf_prevention_enabled`. 
 If this is not set, this will looks at the ENV environment variable. If this is `dev` then CSRF protection will be disabled.
 
 You should also set the `NEXTAUTH_URL` environment variable, as it is used to determine
 whether or not secure cookies are being used. Or you can set the cookie names manually.
 
-# TODO
-
-- [ ] Add check to see if token has expired or not
```

