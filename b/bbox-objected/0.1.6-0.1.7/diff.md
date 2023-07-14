# Comparing `tmp/bbox_objected-0.1.6.tar.gz` & `tmp/bbox_objected-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbox_objected-0.1.6.tar", last modified: Fri Jul 14 08:38:00 2023, max compression
+gzip compressed data, was "bbox_objected-0.1.7.tar", last modified: Fri Jul 14 09:19:42 2023, max compression
```

## Comparing `bbox_objected-0.1.6.tar` & `bbox_objected-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1099 2023-03-31 17:02:39.015173 bbox_objected-0.1.6/LICENSE.md
--rw-r--r--   0        0        0     4931 2023-04-01 09:04:33.494896 bbox_objected-0.1.6/README.md
--rw-r--r--   0        0        0      446 2023-03-31 17:02:39.016380 bbox_objected-0.1.6/bbox/__init__.py
--rw-r--r--   0        0        0     3979 2023-03-31 18:05:05.139278 bbox_objected-0.1.6/bbox/bbox_utils.py
--rw-r--r--   0        0        0     1039 2023-03-31 18:05:49.929725 bbox_objected-0.1.6/bbox/cv_utils.py
--rw-r--r--   0        0        0        0 2023-03-31 17:02:39.017168 bbox_objected-0.1.6/bbox/sources/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 17:02:39.017568 bbox_objected-0.1.6/bbox/sources/abs/__init__.py
--rw-r--r--   0        0        0     1383 2023-07-14 08:21:26.453474 bbox_objected-0.1.6/bbox/sources/abs/abs_bbox.py
--rw-r--r--   0        0        0     1460 2023-03-31 17:02:39.032128 bbox_objected-0.1.6/bbox/sources/abs/editor.py
--rw-r--r--   0        0        0     2434 2023-03-31 17:02:39.033369 bbox_objected-0.1.6/bbox/sources/bbox_creator.py
--rw-r--r--   0        0        0     2703 2023-03-31 17:02:39.033983 bbox_objected-0.1.6/bbox/sources/bbox_getter.py
--rw-r--r--   0        0        0     1513 2023-07-14 08:21:26.472371 bbox_objected-0.1.6/bbox/sources/bbox_img.py
--rw-r--r--   0        0        0        0 2023-03-31 17:02:39.034122 bbox_objected-0.1.6/bbox/sources/pywinauto/__init__.py
--rw-r--r--   0        0        0     3290 2023-03-31 17:02:39.035119 bbox_objected-0.1.6/bbox/sources/pywinauto/getter.py
--rw-r--r--   0        0        0      629 2023-03-31 17:02:39.035578 bbox_objected-0.1.6/bbox/sources/pywinauto/pywinauto_bbox.py
--rw-r--r--   0        0        0        0 2023-03-31 17:02:39.036109 bbox_objected-0.1.6/bbox/sources/rel/__init__.py
--rw-r--r--   0        0        0     1281 2023-03-31 17:02:39.036578 bbox_objected-0.1.6/bbox/sources/rel/editor.py
--rw-r--r--   0        0        0     1591 2023-07-14 08:21:26.428842 bbox_objected-0.1.6/bbox/sources/rel/rel_bbox.py
--rw-r--r--   0        0        0      396 2023-03-31 17:02:39.037107 bbox_objected-0.1.6/bbox/types.py
--rw-r--r--   0        0        0      686 2023-07-14 08:38:00.658496 bbox_objected-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5057 1970-01-01 00:00:00.000000 bbox_objected-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-03-31 17:02:39.015173 bbox_objected-0.1.7/LICENSE.md
+-rw-r--r--   0        0        0     4931 2023-04-01 09:04:33.494896 bbox_objected-0.1.7/README.md
+-rw-r--r--   0        0        0      446 2023-03-31 17:02:39.016380 bbox_objected-0.1.7/bbox/__init__.py
+-rw-r--r--   0        0        0     3979 2023-03-31 18:05:05.139278 bbox_objected-0.1.7/bbox/bbox_utils.py
+-rw-r--r--   0        0        0     1039 2023-03-31 18:05:49.929725 bbox_objected-0.1.7/bbox/cv_utils.py
+-rw-r--r--   0        0        0        0 2023-03-31 17:02:39.017168 bbox_objected-0.1.7/bbox/sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-31 17:02:39.017568 bbox_objected-0.1.7/bbox/sources/abs/__init__.py
+-rw-r--r--   0        0        0     1346 2023-07-14 09:18:37.977386 bbox_objected-0.1.7/bbox/sources/abs/abs_bbox.py
+-rw-r--r--   0        0        0     1460 2023-03-31 17:02:39.032128 bbox_objected-0.1.7/bbox/sources/abs/editor.py
+-rw-r--r--   0        0        0     2434 2023-03-31 17:02:39.033369 bbox_objected-0.1.7/bbox/sources/bbox_creator.py
+-rw-r--r--   0        0        0     2703 2023-03-31 17:02:39.033983 bbox_objected-0.1.7/bbox/sources/bbox_getter.py
+-rw-r--r--   0        0        0     1515 2023-07-14 08:44:53.999090 bbox_objected-0.1.7/bbox/sources/bbox_img.py
+-rw-r--r--   0        0        0        0 2023-03-31 17:02:39.034122 bbox_objected-0.1.7/bbox/sources/pywinauto/__init__.py
+-rw-r--r--   0        0        0     3290 2023-03-31 17:02:39.035119 bbox_objected-0.1.7/bbox/sources/pywinauto/getter.py
+-rw-r--r--   0        0        0      629 2023-03-31 17:02:39.035578 bbox_objected-0.1.7/bbox/sources/pywinauto/pywinauto_bbox.py
+-rw-r--r--   0        0        0        0 2023-03-31 17:02:39.036109 bbox_objected-0.1.7/bbox/sources/rel/__init__.py
+-rw-r--r--   0        0        0     1281 2023-03-31 17:02:39.036578 bbox_objected-0.1.7/bbox/sources/rel/editor.py
+-rw-r--r--   0        0        0     1556 2023-07-14 09:19:09.082778 bbox_objected-0.1.7/bbox/sources/rel/rel_bbox.py
+-rw-r--r--   0        0        0      396 2023-03-31 17:02:39.037107 bbox_objected-0.1.7/bbox/types.py
+-rw-r--r--   0        0        0      686 2023-07-14 09:19:42.270830 bbox_objected-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5057 1970-01-01 00:00:00.000000 bbox_objected-0.1.7/PKG-INFO
```

### Comparing `bbox_objected-0.1.6/LICENSE.md` & `bbox_objected-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bbox_objected-0.1.6/README.md` & `bbox_objected-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `bbox_objected-0.1.6/bbox/bbox_utils.py` & `bbox_objected-0.1.7/bbox/bbox_utils.py`

 * *Files identical despite different names*

### Comparing `bbox_objected-0.1.6/bbox/cv_utils.py` & `bbox_objected-0.1.7/bbox/cv_utils.py`

 * *Files identical despite different names*

### Comparing `bbox_objected-0.1.6/bbox/sources/abs/abs_bbox.py` & `bbox_objected-0.1.7/bbox/sources/abs/abs_bbox.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     ):
         super().__init__(coords, kind)
         self.is_valid()
         self.text = text
         self.__dict__.update(kwargs)
 
     def crop_from(self, img):
-        return img[self.y1 : self.y2+1, self.x1 : self.x2+1]  # +1 to include all borders
+        return img[self.y1: self.y2, self.x1: self.x2]
 
     def is_valid(self):
         comment = "Use only int coords"
         return (
             isinstance(self.x1, int)
             and isinstance(self.y1, int)
             and isinstance(self.x2, int)
@@ -42,8 +42,7 @@
         return RelBBox((x1, y1, x2, y2), text=self.text)
 
     def __repr__(self):
         bbox = f"AbsBBox(x1={self.x1}, y1={self.y1}, x2={self.x2}, y2={self.y2})"
         if text := self.text:
             text = f" - {self.text}"
         return f"<{bbox}{text}>"
-
```

### Comparing `bbox_objected-0.1.6/bbox/sources/abs/editor.py` & `bbox_objected-0.1.7/bbox/sources/abs/editor.py`

 * *Files identical despite different names*

### Comparing `bbox_objected-0.1.6/bbox/sources/bbox_creator.py` & `bbox_objected-0.1.7/bbox/sources/bbox_creator.py`

 * *Files identical despite different names*

### Comparing `bbox_objected-0.1.6/bbox/sources/bbox_getter.py` & `bbox_objected-0.1.7/bbox/sources/bbox_getter.py`

 * *Files identical despite different names*

### Comparing `bbox_objected-0.1.6/bbox/sources/bbox_img.py` & `bbox_objected-0.1.7/bbox/sources/bbox_img.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -46,8 +46,8 @@
                 0.5,
                 (0, 0, 255),
                 2,
             )
 
         cv2.imshow("temp", resize(img, height=800))
         cv2.waitKey(0)
-        cv2.destroyWindow("temp")
+        cv2.destroyWindow("temp")
```

### Comparing `bbox_objected-0.1.6/bbox/sources/pywinauto/getter.py` & `bbox_objected-0.1.7/bbox/sources/pywinauto/getter.py`

 * *Files identical despite different names*

### Comparing `bbox_objected-0.1.6/bbox/sources/pywinauto/pywinauto_bbox.py` & `bbox_objected-0.1.7/bbox/sources/pywinauto/pywinauto_bbox.py`

 * *Files identical despite different names*

### Comparing `bbox_objected-0.1.6/bbox/sources/rel/editor.py` & `bbox_objected-0.1.7/bbox/sources/rel/editor.py`

 * *Files identical despite different names*

### Comparing `bbox_objected-0.1.6/bbox/sources/rel/rel_bbox.py` & `bbox_objected-0.1.7/bbox/sources/rel/rel_bbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,21 @@
     ):
         super().__init__(coords, kind)
         self.is_valid()
         self.text = text
         self.__dict__.update(kwargs)
 
     def crop_from(self, img):
-
         h, w, *c = img.shape
         x1 = round(self.x1 * w)
         x2 = round(self.x2 * w)
         y1 = round(self.y1 * h)
         y2 = round(self.y2 * h)
 
-        return img[y1:y2+1, x1:x2+1]  # +1 to include all borders
+        return img[y1:y2, x1:x2]
 
     def is_valid(self):
         comment = "Use only float coords in range [0, 1]"
         assert (
             (0.0 <= self.x1 <= 1.0)
             and (0.0 <= self.y1 <= 1.0)
             and (0.0 <= self.x2 <= 1.0)
```

### Comparing `bbox_objected-0.1.6/pyproject.toml` & `bbox_objected-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "pyupgrade>=3.3.1",
     "black>=23.3.0",
     "pre-commit>=3.2.1",
 ]
 
 [project]
 name = "bbox_objected"
-version = "0.1.6"
+version = "0.1.7"
 description = "Manipulate bounding boxes as objects"
 authors = [
     { name = "SEBROVATER", email = "sebrovskiy.k@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.10"
 readme = "README.md"
```

### Comparing `bbox_objected-0.1.6/PKG-INFO` & `bbox_objected-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbox_objected
-Version: 0.1.6
+Version: 0.1.7
 Summary: Manipulate bounding boxes as objects
 Author-Email: SEBROVATER <sebrovskiy.k@gmail.com>
 License: MIT
 Project-URL: Github, https://github.com/SEBROVATER/bbox_objected
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

