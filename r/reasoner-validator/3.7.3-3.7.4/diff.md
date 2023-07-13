# Comparing `tmp/reasoner_validator-3.7.3.tar.gz` & `tmp/reasoner_validator-3.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.7.3.tar", max compression
+gzip compressed data, was "reasoner_validator-3.7.4.tar", max compression
```

## Comparing `reasoner_validator-3.7.3.tar` & `reasoner_validator-3.7.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1153 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/LICENSE
--rw-r--r--   0        0        0    12703 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/README.md
--rw-r--r--   0        0        0      131 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/Makefile
--rw-r--r--   0        0        0     2291 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/conf.py
--rw-r--r--   0        0        0    19869 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/index.rst
--rw-r--r--   0        0        0      795 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/make.bat
--rw-r--r--   0        0        0      136 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    36258 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2177 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/pyproject.toml
--rw-r--r--   0        0        0    38452 2023-07-13 19:01:42.994082 reasoner_validator-3.7.3/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    76464 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    39514 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     3382 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/message.py
--rw-r--r--   0        0        0    29568 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4754 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    11622 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14569 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    12532 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      774 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/conftest.py
--rw-r--r--   0        0        0   117433 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    40085 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/test_semver.py
--rw-r--r--   0        0        0     2248 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    26808 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/test_validate.py
--rw-r--r--   0        0        0    21570 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/test_validation_report.py
--rw-r--r--   0        0        0     2042 2023-07-13 19:01:42.998082 reasoner_validator-3.7.3/tests/test_workflows.py
--rw-r--r--   0        0        0    14690 1970-01-01 00:00:00.000000 reasoner_validator-3.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-07-13 23:22:36.908379 reasoner_validator-3.7.4/LICENSE
+-rw-r--r--   0        0        0    12703 2023-07-13 23:22:36.908379 reasoner_validator-3.7.4/README.md
+-rw-r--r--   0        0        0      131 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/Makefile
+-rw-r--r--   0        0        0     2291 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/conf.py
+-rw-r--r--   0        0        0    19869 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      142 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    36836 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2177 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/pyproject.toml
+-rw-r--r--   0        0        0    38452 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    77837 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    40078 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     3382 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/message.py
+-rw-r--r--   0        0        0    29568 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    11622 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1105 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14569 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    12532 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      774 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:22:36.912379 reasoner_validator-3.7.4/tests/conftest.py
+-rw-r--r--   0        0        0   119662 2023-07-13 23:22:36.916379 reasoner_validator-3.7.4/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2023-07-13 23:22:36.916379 reasoner_validator-3.7.4/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    40085 2023-07-13 23:22:36.916379 reasoner_validator-3.7.4/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2023-07-13 23:22:36.916379 reasoner_validator-3.7.4/tests/test_semver.py
+-rw-r--r--   0        0        0     2248 2023-07-13 23:22:36.916379 reasoner_validator-3.7.4/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    26808 2023-07-13 23:22:36.916379 reasoner_validator-3.7.4/tests/test_validate.py
+-rw-r--r--   0        0        0    21570 2023-07-13 23:22:36.916379 reasoner_validator-3.7.4/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2042 2023-07-13 23:22:36.916379 reasoner_validator-3.7.4/tests/test_workflows.py
+-rw-r--r--   0        0        0    14690 1970-01-01 00:00:00.000000 reasoner_validator-3.7.4/PKG-INFO
```

### Comparing `reasoner_validator-3.7.3/LICENSE` & `reasoner_validator-3.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/README.md` & `reasoner_validator-3.7.4/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/docs/Makefile` & `reasoner_validator-3.7.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/docs/conf.py` & `reasoner_validator-3.7.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/docs/index.rst` & `reasoner_validator-3.7.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/docs/make.bat` & `reasoner_validator-3.7.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/docs/validation_codes_dictionary.md` & `reasoner_validator-3.7.4/docs/validation_codes_dictionary.md`

 * *Files 1% similar despite different names*

```diff
@@ -708,29 +708,37 @@
 
 **Message:** The 'sources' are not an array in Edge
 
 **Context:** identifier
 
 **Description:** Value of the 'sources' property in Knowledge Graph edge must be an array of RetrievalSource entries!
 
+### error.knowledge_graph.edge.sources.retrieval_source.resource_id.infores.missing
+
+**Message:** RetrievalSource 'resource_id' identifier is missing!
+
+**Context:** edge_id
+
+**Description:** A RetrievalSource 'resource_id' value should not be None or empty!
+
 ### error.knowledge_graph.edge.sources.retrieval_source.resource_id.infores.not_curie
 
-**Message:** Infores value is not a valid well-formed CURIE
+**Message:** One (or more) Infores value(s) is not a valid well-formed CURIE
 
 **Context:** edge_id, identifier
 
-**Description:** A 'retrieval_source.resource_id' value must be a well-formed infores CURIE!
+**Description:** A RetrievalSource 'resource_id' Infores value must be a well-formed CURIE!
 
 ### error.knowledge_graph.edge.sources.retrieval_source.resource_id.infores.invalid
 
 **Message:** Invalid Infores namespace
 
 **Context:** edge_id, identifier
 
-**Description:** A 'retrieval_source.resource_id' Infores CURIE must come from the Infores namespace!
+**Description:** A RetrievalSource 'resource_id' Infores CURIE must come from the Infores namespace!
 
 ### error.knowledge_graph.edge.sources.retrieval_source.resource_id.infores.unknown
 
 **Message:** Unregistered infores
 
 **Context:** edge_id, identifier
 
@@ -740,29 +748,37 @@
 
 **Message:** Empty 'resource_id' property in Edge
 
 **Context:** identifier
 
 **Description:** Value of the 'resource_id' property in the RetrievalSource of a Knowledge Graph Edge must be a non-empty Infores identifier!
 
+### error.knowledge_graph.edge.sources.retrieval_source.upstream_resource_ids.infores.missing
+
+**Message:** A RetrievalSource 'upstream_resource_ids' identifier is missing!
+
+**Context:** edge_id
+
+**Description:** A RetrievalSource 'upstream_resource_ids' value should not be None or empty!
+
 ### error.knowledge_graph.edge.sources.retrieval_source.upstream_resource_ids.infores.not_curie
 
-**Message:** Infores value is not a valid well-formed CURIE
+**Message:** One (or more) Infores value(s) is not a valid well-formed CURIE
 
 **Context:** edge_id, identifier
 
-**Description:** A 'retrieval_source.upstream_resource_ids' values must be a well-formed Infores CURIE!
+**Description:** A RetrievalSource 'upstream_resource_ids' Infores value must be a well-formed CURIE!
 
 ### error.knowledge_graph.edge.sources.retrieval_source.upstream_resource_ids.infores.invalid
 
 **Message:** Invalid Infores namespace
 
 **Context:** edge_id, identifier
 
-**Description:** A 'retrieval_source.upstream_resource_ids' Infores CURIEs must come from the Infores namespace!
+**Description:** A RetrievalSource 'upstream_resource_ids' Infores CURIE must come from the Infores namespace!
 
 ### error.knowledge_graph.edge.sources.retrieval_source.upstream_resource_ids.infores.unknown
 
 **Message:** Unregistered Infores
 
 **Context:** edge_id, identifier
```

### Comparing `reasoner_validator-3.7.3/pyproject.toml` & `reasoner_validator-3.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.7.3"
+version = "3.7.4"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-3.7.3/reasoner_validator/__init__.py` & `reasoner_validator-3.7.4/reasoner_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.7.4/reasoner_validator/biolink/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -834,25 +834,59 @@
                     self.validate_qualifier_entry(
                         context="query_graph.edge.qualifier_constraints.qualifier_set",
                         edge_id=edge_id,
                         qualifiers=qualifier_set
                     )
 
     def validate_infores(self, context: str, edge_id: str, identifier: str) -> bool:
+        """
+        Validate that the specified identifier is a well-formed Infores CURIE.
+        Note that here we also now accept that the identifier can
+        be a semi-colon delimited list of such infores.
+
+        :param context: reporting context as specified by a validation code prefix
+        :param edge_id: specific edge validated, for the purpose of reporting validation context
+        :param identifier: candidate (list of) infores curie(s) to be validated.
+        :return:
+        """
         code_prefix: str = f"error.knowledge_graph.edge.sources.retrieval_source.{context}.infores"
-        if not is_curie(identifier):
+
+        # sanity check...
+        if not identifier:
+            # identifier itself is None or empty string
+            self.report(
+                code=f"{code_prefix}.missing",
+                edge_id=edge_id
+            )
+            return False
+
+        # For uniform processing here, we treat every identifier
+        # as a potential list (even if only a list of one entry),
+        ids: list[str] = [token.strip() for token in identifier.split(";")]
+        if not all([i for i in ids]):
+            # if the identifier is a semi-colon delimited array,
+            # then at least one of the entries is None or empty...
+            self.report(
+                code=f"{code_prefix}.missing",
+                identifier=identifier,
+                edge_id=edge_id
+            )
+            return False
+
+        if not all([is_curie(i) for i in ids]):
+            # ... or at least one of the entries is not a CURIE...
             self.report(
                 code=f"{code_prefix}.not_curie",
                 identifier=identifier,
                 edge_id=edge_id
             )
             return False
 
-        if not identifier.startswith("infores:"):
-            # not sure how absolute the need is for this to be an Infores. We'll be lenient for now?
+        if not all([i.startswith("infores:") for i in ids]):
+            # ... or at least one of the entries is not a CURIE...
             self.report(
                 code=f"{code_prefix}.invalid",
                 identifier=identifier,
                 edge_id=edge_id
             )
             return False
```

### Comparing `reasoner_validator-3.7.3/reasoner_validator/codes.yaml` & `reasoner_validator-3.7.4/reasoner_validator/codes.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -543,51 +543,61 @@
           $message: "The 'sources' are not an array in Edge"
           $context:
             - identifier
           $description: "Value of the 'sources' property in Knowledge Graph edge must be an array of RetrievalSource entries!"
         retrieval_source:
           resource_id:
             infores:
+              missing:
+                $message: "RetrievalSource 'resource_id' identifier is missing!"
+                $context:
+                  - edge_id
+                $description: "A RetrievalSource 'resource_id' value should not be None or empty!"
               not_curie:
-                $message: "Infores value is not a valid well-formed CURIE"
+                $message: "One (or more) Infores value(s) is not a valid well-formed CURIE"
                 $context:
                   - edge_id
                   - identifier
-                $description: "A 'retrieval_source.resource_id' value must be a well-formed infores CURIE!"
+                $description: "A RetrievalSource 'resource_id' Infores value must be a well-formed CURIE!"
               invalid:
                 $message: "Invalid Infores namespace"
                 $context:
                   - edge_id
                   - identifier
-                $description: "A 'retrieval_source.resource_id' Infores CURIE must come from the Infores namespace!"
+                $description: "A RetrievalSource 'resource_id' Infores CURIE must come from the Infores namespace!"
               unknown:
                 $message: "Unregistered infores"
                 $context:
                   - edge_id
                   - identifier
                 $description: "A 'retrieval_source.resource_id' value must be a registered Infores identifier!"
             empty:
               $message: "Empty 'resource_id' property in Edge"
               $context:
                 - identifier
               $description: "Value of the 'resource_id' property in the RetrievalSource of a Knowledge Graph Edge must be a non-empty Infores identifier!"
           upstream_resource_ids:
             infores:
+              missing:
+                $message: "A RetrievalSource 'upstream_resource_ids' identifier is missing!"
+                $context:
+                  - edge_id
+                $description: "A RetrievalSource 'upstream_resource_ids' value should not be None or empty!"
               not_curie:
-                $message: "Infores value is not a valid well-formed CURIE"
+                $message: "One (or more) Infores value(s) is not a valid well-formed CURIE"
                 $context:
                   - edge_id
                   - identifier
-                $description: "A 'retrieval_source.upstream_resource_ids' values must be a well-formed Infores CURIE!"
+                $description: "A RetrievalSource 'upstream_resource_ids' Infores value must be a well-formed CURIE!"
               invalid:
                 $message: "Invalid Infores namespace"
                 $context:
                   - edge_id
                   - identifier
-                $description: "A 'retrieval_source.upstream_resource_ids' Infores CURIEs must come from the Infores namespace!"
+                $description: "A RetrievalSource 'upstream_resource_ids' Infores CURIE must come from the Infores namespace!"
               unknown:
                 $message: "Unregistered Infores"
                 $context:
                   - edge_id
                   - identifier
                 $description: "A 'retrieval_source.upstream_resource_ids' values must be registered infores identifiers!"
           resource_role:
```

### Comparing `reasoner_validator-3.7.3/reasoner_validator/message.py` & `reasoner_validator-3.7.4/reasoner_validator/message.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/reasoner_validator/report.py` & `reasoner_validator-3.7.4/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/reasoner_validator/sri/util.py` & `reasoner_validator-3.7.4/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.7.4/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.7.4/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/reasoner_validator/validation_codes.py` & `reasoner_validator-3.7.4/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/reasoner_validator/versioning.py` & `reasoner_validator-3.7.4/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/tests/__init__.py` & `reasoner_validator-3.7.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.7.4/tests/test_biolink_compliance_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1571,14 +1571,59 @@
     qualifier_validator(
         tested_method=BiolinkValidator.validate_qualifier_constraints,
         edge_model="QEdge",
         query=query
     )
 
 
+# This tests identifiers within a RetrievalSource and is only done for the context of
+# 'resource_id' identifiers but the equivalent functionality assumed for 'upstream_resource_ids'
+@pytest.mark.parametrize(
+    "identifier,validation_code",
+    [
+        (   # Query 0: valid single 'infores' curie
+            "infores:molepro",
+            ""  # this shouldn't be an error
+        ),
+        (   # Query 1: semicolon list of 'infores' curies is also accepted
+            "infores:molepro; infores:arax",
+            ""  # this shouldn't be an error
+        ),
+        (   # Query 2: an empty value for the identifier will be caught
+            "",
+            "error.knowledge_graph.edge.sources.retrieval_source.resource_id.infores.missing"
+        ),
+        (   # Query 3: all the entries of an infores list of identifiers must be non-empty strings?
+            "infores:molepro; ",
+            "error.knowledge_graph.edge.sources.retrieval_source.resource_id.infores.missing"
+        ),
+        (   # Query 4: an identifier which is not a CURIE
+            "arax",
+            "error.knowledge_graph.edge.sources.retrieval_source.resource_id.infores.not_curie"
+        ),
+        (   # Query 5: all entries in a list must be a CURIE
+            "infores:molepro; arax",
+            "error.knowledge_graph.edge.sources.retrieval_source.resource_id.infores.not_curie"
+        ),
+        (   # Query 6: any curie given must be from the 'infores:' namespace
+            "NCBIGene:12345",
+            "error.knowledge_graph.edge.sources.retrieval_source.resource_id.infores.invalid"
+        ),
+        (   # Query 7: all curies given in a curie must be from the 'infores:' namespace
+            "infores:molepro; NCBIGene:12345",
+            "error.knowledge_graph.edge.sources.retrieval_source.resource_id.infores.invalid"
+        )
+    ]
+)
+def test_validate_infores(identifier: str, validation_code: str):
+    validator = BiolinkValidator(graph_type=TRAPIGraphType.Knowledge_Graph)
+    validator.validate_infores("resource_id", "test_validate_infores", identifier)
+    check_messages(validator, validation_code)
+
+
 @pytest.mark.parametrize(
     "query",
     [
         (   # Query 0 - 'qualifier_type_id' is the special qualifier case 'biolink:qualified_predicate'
             #            an incorrect value, which is not a Biolink predicate,  but...
             {
                 'qualifier_constraints': [
@@ -1827,15 +1872,15 @@
     )
 
 
 ##################################
 # Validate TRAPI Knowledge Graph #
 ##################################
 @pytest.mark.parametrize(
-    "query",
+    "biolink_version,graph_data,validation_code",
     [
         (
             LATEST_BIOLINK_MODEL_VERSION,  # Biolink Model Version
 
             # Query 0: Sample full valid TRAPI Knowledge Graph
             {
                 # Sample nodes
@@ -2818,19 +2863,20 @@
             },
             # ...since Biolink Model validation is tagged as 'suppress',
             # we  don't expect any validation output here?
             ""
         )
     ]
 )
-def test_check_biolink_model_compliance_of_knowledge_graph(query: Tuple):
+def test_check_biolink_model_compliance_of_knowledge_graph(
+        biolink_version: str, graph_data: Dict, validation_code: str):
     validator: BiolinkValidator = check_biolink_model_compliance_of_knowledge_graph(
-        graph=query[1], biolink_version=query[0]
+        graph=graph_data, biolink_version=biolink_version
     )
-    check_messages(validator, query[2])
+    check_messages(validator, validation_code)
 
 
 MESSAGE_EDGE_WITHOUT_ATTRIBUTES = {
     "nodes": {
         "NCBIGene:29974": {
             "categories": [
                 "biolink:Gene"
```

### Comparing `reasoner_validator-3.7.3/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-3.7.4/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/tests/test_response_validator.py` & `reasoner_validator-3.7.4/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/tests/test_semver.py` & `reasoner_validator-3.7.4/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/tests/test_trapi_versioning.py` & `reasoner_validator-3.7.4/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/tests/test_validate.py` & `reasoner_validator-3.7.4/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/tests/test_validation_report.py` & `reasoner_validator-3.7.4/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/tests/test_workflows.py` & `reasoner_validator-3.7.4/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.7.3/PKG-INFO` & `reasoner_validator-3.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.7.3
+Version: 3.7.4
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```

