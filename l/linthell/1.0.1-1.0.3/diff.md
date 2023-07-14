# Comparing `tmp/linthell-1.0.1.tar.gz` & `tmp/linthell-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linthell-1.0.1.tar", max compression
+gzip compressed data, was "linthell-1.0.3.tar", max compression
```

## Comparing `linthell-1.0.1.tar` & `linthell-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0      146 2023-01-15 15:54:26.327833 linthell-1.0.1/linthell/__init__.py
--rw-r--r--   0        0        0      146 2023-01-15 15:54:26.327833 linthell-1.0.1/linthell/__main__.py
--rw-r--r--   0        0        0     2252 2023-01-15 15:54:26.328832 linthell-1.0.1/linthell/cli.py
--rw-r--r--   0        0        0       21 2023-01-15 15:54:26.328832 linthell-1.0.1/linthell/commands/__init__.py
--rw-r--r--   0        0        0     1220 2023-01-15 15:54:26.329839 linthell-1.0.1/linthell/commands/baseline.py
--rw-r--r--   0        0        0     2370 2023-01-15 15:54:26.329839 linthell-1.0.1/linthell/commands/lint.py
--rw-r--r--   0        0        0       51 2023-01-15 15:54:26.330832 linthell-1.0.1/linthell/commands/pre_commit/__init__.py
--rw-r--r--   0        0        0     1995 2023-01-15 15:54:26.330832 linthell-1.0.1/linthell/commands/pre_commit/baseline.py
--rw-r--r--   0        0        0      378 2023-01-15 15:54:26.330832 linthell-1.0.1/linthell/commands/pre_commit/cli.py
--rw-r--r--   0        0        0     2881 2023-01-15 15:54:26.330832 linthell-1.0.1/linthell/commands/pre_commit/lint.py
--rw-r--r--   0        0        0       18 2023-01-15 15:54:26.331831 linthell-1.0.1/linthell/utils/__init__.py
--rw-r--r--   0        0        0     1752 2023-01-15 15:54:26.331831 linthell-1.0.1/linthell/utils/config.py
--rw-r--r--   0        0        0     1103 2023-01-15 15:54:26.331831 linthell-1.0.1/linthell/utils/id_lines.py
--rw-r--r--   0        0        0      729 2023-01-15 15:54:26.332835 linthell-1.0.1/linthell/utils/linters.py
--rw-r--r--   0        0        0     1109 2023-01-15 15:54:26.332835 linthell-1.0.1/linthell/utils/pre_commit.py
--rw-r--r--   0        0        0      961 2023-01-15 16:01:57.969818 linthell-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3772 2023-01-15 15:54:26.326833 linthell-1.0.1/README.md
--rw-r--r--   0        0        0     4711 1970-01-01 00:00:00.000000 linthell-1.0.1/setup.py
--rw-r--r--   0        0        0     4447 1970-01-01 00:00:00.000000 linthell-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      146 2023-01-15 15:54:26.327833 linthell-1.0.3/linthell/__init__.py
+-rw-r--r--   0        0        0      146 2023-01-15 15:54:26.327833 linthell-1.0.3/linthell/__main__.py
+-rw-r--r--   0        0        0     2252 2023-01-15 15:54:26.328832 linthell-1.0.3/linthell/cli.py
+-rw-r--r--   0        0        0       21 2023-01-15 15:54:26.328832 linthell-1.0.3/linthell/commands/__init__.py
+-rw-r--r--   0        0        0     1220 2023-01-15 15:54:26.329839 linthell-1.0.3/linthell/commands/baseline.py
+-rw-r--r--   0        0        0     2370 2023-01-15 15:54:26.329839 linthell-1.0.3/linthell/commands/lint.py
+-rw-r--r--   0        0        0       51 2023-01-15 15:54:26.330832 linthell-1.0.3/linthell/commands/pre_commit/__init__.py
+-rw-r--r--   0        0        0     1995 2023-01-15 15:54:26.330832 linthell-1.0.3/linthell/commands/pre_commit/baseline.py
+-rw-r--r--   0        0        0      378 2023-01-15 15:54:26.330832 linthell-1.0.3/linthell/commands/pre_commit/cli.py
+-rw-r--r--   0        0        0     2881 2023-01-15 15:54:26.330832 linthell-1.0.3/linthell/commands/pre_commit/lint.py
+-rw-r--r--   0        0        0       18 2023-01-15 15:54:26.331831 linthell-1.0.3/linthell/utils/__init__.py
+-rw-r--r--   0        0        0     1752 2023-01-15 15:54:26.331831 linthell-1.0.3/linthell/utils/config.py
+-rw-r--r--   0        0        0     1179 2023-07-13 21:17:16.393275 linthell-1.0.3/linthell/utils/id_lines.py
+-rw-r--r--   0        0        0      708 2023-07-13 21:17:16.393275 linthell-1.0.3/linthell/utils/linters.py
+-rw-r--r--   0        0        0     1109 2023-01-15 15:54:26.332835 linthell-1.0.3/linthell/utils/pre_commit.py
+-rw-r--r--   0        0        0      961 2023-07-14 20:59:40.846598 linthell-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3772 2023-01-15 15:54:26.326833 linthell-1.0.3/README.md
+-rw-r--r--   0        0        0     4447 1970-01-01 00:00:00.000000 linthell-1.0.3/PKG-INFO
```

### Comparing `linthell-1.0.1/linthell/cli.py` & `linthell-1.0.3/linthell/cli.py`

 * *Files identical despite different names*

### Comparing `linthell-1.0.1/linthell/commands/baseline.py` & `linthell-1.0.3/linthell/commands/baseline.py`

 * *Files identical despite different names*

### Comparing `linthell-1.0.1/linthell/commands/lint.py` & `linthell-1.0.3/linthell/commands/lint.py`

 * *Files identical despite different names*

### Comparing `linthell-1.0.1/linthell/commands/pre_commit/baseline.py` & `linthell-1.0.3/linthell/commands/pre_commit/baseline.py`

 * *Files identical despite different names*

### Comparing `linthell-1.0.1/linthell/commands/pre_commit/lint.py` & `linthell-1.0.3/linthell/commands/pre_commit/lint.py`

 * *Files identical despite different names*

### Comparing `linthell-1.0.1/linthell/utils/config.py` & `linthell-1.0.3/linthell/utils/config.py`

 * *Files identical despite different names*

### Comparing `linthell-1.0.1/linthell/utils/id_lines.py` & `linthell-1.0.3/linthell/utils/id_lines.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 import re
 from pathlib import Path
 from typing import List
 
 
 def get_id_line(path: str, line: str, message: str) -> str:
     """Convert path, line and message to id line (path:code_line:message)."""
-    if not line:
-        code = ''
-    else:
+    code = ''
+    if line:
         lines = Path(path).read_text().splitlines()
-        if not lines:
-            code = ''
-        else:
-            code = lines[int(line) - 1]
+        if lines:
+            try:
+                code = lines[int(line) - 1]
+            except IndexError:
+                code = lines[-1]  # https://github.com/discrimy/linthell/issues/2
     normalized_path = Path(path).as_posix()
     return f'{normalized_path}:{code}:{message}'
 
 
 def get_id_lines(lint_output: str, regex: str) -> List[str]:
     """Search id lines from lint output via provided regex."""
     return [
```

### Comparing `linthell-1.0.1/linthell/utils/linters.py` & `linthell-1.0.3/linthell/utils/linters.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 ) -> str:
     """Execute linter command against files and return its output."""
     linter_process = subprocess.run(
         [*shlex.split(linter_command), *files],
         text=True,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
-        shell=True,
         check=False,
     )
     if linter_output == 'stdout':
         output = linter_process.stdout
     else:
         output = linter_process.stderr
     return output
```

### Comparing `linthell-1.0.1/linthell/utils/pre_commit.py` & `linthell-1.0.3/linthell/utils/pre_commit.py`

 * *Files identical despite different names*

### Comparing `linthell-1.0.1/pyproject.toml` & `linthell-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linthell"
-version = "1.0.1"
+version = "1.0.3"
 description = "Universal flakehell replacement for almost any linter you like"
 authors = ["Alexander Bespalov <discrimy.off@gmail.com>"]
 readme = "README.md"
 homepage = "https://gitea.discrimy.ru/discrimy/linthell"
 repository = "https://gitea.discrimy.ru/discrimy/linthell"
 
 [tool.poetry.scripts]
```

### Comparing `linthell-1.0.1/README.md` & `linthell-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `linthell-1.0.1/setup.py` & `linthell-1.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,115 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['linthell',
- 'linthell.commands',
- 'linthell.commands.pre_commit',
- 'linthell.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click>=8.1.3,<9.0.0', 'typing-extensions>=4.4.0,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['linthell = linthell:cli']}
-
-setup_kwargs = {
-    'name': 'linthell',
-    'version': '1.0.1',
-    'description': 'Universal flakehell replacement for almost any linter you like',
-    'long_description': '# linthell 🔥\nUniversal flakehell alternative that works with almost any linter you like.\n\n## How it works\nlinthell identifies each linter error as \n`(<file path>, <code at specific line>, <error message>)`, so it keep track\nof old errors even you add/delete some line from the same file. linthell\nstores there triplets inside baseline file.\n\nAt setup phase, you generate baseline file which identifies old errors.\nAfter that, linthell filters such errors and shows new only.\n\nIf you modify old code, then you should either fix these errors (refactor)\nor regenerate baseline. The tool\'s philosophy is that baseline should \nbe sharnk only, but how to deal with it is up to you.\n\n## Usage\nAll examples are shown with `flake8`, edit them for you case.\n\nAt first generate baseline file for every linter you use:\n```bash\nflake8 . | linthell baseline -b baseline-flake8.txt -f <linter regex>\n```\n\nThen lint your project via `linthell`:\n```bash\nflake8 . | linthell lint -b baseline-flake8.txt -f <linter regex>\n```\n\n## Custom linter format\nIf you use another linter then you must provide custom regex string\nstring to parse it\'s output. Default format is `flake8` default format.\nSome premade formats for linters:\n- `flake8`: `(?P<path>[a-zA-Z0-9\\._-]+(?:[\\\\/][a-zA-Z0-9\\._-]+)*):(?P<line>\\d+):\\d+: (?P<message>[^\\n]+)`\n- `pydocstyle`: `(?P<path>[a-zA-Z0-9\\._-]+(?:[\\\\/][a-zA-Z0-9\\._-]+)*):(?P<line>\\d+).+\\n\\s+(?P<message>[^\\n]+)`\n- `pylint`: `(?P<path>[a-zA-Z0-9\\._-]+(?:[\\\\/][a-zA-Z0-9\\._-]+)*):(?P<line>\\d+):\\d+: (?P<message>[^\\n]+)`\n\n### Create your own format regex\nYou can use your custom format regex. Suitable regex must\ncontains 3 named [python-like](https://docs.python.org/3/howto/regex.html#:~:text=The%20syntax%20for%20a%20named%20group%20is%20one%20of%20the%20Python%2Dspecific%20extensions%3A%20(%3FP%3Cname%3E...).%20name%20is%2C%20obviously%2C%20the%20name%20of%20the%20group) capturing groups: \n- `path` - relative file path \n- `line` - line number\n- `message` - linter message\n\nYour regex should matches all message related to an issue because \nunfiltered issues are printed by the whole match.\n\nYou can test your regex against linter output with [regexr](https://regexr.com/).\n\n## pre-commit support\nlinthell can be used as [pre-commit](https://pre-commit.com/) hook. Tested with\nflake8, pydocstyle, pylint, black linters.\n\n## Config file\n`linthell` can inject params from config file (`linthell --config path/to/config.ini`). \n`common` section applies for all commands, command specific config \nare specified by their name section, for example `[lint]`.\nNested commands are specified via dot. For example `linthell pre-commit lint`\nreads config from `[pre-commit.lint]` section.\n\nKeys must have same name as argument name of their command function. \nFor example, `baseline_file` and `lint_format`.\n\n\n## How to adapt linthell in project with pre-commit\n1. Create linthell config:\n```ini\n[common]\nbaseline_file=baseline.txt\nlint_format=(?P<path>[a-zA-Z0-9\\._-]+(?:[\\\\/][a-zA-Z0-9\\._-]+)*):(?P<line>\\d+):\\d+: (?P<message>[^\\n]+)\n\n[pre-commit.lint]\nlinter_command=flake8\n\n[pre-commit.baseline]\nlinter_command=flake8\n```\n2. Create a linthell hook inside `.pre-commit-config.yaml` file:\n```yaml\nrepos:\n  - repo: local\n    hooks:\n      - id: linthell\n        name: linthell flake8\n        entry: linthell --config linthell.ini pre-commit lint\n        language: system\n        types: [python]\n```\n3. Generate baseline file based on pre-commit hook definition and linthell config:\n```shell\nlinthell --config linthell.ini pre-commit baseline --hook-name "linthell flake8"\n```\n4. Validate new hook against generated baseline file\n```shell\npre-commit run --all linthell\n```',
-    'author': 'Alexander Bespalov',
-    'author_email': 'discrimy.off@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://gitea.discrimy.ru/discrimy/linthell',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: linthell
+Version: 1.0.3
+Summary: Universal flakehell replacement for almost any linter you like
+Home-page: https://gitea.discrimy.ru/discrimy/linthell
+Author: Alexander Bespalov
+Author-email: discrimy.off@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
+Project-URL: Repository, https://gitea.discrimy.ru/discrimy/linthell
+Description-Content-Type: text/markdown
+
+# linthell 🔥
+Universal flakehell alternative that works with almost any linter you like.
+
+## How it works
+linthell identifies each linter error as 
+`(<file path>, <code at specific line>, <error message>)`, so it keep track
+of old errors even you add/delete some line from the same file. linthell
+stores there triplets inside baseline file.
+
+At setup phase, you generate baseline file which identifies old errors.
+After that, linthell filters such errors and shows new only.
+
+If you modify old code, then you should either fix these errors (refactor)
+or regenerate baseline. The tool's philosophy is that baseline should 
+be sharnk only, but how to deal with it is up to you.
+
+## Usage
+All examples are shown with `flake8`, edit them for you case.
+
+At first generate baseline file for every linter you use:
+```bash
+flake8 . | linthell baseline -b baseline-flake8.txt -f <linter regex>
+```
+
+Then lint your project via `linthell`:
+```bash
+flake8 . | linthell lint -b baseline-flake8.txt -f <linter regex>
+```
+
+## Custom linter format
+If you use another linter then you must provide custom regex string
+string to parse it's output. Default format is `flake8` default format.
+Some premade formats for linters:
+- `flake8`: `(?P<path>[a-zA-Z0-9\._-]+(?:[\\/][a-zA-Z0-9\._-]+)*):(?P<line>\d+):\d+: (?P<message>[^\n]+)`
+- `pydocstyle`: `(?P<path>[a-zA-Z0-9\._-]+(?:[\\/][a-zA-Z0-9\._-]+)*):(?P<line>\d+).+\n\s+(?P<message>[^\n]+)`
+- `pylint`: `(?P<path>[a-zA-Z0-9\._-]+(?:[\\/][a-zA-Z0-9\._-]+)*):(?P<line>\d+):\d+: (?P<message>[^\n]+)`
+
+### Create your own format regex
+You can use your custom format regex. Suitable regex must
+contains 3 named [python-like](https://docs.python.org/3/howto/regex.html#:~:text=The%20syntax%20for%20a%20named%20group%20is%20one%20of%20the%20Python%2Dspecific%20extensions%3A%20(%3FP%3Cname%3E...).%20name%20is%2C%20obviously%2C%20the%20name%20of%20the%20group) capturing groups: 
+- `path` - relative file path 
+- `line` - line number
+- `message` - linter message
+
+Your regex should matches all message related to an issue because 
+unfiltered issues are printed by the whole match.
+
+You can test your regex against linter output with [regexr](https://regexr.com/).
+
+## pre-commit support
+linthell can be used as [pre-commit](https://pre-commit.com/) hook. Tested with
+flake8, pydocstyle, pylint, black linters.
+
+## Config file
+`linthell` can inject params from config file (`linthell --config path/to/config.ini`). 
+`common` section applies for all commands, command specific config 
+are specified by their name section, for example `[lint]`.
+Nested commands are specified via dot. For example `linthell pre-commit lint`
+reads config from `[pre-commit.lint]` section.
+
+Keys must have same name as argument name of their command function. 
+For example, `baseline_file` and `lint_format`.
+
+
+## How to adapt linthell in project with pre-commit
+1. Create linthell config:
+```ini
+[common]
+baseline_file=baseline.txt
+lint_format=(?P<path>[a-zA-Z0-9\._-]+(?:[\\/][a-zA-Z0-9\._-]+)*):(?P<line>\d+):\d+: (?P<message>[^\n]+)
+
+[pre-commit.lint]
+linter_command=flake8
+
+[pre-commit.baseline]
+linter_command=flake8
+```
+2. Create a linthell hook inside `.pre-commit-config.yaml` file:
+```yaml
+repos:
+  - repo: local
+    hooks:
+      - id: linthell
+        name: linthell flake8
+        entry: linthell --config linthell.ini pre-commit lint
+        language: system
+        types: [python]
+```
+3. Generate baseline file based on pre-commit hook definition and linthell config:
+```shell
+linthell --config linthell.ini pre-commit baseline --hook-name "linthell flake8"
+```
+4. Validate new hook against generated baseline file
+```shell
+pre-commit run --all linthell
+```
```

