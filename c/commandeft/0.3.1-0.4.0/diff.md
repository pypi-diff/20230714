# Comparing `tmp/commandeft-0.3.1.tar.gz` & `tmp/commandeft-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commandeft-0.3.1.tar", last modified: Thu Jul 13 18:28:53 2023, max compression
+gzip compressed data, was "commandeft-0.4.0.tar", last modified: Fri Jul 14 13:43:57 2023, max compression
```

## Comparing `commandeft-0.3.1.tar` & `commandeft-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1078 2023-06-10 01:12:32.215348 commandeft-0.3.1/LICENSE
--rw-r--r--   0        0        0     3541 2023-07-13 06:12:07.752921 commandeft-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-06-11 23:37:24.840096 commandeft-0.3.1/commandeft/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 01:40:57.009549 commandeft-0.3.1/commandeft/constants/__init__.py
--rw-r--r--   0        0        0     3266 2023-07-13 18:28:25.093811 commandeft-0.3.1/commandeft/constants/consts.py
--rw-r--r--   0        0        0        0 2023-06-12 01:40:57.009834 commandeft-0.3.1/commandeft/core/__init__.py
--rw-r--r--   0        0        0     3103 2023-07-13 18:28:25.095039 commandeft-0.3.1/commandeft/core/cli.py
--rw-r--r--   0        0        0     1391 2023-07-13 06:12:07.757546 commandeft-0.3.1/commandeft/core/decision.py
--rw-r--r--   0        0        0     5054 2023-07-13 18:28:25.095963 commandeft-0.3.1/commandeft/core/generation.py
--rw-r--r--   0        0        0     2131 2023-07-13 06:12:07.759538 commandeft-0.3.1/commandeft/core/history_cache.py
--rw-r--r--   0        0        0      913 2023-07-13 06:12:07.760737 commandeft-0.3.1/commandeft/main.py
--rw-r--r--   0        0        0        0 2023-06-12 01:40:57.010171 commandeft-0.3.1/commandeft/util/__init__.py
--rw-r--r--   0        0        0     4933 2023-07-13 18:28:25.097250 commandeft-0.3.1/commandeft/util/config_util.py
--rw-r--r--   0        0        0      370 2023-07-13 06:12:07.762484 commandeft-0.3.1/commandeft/util/gen_util.py
--rw-r--r--   0        0        0     2349 2023-07-13 06:12:07.763340 commandeft-0.3.1/commandeft/util/interactive_util.py
--rw-r--r--   0        0        0     1995 2023-07-13 18:28:53.081965 commandeft-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5453 1970-01-01 00:00:00.000000 commandeft-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-10 01:12:32.215348 commandeft-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3541 2023-07-13 06:12:07.752921 commandeft-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-11 23:37:24.840096 commandeft-0.4.0/commandeft/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 01:40:57.009549 commandeft-0.4.0/commandeft/constants/__init__.py
+-rw-r--r--   0        0        0     3265 2023-07-14 13:43:43.639342 commandeft-0.4.0/commandeft/constants/consts.py
+-rw-r--r--   0        0        0        0 2023-06-12 01:40:57.009834 commandeft-0.4.0/commandeft/core/__init__.py
+-rw-r--r--   0        0        0     3065 2023-07-14 13:43:43.640135 commandeft-0.4.0/commandeft/core/cli.py
+-rw-r--r--   0        0        0     1477 2023-07-14 13:43:43.640917 commandeft-0.4.0/commandeft/core/decision.py
+-rw-r--r--   0        0        0     5054 2023-07-13 18:28:25.095963 commandeft-0.4.0/commandeft/core/generation.py
+-rw-r--r--   0        0        0     2131 2023-07-13 06:12:07.759538 commandeft-0.4.0/commandeft/core/history_cache.py
+-rw-r--r--   0        0        0      913 2023-07-13 06:12:07.760737 commandeft-0.4.0/commandeft/main.py
+-rw-r--r--   0        0        0        0 2023-06-12 01:40:57.010171 commandeft-0.4.0/commandeft/util/__init__.py
+-rw-r--r--   0        0        0     4961 2023-07-14 13:43:43.641629 commandeft-0.4.0/commandeft/util/config_util.py
+-rw-r--r--   0        0        0      370 2023-07-13 06:12:07.762484 commandeft-0.4.0/commandeft/util/gen_util.py
+-rw-r--r--   0        0        0     2438 2023-07-14 13:43:43.642519 commandeft-0.4.0/commandeft/util/interactive_util.py
+-rw-r--r--   0        0        0     1995 2023-07-14 13:43:57.206047 commandeft-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5453 1970-01-01 00:00:00.000000 commandeft-0.4.0/PKG-INFO
```

### Comparing `commandeft-0.3.1/LICENSE` & `commandeft-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commandeft-0.3.1/README.md` & `commandeft-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `commandeft-0.3.1/commandeft/constants/consts.py` & `commandeft-0.4.0/commandeft/constants/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 init_messages = [
     "What mischief are we up to now?\n Describe the command you're concocting:\n",
     "Oh no, caught in another coding conundrum?\n Share the details:\n",
     "Here to save the day!\n Enlighten me with the command you're grappling with:\n",
     "When your coding journey hits a snag,\n Describe the task that makes you sag:\n",
     "No shame in seeking guidance.\n What command do you need a helping hand with?:\n",
-    "Trouble seems to find you often.\n nReveal the command conundrum you're facing now:\n",
+    "Trouble seems to find you often.\n Reveal the command conundrum you're facing now:\n",
     "We all need a helping hand sometimes.\n Describe the command that has you reaching out for support:\n",
     "In a pickle again, I see?\n Describe the trouble you're in and let's work it out together:\n",
     "Brave adventurer, share the quest for the command you seek and I shall guide you through:\n",
     "When bugs run rampant, causing you despair,\n Detail the task that makes you pull out your hair:\n",
     "Here to rescue you from the labyrinth of documentation!\n Unravel your challenge to me:\n",
     "Seeking shell enlightenment, are we?\n Unveil the path to wisdom you're pursuing:\n",
     "In the coding realm, when all is grim,\n Describe the prompt that makes you scream:\n",
```

### Comparing `commandeft-0.3.1/commandeft/core/cli.py` & `commandeft-0.4.0/commandeft/core/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from commandeft.constants.consts import COMMANDEFT_ASCII_DESC, COMMANDEFT_NORMAL_DESC, CONFIG_FILE_PATH
 from commandeft.core.decision import decide_and_apply_action
 from commandeft.core.generation import Generation
 from commandeft.util.config_util import create_generation_config, get_configuration_answers, validate_configuration
 from commandeft.util.interactive_util import display_command, get_prompt
 
 
-COMMANDEFT_DESCRIPTION = COMMANDEFT_ASCII_DESC if shutil.get_terminal_size((80, 20)).columns >= 50 else COMMANDEFT_NORMAL_DESC
+COMMANDEFT_DESCRIPTION = COMMANDEFT_ASCII_DESC if shutil.get_terminal_size().columns >= 50 else COMMANDEFT_NORMAL_DESC
 
 
 class CustomCommand(click.Command):
     def get_help(self, ctx):
         # Get the default help message
         help_message = super().get_help(ctx)
 
@@ -42,15 +42,15 @@
     os.makedirs(os.path.dirname(CONFIG_FILE_PATH), exist_ok=True)
     with open(CONFIG_FILE_PATH, "w", encoding="utf-8") as config_file:
         json.dump(answers, config_file)
 
     click.echo(
         "-------------------------------------\n"
         + click.style("Configuration completed successfully.\n", fg="green")
-        + "To change the configuration, edit ~/.commandeft/config or run `commandeft --configure (or -c)]`\n"
+        + "To change the configuration, run `commandeft --configure (or -c)`\n"
     )
 
 
 def interactive_core(is_first_prompt, generation):
     user_prompt: str = get_prompt(is_first_prompt)
     command: str | None = generation.generate_command(user_prompt)
```

### Comparing `commandeft-0.3.1/commandeft/core/decision.py` & `commandeft-0.4.0/commandeft/core/decision.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,18 +18,19 @@
     decision = get_decision(accept_command_behavior, history)
     if history:
         if decision == "exit":
             return "exit"
         if decision == "action":
             if accept_command_behavior == "run":
                 subprocess.run(command, shell=True, check=False)
+                return decide_and_apply_action(command)
             elif accept_command_behavior == "copy":
                 pyperclip.copy(command)
                 click.echo(click.style("> Command copied to clipboard!", fg="green"))
-            return "exit"
+                return decide_and_apply_action(command)
         return "continue"
 
     if decision:
         if accept_command_behavior == "run":
             subprocess.run(command, shell=True, check=False)
         elif accept_command_behavior == "copy":
             pyperclip.copy(command)
```

### Comparing `commandeft-0.3.1/commandeft/core/generation.py` & `commandeft-0.4.0/commandeft/core/generation.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.3.1/commandeft/core/history_cache.py` & `commandeft-0.4.0/commandeft/core/history_cache.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.3.1/commandeft/main.py` & `commandeft-0.4.0/commandeft/main.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.3.1/commandeft/util/config_util.py` & `commandeft-0.4.0/commandeft/util/config_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,22 +106,22 @@
             "message": "Enter the temperature (0-2 with max 2 decimal places):\n",
             "validate": lambda val: False if val == "" else 0 <= float(val) <= 2,
             "filter": lambda val: False if val == "" else float(val),
         },
         {
             "type": "input",
             "name": "max_tokens",
-            "message": "Enter max_tokens (gpt-3.5-turbo:[1-4,096], gpt-4:[1-8,192]).:\n",
+            "message": "Enter max_tokens " + ("[1,8192]" if model_answer["model"] == "gpt-4" else "[1,4096]") + ":\n",
             "validate": lambda val: validate_max_tokens(model_answer, val),
             "filter": lambda val: False if val == "" else int(val),
         },
         {
             "type": "confirm",
             "name": "interactive_history",
-            "message": "Would you like interactive mode to keep generation history?\n)",
+            "message": "Would you like interactive mode to keep generation history?\n",
             "default": True,
         },
         {
             "type": "password",
             "name": "api_key",
             "message": "Enter your OpenAI API key:\n",
         },
```

### Comparing `commandeft-0.3.1/commandeft/util/interactive_util.py` & `commandeft-0.4.0/commandeft/util/interactive_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import json
 import random
+import shutil
 
 from InquirerPy import prompt
 import click
 from commandeft.constants.consts import init_messages
 
 
 def display_command(command):
+    terminal_cols = shutil.get_terminal_size().columns
     num_of_tildes = len(command.splitlines()[0]) + 2
-    click.echo("~" * num_of_tildes)
+    click.echo("~" * min(num_of_tildes, terminal_cols))
     click.echo(click.style("> " + command, fg="green", bold=True))
-    click.echo("~" * num_of_tildes)
+    click.echo("~" * min(num_of_tildes, terminal_cols))
 
 
 def get_prompt(first_prompt=True):
     random_prompt_message = random.choice(init_messages)
     questions = [
         {
             "type": "input",
             "name": "prompt",
-            "message": random_prompt_message if first_prompt is True else "Clarify or expand on your previous prompt:",
+            "message": random_prompt_message if first_prompt is True else "Clarify or expand on your previous prompt:\n",
             "qmark": "-",
             "default": "",
             "filter": lambda val: json.dumps(val.strip()),
         },
     ]
     answers = prompt(questions)
     return answers["prompt"]
@@ -52,19 +54,19 @@
     else:
         choice_question = [
             {
                 "type": "rawlist",
                 "name": "interact",
                 "choices": [
                     {
-                        "name": ("Run it " if accept_command_behavior == "run" else "Copy command to clipboard ") + "and exit?",
+                        "name": ("Run it." if accept_command_behavior == "run" else "Copy to clipboard."),
                         "value": "action",
                     },
-                    {"name": "Continue session?", "value": "continue"},
-                    {"name": "Exit session?", "value": "exit"},
+                    {"name": "Continue session.", "value": "continue"},
+                    {"name": "Exit session.", "value": "exit"},
                 ],
                 "message": "What would you like to do?\n",
                 "default": 1,
                 "mandatory": True,
                 "multiselect": False,
             },
         ]
```

### Comparing `commandeft-0.3.1/pyproject.toml` & `commandeft-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "commandeft"
-version = "0.3.1"
+version = "0.4.0"
 description = "CommanDeft is a CLI tool that converts natural language prompts into executable commands or scripts using OpenAI's chat models."
 readme = "README.md"
 authors = [
     { name = "Petros Sidirokastritis", email = "sidirope@gmail.com" },
 ]
 requires-python = ">=3.8.1, <=3.11.4"
 dependencies = [
```

### Comparing `commandeft-0.3.1/PKG-INFO` & `commandeft-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandeft
-Version: 0.3.1
+Version: 0.4.0
 Summary: CommanDeft is a CLI tool that converts natural language prompts into executable commands or scripts using OpenAI's chat models.
 Keywords: commandeft cli tool shell commands prompt-based command generation natural language prompts shell commands shell scripts shell command generation intelligent code generation language-to-code conversion developer-friendly simplified scripting code efficiency streamline workflow intelligent suggestions efficient command composition gpt-3.5-turbo gpt-4 shell command suggestion interactive mode guided prompt command execution
 Author-Email: Petros Sidirokastritis <sidirope@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Ferrum-Citadel/commandeft
 Requires-Python: <=3.11.4,>=3.8.1
 Requires-Dist: PyJWT==2.7.0
```

