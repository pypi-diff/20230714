# Comparing `tmp/gundi_core-1.1.1.tar.gz` & `tmp/gundi_core-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gundi_core-1.1.1.tar", max compression
+gzip compressed data, was "gundi_core-1.2.0.tar", max compression
```

## Comparing `gundi_core-1.1.1.tar` & `gundi_core-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       40 2023-06-14 17:07:47.722189 gundi_core-1.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-14 20:35:09.913772 gundi_core-1.1.1/gundi_core/__init__.py
--rw-r--r--   0        0        0       47 2023-07-07 19:55:59.544656 gundi_core-1.1.1/gundi_core/events/__init__.py
--rw-r--r--   0        0        0     1019 2023-07-10 15:33:44.398106 gundi_core-1.1.1/gundi_core/events/core.py
--rw-r--r--   0        0        0      308 2023-07-07 18:45:50.769675 gundi_core-1.1.1/gundi_core/events/dispatchers.py
--rw-r--r--   0        0        0      114 2023-06-14 18:33:55.875739 gundi_core-1.1.1/gundi_core/schemas/__init__.py
--rw-r--r--   0        0        0    13847 2023-06-14 19:41:05.310697 gundi_core-1.1.1/gundi_core/schemas/v1.py
--rw-r--r--   0        0        0    12868 2023-07-07 18:59:33.435753 gundi_core-1.1.1/gundi_core/schemas/v2.py
--rw-r--r--   0        0        0      329 2023-07-10 15:32:04.662070 gundi_core-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 gundi_core-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0       40 2023-06-14 17:07:47.722189 gundi_core-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 20:35:09.913772 gundi_core-1.2.0/gundi_core/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-07 19:55:59.544656 gundi_core-1.2.0/gundi_core/events/__init__.py
+-rw-r--r--   0        0        0     1019 2023-07-10 15:33:44.398106 gundi_core-1.2.0/gundi_core/events/core.py
+-rw-r--r--   0        0        0      308 2023-07-07 18:45:50.769675 gundi_core-1.2.0/gundi_core/events/dispatchers.py
+-rw-r--r--   0        0        0      114 2023-06-14 18:33:55.875739 gundi_core-1.2.0/gundi_core/schemas/__init__.py
+-rw-r--r--   0        0        0    13847 2023-06-14 19:41:05.310697 gundi_core-1.2.0/gundi_core/schemas/v1.py
+-rw-r--r--   0        0        0    14678 2023-07-14 12:24:28.304354 gundi_core-1.2.0/gundi_core/schemas/v2.py
+-rw-r--r--   0        0        0      329 2023-07-14 12:15:33.494447 gundi_core-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 gundi_core-1.2.0/PKG-INFO
```

### Comparing `gundi_core-1.1.1/gundi_core/events/core.py` & `gundi_core-1.2.0/gundi_core/events/core.py`

 * *Files identical despite different names*

### Comparing `gundi_core-1.1.1/gundi_core/schemas/v1.py` & `gundi_core-1.2.0/gundi_core/schemas/v1.py`

 * *Files identical despite different names*

### Comparing `gundi_core-1.1.1/gundi_core/schemas/v2.py` & `gundi_core-1.2.0/gundi_core/schemas/v2.py`

 * *Files 12% similar despite different names*

```diff
@@ -372,14 +372,66 @@
     event_type: Optional[str] = Field(
         "",
         example="animal_sighting",
         description="Event type to be applied to event sent to Earth Ranger (Optional).",
     )
 
 
+class GundiTrace(BaseModel):
+    object_id: Union[UUID, str] = Field(
+        None,
+        title="Gundi ID",
+        description="A unique object ID generated by gundi.",
+    )
+    object_type: Optional[str] = Field(
+        "",
+        title="Object type",
+        example="ev",
+        description="Steam type such as event, observation, etc.",
+    )
+    related_to: Optional[Union[UUID, str]] = Field(
+        None,
+        title="Related Object ID",
+        description="The Gundi ID of the related object",
+    )
+    data_provider: Optional[Union[UUID, str]] = Field(
+        None,
+        title="Provider ID",
+        description="The unique ID of the Integration providing the data.",
+    )
+    destination: Optional[Union[UUID, str]] = Field(
+        None,
+        title="Destination ID",
+        description="The unique ID of the Integration with the destination system.",
+    )
+    delivered_at: Optional[datetime] = Field(
+        ...,
+        title="ISO Timestamp",
+        description="The date and time when the observation was sent to the destination system.",
+        example="2023-06-23T12:01:02-0700",
+    )
+    external_id: Optional[Union[UUID, str]] = Field(
+        None,
+        example="901870234",
+        description="The ID provided by the external system after sending the observation",
+    )
+    created_at: Optional[datetime] = Field(
+        ...,
+        title="ISO Timestamp",
+        description="The date and time when the trace of the observation was recorded in the portal db.",
+        example="2023-06-23T12:01:02-0700",
+    )
+    updated_at: Optional[datetime] = Field(
+        ...,
+        title="ISO Timestamp",
+        description="The date and time when the trace of the observation was updated in the portal db.",
+        example="2023-06-23T12:01:02-0700",
+    )
+
+
 # Models used by the Dispatchers
 class DispatchedObservation(BaseModel):
     gundi_id: Union[UUID, str] = Field(
         None,
         title="Gundi ID",
         description="A unique object ID generated by gundi.",
     )
```

### Comparing `gundi_core-1.1.1/PKG-INFO` & `gundi_core-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gundi-core
-Version: 1.1.1
+Version: 1.2.0
 Summary: 
 Author: Mariano M
 Author-email: marianom@earthranger.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```
