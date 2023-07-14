# Comparing `tmp/gmail_draft_creator-1.2.0.tar.gz` & `tmp/gmail_draft_creator-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmail_draft_creator-1.2.0.tar", max compression
+gzip compressed data, was "gmail_draft_creator-1.2.1.tar", max compression
```

## Comparing `gmail_draft_creator-1.2.0.tar` & `gmail_draft_creator-1.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1071 2023-07-09 13:14:19.581481 gmail_draft_creator-1.2.0/LICENSE
--rw-r--r--   0        0        0     4554 2023-07-09 13:14:19.581481 gmail_draft_creator-1.2.0/gmail_draft_creator/__init__.py
--rw-r--r--   0        0        0     1079 2023-07-09 13:14:41.669720 gmail_draft_creator-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1917 2023-07-09 13:14:19.581481 gmail_draft_creator-1.2.0/readme.md
--rw-r--r--   0        0        0     2756 1970-01-01 00:00:00.000000 gmail_draft_creator-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-14 21:25:27.494420 gmail_draft_creator-1.2.1/LICENSE
+-rw-r--r--   0        0        0     4719 2023-07-14 21:25:27.494420 gmail_draft_creator-1.2.1/gmail_draft_creator/__init__.py
+-rw-r--r--   0        0        0     1186 2023-07-14 21:25:49.062650 gmail_draft_creator-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1905 2023-07-14 21:25:27.494420 gmail_draft_creator-1.2.1/readme.md
+-rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 gmail_draft_creator-1.2.1/PKG-INFO
```

### Comparing `gmail_draft_creator-1.2.0/LICENSE` & `gmail_draft_creator-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gmail_draft_creator-1.2.0/gmail_draft_creator/__init__.py` & `gmail_draft_creator-1.2.1/gmail_draft_creator/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,21 @@
     with open(template_file_path, "r") as template_file:
         template_string = template_file.read()
 
     with open(csv_file_path, "r") as file:
         reader = csv.DictReader(file)
         for row in reader:
             email = row.pop("email", None) or row.pop("Email", None)
-            template_params = {k.lower(): v for k, v in row.items()}
+
+            if email is None:
+                print("No email found for row, skipping")
+                continue
+
+            email = email.strip()
+            template_params = {k.lower().strip(): v.strip() for k, v in row.items()}
 
             if email is not None:
                 create_draft(email, template_string, template_params, subject, dry_run)
 
 
 # TODO this should really be much smarter
 def _extract_credentials():
```

### Comparing `gmail_draft_creator-1.2.0/pyproject.toml` & `gmail_draft_creator-1.2.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 [tool.poetry]
 name = "gmail_draft_creator"
-version = "1.2.0"
+version = "1.2.1"
 description = "Create draft messages in Gmail"
 authors = ["Michael Bianco <mike@mikebian.co>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/iloveitaly/gmail-draft-creator"
 
+[project.urls]
+'Changelog' = 'https://github.com/iloveitaly/gmail-draft-creator/blob/master/CHANGELOG.md'
+
 [tool.poetry.dependencies]
 python = "^3.9"
 google-api-python-client = "^2.21.0"
 python-decouple = "^3.5"
 google-auth-httplib2 = "^0.1.0"
 google-auth-oauthlib = "^0.4.6"
 click = "^8.1.3"
```

### Comparing `gmail_draft_creator-1.2.0/readme.md` & `gmail_draft_creator-1.2.1/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 ```shell
 Usage: gmail-draft-creator [OPTIONS]
 
 Options:
   --csv PATH       Path to the CSV file.  [required]
   --template PATH  Path to the template file.  [required]
-  --subject TEXT   Subject for the email drafts.  [required]
+  --subject TEXT   Subject for the email drafts.
   --dry-run        Run script without creating drafts.
   --help           Show this message and exit.
 
 ```
 
 You can also import the `create_draft` function and use it in your own scripts.
```

### Comparing `gmail_draft_creator-1.2.0/PKG-INFO` & `gmail_draft_creator-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmail-draft-creator
-Version: 1.2.0
+Version: 1.2.1
 Summary: Create draft messages in Gmail
 Home-page: https://github.com/iloveitaly/gmail-draft-creator
 License: MIT
 Author: Michael Bianco
 Author-email: mike@mikebian.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -35,15 +35,15 @@
 
 ```shell
 Usage: gmail-draft-creator [OPTIONS]
 
 Options:
   --csv PATH       Path to the CSV file.  [required]
   --template PATH  Path to the template file.  [required]
-  --subject TEXT   Subject for the email drafts.  [required]
+  --subject TEXT   Subject for the email drafts.
   --dry-run        Run script without creating drafts.
   --help           Show this message and exit.
 
 ```
 
 You can also import the `create_draft` function and use it in your own scripts.
```

