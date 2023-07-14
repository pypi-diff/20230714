# Comparing `tmp/formkit_ninja-0.3.4.tar.gz` & `tmp/formkit_ninja-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formkit_ninja-0.3.4.tar", max compression
+gzip compressed data, was "formkit_ninja-0.3.5.tar", max compression
```

## Comparing `formkit_ninja-0.3.4.tar` & `formkit_ninja-0.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      813 2023-04-06 13:15:44.220033 formkit_ninja-0.3.4/README.md
--rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.3.4/formkit_ninja/__init__.py
--rw-r--r--   0        0        0       21 2023-04-06 13:15:44.224033 formkit_ninja-0.3.4/formkit_ninja/__main__.py
--rw-r--r--   0        0        0    14860 2023-05-09 05:40:10.838963 formkit_ninja-0.3.4/formkit_ninja/admin.py
--rw-r--r--   0        0        0     2568 2023-05-09 05:38:40.651974 formkit_ninja-0.3.4/formkit_ninja/api.py
--rw-r--r--   0        0        0     4333 2023-04-10 00:27:28.783846 formkit_ninja-0.3.4/formkit_ninja/fields.py
--rw-r--r--   0        0        0    13644 2023-06-22 13:58:55.603624 formkit_ninja-0.3.4/formkit_ninja/formkit_schema.py
--rw-r--r--   0        0        0        0 2023-04-23 01:43:59.588049 formkit_ninja-0.3.4/formkit_ninja/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.3.4/formkit_ninja/management/commands/__init__.py
--rw-r--r--   0        0        0     3807 2023-05-09 05:37:21.012799 formkit_ninja-0.3.4/formkit_ninja/management/commands/common_nodes.py
--rw-r--r--   0        0        0    19033 2023-05-09 05:17:09.351553 formkit_ninja-0.3.4/formkit_ninja/management/commands/create_sf11_form.py
--rw-r--r--   0        0        0     3190 2023-04-26 06:36:11.021575 formkit_ninja-0.3.4/formkit_ninja/management/commands/create_sf12_form.py
--rw-r--r--   0        0        0     1360 2023-04-26 06:10:12.411087 formkit_ninja-0.3.4/formkit_ninja/management/commands/create_sf13_form.py
--rw-r--r--   0        0        0    15059 2023-05-09 05:38:40.671974 formkit_ninja-0.3.4/formkit_ninja/migrations/0001_initial.py
--rw-r--r--   0        0        0      605 2023-05-09 05:15:03.707613 formkit_ninja-0.3.4/formkit_ninja/migrations/0002_alter_formcomponents_label_alter_formkitschema_key.py
--rw-r--r--   0        0        0      339 2023-05-09 05:37:27.484727 formkit_ninja-0.3.4/formkit_ninja/migrations/0003_delete_translatable.py
--rw-r--r--   0        0        0        0 2023-04-13 11:58:36.247052 formkit_ninja-0.3.4/formkit_ninja/migrations/__init__.py
--rw-r--r--   0        0        0     9588 2023-05-09 05:38:40.647974 formkit_ninja-0.3.4/formkit_ninja/models.py
--rw-r--r--   0        0        0      101 2023-04-06 13:15:44.224033 formkit_ninja-0.3.4/formkit_ninja/urls.py
--rw-r--r--   0        0        0     1199 2023-06-22 13:59:00.359823 formkit_ninja-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1572 1970-01-01 00:00:00.000000 formkit_ninja-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      813 2023-04-06 13:15:44.220033 formkit_ninja-0.3.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.3.5/formkit_ninja/__init__.py
+-rw-r--r--   0        0        0       21 2023-04-06 13:15:44.224033 formkit_ninja-0.3.5/formkit_ninja/__main__.py
+-rw-r--r--   0        0        0    14860 2023-05-09 05:40:10.838963 formkit_ninja-0.3.5/formkit_ninja/admin.py
+-rw-r--r--   0        0        0     2568 2023-05-09 05:38:40.651974 formkit_ninja-0.3.5/formkit_ninja/api.py
+-rw-r--r--   0        0        0     4333 2023-04-10 00:27:28.783846 formkit_ninja-0.3.5/formkit_ninja/fields.py
+-rw-r--r--   0        0        0    14103 2023-07-14 02:28:58.188490 formkit_ninja-0.3.5/formkit_ninja/formkit_schema.py
+-rw-r--r--   0        0        0        0 2023-04-23 01:43:59.588049 formkit_ninja-0.3.5/formkit_ninja/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.3.5/formkit_ninja/management/commands/__init__.py
+-rw-r--r--   0        0        0     3807 2023-05-09 05:37:21.012799 formkit_ninja-0.3.5/formkit_ninja/management/commands/common_nodes.py
+-rw-r--r--   0        0        0    19033 2023-05-09 05:17:09.351553 formkit_ninja-0.3.5/formkit_ninja/management/commands/create_sf11_form.py
+-rw-r--r--   0        0        0     3190 2023-04-26 06:36:11.021575 formkit_ninja-0.3.5/formkit_ninja/management/commands/create_sf12_form.py
+-rw-r--r--   0        0        0     1360 2023-04-26 06:10:12.411087 formkit_ninja-0.3.5/formkit_ninja/management/commands/create_sf13_form.py
+-rw-r--r--   0        0        0    15059 2023-05-09 05:38:40.671974 formkit_ninja-0.3.5/formkit_ninja/migrations/0001_initial.py
+-rw-r--r--   0        0        0      605 2023-05-09 05:15:03.707613 formkit_ninja-0.3.5/formkit_ninja/migrations/0002_alter_formcomponents_label_alter_formkitschema_key.py
+-rw-r--r--   0        0        0      339 2023-05-09 05:37:27.484727 formkit_ninja-0.3.5/formkit_ninja/migrations/0003_delete_translatable.py
+-rw-r--r--   0        0        0        0 2023-04-13 11:58:36.247052 formkit_ninja-0.3.5/formkit_ninja/migrations/__init__.py
+-rw-r--r--   0        0        0     9588 2023-05-09 05:38:40.647974 formkit_ninja-0.3.5/formkit_ninja/models.py
+-rw-r--r--   0        0        0      101 2023-04-06 13:15:44.224033 formkit_ninja-0.3.5/formkit_ninja/urls.py
+-rw-r--r--   0        0        0     1199 2023-07-14 02:29:38.161397 formkit_ninja-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1572 1970-01-01 00:00:00.000000 formkit_ninja-0.3.5/PKG-INFO
```

### Comparing `formkit_ninja-0.3.4/README.md` & `formkit_ninja-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.4/formkit_ninja/admin.py` & `formkit_ninja-0.3.5/formkit_ninja/admin.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.4/formkit_ninja/api.py` & `formkit_ninja-0.3.5/formkit_ninja/api.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.4/formkit_ninja/fields.py` & `formkit_ninja-0.3.5/formkit_ninja/fields.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.4/formkit_ninja/formkit_schema.py` & `formkit_ninja-0.3.5/formkit_ninja/formkit_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     """
 
     # "ForwardRefs" do not work well with django-ninja.
     # This would ideally be:
     # children: str | list[FormKitSchemaProps] | FormKitSchemaCondition | None = Field(
     #     default_factory=list
     # )
-    children: str | list[FormKitSchemaProps] | FormKitSchemaConditionNoCircularRefs | None = Field()
+    children: str | list[FormKitSchemaProps | str] | FormKitSchemaConditionNoCircularRefs | None = Field()
     key: str | None
     if_condition: str | None = Field(alias="if")
     for_loop: FormKitListStatement | None = Field(alias="for")
     bind: str | None
     meta: FormKitSchemaMeta | None
 
     # These are not formal parts of spec, but
@@ -143,14 +143,20 @@
 
 class DateNode(FormKitSchemaProps):
     node_type: Literal["formkit"] = "formkit"
     formkit: Literal["date"] = "date"
     dollar_formkit: str = Field(default="date", alias="$formkit")
 
 
+class CurrencyNode(FormKitSchemaProps):
+    node_type: Literal["formkit"] = "formkit"
+    formkit: Literal["currency"] = "currency"
+    dollar_formkit: str = Field(default="currency", alias="$formkit")
+
+
 class DatePickerNode(FormKitSchemaProps):
     node_type: Literal["formkit"] = "formkit"
     formkit: Literal["datepicker"] = "datepicker"
     dollar_formkit: str = Field(default="datepicker", alias="$formkit")
     calendarIcon: str = "calendar"
     format: str = 'DD/MM/YY'
     nextIcon: str = 'angleRight'
@@ -197,14 +203,20 @@
 
 class EmailNode(FormKitSchemaProps):
     node_type: Literal["formkit"] = "formkit"
     formkit: Literal["email"] = "email"
     dollar_formkit: str = Field(default="email", alias="$formkit")
 
 
+class TelNode(FormKitSchemaProps):
+    node_type: Literal["formkit"] = "formkit"
+    formkit: Literal["tel"] = "tel"
+    dollar_formkit: str = Field(default="tel", alias="$formkit")
+
+
 class DropDownNode(FormKitSchemaProps):
     node_type: Literal["formkit"] = "formkit"
     formkit: Literal["dropdown"] = "dropdown"
     dollar_formkit: str = Field(default="dropdown", alias="$formkit")
     options: str | list[dict[str, Any]] | list[str] | dict[str, str] | None = Field(None)
     empty_message: str | None = Field(None, alias="empty-message")
     select_icon: str | None = Field(None, alias="selectIcon")
@@ -238,14 +250,16 @@
         NumberNode,
         RadioNode,
         GroupNode,
         DateNode,
         DatePickerNode,
         DropDownNode,
         RepeaterNode,
+        TelNode,
+        CurrencyNode
     ],
     Field(discriminator="formkit"),
 ]
 
 
 class FormKitSchemaDOMNode(FormKitSchemaProps):
     """
@@ -352,14 +366,16 @@
         FormKitSchemaCondition,
     ],
     Field(discriminator="node_type"),
 ]
 
 NODE_TYPE = Literal["condition", "formkit", "element", "component"]
 FORMKIT_TYPE = Literal[
+    "tel",
+    "currency",
     "select",
     "checkbox",
     "number",
     "group",
     "list",
     "password",
     "button",
```

### Comparing `formkit_ninja-0.3.4/formkit_ninja/management/commands/common_nodes.py` & `formkit_ninja-0.3.5/formkit_ninja/management/commands/common_nodes.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.4/formkit_ninja/management/commands/create_sf11_form.py` & `formkit_ninja-0.3.5/formkit_ninja/management/commands/create_sf11_form.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.4/formkit_ninja/management/commands/create_sf12_form.py` & `formkit_ninja-0.3.5/formkit_ninja/management/commands/create_sf12_form.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.4/formkit_ninja/management/commands/create_sf13_form.py` & `formkit_ninja-0.3.5/formkit_ninja/management/commands/create_sf13_form.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.4/formkit_ninja/migrations/0001_initial.py` & `formkit_ninja-0.3.5/formkit_ninja/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.4/formkit_ninja/migrations/0002_alter_formcomponents_label_alter_formkitschema_key.py` & `formkit_ninja-0.3.5/formkit_ninja/migrations/0002_alter_formcomponents_label_alter_formkitschema_key.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.4/formkit_ninja/models.py` & `formkit_ninja-0.3.5/formkit_ninja/models.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.4/pyproject.toml` & `formkit_ninja-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "formkit-ninja"
-version = "0.3.4"
+version = "0.3.5"
 description = "A Django-Ninja backend to specify FormKit schemas"
 authors = ["Josh Brooks <josh@catalpa.io>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/catalpainternational/formkit-ninja"
 repository = "https://github.com/catalpainternational/formkit-ninja"
 packages = [{include = "formkit_ninja"}]
```

### Comparing `formkit_ninja-0.3.4/PKG-INFO` & `formkit_ninja-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formkit-ninja
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Django-Ninja backend to specify FormKit schemas
 Home-page: https://github.com/catalpainternational/formkit-ninja
 License: GPLv3
 Author: Josh Brooks
 Author-email: josh@catalpa.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

