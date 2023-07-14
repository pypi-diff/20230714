# Comparing `tmp/pydantic_xmlmodel-0.3.2.tar.gz` & `tmp/pydantic_xmlmodel-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_xmlmodel-0.3.2.tar", max compression
+gzip compressed data, was "pydantic_xmlmodel-0.3.3.tar", max compression
```

## Comparing `pydantic_xmlmodel-0.3.2.tar` & `pydantic_xmlmodel-0.3.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-05-17 13:32:22.273043 pydantic_xmlmodel-0.3.2/LICENSE
--rw-r--r--   0        0        0     2190 2023-06-15 14:01:43.476858 pydantic_xmlmodel-0.3.2/README.md
--rw-r--r--   0        0        0       55 2023-05-17 13:44:08.514440 pydantic_xmlmodel-0.3.2/pydantic_xmlmodel/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 08:52:39.775359 pydantic_xmlmodel-0.3.2/pydantic_xmlmodel/py.typed
--rw-r--r--   0        0        0    14980 2023-06-17 20:27:41.893387 pydantic_xmlmodel-0.3.2/pydantic_xmlmodel/xmlmodel.py
--rw-r--r--   0        0        0      613 2023-06-17 20:28:05.134691 pydantic_xmlmodel-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2934 1970-01-01 00:00:00.000000 pydantic_xmlmodel-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-17 13:32:22.273043 pydantic_xmlmodel-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2190 2023-06-15 14:01:43.476858 pydantic_xmlmodel-0.3.3/README.md
+-rw-r--r--   0        0        0       55 2023-05-17 13:44:08.514440 pydantic_xmlmodel-0.3.3/pydantic_xmlmodel/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:52:39.775359 pydantic_xmlmodel-0.3.3/pydantic_xmlmodel/py.typed
+-rw-r--r--   0        0        0    15113 2023-07-14 18:17:36.791473 pydantic_xmlmodel-0.3.3/pydantic_xmlmodel/xmlmodel.py
+-rw-r--r--   0        0        0      613 2023-07-14 18:16:44.722854 pydantic_xmlmodel-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2934 1970-01-01 00:00:00.000000 pydantic_xmlmodel-0.3.3/PKG-INFO
```

### Comparing `pydantic_xmlmodel-0.3.2/LICENSE` & `pydantic_xmlmodel-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_xmlmodel-0.3.2/README.md` & `pydantic_xmlmodel-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_xmlmodel-0.3.2/pydantic_xmlmodel/xmlmodel.py` & `pydantic_xmlmodel-0.3.3/pydantic_xmlmodel/xmlmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
     It's a subclass of `ModelMetaclass` (the metaclass of `pydantic.BaseModel`).
 
     It adds the following class attributes to XMLModel:
         - `__xml_name__`: The name of the XML element. If not specified, the name of the class is used.
     """
 
+    @no_type_check
     def __new__(cls, name, bases, attrs, **kwargs):
         """Add the following class attributes to XMLModel.
 
         - xml_name: The name of the XML element. If not specified, the name of the class is used.
         """
         xml_name = kwargs.pop("xml_name", None)
         if xml_name is not None:
@@ -87,15 +88,18 @@
             return cls.__xml_name__
         else:
             if cls.__xml_name_function__ is not None:
                 return cls.__xml_name_function__(cls.__name__)
             return cls.__name__
 
     def to_xml(
-        self, indent: Optional[int] = None, include_xml_version: bool = True
+        self,
+        indent: Optional[int] = None,
+        include_xml_version: bool = True,
+        exclude_none=False,
     ) -> str:
         """Convert the model to XML string.
 
         Args:
             indent: If specified, the XML will be indented with the specified number of spaces.
 
         Returns:
@@ -167,16 +171,17 @@
                 else:
                     # Get the name of the XML attribute
                     pydantic_field = obj.__fields__[field]
                     # If the field has an alias, we use it as the name of the XML attribute
                     name = pydantic_field.name
                     if pydantic_field.alias is not None:
                         name = pydantic_field.alias
-                    # Add the attribute to the XML element
-                    e.set(name, str(value))
+                    if not (exclude_none and value is None):
+                        # Add the attribute to the XML element
+                        e.set(name, str(value))
             # If the model has content, we add it to the XML element
             if isinstance(obj, XMLModel) and obj.xml_content is not None:
                 xml_content_field = obj.__fields__["xml_content"]
                 # if field is a list-like field but not a list of BaseModel, we raise an error
                 if xml_content_field.sub_fields is not None and not _issubclass_safe(
                     xml_content_field.sub_fields[0].type_, BaseModel
                 ):
```

### Comparing `pydantic_xmlmodel-0.3.2/pyproject.toml` & `pydantic_xmlmodel-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-xmlmodel"
-version = "0.3.2"
+version = "0.3.3"
 description = "PydanticXML is a Python library that provides a way to convert Pydantic models to XML and vice versa."
 authors = ["cofob <cofob@riseup.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cofob/pydanticxml"
 homepage = "https://github.com/cofob/pydanticxml"
```

### Comparing `pydantic_xmlmodel-0.3.2/PKG-INFO` & `pydantic_xmlmodel-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-xmlmodel
-Version: 0.3.2
+Version: 0.3.3
 Summary: PydanticXML is a Python library that provides a way to convert Pydantic models to XML and vice versa.
 Home-page: https://github.com/cofob/pydanticxml
 License: MIT
 Author: cofob
 Author-email: cofob@riseup.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

