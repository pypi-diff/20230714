# Comparing `tmp/hojichar-0.5.3.tar.gz` & `tmp/hojichar-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hojichar-0.5.3.tar", max compression
+gzip compressed data, was "hojichar-0.6.0.tar", max compression
```

## Comparing `hojichar-0.5.3.tar` & `hojichar-0.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2023-06-07 06:57:14.579550 hojichar-0.5.3/LICENSE
--rw-r--r--   0        0        0    11137 2023-06-07 06:57:14.583551 hojichar-0.5.3/README.md
--rw-r--r--   0        0        0      534 2023-06-07 06:57:36.551757 hojichar-0.5.3/hojichar/__init__.py
--rw-r--r--   0        0        0     2761 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/__main__.py
--rw-r--r--   0        0        0       42 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/core/__init__.py
--rw-r--r--   0        0        0     4504 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/core/composition.py
--rw-r--r--   0        0        0     3122 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/core/filter_interface.py
--rw-r--r--   0        0        0     5031 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/core/inspection.py
--rw-r--r--   0        0        0      884 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/core/models.py
--rw-r--r--   0        0        0      147 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/dict/__init__.py
--rw-r--r--   0        0        0      941 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/dict/adult_keywords_en.txt
--rw-r--r--   0        0        0    18091 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/dict/adult_keywords_ja.txt
--rw-r--r--   0        0        0      426 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/dict/advertisement_keywords_ja.txt
--rw-r--r--   0        0        0     1740 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/dict/discrimination_keywords_ja.txt
--rw-r--r--   0        0        0       67 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/dict/dummy_ng_words.txt
--rw-r--r--   0        0        0      577 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/dict/header_footer_keywords_ja.txt
--rw-r--r--   0        0        0      665 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/dict/violence_keywords_ja.txt
--rw-r--r--   0        0        0      711 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/filters/__init__.py
--rw-r--r--   0        0        0    11980 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/filters/deduplication.py
--rw-r--r--   0        0        0    21705 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/filters/document_filters.py
--rw-r--r--   0        0        0     1572 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/filters/token_filters.py
--rw-r--r--   0        0        0     2520 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/filters/tokenization.py
--rw-r--r--   0        0        0        0 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/py.typed
--rw-r--r--   0        0        0      595 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/utils/__init__.py
--rw-r--r--   0        0        0     1716 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/utils/io_iter.py
--rw-r--r--   0        0        0     3335 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/utils/load_compose.py
--rw-r--r--   0        0        0     1299 2023-06-07 06:57:14.583551 hojichar-0.5.3/hojichar/utils/process.py
--rw-r--r--   0        0        0     1560 2023-06-07 06:57:36.547757 hojichar-0.5.3/pyproject.toml
--rw-r--r--   0        0        0    11881 1970-01-01 00:00:00.000000 hojichar-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-14 04:13:08.916324 hojichar-0.6.0/LICENSE
+-rw-r--r--   0        0        0    13408 2023-07-14 04:13:08.916324 hojichar-0.6.0/README.md
+-rw-r--r--   0        0        0      547 2023-07-14 04:13:30.906187 hojichar-0.6.0/hojichar/__init__.py
+-rw-r--r--   0        0        0     3261 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/__main__.py
+-rw-r--r--   0        0        0       42 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/core/__init__.py
+-rw-r--r--   0        0        0     4331 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/core/composition.py
+-rw-r--r--   0        0        0     5269 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/core/filter_interface.py
+-rw-r--r--   0        0        0     4914 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/core/inspection.py
+-rw-r--r--   0        0        0     1087 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/core/models.py
+-rw-r--r--   0        0        0      147 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/dict/__init__.py
+-rw-r--r--   0        0        0      941 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/dict/adult_keywords_en.txt
+-rw-r--r--   0        0        0    18091 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/dict/adult_keywords_ja.txt
+-rw-r--r--   0        0        0      426 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/dict/advertisement_keywords_ja.txt
+-rw-r--r--   0        0        0     1740 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/dict/discrimination_keywords_ja.txt
+-rw-r--r--   0        0        0       67 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/dict/dummy_ng_words.txt
+-rw-r--r--   0        0        0      577 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/dict/header_footer_keywords_ja.txt
+-rw-r--r--   0        0        0      665 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/dict/violence_keywords_ja.txt
+-rw-r--r--   0        0        0      711 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/filters/__init__.py
+-rw-r--r--   0        0        0    12104 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/filters/deduplication.py
+-rw-r--r--   0        0        0    23692 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/filters/document_filters.py
+-rw-r--r--   0        0        0     1606 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/filters/token_filters.py
+-rw-r--r--   0        0        0     2530 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/filters/tokenization.py
+-rw-r--r--   0        0        0        0 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/py.typed
+-rw-r--r--   0        0        0      595 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/utils/__init__.py
+-rw-r--r--   0        0        0     1716 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/utils/io_iter.py
+-rw-r--r--   0        0        0     3380 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/utils/load_compose.py
+-rw-r--r--   0        0        0     1920 2023-07-14 04:13:08.916324 hojichar-0.6.0/hojichar/utils/process.py
+-rw-r--r--   0        0        0     1714 2023-07-14 04:13:30.902187 hojichar-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    14141 1970-01-01 00:00:00.000000 hojichar-0.6.0/PKG-INFO
```

### Comparing `hojichar-0.5.3/LICENSE` & `hojichar-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.3/README.md` & `hojichar-0.6.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -128,27 +128,29 @@
   ```bash
   cat <your_text.jsonl> | hojichar -p your_preprocessing_profile.py -o your_text_preprocessed.jsonl
   ```
 
 - `hojichar --help`
 
   ```man
-  usage: hojichar [-h] --profile <your_filter.py> [--output OUTPUT] [--dump-stats <path to stats.json>] [--exit-on-error] [--args ARGS [ARGS ...]]
-  
-  options:
+
+    options:
     -h, --help            show this help message and exit
-    --profile <your_filter.py>, -p <your_filter.py>
-                          Path to a Python file that implements your custom filter. hojichar.Compose must be defined as FILTER variable in the file.
+    --profile <profile.py>, -p <profile.py>
+                            Path to a Python file that implements your custom filter.
+    --args ARGS [ARGS ...]
+                            Pass additional arguments to the profile. Use it like `--args arg1 arg2` etc. The arguments should be space-separated.
     --output OUTPUT, -o OUTPUT
-                          Output file path. If not given, stdout is used.
+                            Specifies the path for the output file. Defaults to standard output.
     --dump-stats <path to stats.json>
-                          Dump statistics to a file.
+                            Dump statistics to file. If the file exists, it will be appended.
     --exit-on-error       Exit if an exception occurs during filtering. Useful for debugging custom filters.
-    --args ARGS [ARGS ...]
-                          Argument for the profile which receives arguments.
+    --redirect-stdout REDIRECT_STDOUT
+                            This option is used to redirect standard output to a specified file during the profile. By default, it redirects to /dev/null.
+
   ```
 
 ## Definition of Profile
 
 - HojiChar CLI receives a series of preprocessing as a profile.
 - The preprocessing profile is provided as a Python file. Two patterns of the file are allowed.
 - hojichar.utils.load_compose.load_compose() loads these profile.
@@ -229,56 +231,108 @@
           ]
       )
   
   # FACTORY must be callable which returns Compose object.
   FACTORY = callback
   ```
 
-  - Using `FACTORY` profile with arguments in CLI.
+- Using `FACTORY` profile with arguments in CLI.
 
     ```bash
     cat <your_file> | hojichar -p example_profile.py --args arg1 arg2
     ```
 
 - `hojichar.utils.load_compose.load_parametrized_filter_from_file()` or `load_factory_from_file` loads this type of profile.
 
 ## For Developers
 
-**Local Installation with Poetry**
+### Installing from the Source Directory
 
-Requirements: `python >= 3.8, poetry >= 1.2`
-
-To install the package, run the following commands:
+To install the package, execute the following commands:
 
 ```
 git clone https://github.com/HojiChar/HojiChar.git
 cd HojiChar
 poetry install
 ```
 
-For installing development-related packages, you can run:
+To install packages related to development, use:
 
 ```
-poetry install --extras "dev lint test"
+poetry install --extras "dev lint test doc"
 ```
 
 ### Testing
 
-You can run the tests with:
+Some filters incorporate doctests. You can run these tests with the command:
 
 ```
 pytest --doctest-modules .
 ```
 
-This will execute both mypy and pytest tests.
+This command should be executed from the root of the project.
+
+### Code style
 
-Linting can be done using:
+- HojiChar requires type hints for all code. Type checking is performed in continuous integration (CI) in addition to the pytest tests.
+- HojiChar code is subject to inspection by the Flake8 Linter and is formatted using Black and isort. For configuration details, please refer to `pyproject.toml`. You can perform linting and formatting from the root of the project using the following commands:
+
+Linting
 
 ```
 poetry run task lint
 ```
 
-And for formatting:
+Formtatting
 
 ```
 poetry run task format
 ```
+
+### Building the Documentation
+
+We use Pdoc for building the documentation. You can build the documentation using the following command:
+
+```
+pdoc -o docs hojichar
+```
+
+Run this command from the project root.
+
+In practice, the process of building the documentation is automated by CI. When a Pull Request is merged into the main branch, the documentation is built in the `docs/` directory of the `docs` branch. This directory is then deployed to the official documentation site by GitHub Pages.
+
+### Creating a Source Tarball
+
+To create a source tarball, for instance, for packaging or distribution, run the following command:
+
+```
+poetry build
+```
+
+The tarball will be created in the dist directory. This command will compile the source code, and the resulting tarball can be installed with no additional dependencies other than the Python standard library.
+
+### Creating a Release and Uploading it to PyPI
+
+This command is primarily used by the project manager to create a release and upload it to PyPI.
+
+Versions uploaded to PyPI are identified by git tags. The `__version__` variable in `__init__.py` or the `version` entry in `pyproject.toml` are ignored. The `poetry-dynamic-versioning` Poetry plugin is used to implement this process.
+
+To add the plugin, use:
+
+```
+poetry self add "poetry-dynamic-versioning[plugin]"
+```
+
+The steps to push to PyPI are as follows, although in actuality, the process is automated by CI when a GitHub release is created from the tag.
+
+```
+git checkout v0.1.2
+poetry config pypi-token.pypi <API TOKEN>
+poetry build 
+poetry publish
+```
+
+The actual task for the manager is to apply the appropriate tag to the commit to be released and to create the release from GitHub:
+
+```
+git tag -a v0.1.2 -m "Version 0.1.2"
+```
```

### Comparing `hojichar-0.5.3/hojichar/__init__.py` & `hojichar-0.6.0/hojichar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 .. include:: ../README.md
 """
 from .core.composition import Compose
 from .core.filter_interface import Filter, TokenFilter
 from .core.models import Document, Token
 from .filters import deduplication, document_filters, token_filters, tokenization
 
-__version__ = "0.5.3"  # Replaced by poetry-dynamic-versioning when deploying
+__version__ = "0.6.0"  # Replaced by poetry-dynamic-versioning when deploying
 
 __all__ = [
     "core",
     "filters",
+    "utils",
     "Compose",
     "Filter",
     "TokenFilter",
     "Document",
     "Token",
     "deduplication",
     "document_filters",
```

### Comparing `hojichar-0.5.3/hojichar/__main__.py` & `hojichar-0.6.0/hojichar/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import argparse
 import json
 import logging
 import os
 import signal
 import sys
+from types import FrameType
+from typing import Optional
 
 import hojichar
 from hojichar.utils.io_iter import fileout_from_iter, stdin_iter, stdout_from_iter
 from hojichar.utils.load_compose import load_compose
-from hojichar.utils.process import process_iter
+from hojichar.utils.process import process_iter, reject_iter
 
 FILTER: hojichar.Compose
 logger = logging.getLogger("hojichar.__main__")
 
 
 def finalize() -> None:
     print(json.dumps(FILTER.statistics), file=sys.stderr, end="")
 
 
-def sigint_handler(signum, frame) -> None:
+# Typing of signal handler: https://github.com/python/typing/discussions/1042
+def sigint_handler(signum: int, frame: Optional[FrameType]) -> None:
     print(file=sys.stderr)
     finalize()
     sys.exit(0)
 
 
 def argparser() -> argparse.Namespace:
     parser = argparse.ArgumentParser()
@@ -60,14 +63,21 @@
     )
     parser.add_argument(
         "--redirect-stdout",
         default=None,
         help="This option is used to redirect standard output to a specified file during the \
         profile. By default, it redirects to /dev/null.",
     )
+    parser.add_argument(
+        "--all",
+        action="store_true",
+        default=False,
+        help="A flag that specifies whether to include discarded samples. \
+            This is useful when inspecting discarded samples.",
+    )
     args = parser.parse_args()
     return args
 
 
 def main() -> None:
     global FILTER
     signal.signal(signal.SIGINT, sigint_handler)
@@ -78,17 +88,18 @@
         stdout_fp = open(args.redirect_stdout, "w")
 
     FILTER = load_compose(
         args.profile,
         *tuple(args.args),
     )
     input_iter = stdin_iter()
-    out_str_iter = process_iter(
+    out_doc_iter = process_iter(
         input_iter=input_iter, filter=FILTER, exit_on_error=args.exit_on_error, stdout_fp=stdout_fp
     )
+    out_str_iter = reject_iter(input_iter=out_doc_iter, discard_rejected=not args.all)
     if args.output:
         with open(args.output, "w") as fp:
             fileout_from_iter(out_str_iter, fp)
     else:
         stdout_from_iter(out_str_iter)
     finalize()
     if args.dump_stats:
```

### Comparing `hojichar-0.5.3/hojichar/core/composition.py` & `hojichar-0.6.0/hojichar/core/composition.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,107 +1,107 @@
 import json
 import logging
-import numbers
 import pprint
-from typing import List, Union
+from typing import Any, List, Optional, Union
 
 import numpy as np
 
 from hojichar.core.filter_interface import Filter, TokenFilter
 from hojichar.core.inspection import Inspector, StatisticsCounter
 from hojichar.core.models import Document
 
 
+class BeforeProcessFilter(Filter):
+    def apply(self, doc: Document) -> Document:
+        return doc
+
+
 class Compose(Filter):
     def __init__(
         self,
         filters: List[Union[Filter, TokenFilter]],
-        ignore_filtered: bool = True,
-        random_state: Union[None, int, np.random.Generator] = None,
-        *args,
-        **kwargs,
+        random_state: Optional[Union[int, np.random.Generator]] = None,
+        *args: Any,
+        **kwargs: Any,
     ) -> None:
         """
         Compose a filter from pre-defined filter-objects.
+        Filter which has `skip_rejected` flag ignores a document which has `is_rejected` flag.
+        By doing so, Compose avoid applying filters that do not affect the output.
 
         Parameters
         ----------
         filters : List[Union[Filter, TokenFilter]]
             Filter instances which apply to the corpus.
 
-        ignore_filtered : bool, optional
-            Default = True
-            If True, filters ignore a document which has `is_rejected` flag.
-            By doing so, we avoid applying filters that do not affect the output.
-
-            However, for the purpose of corpus survay, e.g., to determine how many documents
-            in the corpus are removed by a certain filter, it is preferable not to be
-            affected by the upstream filter. In such a case, you should
-            set `ignore_filter` to False.
-
         random_state : Union[None, int, np.random.Generator], optional
             Default = None
             Seed for applying filters randomly.
             `random_state` must be int or np.random.Generator instance.
         """
         super().__init__(*args, **kwargs)
         self.filters = filters
-        self.filter_name_list = [f"{i}-{filt.name}" for i, filt in enumerate(self.filters)]
         self.logger = logging.getLogger("hojichar.Compose")
-        self.ignore_filtered = ignore_filtered
         self.before_process_inspector = Inspector(
-            target="before_process", ignore_filtered=ignore_filtered
+            target_filter=BeforeProcessFilter(), filter_idx=-1
         )
         self.inspectors = [
-            Inspector(target=name, ignore_filtered=ignore_filtered)
-            for name in self.filter_name_list
+            Inspector(target_filter=filter, filter_idx=idx)
+            for idx, filter in enumerate(self.filters)
         ]
-        self._statistics = StatisticsCounter(self.inspectors, ignore_filtered=self.ignore_filtered)
+        self._statistics = StatisticsCounter(self.inspectors)
 
         # Turn random_state into a `np.random.Generator` instance.
         if random_state is None:
             self.rng = np.random.default_rng()
-        elif isinstance(random_state, numbers.Integral):
+        elif isinstance(random_state, int):
             self.rng = np.random.default_rng(random_state)
         elif isinstance(random_state, np.random.Generator):
             self.rng = random_state
         else:
             raise ValueError(f"{random_state} cannot be used to seed.")
 
     def __call__(self, text: str) -> str:
         document = Document(text)
         document = self.apply(document)
-        return document.text
+        if document.is_rejected:
+            return ""
+        else:
+            return document.text
 
-    def apply(self, document: Document) -> Document:
-        document = self.before_process_inspector.apply(document)
-        for i, filt in enumerate(self.filters):
-            if (filt.p == 1) or (filt.p is None):
-                document = filt.filter_apply(document)
+    def _apply_filter(self, filt: Union[Filter, TokenFilter], document: Document) -> Document:
+        if document.is_rejected and filt.skip_rejected:
+            pass
+        else:
+            if filt.p == 1:
+                document = filt.apply_filter(document)
             else:
                 if self.rng.random() < filt.p:
-                    document = filt.filter_apply(document)
+                    document = filt.apply_filter(document)
+        return document
 
-            # If `ignore_filtered==False`, filters process a doc which is rejected
-            # Under the setting, each inspector always re-set `doc.is_rejected` to `False`.
-            document = self.inspectors[i].apply(document)
-
-        document.processed_text = document.text
-        if sum([inspector.is_rejected for inspector in self.inspectors]):
-            document.is_rejected = True
-            document.text = ""
+    def apply(self, document: Document) -> Document:
+        document = self.before_process_inspector.apply(document)
+        previous_inspector = self.before_process_inspector
+        for i, filt in enumerate(self.filters):
+            inspector = self.inspectors[i]
+            document = self._apply_filter(filt=filt, document=document)
+            document = inspector.apply(document)
+            if (not previous_inspector.is_rejected) and inspector.is_rejected:
+                document.reject_reason = filt.get_jsonalbe_vars(exclude_keys={"skip_rejected"})
+            previous_inspector = inspector
 
         self._statistics.update_changes(document, self.before_process_inspector, self.inspectors)
         return document
 
     @property
     def statistics(self) -> dict:
         return self._statistics.get_statistics()
 
-    def summary(self, format="print"):
+    def summary(self, format: str = "print") -> None:
         info = [
             {
                 "layer": i,
                 "name": filt.name,
                 "doc": filt.__doc__,
             }
             for i, filt in enumerate(self.filters)
```

### Comparing `hojichar-0.5.3/hojichar/core/inspection.py` & `hojichar-0.6.0/hojichar/core/inspection.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import dataclasses
 import logging
 import time
-from typing import List
+from typing import Any, Dict, List, Union
 
-from hojichar.core.filter_interface import Filter
+from hojichar.core.filter_interface import Filter, TokenFilter
 from hojichar.core.models import Document
 
 logger = logging.getLogger(__name__)
 
 
 class Inspector(Filter):
-    def __init__(self, target: str, ignore_filtered, *args, **kwargs):
+    def __init__(
+        self, target_filter: Union[Filter, TokenFilter], filter_idx: int, *args: Any, **kwargs: Any
+    ) -> None:
         super().__init__(*args, **kwargs)
         self.logger = logging.getLogger("hojichar.Inspector")
-        self.target = target
-        self.ignore_filtered = ignore_filtered
+        self.target_filter = target_filter
+        self.filter_idx = filter_idx
+        self.target = f"{filter_idx}-{target_filter.name}"
 
         self.is_rejected = False
         self.text_hash = 0
         self.tokens_hash = 0
 
     def apply(self, document: Document) -> Document:
         self.inspect(document)
-        if not self.ignore_filtered:
-            document.is_rejected = False
         return document
 
-    def inspect(self, document) -> None:
+    def inspect(self, document: Document) -> None:
         self.is_rejected = False
         self.is_rejected = document.is_rejected
         self.bytes = len(document.text.encode("utf-8"))
         self.time_ns = time.perf_counter_ns()
 
 
 @dataclasses.dataclass
@@ -39,15 +40,15 @@
     diff_bytes: int = 0
     cumulative_time_ns: int = 0
 
     def get_human_readable_values(self) -> dict:
         ret = {
             "discard_num": self.discard_num,
             "diff_MB": (self.diff_bytes / 1048576),
-            "cumlative_time": (self.cumulative_time_ns / 10**9),
+            "cumulative_time": (self.cumulative_time_ns / 10**9),
         }
         return ret
 
 
 @dataclasses.dataclass
 class DocStatistics:
     processed_num: int = 0
@@ -66,78 +67,73 @@
             "cumulative_time": (self.cumulative_time_ns / 10**9),
             "total_token_num": self.total_token_num,
         }
         return ret
 
 
 class StatisticsCounter:
-    def __init__(self, inspectors: List[Inspector], ignore_filtered):
+    def __init__(self, inspectors: List[Inspector]) -> None:
         counts = dict()
+        self.inspectors = inspectors
         for inspector in inspectors:
             counts[inspector.target] = FilterStatistics()
         self.counts = counts
         self.doc_counts = DocStatistics()
-        self.ignore_filtered = ignore_filtered
 
     def update_changes(
         self,
         document: Document,
         before_process_inspector: Inspector,
         inspectors: List[Inspector],
     ) -> None:
 
+        # Counting statistics for each filter
         previous_inspector = before_process_inspector
         for idx, inspector in enumerate(inspectors):
-            # logging how many docs are discarded in each filter.
-            if self.ignore_filtered:
-                if (not previous_inspector.is_rejected) and inspector.is_rejected:
-                    self.counts[inspector.target].discard_num += 1
-            else:
-                if inspector.is_rejected:
-                    self.counts[inspector.target].discard_num += 1
+            # Logging how many docs are discarded in each filter
+            if (not previous_inspector.is_rejected) and inspector.is_rejected:
+                self.counts[inspector.target].discard_num += 1
 
             # logging how much volume of docs are changed in each filter.
-            if self.ignore_filtered:
-                if (not previous_inspector.is_rejected) and inspector.is_rejected:
-                    diff_bytes = -inspector.bytes
-                elif previous_inspector.is_rejected and inspector.is_rejected:
-                    diff_bytes = 0
-                else:
-                    diff_bytes = inspector.bytes - previous_inspector.bytes
+            if (not previous_inspector.is_rejected) and inspector.is_rejected:
+                diff_bytes = -inspector.bytes
+            elif previous_inspector.is_rejected and inspector.is_rejected:
+                diff_bytes = 0
             else:
-                if inspector.is_rejected:
-                    diff_bytes = -inspector.bytes
-                else:
-                    diff_bytes = inspector.bytes - previous_inspector.bytes
+                diff_bytes = inspector.bytes - previous_inspector.bytes
 
             self.counts[inspector.target].diff_bytes += diff_bytes
 
             process_time_ns = inspector.time_ns - previous_inspector.time_ns
             self.counts[inspector.target].cumulative_time_ns += process_time_ns
 
             previous_inspector = inspector
 
+        # Counting total statistics
         self.doc_counts.processed_num += 1
         self.doc_counts.discard_num += (
             1 if sum([inspector.is_rejected for inspector in inspectors]) > 0 else 0
         )
         self.doc_counts.input_bytes += len(document.original.encode("utf-8"))
-        self.doc_counts.output_bytes += len(document.text.encode("utf-8"))
+        self.doc_counts.output_bytes += (
+            0 if document.is_rejected else len(document.text.encode("utf-8"))
+        )
         self.doc_counts.cumulative_time_ns += inspectors[-1].time_ns - inspectors[0].time_ns
         self.doc_counts.total_token_num += len(document.tokens)
 
     def get_statistics(self) -> dict:
         # about_layers = dict()
         about_layers = []
-        for filter_name, stats in self.counts.items():
+        for idx, (filter_name, stats) in enumerate(self.counts.items()):
             # about_layers[key] = self.counts[key].get_human_readable_values()
-            item = dict()
+            item: Dict[str, Any] = dict()
             item["name"] = filter_name
             stats = self.counts[filter_name]
             for key, stat in stats.get_human_readable_values().items():
                 item[key] = stat
+            item["params"] = self.inspectors[idx].target_filter.get_jsonalbe_vars()
             about_layers.append(item)
 
         return {
             "total_info": self.doc_counts.get_human_readable_values(),
             "layers_info": about_layers,
         }
```

### Comparing `hojichar-0.5.3/hojichar/core/models.py` & `hojichar-0.6.0/hojichar/core/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,42 @@
-from typing import List
+from typing import Any, Dict, List, Optional
 
 
 class Token:
-    def __init__(self, text: str, is_rejected=False) -> None:
+    def __init__(self, text: str, is_rejected: bool = False) -> None:
         self.text = text
         self.__original = text
         self.is_rejected = is_rejected
 
     @property
     def original(self) -> str:
         return self.__original
 
+    def __str__(self) -> str:
+        return self.text
+
 
 class Document:
-    def __init__(self, text: str, is_rejected=False, tokens=None) -> None:
+    def __init__(
+        self, text: str, is_rejected: bool = False, tokens: Optional[List[Token]] = None
+    ) -> None:
         self.text = text
         self.__original = text
         self.is_rejected = is_rejected
-        self.processed_text = ""
         if tokens is None:
             self.tokens: List[Token] = []
 
         self.dedup_lsh: List[str] = []
+        self.reject_reason: Dict[str, Any] = {}
 
     @property
     def original(self) -> str:
         return self.__original
 
     def set_tokens(self, tokens: List[str]) -> None:
         self.tokens = [Token(token) for token in tokens]
 
     def get_tokens(self) -> List[str]:
         return [token.text for token in self.tokens]
+
+    def __str__(self) -> str:
+        return self.text
```

### Comparing `hojichar-0.5.3/hojichar/dict/adult_keywords_en.txt` & `hojichar-0.6.0/hojichar/dict/adult_keywords_en.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.3/hojichar/dict/adult_keywords_ja.txt` & `hojichar-0.6.0/hojichar/dict/adult_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.3/hojichar/dict/discrimination_keywords_ja.txt` & `hojichar-0.6.0/hojichar/dict/discrimination_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.3/hojichar/dict/header_footer_keywords_ja.txt` & `hojichar-0.6.0/hojichar/dict/header_footer_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.3/hojichar/dict/violence_keywords_ja.txt` & `hojichar-0.6.0/hojichar/dict/violence_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.3/hojichar/filters/__init__.py` & `hojichar-0.6.0/hojichar/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.3/hojichar/filters/deduplication.py` & `hojichar-0.6.0/hojichar/filters/deduplication.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 文書の(近似)重複処理のためのモジュール.
 """
 import copy
-from typing import Callable, List
+from os import PathLike
+from typing import Any, Callable, List, Union
 
 import mmh3
 
 from hojichar.core.filter_interface import Filter
 from hojichar.core.models import Document
 
 
@@ -17,20 +18,20 @@
     2つの文書間で少なくとも1つのハッシュ値が一致する場合に重複として判定することができます。
     生成されたハッシュは `Document.dedup_lsh` 属性に文字列のリストとして保存されます。
     重複処理を実施する場合は、本フィルタを `hojichar.filters.deduplication.LSHDeduplicator` の前に適用します。
     """
 
     def __init__(
         self,
-        n_minhash=200,
-        n_gram=5,
-        n_buckets=20,
-        bucket_size=10,
-        *args,
-        **kwargs,
+        n_minhash: int = 200,
+        n_gram: int = 5,
+        n_buckets: int = 20,
+        bucket_size: int = 10,
+        *args: Any,
+        **kwargs: Any,
     ) -> None:
         super().__init__(*args, **kwargs)
         assert n_minhash == n_buckets * bucket_size
         self.N_MINHASH = n_minhash
         self.N_GRAM = n_gram
         self.N_BUCKETS = n_buckets
         self.BUCKET_SIZE = bucket_size
@@ -199,19 +200,19 @@
     `GenerateDedupLSH`で生成したハッシュ値が記録されていることを仮定します。
     `store_blacklist` フラグを `True` にすると、重複のあったハッシュ値を `LSHDeduplicator.blacklist` 属性に 文字列の集合として記録します。
     このオプションは、ブラックリストのハッシュ値のファイルの作成時などに有効です。`store_blacklist` フラグのデフォルト値は `False`です。
     """
 
     def __init__(
         self,
-        online_dedup=True,
-        blacklist_path="",
-        store_blacklist=False,
-        *args,
-        **kwargs,
+        online_dedup: bool = True,
+        blacklist_path: Union[str, PathLike] = "",
+        store_blacklist: bool = False,
+        *args: Any,
+        **kwargs: Any,
     ) -> None:
         super().__init__(*args, **kwargs)
         self.online_dedup = online_dedup
         self.store_blacklist = store_blacklist
         self.seen = set()
         if blacklist_path:
             with open(blacklist_path) as fp:
```

### Comparing `hojichar-0.5.3/hojichar/filters/document_filters.py` & `hojichar-0.6.0/hojichar/filters/document_filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 import logging
 import pathlib
 import re
 import time
 import unicodedata
+from os import PathLike
+from typing import Any, Optional, Union
 
 import hojichar
 from hojichar.core.filter_interface import Filter
 from hojichar.core.models import Document, Token
 
 BASE_PATH = pathlib.Path(hojichar.__path__[0])
 logger = logging.getLogger(__name__)
@@ -24,15 +26,15 @@
         document.text += "<hojichar>"
         return document
 
 
 class ExampleDiscardDocumentContainKeyword(Filter):
     """特定のキーワードを持つドキュメントを破棄するようなフィルタの実装例です."""
 
-    def __init__(self, keyword: str, *args, **kwargs):
+    def __init__(self, keyword: str, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.keyword = keyword
 
     def apply(self, document: Document) -> Document:
         """
         >>> ExampleDiscardDocumentContainKeyword("バカ").apply(Document("あいつはバカだ")).is_rejected
         True
@@ -41,40 +43,40 @@
             document.is_rejected = True
         return document
 
 
 class Identity(Filter):
     """何も変化を加えないフィルタです. テスト・デバッグに用いられます."""
 
-    def apply(self, document):
+    def apply(self, document: Document) -> Document:
         return document
 
 
 class DiscardAll(Filter):
     """
     すべてのドキュメントを破棄するフィルタです.
     テスト・デバッグに用いられます.
     """
 
-    def apply(self, document):
+    def apply(self, document: Document) -> Document:
         document.is_rejected = True
         return document
 
 
 class ApplyDiscard(Filter):
     """
     上流フィルタで破棄された`Document`を空文字列にします.
 
     `Document.is_rejected=True` の ドキュメントは無視されるため,
     このフィルタを `Compose` のコンストラクタに渡しても動作しません.
     このフィルタは主に`Compose` 内部や, `discard_filtered=False` を指定
     したデバッグ時などに利用されます.
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
 
     def apply(self, document: Document) -> Document:
         """
         >>> ApplyDiscard().apply(Document(text="hello", is_rejected=True)).text
         ''
         """
@@ -85,33 +87,33 @@
 
 
 class Sleep(Filter):
     """
     デバッグ用のフィルタです. 指定秒スリープします.
     """
 
-    def __init__(self, time: float = 1.0, *args, **kwargs) -> None:
+    def __init__(self, time: float = 1.0, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.time = time
 
-    def apply(self, document):
+    def apply(self, document: Document) -> Document:
         """
         >>> Sleep(0.1)('hello')  # After 0.1 seconds,
         'hello'
         """
         time.sleep(self.time)
         return document
 
 
 class DocumentNormalizer(Filter):
     """
     Unicode の正規化をします.
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
 
     def apply(self, document: Document) -> Document:
         document.text = unicodedata.normalize("NFKC", document.text)
         return document
 
 
@@ -121,15 +123,15 @@
     doument に格納します.デフォルトの `key` は 'text' です.
 
     Json の読み込み, あるいは `key` の読み込みに失敗した際には例外を送出します.
     これらを無視する場合は, `ignore=True` にします. その際, 読み込みに失敗
     したドキュメントは破棄されます.
     """
 
-    def __init__(self, key="text", ignore=False, *args, **kwargs):
+    def __init__(self, key: str = "text", ignore: bool = False, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.key = key
         self.ignore = ignore
 
     def apply(self, document: Document) -> Document:
         """
         >>> JSONLoader()( '{"text": "hello, world", "words": 2}' )
@@ -159,35 +161,68 @@
                 raise e
 
         return document
 
 
 class JSONDumper(Filter):
     """
-    Doucment.text の値を, エントリ名が "text" という名前の Json に格納します.
-    出力が json lines 欲しいときに Compose の出力前に使用します.
+    Document.text の文字列を json に変換します.
+    必要に応じ Document のメタデータを付与します.
     """
 
+    def __init__(
+        self,
+        dump_reason: bool = False,
+        p: float = 1,
+        skip_rejected: bool = False,
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
+        """
+        Args:
+            dump_reason (bool, optional): `is_rejected`, `reason` エントリをダンプします. Defaults to False.
+            p (float, optional): Apply probability. Defaults to 1.
+            skip_rejected (bool, optional): 破棄済みサンプルを排除しません.
+        """
+        super().__init__(p, skip_rejected, *args, **kwargs)
+        self.dump_reason = dump_reason
+
     def apply(self, document: Document) -> Document:
         """
         >>> JSONDumper()("hojichar")
         '{"text": "hojichar"}'
         """
         text = document.text
-        document.text = json.dumps({"text": text}, ensure_ascii=False)
+        if self.dump_reason:
+            document.text = json.dumps(
+                {
+                    "text": text,
+                    "is_rejected": document.is_rejected,
+                    "reason": document.reject_reason,
+                },
+                ensure_ascii=False,
+            )
+        else:
+            document.text = json.dumps({"text": text}, ensure_ascii=False)
         return document
 
 
 class DocumentLengthFilter(Filter):
     """
     `min_doc_len`, `max_doc_len` で指定した上限・下限の範囲内にないドキュメントを破棄します.
     デフォルトでは 200字 以上 50000字以内のテキストが受理されます.
     """
 
-    def __init__(self, min_doc_len=None, max_doc_len=None, *args, **kwargs):
+    def __init__(
+        self,
+        min_doc_len: Optional[int] = None,
+        max_doc_len: Optional[int] = None,
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
         super().__init__(*args, **kwargs)
 
         self.min_doc_len = min_doc_len
         self.max_doc_len = max_doc_len
 
     def apply(self, doc: Document) -> Document:
         """
@@ -211,15 +246,21 @@
     ファイルは単語が改行で羅列されたテキストファイルです.
 
     `ignore_confused` を `True` にすると,
     偽陽性を軽減するために, カタカナのNGワードは前後にカタカナが無い場合のみNG判定されます.
     デフォルト値は `False` です.
     """
 
-    def __init__(self, dict_path, ignore_confused=False, *args, **kwargs):
+    def __init__(
+        self,
+        dict_path: Union[str, PathLike],
+        ignore_confused: bool = False,
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
         super().__init__(*args, **kwargs)
 
         with open(dict_path, encoding="utf-8") as fp:
             ng_words = fp.read().split("\n")
         ng_words = [w.strip() for w in ng_words if not len(w) == 0]
 
         if ignore_confused:
@@ -236,27 +277,33 @@
             self.keyword_pat = re.compile(pat)
         else:
             ng_words = [re.escape(w) for w in ng_words]
             pat = "|".join(ng_words)
             self.keyword_pat = re.compile(pat)
 
     def apply(self, doc: Document) -> Document:
-        if self.keyword_pat.search(doc.text):
+        regex_match = self.keyword_pat.search(doc.text)
+        if regex_match:
             doc.is_rejected = True
+            self.matched_text = regex_match.group()
+            self.matched_text_neighbor = doc.text[
+                regex_match.start() - 20 : regex_match.end() + 20
+            ]
+
         return doc
 
 
 class NgWordsFilterEn(Filter):
     """
     英語のNGワード(および不適切語)を含む文書を破棄します.
     `dict_path` で指定したファイルから, キーワードのリストを得ます.
     ファイルは単語が改行で羅列されたテキストファイルです.
     """
 
-    def __init__(self, dict_path, *args, **kwargs):
+    def __init__(self, dict_path: Union[str, PathLike], *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
 
         with open(dict_path, encoding="utf-8") as fp:
             ng_words = fp.read().split("\n")
         ng_words = [re.escape(w.strip()) for w in ng_words if not len(w) == 0]
         pat = "|".join(ng_words)
         # 英語のパターンにマッチするようにしている, \s[単語]\s や [単語]. [単語], などにマッチ.
@@ -272,15 +319,20 @@
     """
     日本語のアダルトキーワード(および不適切語)を含む文書を破棄します.
     `dict_path` で指定したファイルから, キーワードのリストを得ます.
     ファイルは単語が改行で羅列されたテキストファイルです.
     デフォルトの`dict_path` は /hojichar/dict/adult_keywords_ja.txt です.
     """
 
-    def __init__(self, dict_path=BASE_PATH / "dict/adult_keywords_ja.txt", *args, **kwargs):
+    def __init__(
+        self,
+        dict_path: Union[str, PathLike] = BASE_PATH / "dict/adult_keywords_ja.txt",
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
         super().__init__(dict_path, *args, **kwargs)
 
     def apply(self, doc: Document) -> Document:
         """
         >>> DiscardAdultContentJa().apply(Document("<TEST_STRING_OF_ADULT_KEYWORD>")).is_rejected
         True
 
@@ -299,15 +351,20 @@
     """
     英語のアダルトキーワード(および不適切語)を含む文書を破棄します.
     `dict_path` で指定したファイルから, キーワードのリストを得ます.
     ファイルは単語が改行で羅列されたテキストファイルです.
     デフォルトの`dict_path` は /hojichar/dict/adult_keywords_en.txt です.
     """
 
-    def __init__(self, dict_path=BASE_PATH / "dict/adult_keywords_en.txt", *args, **kwargs):
+    def __init__(
+        self,
+        dict_path: Union[str, PathLike] = BASE_PATH / "dict/adult_keywords_en.txt",
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
         super().__init__(dict_path, *args, **kwargs)
 
     def apply(self, doc: Document) -> Document:
         """
         >>> DiscardAdultContentEn().apply(Document("<TEST_STRING_OF_ADULT_KEYWORD>")).is_rejected
         True
 
@@ -323,17 +380,17 @@
     `dict_path` で指定したファイルから, キーワードのリストを得ます.
     ファイルは単語が改行で羅列されたテキストファイルです.
     デフォルトの`dict_path` は /hojichar/dict/discrimination_keywords_ja.txt です.
     """
 
     def __init__(
         self,
-        dict_path=BASE_PATH / "dict/discrimination_keywords_ja.txt",
-        *args,
-        **kwargs,
+        dict_path: Union[str, PathLike] = BASE_PATH / "dict/discrimination_keywords_ja.txt",
+        *args: Any,
+        **kwargs: Any,
     ):
         super().__init__(dict_path, *args, **kwargs)
 
     def apply(self, doc: Document) -> Document:
         """
         >>> DiscardDiscriminationContentJa().\
             apply(Document("<TEST_STRING_OF_DISCRIMINATION_KEYWORD>")).is_rejected
@@ -349,15 +406,20 @@
     """
     日本語の暴力・脅迫を示唆するキーワードを含む文書を破棄します.
     `dict_path` で指定したファイルから, キーワードのリストを得ます.
     ファイルは単語が改行で羅列されたテキストファイルです.
     デフォルトの`dict_path` は /hojichar/dict/violence_keywords_ja.txt です.
     """
 
-    def __init__(self, dict_path=BASE_PATH / "dict/violence_keywords_ja.txt", *args, **kwargs):
+    def __init__(
+        self,
+        dict_path: Union[str, PathLike] = BASE_PATH / "dict/violence_keywords_ja.txt",
+        *args: Any,
+        **kwargs: Any,
+    ) -> None:
         super().__init__(dict_path, *args, **kwargs)
 
     def apply(self, doc: Document) -> Document:
         """
         >>> DiscardViolenceContentJa()\
             .apply(Document("<TEST_STRING_OF_VIOLENCE_KEYWORD>")).is_rejected
         True
@@ -372,23 +434,23 @@
     """
     正規表現 "BBS Patern" に `max_allow_num` 回よりたくさんマッチする文書を破棄します.
     `max_allow_num` のデフォルト値は14です.
     正規表現 "BBS Patern" は下記のリンクで検証可能です.
     https://regex101.com/r/ybQvL2/1
     """
 
-    def __init__(self, max_allowed_num=14, *args, **kwargs):
+    def __init__(self, max_allowed_num: int = 14, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
 
         self.max_allowed_num = max_allowed_num
         self.keyword_pat = re.compile(
             r"\d{4}[年\.\-\/][\ ]*\d{1,2}[月\.\-\/][\ ]*\d{1,2}[日]*|コメント|SOLD OUT|レビュー|投稿|ページ|\([月火水木金土日]\)|質問|\d+話|楽天市場|-"  # noqa
         )
 
-    def apply(self, doc):
+    def apply(self, doc: Document) -> Document:
         """
         >>> DiscardBBSComments().apply(Document("楽天市場 質問 投稿 コメント レビュー "*3)).is_rejected
         True
 
         >>> DiscardBBSComments().apply(Document("鏡餅")).is_rejected
         False
         """
@@ -396,27 +458,27 @@
         if len(bbs_factor) > self.max_allowed_num:
             doc.is_rejected = True
         return doc
 
 
 class DiscardAds(Filter):
     """
-    主に広告キーワーを`max_allow_num`より多く含む文書を破棄します.
+    主に広告キーワードを`max_allow_num`より多く含む文書を破棄します.
     デフォルトで`max_allow_num` は14です.
     `dict_path` で指定したファイルから, 広告キーワードのリストを得ます.
     ファイルは単語が改行で羅列されたテキストファイルです.
     デフォルトの`dict_path` は /hojichar/dict/advertisement_keywords_ja.txt です.
     """
 
     def __init__(
         self,
-        dict_path=BASE_PATH / "dict/advertisement_keywords_ja.txt",
-        max_allowed_num=14,
-        *args,
-        **kwargs,
+        dict_path: Union[str, PathLike] = BASE_PATH / "dict/advertisement_keywords_ja.txt",
+        max_allowed_num: int = 14,
+        *args: Any,
+        **kwargs: Any,
     ):
         super().__init__(*args, **kwargs)
 
         self.max_allow_num = max_allowed_num
         with open(dict_path, encoding="utf-8") as fp:
             ng_words = fp.read().split("\n")
         ng_words = [re.escape(w.strip()) for w in ng_words if not len(w) == 0]
@@ -440,15 +502,15 @@
 class AcceptJapanese(Filter):
     """
     日本語でないドキュメントを破棄します. 日本語判定は次の手順で行われます.
         1. テキストを左から`lookup_size` (デフォルトで50字) 参照し,
         ひらがな・カタカナが存在すれば日本語と判定する.
     """
 
-    def __init__(self, lookup_size=50, *args, **kwargs) -> None:
+    def __init__(self, lookup_size: int = 50, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
 
         self.lookup_size = 50
         self.hiragana_katakana_pat = re.compile(r"[ぁ-んァ-ン]")
 
     def apply(self, doc: Document) -> Document:
         """
@@ -471,15 +533,15 @@
     日本語でないドキュメントを破棄します. 日本語判定は次の手順で行われます
     ドキュメントを句点"。"で区切り, 平均文長が
     `max_avarage_sentence_length` より長い場合は破棄します.
     `max_avarage_sentence_length` のデフォルト値は100です.
     このフィルタは, 文章中の句点の割合が少なすぎるドキュメントを破棄します.
     """
 
-    def __init__(self, max_average_sentence_length=100, *args, **kwargs) -> None:
+    def __init__(self, max_average_sentence_length: int = 100, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
 
         self.max_average_sentence_length = max_average_sentence_length
         self.kuten_pat = re.compile(r"。")
 
     def apply(self, doc: Document) -> Document:
         """
@@ -503,17 +565,17 @@
     このフィルタを通す前に, 事前にセンテンスレベルにトーカナイズしておいてください.
     このフィルタでは Document.token にのみ変更が加えられるので, 出力前 あるいは 下流フィルタで
     Document.text に変更を加える前にトークンをマージしておいてください.
     """
 
     def __init__(
         self,
-        dict_path=BASE_PATH / "dict/header_footer_keywords_ja.txt",
-        *args,
-        **kwargs,
+        dict_path: Union[str, PathLike] = BASE_PATH / "dict/header_footer_keywords_ja.txt",
+        *args: Any,
+        **kwargs: Any,
     ) -> None:
         super().__init__(*args, **kwargs)
 
         with open(dict_path) as fp:
             keywords = fp.read().split("\n")
         keywords = [re.escape(w.strip()) for w in keywords if not len(w) == 0]
         self.keyword_pat = re.compile(r"|".join(keywords))
@@ -558,15 +620,15 @@
 
 
 class MaskPersonalInformation(Filter):
     """
     ドキュメントに含まれる電話番号・電子メールアドレスを一部マスキングします.
     """
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
 
         self.phone_pat = re.compile(
             r"((0|\+\d{1,3}[- ]?)(\d{2}[- ]?\d{4}[- ]?|\d[- ]?\d{4}[- ]?|\d{2}[- ]?\d{3}[- ]?|\d{3}[- ]?\d{2}[- ]?|\d{4}[- ]?\d{1}[- ]?))\d{4}"  # noqa
         )
         self.email_pat = re.compile(
             r"[a-zA-Z0-9!#$%&'*+\-/=?^_`{|}~.]+@[A-Za-z0-9!#$%&'*+\-/=?^_`{|}~.]+(\.[A-Za-z0-9\-]+)"  # noqa
```

### Comparing `hojichar-0.5.3/hojichar/filters/tokenization.py` & `hojichar-0.6.0/hojichar/filters/tokenization.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """
 
     def apply(self, document: Document) -> Document:
         tokens = self.tokenize(document.text)
         document.set_tokens(tokens)
         return document
 
-    def tokenize(self, text) -> List[str]:
+    def tokenize(self, text: str) -> List[str]:
         """
         >>> BlankCharTokenizer().tokenize("hello world")
         ['hello', 'world']
         """
         return text.split()
 
 
@@ -51,15 +51,15 @@
     """
 
     def apply(self, document: Document) -> Document:
         tokens = self.tokenize(document.text)
         document.set_tokens(tokens)
         return document
 
-    def tokenize(self, text) -> List[str]:
+    def tokenize(self, text: str) -> List[str]:
         """
         >>> SentenceTokenizer().tokenize("おはよう。おやすみ。ありがとう。さよなら。")
         ['おはよう。', 'おやすみ。', 'ありがとう。', 'さよなら。']
 
         >>> SentenceTokenizer().tokenize("さよなら。また来週")
         ['さよなら。', 'また来週']
         """
```

### Comparing `hojichar-0.5.3/hojichar/utils/__init__.py` & `hojichar-0.6.0/hojichar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.3/hojichar/utils/io_iter.py` & `hojichar-0.6.0/hojichar/utils/io_iter.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.5.3/hojichar/utils/load_compose.py` & `hojichar-0.6.0/hojichar/utils/load_compose.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     Returns:
         Callable[[Optional[Any]], hojichar.Compose]:
             An alias of the function which returns Compose.
     """
     sys.path.append(str(Path(profile_path).parent))
     module = _load_module(profile_path)
     if hasattr(module, "FACTORY"):
-        factory = getattr(module, "FACTORY")
+        factory: Callable[[Optional[Any]], hojichar.Compose] = getattr(module, "FACTORY")
         return factory
     else:
         raise NotImplementedError("FACTORY is not defined in the profile")
 
 
 def load_parametrized_filter_from_file(
     profile_path: Union[str, PathLike], *factory_args: str
```

### Comparing `hojichar-0.5.3/pyproject.toml` & `hojichar-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 [tool.poetry]
 name = "hojichar"
-version = "0.5.3" # Versioning by git tag dinamically with https://github.com/mtkennerly/poetry-dynamic-versioning
+version = "0.6.0" # Versioning by git tag dinamically with https://github.com/mtkennerly/poetry-dynamic-versioning
 description = "Text preprocessing management system."
 license = "Apache-2.0"
 authors = ["kenta.shinzato <hoppiece@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/HojiChar/HojiChar"
 repository = "https://github.com/HojiChar/HojiChar"
 
 [tool.poetry.scripts]
 hojichar = "hojichar.__main__:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-numpy = "^1.23.4"
-mmh3 = "^3.0.0"
+numpy = ">=1.17.0"
+mmh3 = "^4.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 black = "^22.3.0"
 flake8 = "^4.0.1"
 isort = "^5.10.1"
+mypy = "^1.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.2"
-mypy = ">=0.982"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 taskipy = "^1.10.3"
 
 
 [tool.poetry.group.doc.dependencies]
@@ -50,15 +50,21 @@
 line-length = 99
 
 [tool.isort]
 profile = "black"
 line_length = 99
 
 [tool.mypy]
-ignore_missing_imports = true
+disallow_untyped_defs = true
+disallow_any_unimported = true
+no_implicit_optional = true
+check_untyped_defs = true
+warn_return_any = true
+warn_unused_ignores = true
+show_error_codes = true
 
 [tool.taskipy.tasks]
 lint = "flake8 --show-source hojichar/ tests/ && isort --check-only --diff hojichar/ tests/"
 format = "black hojichar/ tests/ && isort hojichar/ tests"
 test = "pytest . --doctest-modules && mypy ."
 
 [tool.poetry-dynamic-versioning]
```

### Comparing `hojichar-0.5.3/PKG-INFO` & `hojichar-0.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: hojichar
-Version: 0.5.3
+Version: 0.6.0
 Summary: Text preprocessing management system.
 Home-page: https://github.com/HojiChar/HojiChar
 License: Apache-2.0
 Author: kenta.shinzato
 Author-email: hoppiece@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: mmh3 (>=3.0.0,<4.0.0)
-Requires-Dist: numpy (>=1.23.4,<2.0.0)
+Requires-Dist: mmh3 (>=4.0,<5.0)
+Requires-Dist: numpy (>=1.17.0)
 Project-URL: Repository, https://github.com/HojiChar/HojiChar
 Description-Content-Type: text/markdown
 
 # HojiChar
 
 [![PyPI version](https://badge.fury.io/py/hojichar.svg)](https://badge.fury.io/py/hojichar)
 [![Python Versions](https://img.shields.io/pypi/pyversions/hojichar.svg)](https://pypi.org/project/hojichar/)
@@ -148,27 +148,29 @@
   ```bash
   cat <your_text.jsonl> | hojichar -p your_preprocessing_profile.py -o your_text_preprocessed.jsonl
   ```
 
 - `hojichar --help`
 
   ```man
-  usage: hojichar [-h] --profile <your_filter.py> [--output OUTPUT] [--dump-stats <path to stats.json>] [--exit-on-error] [--args ARGS [ARGS ...]]
-  
-  options:
+
+    options:
     -h, --help            show this help message and exit
-    --profile <your_filter.py>, -p <your_filter.py>
-                          Path to a Python file that implements your custom filter. hojichar.Compose must be defined as FILTER variable in the file.
+    --profile <profile.py>, -p <profile.py>
+                            Path to a Python file that implements your custom filter.
+    --args ARGS [ARGS ...]
+                            Pass additional arguments to the profile. Use it like `--args arg1 arg2` etc. The arguments should be space-separated.
     --output OUTPUT, -o OUTPUT
-                          Output file path. If not given, stdout is used.
+                            Specifies the path for the output file. Defaults to standard output.
     --dump-stats <path to stats.json>
-                          Dump statistics to a file.
+                            Dump statistics to file. If the file exists, it will be appended.
     --exit-on-error       Exit if an exception occurs during filtering. Useful for debugging custom filters.
-    --args ARGS [ARGS ...]
-                          Argument for the profile which receives arguments.
+    --redirect-stdout REDIRECT_STDOUT
+                            This option is used to redirect standard output to a specified file during the profile. By default, it redirects to /dev/null.
+
   ```
 
 ## Definition of Profile
 
 - HojiChar CLI receives a series of preprocessing as a profile.
 - The preprocessing profile is provided as a Python file. Two patterns of the file are allowed.
 - hojichar.utils.load_compose.load_compose() loads these profile.
@@ -249,57 +251,109 @@
           ]
       )
   
   # FACTORY must be callable which returns Compose object.
   FACTORY = callback
   ```
 
-  - Using `FACTORY` profile with arguments in CLI.
+- Using `FACTORY` profile with arguments in CLI.
 
     ```bash
     cat <your_file> | hojichar -p example_profile.py --args arg1 arg2
     ```
 
 - `hojichar.utils.load_compose.load_parametrized_filter_from_file()` or `load_factory_from_file` loads this type of profile.
 
 ## For Developers
 
-**Local Installation with Poetry**
+### Installing from the Source Directory
 
-Requirements: `python >= 3.8, poetry >= 1.2`
-
-To install the package, run the following commands:
+To install the package, execute the following commands:
 
 ```
 git clone https://github.com/HojiChar/HojiChar.git
 cd HojiChar
 poetry install
 ```
 
-For installing development-related packages, you can run:
+To install packages related to development, use:
 
 ```
-poetry install --extras "dev lint test"
+poetry install --extras "dev lint test doc"
 ```
 
 ### Testing
 
-You can run the tests with:
+Some filters incorporate doctests. You can run these tests with the command:
 
 ```
 pytest --doctest-modules .
 ```
 
-This will execute both mypy and pytest tests.
+This command should be executed from the root of the project.
+
+### Code style
 
-Linting can be done using:
+- HojiChar requires type hints for all code. Type checking is performed in continuous integration (CI) in addition to the pytest tests.
+- HojiChar code is subject to inspection by the Flake8 Linter and is formatted using Black and isort. For configuration details, please refer to `pyproject.toml`. You can perform linting and formatting from the root of the project using the following commands:
+
+Linting
 
 ```
 poetry run task lint
 ```
 
-And for formatting:
+Formtatting
 
 ```
 poetry run task format
 ```
 
+### Building the Documentation
+
+We use Pdoc for building the documentation. You can build the documentation using the following command:
+
+```
+pdoc -o docs hojichar
+```
+
+Run this command from the project root.
+
+In practice, the process of building the documentation is automated by CI. When a Pull Request is merged into the main branch, the documentation is built in the `docs/` directory of the `docs` branch. This directory is then deployed to the official documentation site by GitHub Pages.
+
+### Creating a Source Tarball
+
+To create a source tarball, for instance, for packaging or distribution, run the following command:
+
+```
+poetry build
+```
+
+The tarball will be created in the dist directory. This command will compile the source code, and the resulting tarball can be installed with no additional dependencies other than the Python standard library.
+
+### Creating a Release and Uploading it to PyPI
+
+This command is primarily used by the project manager to create a release and upload it to PyPI.
+
+Versions uploaded to PyPI are identified by git tags. The `__version__` variable in `__init__.py` or the `version` entry in `pyproject.toml` are ignored. The `poetry-dynamic-versioning` Poetry plugin is used to implement this process.
+
+To add the plugin, use:
+
+```
+poetry self add "poetry-dynamic-versioning[plugin]"
+```
+
+The steps to push to PyPI are as follows, although in actuality, the process is automated by CI when a GitHub release is created from the tag.
+
+```
+git checkout v0.1.2
+poetry config pypi-token.pypi <API TOKEN>
+poetry build 
+poetry publish
+```
+
+The actual task for the manager is to apply the appropriate tag to the commit to be released and to create the release from GitHub:
+
+```
+git tag -a v0.1.2 -m "Version 0.1.2"
+```
+
```

