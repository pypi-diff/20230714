# Comparing `tmp/eyeflow_sdk-1.1.7.tar.gz` & `tmp/eyeflow_sdk-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyeflow_sdk-1.1.7.tar", last modified: Wed Mar 29 19:09:49 2023, max compression
+gzip compressed data, was "eyeflow_sdk-1.1.8.tar", last modified: Fri Jul 14 20:14:36 2023, max compression
```

## Comparing `eyeflow_sdk-1.1.7.tar` & `eyeflow_sdk-1.1.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 alexsobral  (1000) alexsobral  (1000)        0 2023-03-29 19:09:49.728777 eyeflow_sdk-1.1.7/
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)      587 2023-03-29 19:09:49.728777 eyeflow_sdk-1.1.7/PKG-INFO
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)       66 2021-03-18 12:41:25.000000 eyeflow_sdk-1.1.7/README.md
-drwxrwxr-x   0 alexsobral  (1000) alexsobral  (1000)        0 2023-03-29 19:09:49.728777 eyeflow_sdk-1.1.7/eyeflow_sdk/
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)        0 2021-03-18 12:41:25.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/__init__.py
-drwxrwxr-x   0 alexsobral  (1000) alexsobral  (1000)        0 2023-03-29 19:09:49.728777 eyeflow_sdk-1.1.7/eyeflow_sdk/cloud_store/
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)        0 2021-03-18 12:41:25.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/cloud_store/__init__.py
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     5880 2021-04-26 23:09:11.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/cloud_store/azure.py
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     1235 2021-10-05 23:35:05.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/data_augmentation_default_parms.json
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)    11109 2022-07-05 20:26:49.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/dataset_default_parms.json
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     1236 2022-07-05 20:27:11.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/dataset_types.json
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)    14511 2021-11-23 15:53:36.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/dataset_utils.py
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)    33829 2023-02-14 22:09:27.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/edge_client.py
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)      928 2022-03-30 17:25:21.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/eyeflow_conf.yaml
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)    10325 2021-03-18 12:41:25.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/file_access.py
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     8353 2023-03-29 19:08:36.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/img_utils.py
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)      804 2021-03-18 12:41:25.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/jetson_utils.py
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     4378 2022-03-30 17:25:21.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/log_obj.py
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)    12810 2021-03-22 13:22:20.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/message_queue.py
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     4191 2022-05-31 23:08:32.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/metrics.py
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     5312 2021-03-18 12:41:25.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/nv_gpu.py
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     2225 2021-03-18 12:41:25.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/reset_usb.py
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     4680 2022-07-04 20:07:11.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/video_log.py
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     4066 2021-12-22 19:02:25.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/video_play.py
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)    10930 2021-03-18 12:41:25.000000 eyeflow_sdk-1.1.7/eyeflow_sdk/visualization.py
-drwxrwxr-x   0 alexsobral  (1000) alexsobral  (1000)        0 2023-03-29 19:09:49.728777 eyeflow_sdk-1.1.7/eyeflow_sdk.egg-info/
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)      587 2023-03-29 19:09:49.000000 eyeflow_sdk-1.1.7/eyeflow_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)      772 2023-03-29 19:09:49.000000 eyeflow_sdk-1.1.7/eyeflow_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)        1 2023-03-29 19:09:49.000000 eyeflow_sdk-1.1.7/eyeflow_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)      142 2023-03-29 19:09:49.000000 eyeflow_sdk-1.1.7/eyeflow_sdk.egg-info/requires.txt
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)       12 2023-03-29 19:09:49.000000 eyeflow_sdk-1.1.7/eyeflow_sdk.egg-info/top_level.txt
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)       38 2023-03-29 19:09:49.728777 eyeflow_sdk-1.1.7/setup.cfg
--rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     1101 2023-03-29 19:08:53.000000 eyeflow_sdk-1.1.7/setup.py
+drwxrwxr-x   0 alexsobral  (1000) alexsobral  (1000)        0 2023-07-14 20:14:36.923274 eyeflow_sdk-1.1.8/
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)      587 2023-07-14 20:14:36.923274 eyeflow_sdk-1.1.8/PKG-INFO
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)       66 2021-03-18 12:41:25.000000 eyeflow_sdk-1.1.8/README.md
+drwxrwxr-x   0 alexsobral  (1000) alexsobral  (1000)        0 2023-07-14 20:14:36.919274 eyeflow_sdk-1.1.8/eyeflow_sdk/
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)        0 2021-03-18 12:41:25.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/__init__.py
+drwxrwxr-x   0 alexsobral  (1000) alexsobral  (1000)        0 2023-07-14 20:14:36.923274 eyeflow_sdk-1.1.8/eyeflow_sdk/cloud_store/
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)        0 2021-03-18 12:41:25.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/cloud_store/__init__.py
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     5880 2021-04-26 23:09:11.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/cloud_store/azure.py
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     1235 2021-10-05 23:35:05.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/data_augmentation_default_parms.json
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)    10312 2023-03-31 11:57:57.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/dataset_default_parms.json
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     1236 2022-07-05 20:27:11.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/dataset_types.json
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)    14762 2023-07-14 20:12:52.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/dataset_utils.py
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)    33829 2023-02-14 22:09:27.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/edge_client.py
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)      928 2022-03-30 17:25:21.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/eyeflow_conf.yaml
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)    10325 2021-03-18 12:41:25.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/file_access.py
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     8353 2023-03-29 19:08:36.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/img_utils.py
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)      804 2021-03-18 12:41:25.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/jetson_utils.py
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     4378 2022-03-30 17:25:21.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/log_obj.py
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)    12810 2021-03-22 13:22:20.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/message_queue.py
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     4191 2022-05-31 23:08:32.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/metrics.py
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     5312 2021-03-18 12:41:25.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/nv_gpu.py
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     2225 2021-03-18 12:41:25.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/reset_usb.py
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     4680 2022-07-04 20:07:11.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/video_log.py
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     4066 2021-12-22 19:02:25.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/video_play.py
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)    10930 2021-03-18 12:41:25.000000 eyeflow_sdk-1.1.8/eyeflow_sdk/visualization.py
+drwxrwxr-x   0 alexsobral  (1000) alexsobral  (1000)        0 2023-07-14 20:14:36.919274 eyeflow_sdk-1.1.8/eyeflow_sdk.egg-info/
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)      587 2023-07-14 20:14:36.000000 eyeflow_sdk-1.1.8/eyeflow_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)      772 2023-07-14 20:14:36.000000 eyeflow_sdk-1.1.8/eyeflow_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)        1 2023-07-14 20:14:36.000000 eyeflow_sdk-1.1.8/eyeflow_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)      142 2023-07-14 20:14:36.000000 eyeflow_sdk-1.1.8/eyeflow_sdk.egg-info/requires.txt
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)       12 2023-07-14 20:14:36.000000 eyeflow_sdk-1.1.8/eyeflow_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)       38 2023-07-14 20:14:36.923274 eyeflow_sdk-1.1.8/setup.cfg
+-rw-rw-r--   0 alexsobral  (1000) alexsobral  (1000)     1101 2023-07-14 20:13:44.000000 eyeflow_sdk-1.1.8/setup.py
```

### Comparing `eyeflow_sdk-1.1.7/PKG-INFO` & `eyeflow_sdk-1.1.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyeflow_sdk
-Version: 1.1.7
+Version: 1.1.8
 Summary: Functions and classes for development of Eyeflow Applications
 Home-page: https://github.com/siliconlife-ai/eyeflow_sdk-pkg
 Author: SiliconLife.AI
 Author-email: support@siliconlife.ai
 License: UNKNOWN
 Description: # eyeflow_sdk-pkg
         Package for development of Eyeflow applications
```

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk/cloud_store/azure.py` & `eyeflow_sdk-1.1.8/eyeflow_sdk/cloud_store/azure.py`

 * *Files identical despite different names*

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk/data_augmentation_default_parms.json` & `eyeflow_sdk-1.1.8/eyeflow_sdk/data_augmentation_default_parms.json`

 * *Files identical despite different names*

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk/dataset_default_parms.json` & `eyeflow_sdk-1.1.8/eyeflow_sdk/dataset_default_parms.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997543580551393%*

 * *Differences: {"'default_parms'": "{'object_detection': {'train_parms': {'reduce_lr_on_plateau': {'factor': "*

 * *                    "0.5}}, 'dnn_parms': {delete: ['anchor_parms', 'negative_overlap', "*

 * *                    "'positive_overlap']}}, 'object_location': {'train_parms': "*

 * *                    "{'reduce_lr_on_plateau': {'factor': 0.5}}, 'dnn_parms': {'pyramid_levels': "*

 * *                    "{delete: [0]}, 'strides': {delete: [0]}, 'interest_sizes': {0: {insert: [(0, "*

 * *                    "-1)], delete: [0]}, delete: […]*

```diff
@@ -221,51 +221,23 @@
                 "steps_per_epoch": 200,
                 "test_size": 0.1,
                 "val_size": 0.1
             }
         },
         "object_detection": {
             "dnn_parms": {
-                "anchor_parms": {
-                    "ratios": [
-                        0.5,
-                        1,
-                        2
-                    ],
-                    "scales": [
-                        1,
-                        1.2,
-                        1.5
-                    ],
-                    "sizes": [
-                        12,
-                        24,
-                        48,
-                        96,
-                        192
-                    ],
-                    "strides": [
-                        8,
-                        16,
-                        32,
-                        64,
-                        128
-                    ]
-                },
                 "backbone": "vgg7",
                 "component": "objdet_af",
                 "component_id": "6143a1faef5cc63fd4c177b1",
                 "input_shape": {
                     "channels": 1,
                     "max_side": 320,
                     "min_side": 256
                 },
-                "negative_overlap": 0.3,
                 "net_width": 20,
-                "positive_overlap": 0.45,
                 "preprocess_mode": "caffe"
             },
             "train_parms": {
                 "batch_size": 5,
                 "confidence_threshold": 0.6,
                 "early_stopping": {
                     "min_delta": 0,
@@ -282,15 +254,15 @@
                     "amsgrad": false,
                     "beta_1": 0.9,
                     "beta_2": 0.999,
                     "learning_rate": 0.001
                 },
                 "reduce_lr_on_plateau": {
                     "cooldown": 0,
-                    "factor": 0.2,
+                    "factor": 0.5,
                     "min_delta": 0.0001,
                     "min_lr": 1e-06,
                     "mode": "auto",
                     "monitor": "val_loss",
                     "patience": 4
                 },
                 "save_checkpoint": {
@@ -311,40 +283,35 @@
                     "channels": 1,
                     "max_side": 1280,
                     "min_side": 640
                 },
                 "interest_sizes": [
                     [
                         -1,
-                        8
-                    ],
-                    [
-                        8,
                         16
                     ],
                     [
                         16,
                         32
                     ],
                     [
                         32,
                         512
                     ]
                 ],
+                "min_box_area": 0.9,
                 "net_width": 20,
                 "patch_size": 64,
                 "preprocess_mode": "caffe",
                 "pyramid_levels": [
-                    1,
                     2,
                     3,
                     4
                 ],
                 "strides": [
-                    2,
                     4,
                     8,
                     16
                 ]
             },
             "train_parms": {
                 "batch_size": 10,
@@ -363,15 +330,15 @@
                     "amsgrad": false,
                     "beta_1": 0.9,
                     "beta_2": 0.999,
                     "learning_rate": 0.001
                 },
                 "reduce_lr_on_plateau": {
                     "cooldown": 0,
-                    "factor": 0.2,
+                    "factor": 0.5,
                     "min_delta": 0.0001,
                     "min_lr": 1e-06,
                     "mode": "auto",
                     "monitor": "val_loss",
                     "patience": 4
                 },
                 "save_checkpoint": {
```

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk/dataset_types.json` & `eyeflow_sdk-1.1.8/eyeflow_sdk/dataset_types.json`

 * *Files identical despite different names*

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk/dataset_utils.py` & `eyeflow_sdk-1.1.8/eyeflow_sdk/dataset_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,23 +164,30 @@
         self.examples = dataset["annotations"]
         self.update_default_parms()
         log.info(f"Load dataset from database {len(self.examples)} examples")
 
 
     @staticmethod
     def load_file_from_cloud(url):
-        with requests.get(url, stream=True) as r:
-            r.raise_for_status()
-            img = b""
-            for chunk in r.iter_content(chunk_size=8192):
-                # If you have chunk encoded response uncomment 'if' and set chunk_size parameter to None.
-                #if chunk:
-                img += chunk
+        tries = 0
+        while tries < 3:
+            try:
+                with requests.get(url, stream=True) as r:
+                    r.raise_for_status()
+                    img = b""
+                    for chunk in r.iter_content(chunk_size=8192):
+                        # If you have chunk encoded response uncomment 'if' and set chunk_size parameter to None.
+                        #if chunk:
+                        img += chunk
 
-            return img
+                    return img
+            except Exception as excp:
+                tries += 1
+                if tries >= 3:
+                    raise excp
 
 
     def load_image(self, example_img):
         """
         Load image to memory from disk or cloud
         """
         for exp in self.examples:
```

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk/edge_client.py` & `eyeflow_sdk-1.1.8/eyeflow_sdk/edge_client.py`

 * *Files identical despite different names*

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk/eyeflow_conf.yaml` & `eyeflow_sdk-1.1.8/eyeflow_sdk/eyeflow_conf.yaml`

 * *Files identical despite different names*

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk/file_access.py` & `eyeflow_sdk-1.1.8/eyeflow_sdk/file_access.py`

 * *Files identical despite different names*

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk/img_utils.py` & `eyeflow_sdk-1.1.8/eyeflow_sdk/img_utils.py`

 * *Files identical despite different names*

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk/jetson_utils.py` & `eyeflow_sdk-1.1.8/eyeflow_sdk/jetson_utils.py`

 * *Files identical despite different names*

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk/log_obj.py` & `eyeflow_sdk-1.1.8/eyeflow_sdk/log_obj.py`

 * *Files identical despite different names*

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk/message_queue.py` & `eyeflow_sdk-1.1.8/eyeflow_sdk/message_queue.py`

 * *Files identical despite different names*

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk/metrics.py` & `eyeflow_sdk-1.1.8/eyeflow_sdk/metrics.py`

 * *Files identical despite different names*

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk/nv_gpu.py` & `eyeflow_sdk-1.1.8/eyeflow_sdk/nv_gpu.py`

 * *Files identical despite different names*

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk/reset_usb.py` & `eyeflow_sdk-1.1.8/eyeflow_sdk/reset_usb.py`

 * *Files identical despite different names*

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk/video_log.py` & `eyeflow_sdk-1.1.8/eyeflow_sdk/video_log.py`

 * *Files identical despite different names*

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk/video_play.py` & `eyeflow_sdk-1.1.8/eyeflow_sdk/video_play.py`

 * *Files identical despite different names*

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk/visualization.py` & `eyeflow_sdk-1.1.8/eyeflow_sdk/visualization.py`

 * *Files identical despite different names*

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk.egg-info/PKG-INFO` & `eyeflow_sdk-1.1.8/eyeflow_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyeflow-sdk
-Version: 1.1.7
+Version: 1.1.8
 Summary: Functions and classes for development of Eyeflow Applications
 Home-page: https://github.com/siliconlife-ai/eyeflow_sdk-pkg
 Author: SiliconLife.AI
 Author-email: support@siliconlife.ai
 License: UNKNOWN
 Description: # eyeflow_sdk-pkg
         Package for development of Eyeflow applications
```

### Comparing `eyeflow_sdk-1.1.7/eyeflow_sdk.egg-info/SOURCES.txt` & `eyeflow_sdk-1.1.8/eyeflow_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eyeflow_sdk-1.1.7/setup.py` & `eyeflow_sdk-1.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="eyeflow_sdk",
-    version="1.1.7",
+    version="1.1.8",
     author="SiliconLife.AI",
     author_email="support@siliconlife.ai",
     description="Functions and classes for development of Eyeflow Applications",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/siliconlife-ai/eyeflow_sdk-pkg",
     packages=setuptools.find_packages(),
```

