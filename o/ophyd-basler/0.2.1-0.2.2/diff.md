# Comparing `tmp/ophyd-basler-0.2.1.tar.gz` & `tmp/ophyd-basler-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ophyd-basler-0.2.1.tar", last modified: Fri Jan 27 04:17:01 2023, max compression
+gzip compressed data, was "ophyd-basler-0.2.2.tar", last modified: Fri Jul 14 14:46:54 2023, max compression
```

## Comparing `ophyd-basler-0.2.1.tar` & `ophyd-basler-0.2.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 04:17:01.528004 ophyd-basler-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-01-27 04:17:01.528004 ophyd-basler-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 04:17:01.524004 ophyd-basler-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 04:17:01.524004 ophyd-basler-0.2.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/docs/source/min_versions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/docs/source/release-history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 04:17:01.528004 ophyd-basler-0.2.1/ophyd_basler/
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/ophyd_basler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-27 04:17:01.528004 ophyd-basler-0.2.1/ophyd_basler/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/ophyd_basler/basler_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/ophyd_basler/basler_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/ophyd_basler/custom_images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 04:17:01.528004 ophyd-basler-0.2.1/ophyd_basler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/ophyd_basler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/ophyd_basler/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/ophyd_basler/tests/test_emulated_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/ophyd_basler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 04:17:01.524004 ophyd-basler-0.2.1/ophyd_basler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-01-27 04:17:01.000000 ophyd-basler-0.2.1/ophyd_basler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-01-27 04:17:01.000000 ophyd-basler-0.2.1/ophyd_basler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 04:17:01.000000 ophyd-basler-0.2.1/ophyd_basler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-01-27 04:17:01.000000 ophyd-basler-0.2.1/ophyd_basler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-27 04:17:01.000000 ophyd-basler-0.2.1/ophyd_basler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-27 04:17:01.528004 ophyd-basler-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68314 2023-01-27 04:16:51.000000 ophyd-basler-0.2.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:46:54.618903 ophyd-basler-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-14 14:46:54.618903 ophyd-basler-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:46:54.614903 ophyd-basler-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:46:54.614903 ophyd-basler-0.2.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/docs/source/min_versions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/docs/source/release-history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:46:54.618903 ophyd-basler-0.2.2/ophyd_basler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/ophyd_basler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 14:46:54.618903 ophyd-basler-0.2.2/ophyd_basler/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/ophyd_basler/basler_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/ophyd_basler/basler_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/ophyd_basler/custom_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:46:54.618903 ophyd-basler-0.2.2/ophyd_basler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/ophyd_basler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/ophyd_basler/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/ophyd_basler/tests/test_emulated_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/ophyd_basler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:46:54.614903 ophyd-basler-0.2.2/ophyd_basler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-14 14:46:54.000000 ophyd-basler-0.2.2/ophyd_basler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-14 14:46:54.000000 ophyd-basler-0.2.2/ophyd_basler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:46:54.000000 ophyd-basler-0.2.2/ophyd_basler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-14 14:46:54.000000 ophyd-basler-0.2.2/ophyd_basler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 14:46:54.000000 ophyd-basler-0.2.2/ophyd_basler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-14 14:46:54.618903 ophyd-basler-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68314 2023-07-14 14:46:42.000000 ophyd-basler-0.2.2/versioneer.py
```

### Comparing `ophyd-basler-0.2.1/CONTRIBUTING.rst` & `ophyd-basler-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ophyd-basler-0.2.1/LICENSE` & `ophyd-basler-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd-basler-0.2.1/PKG-INFO` & `ophyd-basler-0.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ophyd-basler
-Version: 0.2.1
+Version: 0.2.2
 Summary: Basler camera API integration with ophyd
 Home-page: https://github.com/BNL-ATF/ophyd-basler
 Author: Brookhaven National Lab
 Author-email: tmorris@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `ophyd-basler-0.2.1/docs/Makefile` & `ophyd-basler-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ophyd-basler-0.2.1/docs/make.bat` & `ophyd-basler-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ophyd-basler-0.2.1/docs/source/conf.py` & `ophyd-basler-0.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ophyd-basler-0.2.1/docs/source/min_versions.rst` & `ophyd-basler-0.2.2/docs/source/min_versions.rst`

 * *Files identical despite different names*

### Comparing `ophyd-basler-0.2.1/ophyd_basler/__init__.py` & `ophyd-basler-0.2.2/ophyd_basler/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     device_metadata = pd.DataFrame(
         columns=["user_defined_name", "camera_model", "serial_number", "supported_formats"]
     )
 
     devices = []
 
     for device_info in device_info_list:
-
         device = transport_layer_factory.CreateDevice(device_info)
         camera_object = pylon.InstantCamera(device)
         devices.append(camera_object)
 
         user_defined_name = camera_object.GetDeviceInfo().GetUserDefinedName()
         camera_model = camera_object.GetDeviceInfo().GetModelName()
         camera_serial_number = camera_object.GetDeviceInfo().GetSerialNumber()
```

### Comparing `ophyd-basler-0.2.1/ophyd_basler/basler_camera.py` & `ophyd-basler-0.2.2/ophyd_basler/basler_camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 from . import ExternalFileReference
 from .custom_images import save_images
 from .utils import logger_basler as logger
 
 
 class BaslerCamera(Device):
-
     image = Cpt(ExternalFileReference, kind="normal")
     mean = Cpt(Signal, kind="hinted")
     exposure_time = Cpt(Signal, value=1000, kind="config")  # exposure time, in milliseconds
     user_defined_name = Cpt(Signal, kind="config")
     camera_model = Cpt(Signal, kind="config")
     serial_number = Cpt(Signal, kind="config")
     image_shape = Cpt(Signal, kind="config")
@@ -39,14 +38,17 @@
         root_dir="/tmp/basler",
         cam_num=0,
         pixel_format="Mono8",
         trigger_mode="Off",
         verbose=False,
         **kwargs,
     ):
+        """
+        A class to instantiate a Basler ophyd object.
+        """
         super().__init__(*args, **kwargs)
 
         self._root_dir = root_dir
         self._cam_num = cam_num
         self._pixel_format = pixel_format
         self._trigger_mode = trigger_mode
         self._verbose = verbose
@@ -129,45 +131,43 @@
         self.camera_object.PixelFormat = (
             "Mono8"  # choose one pixel format; camera emulation does conversion on the fly
         )
 
         self.camera_object.Close()
 
     def grab_image(self):
-
         self.camera_object.StartGrabbingMax(1)
 
         while self.camera_object.IsGrabbing():
             with self.camera_object.RetrieveResult(
                 self.grab_timeout.get(), pylon.TimeoutHandling_ThrowException
             ) as res:
-
                 if res.GrabSucceeded():
                     image = np.array(res.Array)
                 else:
                     raise Exception("Could not grab image with pylon")
 
         self.camera_object.StopGrabbing()
 
         logger.debug(f"grabbed a frame with the shape {image.shape}")
         logger.debug(f"{np.where(image.max()) = }  |  {image.max() = }")
         return image
 
     def trigger(self):
-
         logger.debug("started trigger")
 
         super().trigger()
         logger.debug("started grabbing")
         image = self.grab_image()
 
-        logger.debug("finisihed grabbing")
+        current_frame = next(self._counter)
+
+        logger.debug(f"finisihed grabbing frame {current_frame}")
         logger.debug(f"original shape: {image.shape}")
 
-        current_frame = next(self._counter)
         self._dataset.resize((current_frame + 1, *self.image_shape.get()))
 
         logger.debug(f"{self._dataset = }\n{self._dataset.shape = }")
 
         self._dataset[current_frame, :, :] = image
 
         datum_document = self._datum_factory(datum_kwargs={"frame": current_frame})
@@ -179,15 +179,14 @@
         super().trigger()
 
         logger.debug("finisihed trigger")
 
         return NullStatus()
 
     def stage(self):
-
         super().stage()
         date = datetime.datetime.now()
         self._assets_dir = date.strftime("%Y/%m/%d")
         data_file = f"{new_uid()}.h5"
 
         self._resource_document, self._datum_factory, _ = compose_resource(
             start={"uid": "needed for compose_resource() but will be discarded"},
@@ -225,15 +224,14 @@
             # This setting makes sure we continue our iteration over the set of
             # predefined images on each trigger.
             self.camera_object.AcquisitionMode.SetValue("SingleFrame")
 
         # Exposure time can't be less than self.camera_object.ExposureTime.Min.
         # We use seconds for ophyd, and microseconds for pylon:
         if not self.camera_object.ExposureTimeAbs == 1e3 * self.exposure_time.get():
-
             if self._verbose:
                 logger.debug(f"Setting exposure time to {self.exposure_time.get()} ms")
 
             min_exposure_us = self.camera_object.ExposureTimeAbs.Min
             max_exposure_us = self.camera_object.ExposureTimeAbs.Max
 
             # If the requested value is less than the minimum exposure time, use the minimum exposure time.
@@ -252,15 +250,14 @@
                     f"the maximum exposure time ({max_exposure_us} us). Proceeding with maximum exposure time."
                 )
 
             else:
                 self.camera_object.ExposureTimeAbs.SetValue(1e3 * self.exposure_time.get())
 
     def unstage(self):
-
         self.camera_object.Close()
         super().unstage()
         del self._dataset
         self._h5file_desc.close()
         self._resource_document = None
         self._datum_factory = None
```

### Comparing `ophyd-basler-0.2.1/ophyd_basler/custom_images.py` & `ophyd-basler-0.2.2/ophyd_basler/custom_images.py`

 * *Files identical despite different names*

### Comparing `ophyd-basler-0.2.1/ophyd_basler/tests/conftest.py` & `ophyd-basler-0.2.2/ophyd_basler/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,22 +19,20 @@
     db.reg.register_handler("BASLER_CAM_HDF5", BaslerCamHDF5Handler, overwrite=True)
 
     return db
 
 
 @pytest.fixture(scope="function")
 def RE(db):
-
     RE = RunEngine({})
     bec = best_effort.BestEffortCallback()
     bec.disable_plots()
     RE.subscribe(bec)
     RE.subscribe(db.insert)
 
     return RE
 
 
 @pytest.fixture(scope="function")
 def make_dirs():
-
     root_dir = "/tmp/basler"
     _ = make_dir_tree(datetime.now().year, base_path=root_dir)
```

### Comparing `ophyd-basler-0.2.1/ophyd_basler/tests/test_emulated_camera.py` & `ophyd-basler-0.2.2/ophyd_basler/tests/test_emulated_camera.py`

 * *Files identical despite different names*

### Comparing `ophyd-basler-0.2.1/ophyd_basler/utils.py` & `ophyd-basler-0.2.2/ophyd_basler/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd-basler-0.2.1/ophyd_basler.egg-info/PKG-INFO` & `ophyd-basler-0.2.2/ophyd_basler.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ophyd-basler
-Version: 0.2.1
+Version: 0.2.2
 Summary: Basler camera API integration with ophyd
 Home-page: https://github.com/BNL-ATF/ophyd-basler
 Author: Brookhaven National Lab
 Author-email: tmorris@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `ophyd-basler-0.2.1/ophyd_basler.egg-info/SOURCES.txt` & `ophyd-basler-0.2.2/ophyd_basler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ophyd-basler-0.2.1/setup.py` & `ophyd-basler-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `ophyd-basler-0.2.1/versioneer.py` & `ophyd-basler-0.2.2/versioneer.py`

 * *Files identical despite different names*

