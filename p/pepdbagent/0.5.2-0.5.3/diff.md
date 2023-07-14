# Comparing `tmp/pepdbagent-0.5.2.tar.gz` & `tmp/pepdbagent-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepdbagent-0.5.2.tar", last modified: Thu Jul 13 16:11:43 2023, max compression
+gzip compressed data, was "pepdbagent-0.5.3.tar", last modified: Fri Jul 14 00:39:13 2023, max compression
```

## Comparing `pepdbagent-0.5.2.tar` & `pepdbagent-0.5.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:11:43.132439 pepdbagent-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-13 16:11:43.132439 pepdbagent-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:11:43.128439 pepdbagent-0.5.2/pepdbagent/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:11:43.132439 pepdbagent-0.5.2/pepdbagent/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/modules/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/modules/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    21637 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/modules/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/pepdbagent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pepdbagent/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:11:43.132439 pepdbagent-0.5.2/pepdbagent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-13 16:11:43.000000 pepdbagent-0.5.2/pepdbagent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-13 16:11:43.000000 pepdbagent-0.5.2/pepdbagent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:11:43.000000 pepdbagent-0.5.2/pepdbagent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-13 16:11:43.000000 pepdbagent-0.5.2/pepdbagent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 16:11:43.000000 pepdbagent-0.5.2/pepdbagent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:11:43.132439 pepdbagent-0.5.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:11:43.132439 pepdbagent-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:11:43.132439 pepdbagent-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13817 2023-07-13 16:11:32.000000 pepdbagent-0.5.2/tests/test_pepagent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:39:13.353765 pepdbagent-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-14 00:39:13.353765 pepdbagent-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:39:13.349764 pepdbagent-0.5.3/pepdbagent/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:39:13.353765 pepdbagent-0.5.3/pepdbagent/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/modules/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/modules/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22623 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/modules/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/pepdbagent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pepdbagent/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:39:13.353765 pepdbagent-0.5.3/pepdbagent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-14 00:39:13.000000 pepdbagent-0.5.3/pepdbagent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-14 00:39:13.000000 pepdbagent-0.5.3/pepdbagent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 00:39:13.000000 pepdbagent-0.5.3/pepdbagent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-14 00:39:13.000000 pepdbagent-0.5.3/pepdbagent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 00:39:13.000000 pepdbagent-0.5.3/pepdbagent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:39:13.353765 pepdbagent-0.5.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 00:39:13.353765 pepdbagent-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:39:13.353765 pepdbagent-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-14 00:39:01.000000 pepdbagent-0.5.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13817 2023-07-14 00:39:02.000000 pepdbagent-0.5.3/tests/test_pepagent.py
```

### Comparing `pepdbagent-0.5.2/LICENSE.txt` & `pepdbagent-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.2/PKG-INFO` & `pepdbagent-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepdbagent
-Version: 0.5.2
+Version: 0.5.3
 Summary: A python-based project metadata manager for portable encapsulated projects
 Home-page: https://github.com/pepkit/pepdbagent/
 Author: Oleksandr Khoroshevskyi
 License: BSD2
 Keywords: project,metadata,bioinformatics,database
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pepdbagent-0.5.2/README.md` & `pepdbagent-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.2/pepdbagent/db_utils.py` & `pepdbagent-0.5.3/pepdbagent/db_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,19 +59,16 @@
     """
     if tables:
         _LOGGER.info("A table was created")
     else:
         _LOGGER.info("A table was not created")
 
 
-def deliver_description(context):
-    try:
-        return context.get_current_parameters()["config"]["description"]
-    except KeyError:
-        return ""
+# def deliver_description(context):
+#     return context.get_current_parameters()["config"]["description"]
 
 
 def deliver_update_date(context):
     return datetime.datetime.now(datetime.timezone.utc)
 
 
 class Projects(Base):
@@ -82,23 +79,21 @@
     __tablename__ = "projects"
 
     id: Mapped[int] = mapped_column(primary_key=True)
     namespace: Mapped[str] = mapped_column()
     name: Mapped[str] = mapped_column()
     tag: Mapped[str] = mapped_column()
     digest: Mapped[str] = mapped_column(String(32))
-    description: Mapped[Optional[str]] = mapped_column(
-        default=deliver_description, onupdate=deliver_description
-    )
+    description: Mapped[Optional[str]]
     config: Mapped[dict] = mapped_column(JSON, server_default=FetchedValue())
     private: Mapped[bool]
     number_of_samples: Mapped[int]
     submission_date: Mapped[datetime.datetime]
     last_update_date: Mapped[Optional[datetime.datetime]] = mapped_column(
-        onupdate=deliver_update_date,
+        onupdate=deliver_update_date, default=deliver_update_date
     )
     pep_schema: Mapped[Optional[str]]
     samples_mapping: Mapped[List["Samples"]] = relationship(
         back_populates="sample_mapping", cascade="all, delete-orphan"
     )
     subsamples_mapping: Mapped[List["Subsamples"]] = relationship(
         back_populates="subsample_mapping", cascade="all, delete-orphan"
```

### Comparing `pepdbagent-0.5.2/pepdbagent/exceptions.py` & `pepdbagent-0.5.3/pepdbagent/exceptions.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.2/pepdbagent/models.py` & `pepdbagent-0.5.3/pepdbagent/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     tag: Optional[str]
     is_private: Optional[bool]
     pep_schema: Optional[str]
     digest: Optional[str]
     config: Optional[dict]
     samples: Optional[List[dict]]
     subsamples: Optional[List[List[dict]]]
+    description: Optional[str]
 
     class Config:
         arbitrary_types_allowed = True
         extra = Extra.forbid
 
     @property
     def number_of_samples(self) -> Union[int, None]:
@@ -101,14 +102,15 @@
     config: Optional[dict]
     name: Optional[str] = None
     tag: Optional[str] = None
     private: Optional[bool] = Field(alias="is_private")
     digest: Optional[str]
     number_of_samples: Optional[int]
     pep_schema: Optional[str]
+    description: Optional[str] = ""
     # last_update_date: Optional[datetime.datetime] = datetime.datetime.now(datetime.timezone.utc)
 
     @validator("tag", "name")
     def value_must_not_be_empty(cls, v):
         if "" == v:
             return None
         return v
```

### Comparing `pepdbagent-0.5.2/pepdbagent/modules/annotation.py` & `pepdbagent-0.5.3/pepdbagent/modules/annotation.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.2/pepdbagent/modules/namespace.py` & `pepdbagent-0.5.3/pepdbagent/modules/namespace.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.2/pepdbagent/modules/project.py` & `pepdbagent-0.5.3/pepdbagent/modules/project.py`

 * *Files 6% similar despite different names*

```diff
@@ -220,40 +220,41 @@
         :param update_only: if project exists overwrite it, otherwise do nothing.  [Default: False]
         :param description: description of the project
         :return: None
         """
         proj_dict = project.to_dict(extended=True, orient="records")
         if not description:
             description = project.description
-        proj_dict[CONFIG_KEY]["description"] = description
+        proj_dict[CONFIG_KEY][DESCRIPTION_KEY] = description
 
         namespace = namespace.lower()
         if name:
-            name = name.lower()
-            proj_name = name
-            proj_dict[CONFIG_KEY]["name"] = proj_name
-        elif proj_dict[CONFIG_KEY]["name"]:
-            proj_name = proj_dict[CONFIG_KEY]["name"].lower()
+            proj_name = name.lower()
+        elif proj_dict[CONFIG_KEY][NAME_KEY]:
+            proj_name = proj_dict[CONFIG_KEY][NAME_KEY].lower()
         else:
             raise ValueError(f"Name of the project wasn't provided. Project will not be uploaded.")
 
+        proj_dict[CONFIG_KEY][NAME_KEY] = proj_name
+
         proj_digest = create_digest(proj_dict)
         number_of_samples = len(project.samples)
 
         if update_only:
             _LOGGER.info(f"Update_only argument is set True. Updating project {proj_name} ...")
             self._overwrite(
                 project_dict=proj_dict,
                 namespace=namespace,
                 proj_name=proj_name,
                 tag=tag,
                 project_digest=proj_digest,
                 number_of_samples=number_of_samples,
                 private=is_private,
                 pep_schema=pep_schema,
+                description=description,
             )
             return None
         else:
             try:
                 _LOGGER.info(f"Uploading {namespace}/{proj_name}:{tag} project...")
                 new_prj = Projects(
                     namespace=namespace,
@@ -262,14 +263,15 @@
                     digest=proj_digest,
                     config=proj_dict[CONFIG_KEY],
                     number_of_samples=number_of_samples,
                     private=is_private,
                     submission_date=datetime.datetime.now(datetime.timezone.utc),
                     last_update_date=datetime.datetime.now(datetime.timezone.utc),
                     pep_schema=pep_schema,
+                    description=description,
                 )
 
                 self._add_samples_to_project(new_prj, proj_dict[SAMPLE_RAW_DICT_KEY])
 
                 if proj_dict[SUBSAMPLE_RAW_LIST_KEY]:
                     subsamples = proj_dict[SUBSAMPLE_RAW_LIST_KEY]
                     self._add_subsamples_to_project(new_prj, subsamples)
@@ -287,14 +289,15 @@
                         namespace=namespace,
                         proj_name=proj_name,
                         tag=tag,
                         project_digest=proj_digest,
                         number_of_samples=number_of_samples,
                         private=is_private,
                         pep_schema=pep_schema,
+                        description=description,
                     )
                     return None
 
                 else:
                     raise ProjectUniqueNameError(
                         f"Namespace, name and tag already exists. Project won't be "
                         f"uploaded. Solution: Set overwrite value as True"
@@ -307,48 +310,50 @@
         namespace: str,
         proj_name: str,
         tag: str,
         project_digest: str,
         number_of_samples: int,
         private: bool = False,
         pep_schema: str = None,
+        description: str = "",
     ) -> None:
         """
         Update existing project by providing all necessary information.
 
         :param project_dict: project dictionary in json format
         :param namespace: project namespace
         :param proj_name: project name
         :param tag: project tag
         :param project_digest: project digest
         :param number_of_samples: number of samples in project
         :param private: boolean value if the project should be visible just for user that creates it.
         :param pep_schema: assign PEP to a specific schema. [DefaultL: None]
+        :param description: project description
         :return: None
         """
         proj_name = proj_name.lower()
         namespace = namespace.lower()
         if self.exists(namespace=namespace, name=proj_name, tag=tag):
             _LOGGER.info(f"Updating {proj_name} project...")
             statement = self._create_select_statement(proj_name, namespace, tag)
 
             with Session(self._sa_engine) as session:
-                found_prj = session.scalars(statement).one()
+                found_prj = session.scalar(statement)
 
                 if found_prj:
                     _LOGGER.debug(
                         f"Project has been found: {found_prj.namespace}, {found_prj.name}"
                     )
 
                     found_prj.digest = project_digest
                     found_prj.number_of_samples = number_of_samples
                     found_prj.private = private
                     found_prj.pep_schema = pep_schema
-                    found_prj.last_update_date = datetime.datetime.now(datetime.timezone.utc)
-                    found_prj.description = project_dict[CONFIG_KEY].get("description")
+                    found_prj.config = project_dict[CONFIG_KEY]
+                    found_prj.description = description
 
                     # Deleting old samples and subsamples
                     if found_prj.samples_mapping:
                         for sample in found_prj.samples_mapping:
                             _LOGGER.info(f"deleting samples: {str(sample)}")
                             session.delete(sample)
 
@@ -422,20 +427,20 @@
                     )
 
                     for k, v in update_values.items():
                         if getattr(found_prj, k) != v:
                             setattr(found_prj, k, v)
 
                             # standardizing project name
-                            if k == "name":
+                            if k == NAME_KEY:
                                 if "config" in update_values:
-                                    update_values["config"]["name"] = v
+                                    update_values["config"][NAME_KEY] = v
                                 else:
-                                    found_prj.config["name"] = v
-                                found_prj.name = found_prj.config["name"]
+                                    found_prj.config[NAME_KEY] = v
+                                found_prj.name = found_prj.config[NAME_KEY]
 
                     if "samples" in update_dict:
                         if found_prj.samples_mapping:
                             for sample in found_prj.samples_mapping:
                                 _LOGGER.debug(f"deleting samples: {str(sample)}")
                                 session.delete(sample)
 
@@ -447,14 +452,16 @@
                                 _LOGGER.debug(f"deleting subsamples: {str(subsample)}")
                                 session.delete(subsample)
 
                         # Adding new subsamples
                         if update_dict["subsamples"]:
                             self._add_subsamples_to_project(found_prj, update_dict["subsamples"])
 
+                    found_prj.last_update_date = datetime.datetime.now(datetime.timezone.utc)
+
                     session.commit()
 
             return None
 
         else:
             raise ProjectNotFoundError("No items will be updated!")
 
@@ -466,40 +473,57 @@
 
          :param update_values: UpdateItems (pydantic class) with
             updating values
         :return: unified update dict
         """
         update_final = UpdateModel()
 
+        if update_values.name is not None:
+            if update_values.config is not None:
+                update_values.config[NAME_KEY] = update_values.name
+            update_final = UpdateModel(
+                name=update_values.name,
+                **update_final.dict(exclude_unset=True),
+            )
+
+        if update_values.description is not None:
+            if update_values.config is not None:
+                update_values.config[DESCRIPTION_KEY] = update_values.description
+            update_final = UpdateModel(
+                description=update_values.description,
+                **update_final.dict(exclude_unset=True),
+            )
         if update_values.config is not None:
-            if update_values.description is not None:
-                update_values.config["description"] = update_values.description
-            if update_values.name is not None:
-                update_values.config["name"] = update_values.name
             update_final = UpdateModel(
                 config=update_values.config, **update_final.dict(exclude_unset=True)
             )
+            name = update_values.config.get(NAME_KEY)
+            description = update_values.config.get(DESCRIPTION_KEY)
+            if name:
+                update_final = UpdateModel(
+                    name=name,
+                    **update_final.dict(exclude_unset=True, exclude={NAME_KEY}),
+                )
+            if description:
+                update_final = UpdateModel(
+                    description=description,
+                    **update_final.dict(exclude_unset=True, exclude={DESCRIPTION_KEY}),
+                )
 
         if update_values.tag is not None:
             update_final = UpdateModel(
                 tag=update_values.tag, **update_final.dict(exclude_unset=True)
             )
 
         if update_values.is_private is not None:
             update_final = UpdateModel(
                 is_private=update_values.is_private,
                 **update_final.dict(exclude_unset=True),
             )
 
-        if update_values.name is not None:
-            update_final = UpdateModel(
-                name=update_values.name,
-                **update_final.dict(exclude_unset=True),
-            )
-
         if update_values.pep_schema is not None:
             update_final = UpdateModel(
                 pep_schema=update_values.pep_schema,
                 **update_final.dict(exclude_unset=True),
             )
 
         if update_values.number_of_samples is not None:
```

### Comparing `pepdbagent-0.5.2/pepdbagent/pepdbagent.py` & `pepdbagent-0.5.3/pepdbagent/pepdbagent.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.2/pepdbagent/utils.py` & `pepdbagent-0.5.3/pepdbagent/utils.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.2/pepdbagent.egg-info/PKG-INFO` & `pepdbagent-0.5.3/pepdbagent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepdbagent
-Version: 0.5.2
+Version: 0.5.3
 Summary: A python-based project metadata manager for portable encapsulated projects
 Home-page: https://github.com/pepkit/pepdbagent/
 Author: Oleksandr Khoroshevskyi
 License: BSD2
 Keywords: project,metadata,bioinformatics,database
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pepdbagent-0.5.2/pepdbagent.egg-info/SOURCES.txt` & `pepdbagent-0.5.3/pepdbagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.2/setup.py` & `pepdbagent-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.2/tests/conftest.py` & `pepdbagent-0.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pepdbagent-0.5.2/tests/test_pepagent.py` & `pepdbagent-0.5.3/tests/test_pepagent.py`

 * *Files identical despite different names*

