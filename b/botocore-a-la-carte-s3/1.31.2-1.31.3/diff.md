# Comparing `tmp/botocore-a-la-carte-s3-1.31.2.tar.gz` & `tmp/botocore-a-la-carte-s3-1.31.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-s3-1.31.2.tar", last modified: Wed Jul 12 01:44:57 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-s3-1.31.3.tar", last modified: Fri Jul 14 01:46:39 2023, max compression
```

## Comparing `botocore-a-la-carte-s3-1.31.2.tar` & `botocore-a-la-carte-s3-1.31.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:57.763473 botocore-a-la-carte-s3-1.31.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-12 01:44:57.000000 botocore-a-la-carte-s3-1.31.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-12 01:44:57.763473 botocore-a-la-carte-s3-1.31.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:57.759473 botocore-a-la-carte-s3-1.31.2/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:57.759473 botocore-a-la-carte-s3-1.31.2/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:57.759473 botocore-a-la-carte-s3-1.31.2/botocore/data/s3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:57.763473 botocore-a-la-carte-s3-1.31.2/botocore/data/s3/2006-03-01/
--rw-r--r--   0 runner    (1001) docker     (123)  1674528 2023-07-12 01:44:12.000000 botocore-a-la-carte-s3-1.31.2/botocore/data/s3/2006-03-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    57596 2023-07-12 01:44:12.000000 botocore-a-la-carte-s3-1.31.2/botocore/data/s3/2006-03-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-12 01:44:12.000000 botocore-a-la-carte-s3-1.31.2/botocore/data/s3/2006-03-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-12 01:44:12.000000 botocore-a-la-carte-s3-1.31.2/botocore/data/s3/2006-03-01/paginators-1.sdk-extras.json
--rw-r--r--   0 runner    (1001) docker     (123)   852245 2023-07-12 01:44:12.000000 botocore-a-la-carte-s3-1.31.2/botocore/data/s3/2006-03-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-12 01:44:12.000000 botocore-a-la-carte-s3-1.31.2/botocore/data/s3/2006-03-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:44:57.763473 botocore-a-la-carte-s3-1.31.2/botocore_a_la_carte_s3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-12 01:44:57.000000 botocore-a-la-carte-s3-1.31.2/botocore_a_la_carte_s3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-12 01:44:57.000000 botocore-a-la-carte-s3-1.31.2/botocore_a_la_carte_s3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:44:57.000000 botocore-a-la-carte-s3-1.31.2/botocore_a_la_carte_s3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 01:44:57.000000 botocore-a-la-carte-s3-1.31.2/botocore_a_la_carte_s3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:44:57.763473 botocore-a-la-carte-s3-1.31.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-12 01:44:57.000000 botocore-a-la-carte-s3-1.31.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:39.198963 botocore-a-la-carte-s3-1.31.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-14 01:46:38.000000 botocore-a-la-carte-s3-1.31.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-14 01:46:39.198963 botocore-a-la-carte-s3-1.31.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:39.194963 botocore-a-la-carte-s3-1.31.3/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:39.194963 botocore-a-la-carte-s3-1.31.3/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:39.194963 botocore-a-la-carte-s3-1.31.3/botocore/data/s3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:39.198963 botocore-a-la-carte-s3-1.31.3/botocore/data/s3/2006-03-01/
+-rw-r--r--   0 runner    (1001) docker     (123)  1674528 2023-07-14 01:45:45.000000 botocore-a-la-carte-s3-1.31.3/botocore/data/s3/2006-03-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57596 2023-07-14 01:45:45.000000 botocore-a-la-carte-s3-1.31.3/botocore/data/s3/2006-03-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-14 01:45:45.000000 botocore-a-la-carte-s3-1.31.3/botocore/data/s3/2006-03-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-14 01:45:45.000000 botocore-a-la-carte-s3-1.31.3/botocore/data/s3/2006-03-01/paginators-1.sdk-extras.json
+-rw-r--r--   0 runner    (1001) docker     (123)   852471 2023-07-14 01:45:45.000000 botocore-a-la-carte-s3-1.31.3/botocore/data/s3/2006-03-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-14 01:45:45.000000 botocore-a-la-carte-s3-1.31.3/botocore/data/s3/2006-03-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:39.198963 botocore-a-la-carte-s3-1.31.3/botocore_a_la_carte_s3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-14 01:46:39.000000 botocore-a-la-carte-s3-1.31.3/botocore_a_la_carte_s3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-14 01:46:39.000000 botocore-a-la-carte-s3-1.31.3/botocore_a_la_carte_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:46:39.000000 botocore-a-la-carte-s3-1.31.3/botocore_a_la_carte_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 01:46:39.000000 botocore-a-la-carte-s3-1.31.3/botocore_a_la_carte_s3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 01:46:39.198963 botocore-a-la-carte-s3-1.31.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:46:38.000000 botocore-a-la-carte-s3-1.31.3/setup.py
```

### Comparing `botocore-a-la-carte-s3-1.31.2/LICENSE.txt` & `botocore-a-la-carte-s3-1.31.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-s3-1.31.2/PKG-INFO` & `botocore-a-la-carte-s3-1.31.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-s3
-Version: 1.31.2
+Version: 1.31.3
 Summary: s3 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-s3-1.31.2/botocore/data/s3/2006-03-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-s3-1.31.3/botocore/data/s3/2006-03-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-s3-1.31.2/botocore/data/s3/2006-03-01/examples-1.json` & `botocore-a-la-carte-s3-1.31.3/botocore/data/s3/2006-03-01/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-s3-1.31.2/botocore/data/s3/2006-03-01/paginators-1.json` & `botocore-a-la-carte-s3-1.31.3/botocore/data/s3/2006-03-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-s3-1.31.2/botocore/data/s3/2006-03-01/paginators-1.sdk-extras.json` & `botocore-a-la-carte-s3-1.31.3/botocore/data/s3/2006-03-01/paginators-1.sdk-extras.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-s3-1.31.2/botocore/data/s3/2006-03-01/service-2.json` & `botocore-a-la-carte-s3-1.31.3/botocore/data/s3/2006-03-01/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999694690927964%*

 * *Differences: {"'operations'": "{'CopyObject': {'documentation': '<p>Creates a copy of an object that is already "*

 * *                 'stored in Amazon S3.</p> <note> <p>You can store individual objects of up to 5 '*

 * *                 'TB in Amazon S3. You create a copy of your object up to 5 GB in size in a single '*

 * *                 'atomic action using this API. However, to copy an object greater than 5 GB, you '*

 * *                 'must use the multipart upload Upload Part - Copy (UploadPartCopy) API. For more '*

 * *            […]*

```diff
@@ -65,15 +65,15 @@
             "name": "CompleteMultipartUpload",
             "output": {
                 "shape": "CompleteMultipartUploadOutput"
             }
         },
         "CopyObject": {
             "alias": "PutObjectCopy",
-            "documentation": "<p>Creates a copy of an object that is already stored in Amazon S3.</p> <note> <p>You can store individual objects of up to 5 TB in Amazon S3. You create a copy of your object up to 5 GB in size in a single atomic action using this API. However, to copy an object greater than 5 GB, you must use the multipart upload Upload Part - Copy (UploadPartCopy) API. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/CopyingObjctsUsingRESTMPUapi.html\">Copy Object Using the REST Multipart Upload API</a>.</p> </note> <p>All copy requests must be authenticated. Additionally, you must have <i>read</i> access to the source object and <i>write</i> access to the destination bucket. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html\">REST Authentication</a>. Both the Region that you want to copy the object from and the Region that you want to copy the object to must be enabled for your account.</p> <p>A copy request might return an error when Amazon S3 receives the copy request or while Amazon S3 is copying the files. If the error occurs before the copy action starts, you receive a standard Amazon S3 error. If the error occurs during the copy operation, the error response is embedded in the <code>200 OK</code> response. This means that a <code>200 OK</code> response can contain either a success or an error. If you call the S3 API directly, make sure to design your application to parse the contents of the response and handle it appropriately. If you use Amazon Web Services SDKs, SDKs handle this condition. The SDKs detect the embedded error and apply error handling per your configuration settings (including automatically retrying the request as appropriate). If the condition persists, the SDKs throws an exception (or, for the SDKs that don't use exceptions, they return the error).</p> <p>If the copy is successful, you receive a response with information about the copied object.</p> <note> <p>If the request is an HTTP 1.1 request, the response is chunk encoded. If it were not, it would not contain the content-length, and you would need to read the entire body.</p> </note> <p>The copy request charge is based on the storage class and Region that you specify for the destination object. For pricing information, see <a href=\"http://aws.amazon.com/s3/pricing/\">Amazon S3 pricing</a>.</p> <important> <p>Amazon S3 transfer acceleration does not support cross-Region copies. If you request a cross-Region copy using a transfer acceleration endpoint, you get a 400 <code>Bad Request</code> error. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/transfer-acceleration.html\">Transfer Acceleration</a>.</p> </important> <dl> <dt>Metadata</dt> <dd> <p>When copying an object, you can preserve all metadata (the default) or specify new metadata. However, the access control list (ACL) is not preserved and is set to private for the user making the request. To override the default ACL setting, specify a new ACL when generating a copy request. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/S3_ACLs_UsingACLs.html\">Using ACLs</a>. </p> <p>To specify whether you want the object metadata copied from the source object or replaced with metadata provided in the request, you can optionally add the <code>x-amz-metadata-directive</code> header. When you grant permissions, you can use the <code>s3:x-amz-metadata-directive</code> condition key to enforce certain metadata behavior when objects are uploaded. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/amazon-s3-policy-keys.html\">Specifying Conditions in a Policy</a> in the <i>Amazon S3 User Guide</i>. For a complete list of Amazon S3-specific condition keys, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/list_amazons3.html\">Actions, Resources, and Condition Keys for Amazon S3</a>.</p> <note> <p> <code>x-amz-website-redirect-location</code> is unique to each object and must be specified in the request headers to copy the value.</p> </note> </dd> <dt>x-amz-copy-source-if Headers</dt> <dd> <p>To only copy an object under certain conditions, such as whether the <code>Etag</code> matches or whether the object was modified before or after a specified date, use the following request parameters:</p> <ul> <li> <p> <code>x-amz-copy-source-if-match</code> </p> </li> <li> <p> <code>x-amz-copy-source-if-none-match</code> </p> </li> <li> <p> <code>x-amz-copy-source-if-unmodified-since</code> </p> </li> <li> <p> <code>x-amz-copy-source-if-modified-since</code> </p> </li> </ul> <p> If both the <code>x-amz-copy-source-if-match</code> and <code>x-amz-copy-source-if-unmodified-since</code> headers are present in the request and evaluate as follows, Amazon S3 returns <code>200 OK</code> and copies the data:</p> <ul> <li> <p> <code>x-amz-copy-source-if-match</code> condition evaluates to true</p> </li> <li> <p> <code>x-amz-copy-source-if-unmodified-since</code> condition evaluates to false</p> </li> </ul> <p>If both the <code>x-amz-copy-source-if-none-match</code> and <code>x-amz-copy-source-if-modified-since</code> headers are present in the request and evaluate as follows, Amazon S3 returns the <code>412 Precondition Failed</code> response code:</p> <ul> <li> <p> <code>x-amz-copy-source-if-none-match</code> condition evaluates to false</p> </li> <li> <p> <code>x-amz-copy-source-if-modified-since</code> condition evaluates to true</p> </li> </ul> <note> <p>All headers with the <code>x-amz-</code> prefix, including <code>x-amz-copy-source</code>, must be signed.</p> </note> </dd> <dt>Server-side encryption</dt> <dd> <p>Amazon S3 automatically encrypts all new objects that are copied to an S3 bucket. When copying an object, if you don't specify encryption information in your copy request, the encryption setting of the target object is set to the default encryption configuration of the destination bucket. By default, all buckets have a base level of encryption configuration that uses server-side encryption with Amazon S3 managed keys (SSE-S3). If the destination bucket has a default encryption configuration that uses server-side encryption with Key Management Service (KMS) keys (SSE-KMS), dual-layer server-side encryption with Amazon Web Services KMS keys (DSSE-KMS), or server-side encryption with customer-provided encryption keys (SSE-C), Amazon S3 uses the corresponding KMS key, or a customer-provided key to encrypt the target object copy.</p> <p>When you perform a <code>CopyObject</code> operation, if you want to use a different type of encryption setting for the target object, you can use other appropriate encryption-related headers to encrypt the target object with a KMS key, an Amazon S3 managed key, or a customer-provided key. With server-side encryption, Amazon S3 encrypts your data as it writes your data to disks in its data centers and decrypts the data when you access it. If the encryption setting in your request is different from the default encryption configuration of the destination bucket, the encryption setting in your request takes precedence. If the source object for the copy is stored in Amazon S3 using SSE-C, you must provide the necessary encryption information in your request so that Amazon S3 can decrypt the object for copying. For more information about server-side encryption, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/serv-side-encryption.html\">Using Server-Side Encryption</a>.</p> <p>If a target object uses SSE-KMS, you can enable an S3 Bucket Key for the object. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/bucket-key.html\">Amazon S3 Bucket Keys</a> in the <i>Amazon S3 User Guide</i>.</p> </dd> <dt>Access Control List (ACL)-Specific Request Headers</dt> <dd> <p>When copying an object, you can optionally use headers to grant ACL-based permissions. By default, all objects are private. Only the owner has full access control. When adding a new object, you can grant permissions to individual Amazon Web Services accounts or to predefined groups that are defined by Amazon S3. These permissions are then added to the ACL on the object. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/acl-overview.html\">Access Control List (ACL) Overview</a> and <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/acl-using-rest-api.html\">Managing ACLs Using the REST API</a>. </p> <p>If the bucket that you're copying objects to uses the bucket owner enforced setting for S3 Object Ownership, ACLs are disabled and no longer affect permissions. Buckets that use this setting only accept <code>PUT</code> requests that don't specify an ACL or <code>PUT</code> requests that specify bucket owner full control ACLs, such as the <code>bucket-owner-full-control</code> canned ACL or an equivalent form of this ACL expressed in the XML format.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/about-object-ownership.html\"> Controlling ownership of objects and disabling ACLs</a> in the <i>Amazon S3 User Guide</i>.</p> <note> <p>If your bucket uses the bucket owner enforced setting for Object Ownership, all objects written to the bucket by any account will be owned by the bucket owner.</p> </note> </dd> <dt>Checksums</dt> <dd> <p>When copying an object, if it has a checksum, that checksum will be copied to the new object by default. When you copy the object over, you can optionally specify a different checksum algorithm to use with the <code>x-amz-checksum-algorithm</code> header.</p> </dd> <dt>Storage Class Options</dt> <dd> <p>You can use the <code>CopyObject</code> action to change the storage class of an object that is already stored in Amazon S3 by using the <code>StorageClass</code> parameter. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/storage-class-intro.html\">Storage Classes</a> in the <i>Amazon S3 User Guide</i>.</p> <p>If the source object's storage class is GLACIER, you must restore a copy of this object before you can use it as a source object for the copy operation. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/API/API_RestoreObject.html\">RestoreObject</a>. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/CopyingObjectsExamples.html\">Copying Objects</a>.</p> </dd> <dt>Versioning</dt> <dd> <p>By default, <code>x-amz-copy-source</code> header identifies the current version of an object to copy. If the current version is a delete marker, Amazon S3 behaves as if the object was deleted. To copy a different version, use the <code>versionId</code> subresource.</p> <p>If you enable versioning on the target bucket, Amazon S3 generates a unique version ID for the object being copied. This version ID is different from the version ID of the source object. Amazon S3 returns the version ID of the copied object in the <code>x-amz-version-id</code> response header in the response.</p> <p>If you do not enable versioning or suspend it on the target bucket, the version ID that Amazon S3 generates is always null.</p> </dd> </dl> <p>The following operations are related to <code>CopyObject</code>:</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html\">PutObject</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/API/API_GetObject.html\">GetObject</a> </p> </li> </ul>",
+            "documentation": "<p>Creates a copy of an object that is already stored in Amazon S3.</p> <note> <p>You can store individual objects of up to 5 TB in Amazon S3. You create a copy of your object up to 5 GB in size in a single atomic action using this API. However, to copy an object greater than 5 GB, you must use the multipart upload Upload Part - Copy (UploadPartCopy) API. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/CopyingObjctsUsingRESTMPUapi.html\">Copy Object Using the REST Multipart Upload API</a>.</p> </note> <p>All copy requests must be authenticated. Additionally, you must have <i>read</i> access to the source object and <i>write</i> access to the destination bucket. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html\">REST Authentication</a>. Both the Region that you want to copy the object from and the Region that you want to copy the object to must be enabled for your account.</p> <p>A copy request might return an error when Amazon S3 receives the copy request or while Amazon S3 is copying the files. If the error occurs before the copy action starts, you receive a standard Amazon S3 error. If the error occurs during the copy operation, the error response is embedded in the <code>200 OK</code> response. This means that a <code>200 OK</code> response can contain either a success or an error. If you call the S3 API directly, make sure to design your application to parse the contents of the response and handle it appropriately. If you use Amazon Web Services SDKs, SDKs handle this condition. The SDKs detect the embedded error and apply error handling per your configuration settings (including automatically retrying the request as appropriate). If the condition persists, the SDKs throws an exception (or, for the SDKs that don't use exceptions, they return the error).</p> <p>If the copy is successful, you receive a response with information about the copied object.</p> <note> <p>If the request is an HTTP 1.1 request, the response is chunk encoded. If it were not, it would not contain the content-length, and you would need to read the entire body.</p> </note> <p>The copy request charge is based on the storage class and Region that you specify for the destination object. The request can also result in a data retrieval charge for the source if the source storage class bills for data retrieval. For pricing information, see <a href=\"http://aws.amazon.com/s3/pricing/\">Amazon S3 pricing</a>.</p> <important> <p>Amazon S3 transfer acceleration does not support cross-Region copies. If you request a cross-Region copy using a transfer acceleration endpoint, you get a 400 <code>Bad Request</code> error. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/transfer-acceleration.html\">Transfer Acceleration</a>.</p> </important> <dl> <dt>Metadata</dt> <dd> <p>When copying an object, you can preserve all metadata (the default) or specify new metadata. However, the access control list (ACL) is not preserved and is set to private for the user making the request. To override the default ACL setting, specify a new ACL when generating a copy request. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/S3_ACLs_UsingACLs.html\">Using ACLs</a>. </p> <p>To specify whether you want the object metadata copied from the source object or replaced with metadata provided in the request, you can optionally add the <code>x-amz-metadata-directive</code> header. When you grant permissions, you can use the <code>s3:x-amz-metadata-directive</code> condition key to enforce certain metadata behavior when objects are uploaded. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/amazon-s3-policy-keys.html\">Specifying Conditions in a Policy</a> in the <i>Amazon S3 User Guide</i>. For a complete list of Amazon S3-specific condition keys, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/list_amazons3.html\">Actions, Resources, and Condition Keys for Amazon S3</a>.</p> <note> <p> <code>x-amz-website-redirect-location</code> is unique to each object and must be specified in the request headers to copy the value.</p> </note> </dd> <dt>x-amz-copy-source-if Headers</dt> <dd> <p>To only copy an object under certain conditions, such as whether the <code>Etag</code> matches or whether the object was modified before or after a specified date, use the following request parameters:</p> <ul> <li> <p> <code>x-amz-copy-source-if-match</code> </p> </li> <li> <p> <code>x-amz-copy-source-if-none-match</code> </p> </li> <li> <p> <code>x-amz-copy-source-if-unmodified-since</code> </p> </li> <li> <p> <code>x-amz-copy-source-if-modified-since</code> </p> </li> </ul> <p> If both the <code>x-amz-copy-source-if-match</code> and <code>x-amz-copy-source-if-unmodified-since</code> headers are present in the request and evaluate as follows, Amazon S3 returns <code>200 OK</code> and copies the data:</p> <ul> <li> <p> <code>x-amz-copy-source-if-match</code> condition evaluates to true</p> </li> <li> <p> <code>x-amz-copy-source-if-unmodified-since</code> condition evaluates to false</p> </li> </ul> <p>If both the <code>x-amz-copy-source-if-none-match</code> and <code>x-amz-copy-source-if-modified-since</code> headers are present in the request and evaluate as follows, Amazon S3 returns the <code>412 Precondition Failed</code> response code:</p> <ul> <li> <p> <code>x-amz-copy-source-if-none-match</code> condition evaluates to false</p> </li> <li> <p> <code>x-amz-copy-source-if-modified-since</code> condition evaluates to true</p> </li> </ul> <note> <p>All headers with the <code>x-amz-</code> prefix, including <code>x-amz-copy-source</code>, must be signed.</p> </note> </dd> <dt>Server-side encryption</dt> <dd> <p>Amazon S3 automatically encrypts all new objects that are copied to an S3 bucket. When copying an object, if you don't specify encryption information in your copy request, the encryption setting of the target object is set to the default encryption configuration of the destination bucket. By default, all buckets have a base level of encryption configuration that uses server-side encryption with Amazon S3 managed keys (SSE-S3). If the destination bucket has a default encryption configuration that uses server-side encryption with Key Management Service (KMS) keys (SSE-KMS), dual-layer server-side encryption with Amazon Web Services KMS keys (DSSE-KMS), or server-side encryption with customer-provided encryption keys (SSE-C), Amazon S3 uses the corresponding KMS key, or a customer-provided key to encrypt the target object copy.</p> <p>When you perform a <code>CopyObject</code> operation, if you want to use a different type of encryption setting for the target object, you can use other appropriate encryption-related headers to encrypt the target object with a KMS key, an Amazon S3 managed key, or a customer-provided key. With server-side encryption, Amazon S3 encrypts your data as it writes your data to disks in its data centers and decrypts the data when you access it. If the encryption setting in your request is different from the default encryption configuration of the destination bucket, the encryption setting in your request takes precedence. If the source object for the copy is stored in Amazon S3 using SSE-C, you must provide the necessary encryption information in your request so that Amazon S3 can decrypt the object for copying. For more information about server-side encryption, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/serv-side-encryption.html\">Using Server-Side Encryption</a>.</p> <p>If a target object uses SSE-KMS, you can enable an S3 Bucket Key for the object. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/bucket-key.html\">Amazon S3 Bucket Keys</a> in the <i>Amazon S3 User Guide</i>.</p> </dd> <dt>Access Control List (ACL)-Specific Request Headers</dt> <dd> <p>When copying an object, you can optionally use headers to grant ACL-based permissions. By default, all objects are private. Only the owner has full access control. When adding a new object, you can grant permissions to individual Amazon Web Services accounts or to predefined groups that are defined by Amazon S3. These permissions are then added to the ACL on the object. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/acl-overview.html\">Access Control List (ACL) Overview</a> and <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/acl-using-rest-api.html\">Managing ACLs Using the REST API</a>. </p> <p>If the bucket that you're copying objects to uses the bucket owner enforced setting for S3 Object Ownership, ACLs are disabled and no longer affect permissions. Buckets that use this setting only accept <code>PUT</code> requests that don't specify an ACL or <code>PUT</code> requests that specify bucket owner full control ACLs, such as the <code>bucket-owner-full-control</code> canned ACL or an equivalent form of this ACL expressed in the XML format.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/about-object-ownership.html\"> Controlling ownership of objects and disabling ACLs</a> in the <i>Amazon S3 User Guide</i>.</p> <note> <p>If your bucket uses the bucket owner enforced setting for Object Ownership, all objects written to the bucket by any account will be owned by the bucket owner.</p> </note> </dd> <dt>Checksums</dt> <dd> <p>When copying an object, if it has a checksum, that checksum will be copied to the new object by default. When you copy the object over, you can optionally specify a different checksum algorithm to use with the <code>x-amz-checksum-algorithm</code> header.</p> </dd> <dt>Storage Class Options</dt> <dd> <p>You can use the <code>CopyObject</code> action to change the storage class of an object that is already stored in Amazon S3 by using the <code>StorageClass</code> parameter. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/storage-class-intro.html\">Storage Classes</a> in the <i>Amazon S3 User Guide</i>.</p> <p>If the source object's storage class is GLACIER, you must restore a copy of this object before you can use it as a source object for the copy operation. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/API/API_RestoreObject.html\">RestoreObject</a>. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/dev/CopyingObjectsExamples.html\">Copying Objects</a>.</p> </dd> <dt>Versioning</dt> <dd> <p>By default, <code>x-amz-copy-source</code> header identifies the current version of an object to copy. If the current version is a delete marker, Amazon S3 behaves as if the object was deleted. To copy a different version, use the <code>versionId</code> subresource.</p> <p>If you enable versioning on the target bucket, Amazon S3 generates a unique version ID for the object being copied. This version ID is different from the version ID of the source object. Amazon S3 returns the version ID of the copied object in the <code>x-amz-version-id</code> response header in the response.</p> <p>If you do not enable versioning or suspend it on the target bucket, the version ID that Amazon S3 generates is always null.</p> </dd> </dl> <p>The following operations are related to <code>CopyObject</code>:</p> <ul> <li> <p> <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html\">PutObject</a> </p> </li> <li> <p> <a href=\"https://docs.aws.amazon.com/AmazonS3/latest/API/API_GetObject.html\">GetObject</a> </p> </li> </ul>",
             "documentationUrl": "http://docs.amazonwebservices.com/AmazonS3/latest/API/RESTObjectCOPY.html",
             "errors": [
                 {
                     "shape": "ObjectNotInActiveTierError"
                 }
             ],
             "http": {
@@ -1898,15 +1898,17 @@
                 "eu-west-3",
                 "me-south-1",
                 "sa-east-1",
                 "us-east-2",
                 "us-gov-east-1",
                 "us-gov-west-1",
                 "us-west-1",
-                "us-west-2"
+                "us-west-2",
+                "ap-south-2",
+                "eu-south-2"
             ],
             "type": "string"
         },
         "BucketLoggingStatus": {
             "documentation": "<p>Container for logging status information.</p>",
             "members": {
                 "LoggingEnabled": {
@@ -6505,15 +6507,17 @@
                 "ReplicationStatus",
                 "EncryptionStatus",
                 "ObjectLockRetainUntilDate",
                 "ObjectLockMode",
                 "ObjectLockLegalHoldStatus",
                 "IntelligentTieringAccessTier",
                 "BucketKeyStatus",
-                "ChecksumAlgorithm"
+                "ChecksumAlgorithm",
+                "ObjectAccessControlList",
+                "ObjectOwner"
             ],
             "type": "string"
         },
         "InventoryOptionalFields": {
             "member": {
                 "locationName": "Field",
                 "shape": "InventoryOptionalField"
```

### Comparing `botocore-a-la-carte-s3-1.31.2/botocore/data/s3/2006-03-01/waiters-2.json` & `botocore-a-la-carte-s3-1.31.3/botocore/data/s3/2006-03-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-s3-1.31.2/botocore_a_la_carte_s3.egg-info/PKG-INFO` & `botocore-a-la-carte-s3-1.31.3/botocore_a_la_carte_s3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-s3
-Version: 1.31.2
+Version: 1.31.3
 Summary: s3 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-s3-1.31.2/setup.py` & `botocore-a-la-carte-s3-1.31.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-s3',
-    version="1.31.2",
+    version="1.31.3",
     description='s3 data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/s3/*/*.json'],
```

