# Comparing `tmp/cmdcomp-1.1.3.tar.gz` & `tmp/cmdcomp-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdcomp-1.1.3.tar", max compression
+gzip compressed data, was "cmdcomp-1.1.4.tar", max compression
```

## Comparing `cmdcomp-1.1.3.tar` & `cmdcomp-1.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1511 2023-07-11 01:55:54.610686 cmdcomp-1.1.3/README.md
--rw-r--r--   0        0        0       79 2023-07-11 01:55:54.610686 cmdcomp-1.1.3/cmdcomp/__init__.py
--rw-r--r--   0        0        0     2117 2023-07-11 01:55:54.610686 cmdcomp-1.1.3/cmdcomp/app.py
--rw-r--r--   0        0        0     1983 2023-07-11 01:55:54.610686 cmdcomp-1.1.3/cmdcomp/completion.py
--rw-r--r--   0        0        0        0 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/__init__.py
--rw-r--r--   0        0        0      540 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/app_info.py
--rw-r--r--   0        0        0      266 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/cmdcomp_info.py
--rw-r--r--   0        0        0        0 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/command/__init__.py
--rw-r--r--   0        0        0     3193 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/command/command.py
--rw-r--r--   0        0        0      348 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/command/option/__init__.py
--rw-r--r--   0        0        0      336 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/command/option/command_option.py
--rw-r--r--   0        0        0      378 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/command/option/file_option.py
--rw-r--r--   0        0        0      910 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/config.py
--rw-r--r--   0        0        0      115 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/config/model.py
--rw-r--r--   0        0        0      206 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/exception.py
--rw-r--r--   0        0        0       64 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/main.py
--rw-r--r--   0        0        0       81 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/shell_type.py
--rw-r--r--   0        0        0     1623 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/templates/bash.sh.jinja
--rw-r--r--   0        0        0     1169 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/cmdcomp/templates/zsh.sh.jinja
--rw-r--r--   0        0        0     1687 2023-07-11 01:55:54.614687 cmdcomp-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 cmdcomp-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1512 2023-07-14 15:11:02.127905 cmdcomp-1.1.4/README.md
+-rw-r--r--   0        0        0       79 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/__init__.py
+-rw-r--r--   0        0        0     2123 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/app.py
+-rw-r--r--   0        0        0     1983 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/completion.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/__init__.py
+-rw-r--r--   0        0        0      540 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/app_info.py
+-rw-r--r--   0        0        0      266 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/cmdcomp_info.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/command/__init__.py
+-rw-r--r--   0        0        0     3193 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/command/command.py
+-rw-r--r--   0        0        0      348 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/command/option/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/command/option/command_option.py
+-rw-r--r--   0        0        0      378 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/command/option/file_option.py
+-rw-r--r--   0        0        0      910 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/config.py
+-rw-r--r--   0        0        0      115 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/config/model.py
+-rw-r--r--   0        0        0      206 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/exception.py
+-rw-r--r--   0        0        0       64 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/main.py
+-rw-r--r--   0        0        0       81 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/shell_type.py
+-rw-r--r--   0        0        0     1732 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/templates/bash.sh.jinja
+-rw-r--r--   0        0        0     1277 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/cmdcomp/templates/zsh.sh.jinja
+-rw-r--r--   0        0        0     1700 2023-07-14 15:11:02.131905 cmdcomp-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 cmdcomp-1.1.4/PKG-INFO
```

### Comparing `cmdcomp-1.1.3/README.md` & `cmdcomp-1.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 docker run --rm -itv $(pwd):/app/cmdcomp yassun4dev/cmdcomp --file ${YOUR_CONFIG_FILE} --shell-type bash
 ```
 
 ## Config
 
 Configuration can be written in JSON, YAML, and TOML file formats.
 
+### Sample
+
 ```toml
 [cmdcomp]
 version = "1"
 
 [app]
 name = "mycli"
 alias = "my-cli"
@@ -57,12 +59,10 @@
 alias = ["restart", "shell", "log"]
 
 [root.subcommands.cd]
 options = { type = "file", base_path = "$(cd $(dirname $0); pwd)/../apps" }
 
 ```
 
-## JSON Schema
-
-### Config
+### JSON Schema
 
 https://raw.githubusercontent.com/yassun4dev/cmdcomp/main/docs/config.schema.json
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 # Command Completion Generator Tool
                   [Test_Suite] [PIP_Version] [Docker_Version]
 `cmdcomp` generate shell completion file (bash or zsh) from config toml file.
 ## Install ```shell pip install cmdcomp ``` ## Usage ### Local ```shell cmdcomp
 --file ${YOUR_CONFIG_FILE} --shell-type bash ``` ### Docker ```shell docker run
 --rm -itv $(pwd):/app/cmdcomp yassun4dev/cmdcomp --file ${YOUR_CONFIG_FILE} --
 shell-type bash ``` ## Config Configuration can be written in JSON, YAML, and
-TOML file formats. ```toml [cmdcomp] version = "1" [app] name = "mycli" alias =
-"my-cli" [root] options = ["-h", "--help", "--version"] [root.subcommands.list]
-options = ["-a"] alias = "ls" [root.subcommands.execute] options = { type =
-"command", execute = "your_app_name ps -s" } alias = ["restart", "shell",
-"log"] [root.subcommands.cd] options = { type = "file", base_path = "$(cd $
-(dirname $0); pwd)/../apps" } ``` ## JSON Schema ### Config https://
-raw.githubusercontent.com/yassun4dev/cmdcomp/main/docs/config.schema.json
+TOML file formats. ### Sample ```toml [cmdcomp] version = "1" [app] name =
+"mycli" alias = "my-cli" [root] options = ["-h", "--help", "--version"]
+[root.subcommands.list] options = ["-a"] alias = "ls"
+[root.subcommands.execute] options = { type = "command", execute =
+"your_app_name ps -s" } alias = ["restart", "shell", "log"]
+[root.subcommands.cd] options = { type = "file", base_path = "$(cd $(dirname
+$0); pwd)/../apps" } ``` ### JSON Schema https://raw.githubusercontent.com/
+yassun4dev/cmdcomp/main/docs/config.schema.json
```

### Comparing `cmdcomp-1.1.3/cmdcomp/app.py` & `cmdcomp-1.1.4/cmdcomp/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
         parser.add_argument(
             "--file",
             "-f",
             required=True,
             metavar="FILE",
             type=FileType("rb"),
-            help="config file (`json`, `yaml`, `toml` support).",
+            help="config file (`*.json`, `*.yaml`, `*.toml` support).",
         )
 
         parser.add_argument(
             "--shell-type",
             required=True,
             metavar="SHELL_TYPE",
             type=ShellType,
```

### Comparing `cmdcomp-1.1.3/cmdcomp/completion.py` & `cmdcomp-1.1.4/cmdcomp/completion.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.3/cmdcomp/config/app_info.py` & `cmdcomp-1.1.4/cmdcomp/config/app_info.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.3/cmdcomp/config/command/command.py` & `cmdcomp-1.1.4/cmdcomp/config/command/command.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.3/cmdcomp/config/config.py` & `cmdcomp-1.1.4/cmdcomp/config/config.py`

 * *Files identical despite different names*

### Comparing `cmdcomp-1.1.3/cmdcomp/templates/bash.sh.jinja` & `cmdcomp-1.1.4/cmdcomp/templates/bash.sh.jinja`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,41 @@
+{%- set func_name = "_" + app_name|replace("-","_") -%}
 #!/bin/bash
 
-_{{ app_name|replace("-","_") }}() {
+{{ func_name }}() {
     local cur prev words cword split
     _init_completion || return
 
     case $cword in
         1)
-            COMPREPLY=( $(compgen -W "{{ completions_list[0]|join(" ") }}" -- "$cur") ) ;;
+            COMPREPLY=( $(compgen -W "{{ completions_list[0]|join(" ") }}" -- "$cur") )
+            ;;
 {%- for completions in completions_list[1:] %}
         {{ loop.index + 1 }})
             case ${words[{{ loop.depth }}]} in
 {%- for name, completion in completions.items() recursive %}
                 {{ name }})
 {%- if completion is mapping %}
                     case ${words[{{ loop.depth + 1 }}]} in
 {{- loop(completion.items())|indent(width=8) }}
-                    esac ;;
+                    esac
+                    ;;
 {%- elif completion|first is mapping and 'command' in completion|first %}
-                    COMPREPLY=( $(compgen -W "{{ (completion|first).command }}" -- "$cur") ) ;;
+                    COMPREPLY=( $(compgen -W "{{ (completion|first).command }}" -- "$cur") )
+                    ;;
 {%- elif completion|first is mapping and 'file' in completion|first %}
-                    file_completion "{{ (completion|first).file }}" ;;
+                    file_completion "{{ (completion|first).file }}"
+                    ;;
 {%- else %}
-                    COMPREPLY=( $(compgen -W "{{ completion|join(" ") }}" -- "$cur") ) ;;
+                    COMPREPLY=( $(compgen -W "{{ completion|join(" ") }}" -- "$cur") )
+                    ;;
 {%- endif %}
 {%- endfor %}
-            esac ;;
+            esac
+            ;;
 {%- endfor %}
     esac
 }
 
 file_completion() {
     local cur prev cword opts
     _get_comp_words_by_ref -n : cur prev cword
@@ -36,11 +43,11 @@
     if test "${dir}" ;then
         COMPREPLY=( $(compgen -W "$(ls -F $1/${dir} | sed -E "s@(.*)@${dir}\1@g")" -- "${cur}") )
     else
         COMPREPLY=( $(compgen -W "$(ls -F $1/)" -- "${cur}") )
     fi
 }
 
-complete -F _{{ app_name|replace("-","_") }} {{ app_name }}
+complete -F {{ func_name }} {{ app_name }}
 {%- for app_alias in app_aliases %}
-complete -F _{{ app_name|replace("-","_") }} {{ app_alias }}
+complete -F {{ func_name }} {{ app_alias }}
 {%- endfor %}
```

### Comparing `cmdcomp-1.1.3/cmdcomp/templates/zsh.sh.jinja` & `cmdcomp-1.1.4/cmdcomp/templates/zsh.sh.jinja`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,41 @@
+{%- set func_name = "_" + app_name|replace("-","_") -%}
 #!/bin/zsh
 
-_{{ app_name|replace("-","_") }}() {
+{{ func_name }}() {
     shift words
 
     case "$(($CURRENT-1))" in
         1)
-            _values '{{ app_name }}' {{ completions_list[0]|join(" ") }} ;;
+            _values '{{ app_name }}' {{ completions_list[0]|join(" ") }}
+            ;;
 {%- for completions in completions_list[1:] %}
         {{ loop.index + 1 }})
             case ${words[{{ loop.depth }}]} in
 {%- for name, completion in completions.items() recursive %}
                 {{ name }})
 {%- if completion is mapping %}
                     case ${words[{{ loop.depth + 1 }}]} in
 {{- loop(completion.items())|indent(width=8) }}
-                    esac ;;
+                    esac
+                    ;;
 {%- elif completion|first is mapping and 'command' in completion|first %}
-                    _values '{{ name }}' {{ (completion|first).command }} ;;
+                    _values '{{ name }}' {{ (completion|first).command }}
+                    ;;
 {%- elif completion|first is mapping and 'file' in completion|first %}
-                    _files -W "{{ (completion|first).file }}" ;;
+                    _files -W "{{ (completion|first).file }}"
+                    ;;
 {%- else %}
-                    _values '{{ name }}' {{ completion|join(" ") }} ;;
+                    _values '{{ name }}' {{ completion|join(" ") }}
+                    ;;
 {%- endif %}
 {%- endfor %}
-            esac ;;
+            esac
+            ;;
 {%- endfor %}
     esac
 }
 
-compdef _{{ app_name|replace("-","_") }} {{ app_name }}
+compdef {{ func_name }} {{ app_name }}
 {%- for app_alias in app_aliases %}
-compdef _{{ app_name|replace("-","_") }} {{ app_alias }}
+compdef {{ func_name}} {{ app_alias }}
 {%- endfor %}
```

### Comparing `cmdcomp-1.1.3/pyproject.toml` & `cmdcomp-1.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmdcomp"
-version = "1.1.3"
+version = "1.1.4"
 description = "cmdcomp is a cli tool completion generator for shell."
 authors = ["Yasutanium <yassun4dev@outlook.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/yassun4dev/cmdcomp"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3 :: Only",
 ]
 
 [tool.poetry.scripts]
 cmdcomp = "cmdcomp.main:main"
 
 [tool.taskipy.tasks]
-generate-json-schema = "python docs/generate.py > docs/config.schema.json"
+generate-json-schema = "python tasks/generate_json_schema.py > docs/config.schema.json"
 test = "pytest"
 format = "black --target-version py310 ."
 lint = "pyright cmdcomp/** tests/**"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^2.0"
```

### Comparing `cmdcomp-1.1.3/PKG-INFO` & `cmdcomp-1.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdcomp
-Version: 1.1.3
+Version: 1.1.4
 Summary: cmdcomp is a cli tool completion generator for shell.
 Home-page: https://github.com/yassun4dev/cmdcomp
 License: BSD-3-Clause
 Author: Yasutanium
 Author-email: yassun4dev@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -57,14 +57,16 @@
 docker run --rm -itv $(pwd):/app/cmdcomp yassun4dev/cmdcomp --file ${YOUR_CONFIG_FILE} --shell-type bash
 ```
 
 ## Config
 
 Configuration can be written in JSON, YAML, and TOML file formats.
 
+### Sample
+
 ```toml
 [cmdcomp]
 version = "1"
 
 [app]
 name = "mycli"
 alias = "my-cli"
@@ -81,13 +83,11 @@
 alias = ["restart", "shell", "log"]
 
 [root.subcommands.cd]
 options = { type = "file", base_path = "$(cd $(dirname $0); pwd)/../apps" }
 
 ```
 
-## JSON Schema
-
-### Config
+### JSON Schema
 
 https://raw.githubusercontent.com/yassun4dev/cmdcomp/main/docs/config.schema.json
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cmdcomp Version: 1.1.3 Summary: cmdcomp is a cli
+Metadata-Version: 2.1 Name: cmdcomp Version: 1.1.4 Summary: cmdcomp is a cli
 tool completion generator for shell. Home-page: https://github.com/yassun4dev/
 cmdcomp License: BSD-3-Clause Author: Yasutanium Author-email:
 yassun4dev@outlook.com Requires-Python: >=3.11,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
@@ -13,14 +13,15 @@
 text/markdown # Command Completion Generator Tool
                   [Test_Suite] [PIP_Version] [Docker_Version]
 `cmdcomp` generate shell completion file (bash or zsh) from config toml file.
 ## Install ```shell pip install cmdcomp ``` ## Usage ### Local ```shell cmdcomp
 --file ${YOUR_CONFIG_FILE} --shell-type bash ``` ### Docker ```shell docker run
 --rm -itv $(pwd):/app/cmdcomp yassun4dev/cmdcomp --file ${YOUR_CONFIG_FILE} --
 shell-type bash ``` ## Config Configuration can be written in JSON, YAML, and
-TOML file formats. ```toml [cmdcomp] version = "1" [app] name = "mycli" alias =
-"my-cli" [root] options = ["-h", "--help", "--version"] [root.subcommands.list]
-options = ["-a"] alias = "ls" [root.subcommands.execute] options = { type =
-"command", execute = "your_app_name ps -s" } alias = ["restart", "shell",
-"log"] [root.subcommands.cd] options = { type = "file", base_path = "$(cd $
-(dirname $0); pwd)/../apps" } ``` ## JSON Schema ### Config https://
-raw.githubusercontent.com/yassun4dev/cmdcomp/main/docs/config.schema.json
+TOML file formats. ### Sample ```toml [cmdcomp] version = "1" [app] name =
+"mycli" alias = "my-cli" [root] options = ["-h", "--help", "--version"]
+[root.subcommands.list] options = ["-a"] alias = "ls"
+[root.subcommands.execute] options = { type = "command", execute =
+"your_app_name ps -s" } alias = ["restart", "shell", "log"]
+[root.subcommands.cd] options = { type = "file", base_path = "$(cd $(dirname
+$0); pwd)/../apps" } ``` ### JSON Schema https://raw.githubusercontent.com/
+yassun4dev/cmdcomp/main/docs/config.schema.json
```

