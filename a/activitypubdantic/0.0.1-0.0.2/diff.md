# Comparing `tmp/activitypubdantic-0.0.1.tar.gz` & `tmp/activitypubdantic-0.0.2.tar.gz`

## Comparing `activitypubdantic-0.0.1.tar` & `activitypubdantic-0.0.2.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0    22858 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/activitypubdantic_test.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/create_docs.sh
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/developer_requirements.txt
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/requirements.txt
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/.github/workflows/python_package.yaml
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/activitypubdantic/__init__.py
--rw-r--r--   0        0        0     8272 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/activitypubdantic/get_class.py
--rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/activitypubdantic/get_model.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/activitypubdantic/models/__init__.py
--rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/activitypubdantic/models/activity.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/activitypubdantic/models/actor.py
--rw-r--r--   0        0        0    22796 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/activitypubdantic/models/core.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/activitypubdantic/models/link.py
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/activitypubdantic/models/object.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/activitypubdantic/models/_utils/__init__.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/activitypubdantic/models/_utils/language_types.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/activitypubdantic/models/_utils/mime_types.py
--rw-r--r--   0        0        0    47723 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/docs/get_class.html
--rw-r--r--   0        0        0    18035 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/docs/get_model.html
--rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/docs/index.html
--rw-r--r--   0        0        0    94892 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/docs/models/activity.html
--rw-r--r--   0        0        0    41007 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/docs/models/actor.html
--rw-r--r--   0        0        0   113691 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/docs/models/core.html
--rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/docs/models/index.html
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/docs/models/link.html
--rw-r--r--   0        0        0    36238 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/docs/models/object.html
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/activitypub/article.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/activitypub/create.json
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/activitypub/like.json
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/activitypub/note.json
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/activitypub/person.json
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/activitystreams/accept.json
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/activitystreams/add.json
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/activitystreams/article.json
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/activitystreams/collection.json
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/activitystreams/image.json
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/activitystreams/move.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/activitystreams/person.json
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/activitystreams/place.json
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/activitystreams/question.json
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/activitystreams/tombstone.json
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/mastodon/accept.json
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/mastodon/create.json
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/mastodon/follow.json
--rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/mastodon/person.json
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/json/mastodon/poll.json
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/LICENSE
--rw-r--r--   0        0        0     9865 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/README.md
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    10406 2020-02-02 00:00:00.000000 activitypubdantic-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    22858 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic_test.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/create_docs.sh
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/developer_requirements.txt
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/.github/workflows/distribute.yaml
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/__init__.py
+-rw-r--r--   0        0        0     8272 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/get_class.py
+-rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/get_model.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/models/__init__.py
+-rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/models/activity.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/models/actor.py
+-rw-r--r--   0        0        0    22796 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/models/core.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/models/link.py
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/models/object.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/models/_utils/__init__.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/models/_utils/language_types.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/activitypubdantic/models/_utils/mime_types.py
+-rw-r--r--   0        0        0    47723 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/docs/get_class.html
+-rw-r--r--   0        0        0    18035 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/docs/get_model.html
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/docs/index.html
+-rw-r--r--   0        0        0    94892 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/docs/models/activity.html
+-rw-r--r--   0        0        0    41007 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/docs/models/actor.html
+-rw-r--r--   0        0        0   113691 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/docs/models/core.html
+-rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/docs/models/index.html
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/docs/models/link.html
+-rw-r--r--   0        0        0    36238 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/docs/models/object.html
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitypub/article.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitypub/create.json
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitypub/like.json
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitypub/note.json
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitypub/person.json
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/accept.json
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/add.json
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/article.json
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/collection.json
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/image.json
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/move.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/person.json
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/place.json
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/question.json
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/activitystreams/tombstone.json
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/mastodon/accept.json
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/mastodon/create.json
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/mastodon/follow.json
+-rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/mastodon/person.json
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/json/mastodon/poll.json
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/LICENSE
+-rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/README.md
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    10400 2020-02-02 00:00:00.000000 activitypubdantic-0.0.2/PKG-INFO
```

### Comparing `activitypubdantic-0.0.1/activitypubdantic_test.py` & `activitypubdantic-0.0.2/activitypubdantic_test.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/.github/workflows/python_package.yaml` & `activitypubdantic-0.0.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/activitypubdantic/__init__.py` & `activitypubdantic-0.0.2/activitypubdantic/__init__.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/activitypubdantic/get_class.py` & `activitypubdantic-0.0.2/activitypubdantic/get_class.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/activitypubdantic/get_model.py` & `activitypubdantic-0.0.2/activitypubdantic/get_model.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/activitypubdantic/models/__init__.py` & `activitypubdantic-0.0.2/activitypubdantic/models/__init__.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/activitypubdantic/models/activity.py` & `activitypubdantic-0.0.2/activitypubdantic/models/activity.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/activitypubdantic/models/actor.py` & `activitypubdantic-0.0.2/activitypubdantic/models/actor.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/activitypubdantic/models/core.py` & `activitypubdantic-0.0.2/activitypubdantic/models/core.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/activitypubdantic/models/link.py` & `activitypubdantic-0.0.2/activitypubdantic/models/link.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/activitypubdantic/models/object.py` & `activitypubdantic-0.0.2/activitypubdantic/models/object.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/activitypubdantic/models/_utils/language_types.py` & `activitypubdantic-0.0.2/activitypubdantic/models/_utils/language_types.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/activitypubdantic/models/_utils/mime_types.py` & `activitypubdantic-0.0.2/activitypubdantic/models/_utils/mime_types.py`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/docs/get_class.html` & `activitypubdantic-0.0.2/docs/get_class.html`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/docs/get_model.html` & `activitypubdantic-0.0.2/docs/get_model.html`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/docs/index.html` & `activitypubdantic-0.0.2/docs/index.html`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/docs/models/activity.html` & `activitypubdantic-0.0.2/docs/models/activity.html`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/docs/models/actor.html` & `activitypubdantic-0.0.2/docs/models/actor.html`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/docs/models/core.html` & `activitypubdantic-0.0.2/docs/models/core.html`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/docs/models/index.html` & `activitypubdantic-0.0.2/docs/models/index.html`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/docs/models/link.html` & `activitypubdantic-0.0.2/docs/models/link.html`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/docs/models/object.html` & `activitypubdantic-0.0.2/docs/models/object.html`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/json/activitypub/create.json` & `activitypubdantic-0.0.2/json/activitypub/create.json`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/json/activitypub/person.json` & `activitypubdantic-0.0.2/json/activitypub/person.json`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/json/activitystreams/add.json` & `activitypubdantic-0.0.2/json/activitystreams/add.json`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/json/activitystreams/collection.json` & `activitypubdantic-0.0.2/json/activitystreams/collection.json`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/json/activitystreams/question.json` & `activitypubdantic-0.0.2/json/activitystreams/question.json`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/json/mastodon/accept.json` & `activitypubdantic-0.0.2/json/mastodon/accept.json`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/json/mastodon/create.json` & `activitypubdantic-0.0.2/json/mastodon/create.json`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/json/mastodon/person.json` & `activitypubdantic-0.0.2/json/mastodon/person.json`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/json/mastodon/poll.json` & `activitypubdantic-0.0.2/json/mastodon/poll.json`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/.gitignore` & `activitypubdantic-0.0.2/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 __pycache__/
 *.py[cod]
 *$py.class
 
 # Distribution
 .Python
 develop-eggs/
-dist/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
```

### Comparing `activitypubdantic-0.0.1/LICENSE` & `activitypubdantic-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `activitypubdantic-0.0.1/README.md` & `activitypubdantic-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # ActivityPubdantic
 
 ### Validate and Interact with ActivityPub JSON
 
+[GitHub Repository](https://github.com/joewlos/activitypubdantic)
+
 [ActivityPubdantic Documentation](https://www.joewlos.com/activitypubdantic/)
 
 [ActivityPub Protocol](https://www.w3.org/TR/activitypub/)
 
 [ActivityStreams Specification](https://www.w3.org/TR/activitystreams-vocabulary/)
 
 ## Development Note
@@ -22,15 +24,15 @@
 
 However, that flexibility presents challenges for assessing data validity and simplifying developers' code. **ActivityPubdantic** helps solve those challenges by using ActivityPub's "type" field to identify proper checks for other fields and standardize their structures. [Examples](#examples) are available in the sections below.
 
 [Mastodon](https://docs.joinmastodon.org/spec/activitypub/) supports ActivityPub, and Meta's [Threads](https://apps.apple.com/us/app/threads-an-instagram-app/id6446901002) app plans to conform to the protocol sometime in the [near future](https://techcrunch.com/2023/07/05/adam-mosseri-says-metas-threads-app-wont-have-activitypub-support-at-launch/). **ActivityPubdantic** includes a test suite, which uses examples from ActivityPub, ActivityStreams, and Mastodon to test its parsing and validation. As Threads and other platforms implement ActivityPub, those tests (and more broadly, this package) will be updated to stay current.
 
 ## Installation
 
-Download the `activitypubdantic/` directory in this repository and add it to your project, or (preferably) install the package with `pip`:
+Install the package with `pip`:
 
 ```console
 pip install activitypubdantic
 ```
 
 Most developer use cases will use one or both of the following import statements:
 
@@ -199,10 +201,10 @@
 
 ## Contributing
 
 **ActivityPubdantic** is still a work in progress. If you find it valuable for your project but notice bugs, need changes, or require additional features or support for other ActivityPub platforms, [open an issue](https://github.com/joewlos/activitypubdantic/issues) or fork to [start a PR](https://github.com/joewlos/activitypubdantic/pulls).
 
 The `developer_requirements.txt` file includes all of the packages your virtual environment needs to start, including `pdoc3` for generating new documentation and `pytest` for unit tests.
 
-Keep in mind, all PRs require GitHub to successfully complete the test suite, so if your changes significantly alter **ActivityPubdantic**'s structure, be sure to add, alter, or remove relevant tests.
+Keep in mind, all PRs require GitHub to successfully run the test suite, so if you significantly change **ActivityPubdantic**'s structure, be sure to add, alter, or remove relevant tests.
 
 Thank you for your interest!
```

### Comparing `activitypubdantic-0.0.1/pyproject.toml` & `activitypubdantic-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "activitypubdantic"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Joe Wlos", email="joewlos17@gmail.com" },
 ]
-description = "A small example package"
+description = "Pydantic Models for ActivityPub with Classes for Enabling Interactions"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["pydantic>=2.0.2"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `activitypubdantic-0.0.1/PKG-INFO` & `activitypubdantic-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: activitypubdantic
-Version: 0.0.1
-Summary: A small example package
+Version: 0.0.2
+Summary: Pydantic Models for ActivityPub with Classes for Enabling Interactions
 Project-URL: Homepage, https://github.com/joewlos/activitypubdantic
 Project-URL: Documentation, https://www.joewlos.com/activitypubdantic/
 Author-email: Joe Wlos <joewlos17@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,16 @@
 Requires-Dist: pydantic>=2.0.2
 Description-Content-Type: text/markdown
 
 # ActivityPubdantic
 
 ### Validate and Interact with ActivityPub JSON
 
+[GitHub Repository](https://github.com/joewlos/activitypubdantic)
+
 [ActivityPubdantic Documentation](https://www.joewlos.com/activitypubdantic/)
 
 [ActivityPub Protocol](https://www.w3.org/TR/activitypub/)
 
 [ActivityStreams Specification](https://www.w3.org/TR/activitystreams-vocabulary/)
 
 ## Development Note
@@ -37,15 +39,15 @@
 
 However, that flexibility presents challenges for assessing data validity and simplifying developers' code. **ActivityPubdantic** helps solve those challenges by using ActivityPub's "type" field to identify proper checks for other fields and standardize their structures. [Examples](#examples) are available in the sections below.
 
 [Mastodon](https://docs.joinmastodon.org/spec/activitypub/) supports ActivityPub, and Meta's [Threads](https://apps.apple.com/us/app/threads-an-instagram-app/id6446901002) app plans to conform to the protocol sometime in the [near future](https://techcrunch.com/2023/07/05/adam-mosseri-says-metas-threads-app-wont-have-activitypub-support-at-launch/). **ActivityPubdantic** includes a test suite, which uses examples from ActivityPub, ActivityStreams, and Mastodon to test its parsing and validation. As Threads and other platforms implement ActivityPub, those tests (and more broadly, this package) will be updated to stay current.
 
 ## Installation
 
-Download the `activitypubdantic/` directory in this repository and add it to your project, or (preferably) install the package with `pip`:
+Install the package with `pip`:
 
 ```console
 pip install activitypubdantic
 ```
 
 Most developer use cases will use one or both of the following import statements:
 
@@ -214,10 +216,10 @@
 
 ## Contributing
 
 **ActivityPubdantic** is still a work in progress. If you find it valuable for your project but notice bugs, need changes, or require additional features or support for other ActivityPub platforms, [open an issue](https://github.com/joewlos/activitypubdantic/issues) or fork to [start a PR](https://github.com/joewlos/activitypubdantic/pulls).
 
 The `developer_requirements.txt` file includes all of the packages your virtual environment needs to start, including `pdoc3` for generating new documentation and `pytest` for unit tests.
 
-Keep in mind, all PRs require GitHub to successfully complete the test suite, so if your changes significantly alter **ActivityPubdantic**'s structure, be sure to add, alter, or remove relevant tests.
+Keep in mind, all PRs require GitHub to successfully run the test suite, so if you significantly change **ActivityPubdantic**'s structure, be sure to add, alter, or remove relevant tests.
 
 Thank you for your interest!
```

