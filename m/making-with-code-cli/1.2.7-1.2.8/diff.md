# Comparing `tmp/making_with_code_cli-1.2.7.tar.gz` & `tmp/making_with_code_cli-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "making_with_code_cli-1.2.7.tar", max compression
+gzip compressed data, was "making_with_code_cli-1.2.8.tar", max compression
```

## Comparing `making_with_code_cli-1.2.7.tar` & `making_with_code_cli-1.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1342 2023-05-30 14:14:06.604035 making_with_code_cli-1.2.7/README.md
--rw-r--r--   0        0        0     7939 2023-07-12 20:37:31.002674 making_with_code_cli-1.2.7/making_with_code_cli/cli.py
--rw-r--r--   0        0        0    15431 2023-07-12 21:28:15.511664 making_with_code_cli-1.2.7/making_with_code_cli/cli_setup.py
--rw-r--r--   0        0        0      551 2023-07-10 19:39:26.763192 making_with_code_cli-1.2.7/making_with_code_cli/curriculum.py
--rw-r--r--   0        0        0      658 2023-07-10 20:30:48.777211 making_with_code_cli-1.2.7/making_with_code_cli/errors.py
--rw-r--r--   0        0        0      276 2023-06-05 20:21:54.165003 making_with_code_cli-1.2.7/making_with_code_cli/git_backend/__init__.py
--rw-r--r--   0        0        0     1613 2023-07-02 18:57:59.595603 making_with_code_cli-1.2.7/making_with_code_cli/git_backend/base_backend.py
--rw-r--r--   0        0        0     3461 2023-06-05 20:20:21.178737 making_with_code_cli-1.2.7/making_with_code_cli/git_backend/github_backend.py
--rw-r--r--   0        0        0     3845 2023-06-05 20:21:08.636148 making_with_code_cli-1.2.7/making_with_code_cli/git_backend/github_org_backend.py
--rw-r--r--   0        0        0     4048 2023-07-11 16:15:54.845783 making_with_code_cli-1.2.7/making_with_code_cli/git_backend/mwc_backend.py
--rw-r--r--   0        0        0      727 2023-07-12 20:28:47.118456 making_with_code_cli-1.2.7/making_with_code_cli/git_wrapper.py
--rw-r--r--   0        0        0      266 2023-05-30 14:14:06.615290 making_with_code_cli-1.2.7/making_with_code_cli/helpers.py
--rw-r--r--   0        0        0     1526 2023-07-10 20:12:17.374391 making_with_code_cli-1.2.7/making_with_code_cli/mwc_accounts_api.py
--rw-r--r--   0        0        0     1629 2023-05-30 14:14:06.616770 making_with_code_cli-1.2.7/making_with_code_cli/settings.py
--rw-r--r--   0        0        0     1682 2023-05-30 14:14:06.617319 making_with_code_cli-1.2.7/making_with_code_cli/styles.py
--rw-r--r--   0        0        0      663 2023-07-12 21:29:23.546031 making_with_code_cli-1.2.7/pyproject.toml
--rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 making_with_code_cli-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1342 2023-05-30 14:14:06.604035 making_with_code_cli-1.2.8/README.md
+-rw-r--r--   0        0        0     8031 2023-07-13 17:44:41.302864 making_with_code_cli-1.2.8/making_with_code_cli/cli.py
+-rw-r--r--   0        0        0    16558 2023-07-14 12:45:01.156845 making_with_code_cli-1.2.8/making_with_code_cli/cli_setup.py
+-rw-r--r--   0        0        0      551 2023-07-10 19:39:26.763192 making_with_code_cli-1.2.8/making_with_code_cli/curriculum.py
+-rw-r--r--   0        0        0      658 2023-07-10 20:30:48.777211 making_with_code_cli-1.2.8/making_with_code_cli/errors.py
+-rw-r--r--   0        0        0      276 2023-06-05 20:21:54.165003 making_with_code_cli-1.2.8/making_with_code_cli/git_backend/__init__.py
+-rw-r--r--   0        0        0     1613 2023-07-02 18:57:59.595603 making_with_code_cli-1.2.8/making_with_code_cli/git_backend/base_backend.py
+-rw-r--r--   0        0        0     3461 2023-06-05 20:20:21.178737 making_with_code_cli-1.2.8/making_with_code_cli/git_backend/github_backend.py
+-rw-r--r--   0        0        0     3845 2023-06-05 20:21:08.636148 making_with_code_cli-1.2.8/making_with_code_cli/git_backend/github_org_backend.py
+-rw-r--r--   0        0        0     4048 2023-07-11 16:15:54.845783 making_with_code_cli-1.2.8/making_with_code_cli/git_backend/mwc_backend.py
+-rw-r--r--   0        0        0      727 2023-07-12 20:28:47.118456 making_with_code_cli-1.2.8/making_with_code_cli/git_wrapper.py
+-rw-r--r--   0        0        0      266 2023-05-30 14:14:06.615290 making_with_code_cli-1.2.8/making_with_code_cli/helpers.py
+-rw-r--r--   0        0        0     1526 2023-07-10 20:12:17.374391 making_with_code_cli-1.2.8/making_with_code_cli/mwc_accounts_api.py
+-rw-r--r--   0        0        0     1629 2023-05-30 14:14:06.616770 making_with_code_cli-1.2.8/making_with_code_cli/settings.py
+-rw-r--r--   0        0        0     1702 2023-07-13 17:41:17.791340 making_with_code_cli-1.2.8/making_with_code_cli/styles.py
+-rw-r--r--   0        0        0      663 2023-07-14 12:45:08.415566 making_with_code_cli-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 making_with_code_cli-1.2.8/PKG-INFO
```

### Comparing `making_with_code_cli-1.2.7/README.md` & `making_with_code_cli-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.7/making_with_code_cli/cli.py` & `making_with_code_cli-1.2.8/making_with_code_cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     choose_course,
     choose_editor,
     MWCShellConfig,
     InstallCurl,
     InstallHomebrew,
     InstallXCode,
     WriteShellConfig,
-    InstallPython3,
     InstallPoetry,
     InstallGit,
     InstallTree,
     InstallVSCode,
     InstallImageMagick,
     InstallHttpie,
     InstallScipy,
@@ -82,80 +81,86 @@
         sp = get_settings_path(config)
         click.echo(debug_fmt(f"Reading settings from {sp}"))
     rc_tasks = []
     click.echo(address(INTRO_MESSAGE))
     for note in INTRO_NOTES:
         click.echo(address(note, list_format=True))
     click.echo()
-    settings['mwc_username'] = choose_mwc_username(settings.get("mwc_username"))
+    if not yes:
+        settings['mwc_username'] = choose_mwc_username(settings.get("mwc_username"))
     api = MWCAccountsAPI()
     if settings.get('mwc_accounts_token'):
         try:
             status = api.get_status(settings['mwc_accounts_token'])
         except api.RequestFailed as bad_token:
             token = prompt_mwc_password(settings['mwc_username'])
             settings['mwc_accounts_token'] = token
             status = api.get_status(token)
     else:
         token = prompt_mwc_password(settings['mwc_username'])
         settings['mwc_accounts_token'] = token
         status = api.get_status(token)
     settings['mwc_git_token'] = status['git_token']
-    settings['role'] = "teacher" if teacher else "student"
-    settings['work_dir'] = str(choose_work_dir(settings.get("work_dir")).resolve())
-    settings['mwc_site_url'] = choose_mwc_site_url(settings.get('mwc_site_url'))
+    if not yes:
+        settings['role'] = "teacher" if teacher else "student"
+        settings['work_dir'] = str(choose_work_dir(settings.get("work_dir")).resolve())
+        settings['mwc_site_url'] = choose_mwc_site_url(settings.get('mwc_site_url'))
     curriculum = get_curriculum(settings)
-    settings['course'] = choose_course(
-        [course['name'] for course in curriculum['courses']], 
-        default=settings.get('course')
-    )
+    if not yes:
+        settings['course'] = choose_course(
+            [course['name'] for course in curriculum['courses']], 
+            default=settings.get('course')
+        )
     course = [c for c in curriculum['courses'] if c['name'] == settings['course']][0]
-    if Platform.detect() & (Platform.MAC | Platform.UBUNTU):
-        settings['editor'] = choose_editor(settings.get('editor', 'code'))
+    if not yes:
+        if Platform.detect() & (Platform.MAC | Platform.UBUNTU):
+            settings['editor'] = choose_editor(settings.get('editor', 'code'))
     G = get_backend(course['git_backend'])
     settings = G.extend_settings(settings)
     if yes:
-        click.echo(info("Updated settings:"))
+        click.echo(info("MWC settings:"))
         click.echo(info(yaml.dump(settings), preformatted=True))
     else:
         click.echo(info(yaml.dump(settings), preformatted=True))
         click.confirm(
             question("Do these settings look ok?"),
             abort=True
         )
     write_settings(settings, config)
 
-    tasks = [
-        MWCShellConfig(settings),
-        InstallCurl(settings),
-        InstallHomebrew(settings),
-        InstallXCode(settings),
-        InstallPoetry(settings),
-        WriteShellConfig(settings),
-        InstallPython3(settings),
-        InstallGit(settings),
-        InstallTree(settings),
-        InstallVSCode(settings),
-        InstallImageMagick(settings),
-        InstallHttpie(settings),
-        InstallScipy(settings),
-        GitConfiguration(settings),
+    task_classes = [
+        MWCShellConfig,
+        InstallCurl,
+        InstallHomebrew,
+        InstallXCode,
+        InstallPoetry,
+        WriteShellConfig,
+        InstallGit,
+        InstallTree,
+        InstallVSCode,
+        InstallImageMagick,
+        InstallHttpie,
+        #InstallScipy,
+        GitConfiguration,
     ]
     errors = []
-    for task in tasks:
+    for task_class in task_classes:
         try:
+            task = task_class(settings, debug=debug)
             task.run_task_if_needed()
         except Exception as e:
-            errors.append((task, traceback.format_exc()))
+            errors.append(task)
+            click.echo(error('-' * 80))
+            click.echo(error(f"{task.task_description} failed"))
+            if debug:
+                click.echo(debug_fmt(traceback.format_exc(), preformatted=True))
     if errors:
         click.echo(error(f"{len(errors)} setup tasks failed:"))
-        for task, tb in errors:
-            click.echo(error(task.description))
-            if debug:
-                click.echo(debug_fmt(tb, preformatted=True))
+        for task in errors:
+            click.echo(error(f"- {task.description}"))
     else:
         ctx.invoke(update, config=config)
 
 def get_course_by_name(name, courses):
     for course in courses:
         if course['name'] == name:
             return course
```

### Comparing `making_with_code_cli-1.2.7/making_with_code_cli/cli_setup.py` & `making_with_code_cli-1.2.8/making_with_code_cli/cli_setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from pathlib import Path
 from enum import Flag, auto
 from stat import *
 import sys
 import os
 import platform
+from importlib.util import find_spec
 from making_with_code_cli.mwc_accounts_api import MWCAccountsAPI
 from making_with_code_cli.styles import (
     address,
     question,
+    debug,
     confirm,
     info,
     success,
     warn,
     error,
 )
 from making_with_code_cli.curriculum import (
@@ -37,33 +39,55 @@
     "You can quit this program by pressing Control + C at the same time.",
     "Many questions have default values, shown in [brackets]. Press enter to accept the default.",
     "The setup may ask for your password. As a security measure, you won't see any characters when you type it in.",
     "If you get stuck or have any questions, ask a teacher.",
 ]
 WORK_DIR_PERMISSIONS = S_IRWXU | S_IXGRP | S_IXOTH
 
+class PlatformNotSupported(Exception):
+    def __init__(self):
+        err = "This platform is not supported."
+        return super().__init__(err)
+
 class Platform(Flag):
     MAC = auto()
     UBUNTU = auto()
     REPLIT = auto()
     SUPPORTED = MAC | UBUNTU | REPLIT
     UNSUPPORTED = 0
 
     @classmethod
-    def detect(self):
+    def detect(cls):
         if os.environ.get('REPL_ID'):
-            return self.REPLIT
+            return cls.REPLIT
         system_name = platform.system()
         if system_name == "Darwin":
-            return self.MAC
+            return cls.MAC
         if system_name == "Linux" and platform.freedesktop_os_release().get('NAME'):
             release_name = (platform.freedesktop_os_release() or {}).get('NAME')
             if release_name == "Ubuntu":
-                return self.UBUNTU
-        return self.UNSUPPORTED
+                return cls.UBUNTU
+        return cls.UNSUPPORTED
+
+    @classmethod
+    def package_manager(cls, brew_cask=False):
+        """Returns the command for the platform's package manager.
+        """
+        platform = cls.detect()
+        if platform == cls.MAC:
+            if brew_cask: 
+                return "brew install --cask "
+            else:
+                return "brew install "
+        elif platform == cls.UBUNTU:
+            return "sudo apt install "
+        elif platform == cls.REPLIT:
+            return "nix-env -iA nixpkgs."
+        else:
+            raise cls.NotSupported()
 
 def default_work_dir():
     if (Path.home() / "Desktop").exists():
         return Path.home() / "Desktop" / "making_with_code"
     else:
         return Path.home() / "making_with_code"
 
@@ -185,51 +209,57 @@
     raise IOError("Can't find an rc file.")
 
 class SetupTask:
     "An idempotent task"
     platform = Platform.SUPPORTED
     description = "A task"
 
-    def __init__(self, settings):
+    def __init__(self, settings, debug=False):
         self.settings = settings
+        self.debug = debug
 
     def run_task_if_needed(self):
-        if not Platform.detect() & self.platform:
-            return 
-        elif self.is_complete():
-            self.report_not_needed()
-        else:
-            self.run_task()
-            self.report_complete()
+        if Platform.detect() & self.platform:
+            if self.is_complete():
+                self.report_not_needed()
+            else:
+                self.run_task()
+                self.report_complete()
         
     def is_complete(self):
         return True    
 
     def run_task(self):
         pass
 
     def report_not_needed(self):
         click.echo(info(f"{self.description} is already complete."))
         
     def report_complete(self):
         click.echo(success(f"{self.description} is complete!"))
 
+    def debug_log(self, message):
+        if self.debug:
+            click.echo(debug(message))
+
     def executable_on_path(self, name):
         return bool(run(f"which {name}", shell=True, capture_output=True).stdout)
 
 class MWCShellConfig(SetupTask):
     """Writes a line in the rc shell config file sourcing ~/.mwc_rc.
     """
     description = "Link main shell config file to ~/.mwc_rc"
 
     def is_complete(self):
         return f"source {get_mwc_rc_path()}" in platform_rc_file().read_text()
 
     def run_task(self):
-        with platform_rc_file().open('a') as fh:
+        rc_file = platform_rc_file()
+        self.debug_log(f"Adding `mwc` path to {rc_file}")
+        with rc_file.open('a') as fh:
             result = run("which mwc", shell=True, check=True, text=True, capture_output=True)
             mwcpath = Path(result.stdout).parent
             fh.write(f"\n# MAKING WITH CODE\n")
             fh.write(f'export PATH="$PATH:{mwcpath}"\n')
             fh.write(f"source {get_mwc_rc_path()}\n")
 
 class InstallHomebrew(SetupTask):
@@ -290,15 +320,18 @@
 
     def is_complete(self):
         p = get_mwc_rc_path()
         return p.exists() and p.read_text() == self.generate_shell_config()
 
     def run_task(self):
         click.echo(address("Writing the MWC shell configuration file..."))
-        get_mwc_rc_path().write_text(self.generate_shell_config())
+        mwc_rc_path = get_mwc_rc_path()
+        config_text = self.generate_shell_config()
+        self.debug_log(f"Writing to {mwc_rc_path}:\n\n{config_text}\n\n")
+        mwc_rc_path.write_text(config_text)
         run(f"source {get_mwc_rc_path()}", shell=True, check=True)
 
     def generate_shell_config(self):
         "Generates the shell configuration file contents"
         f = ""
         shell = get_shell_name()
         f += "# Making With Code RC File\n\n" 
@@ -308,89 +341,87 @@
             if self.settings['editor'] == "subl":
                 f += "## Add subl to $PATH\n"
                 subldir = "/Applications/Sublime Text.app/Contents/SharedSupport/bin"
                 f += f'export PATH="{subldir}:$PATH"\n\n'
         return f
 
 class InstallPackage(SetupTask):
-    package_name = "package"
+    """A subclass of SetupTask for packages to be installed by the Platform package manager.
+    """
+    executable_name = "package"
     brew_name = "package"
     apt_name = "package"
     nix_name = "package"
-    cask = False
+    brew_cask = False
 
     def __init__(self, *args, **kwargs):
-        self.description = f"Install {self.package_name}"
+        self.description = f"Install {self.executable_name}"
         super().__init__(*args, **kwargs)
 
     def is_complete(self):
-        return self.executable_on_path(self.package_name)
+        return self.executable_on_path(self.executable_name)
+
+    def get_package_name(self):
+        system_platform = Platform.detect()
+        if system_platform == Platform.MAC:
+            return self.brew_name
+        elif system_platform == Platform.UBUNTU:
+            return self.apt_name
+        elif system_platform == Platform.REPLIT:
+            return self.nix_name
+        else:
+            raise PlatformNotSupported()
     
     def run_task(self):
-        platform = Platform.detect()
-        click.echo(address(f"Installing {self.package_name}..."))
-        if platform & Platform.MAC:
-            if self.cask:
-                run(f"brew install {self.brew_name}", shell=True, check=True)
-            else:
-                run(f"brew install --cask {self.brew_name}", shell=True, check=True)
-        elif platform & Platform.UBUNTU:
-            run(f"apt install {self.apt_name}", shell=True, check=True)
-        elif platform & Platform.REPLIT:
-            run(f"nix-env -iA nixpkgs.{self.nix_name}", shell=True, check=True)
-        else:
-            raise IOError(f"Platform {platform} not supported...")
+        click.echo(address(f"Installing {self.executable_name}..."))
+        package_manager = Platform.package_manager(brew_cask=self.brew_cask)
+        package_name = self.get_package_name()
+        self.debug_log(f"Running: {package_manager}{package_name}")
+        run(f"{package_manager}{package_name}", shell=True, check=True)
 
 class InstallCurl(InstallPackage):
     platform = Platform.UBUNTU
-    package_name = brew_name = apt_name = "curl"
-
-class InstallPython3(InstallPackage):
-    platform = Platform.MAC | Platform.UBUNTU
-    package_name = brew_name = apt_name = "python3"
+    executable_name = apt_name = "curl"
 
 class InstallGit(InstallPackage):
     platform = Platform.MAC | Platform.UBUNTU
-    package_name = brew_name = apt_name = "git"
+    executable_name = brew_name = apt_name = "git"
 
 class InstallTree(InstallPackage):
-    package_name = brew_name = apt_name = nix_name = "tree"
+    executable_name = brew_name = apt_name = nix_name = "tree"
 
 class InstallVSCode(InstallPackage):
     platform = Platform.MAC | Platform.UBUNTU
-    package_name = "code"
+    executable_name = "code"
     brew_name = "visual-studio-code"
     cask = True
 
     def run_task(self):
         platform = Platform.detect()
         if platform & Platform.UBUNTU:
             run("sudo snap install --classic code", shell=True, check=True)
         else:
             return super().run_task()
 
 class InstallImageMagick(InstallPackage):
-    package_name = "magick"
+    executable_name = "magick"
     brew_name = apt_name = nix_name = "imagemagick"
 
+    def is_complete(self):
+        return self.executable_on_path("magick") or self.executable_on_path("convert")
+
 class InstallHttpie(InstallPackage):
-    package_name = "http"
+    executable_name = "http"
     brew_name = apt_name = nix_name = "httpie"
 
 class InstallScipy(InstallPackage):
-    package_name = brew_name = apt_name = "scipy"
+    executable_name = brew_name = apt_name = nix_name = "scipy"
 
     def is_complete(self):
-        return True
-        try:
-            import scipy
-            return True
-        except ModuleNotFoundError as e:
-            print(e)
-            return False
+        return find_spec("scipy") is not None
 
 class GitConfiguration(SetupTask):
     """Configure global git settings.
     Can be skipped by setting `skip_git_config: true` in settings.
     """
     description = "Configure git"
 
@@ -433,9 +464,7 @@
         if self.settings.get('git_name'):
             git_config["user.name"] = self.settings['git_name']
         if self.settings.get('github_email'):
             git_config["user.email"] = self.settings['github_email']
         return git_config
 
 
-
-
```

### Comparing `making_with_code_cli-1.2.7/making_with_code_cli/curriculum.py` & `making_with_code_cli-1.2.8/making_with_code_cli/curriculum.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.7/making_with_code_cli/errors.py` & `making_with_code_cli-1.2.8/making_with_code_cli/errors.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.7/making_with_code_cli/git_backend/base_backend.py` & `making_with_code_cli-1.2.8/making_with_code_cli/git_backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.7/making_with_code_cli/git_backend/github_backend.py` & `making_with_code_cli-1.2.8/making_with_code_cli/git_backend/github_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.7/making_with_code_cli/git_backend/github_org_backend.py` & `making_with_code_cli-1.2.8/making_with_code_cli/git_backend/github_org_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.7/making_with_code_cli/git_backend/mwc_backend.py` & `making_with_code_cli-1.2.8/making_with_code_cli/git_backend/mwc_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.7/making_with_code_cli/git_wrapper.py` & `making_with_code_cli-1.2.8/making_with_code_cli/git_wrapper.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.7/making_with_code_cli/mwc_accounts_api.py` & `making_with_code_cli-1.2.8/making_with_code_cli/mwc_accounts_api.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.7/making_with_code_cli/settings.py` & `making_with_code_cli-1.2.8/making_with_code_cli/settings.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.7/making_with_code_cli/styles.py` & `making_with_code_cli-1.2.8/making_with_code_cli/styles.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,17 +21,17 @@
     """Addresses the user qith a question (e.g. a prompt)
     """
     return click.style(fill(message, width=FW) + '\n', fg="cyan")
 
 def debug(message, preformatted=False):
     """Shows the user debug information"""
     if preformatted:
-        return click.style(message)
+        return click.style(message, dim=True)
     else:
-        return click.style(fill(message, width=FW))
+        return click.style(fill(message, width=FW), dim=True)
 
 def info(message, preformatted=False):
     """Shows the user information. 
     Don't use this for boilerplate; the user should have requested the information 
     or may need to check it.
     """
     if preformatted:
```

### Comparing `making_with_code_cli-1.2.7/pyproject.toml` & `making_with_code_cli-1.2.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "making-with-code-cli"
-version = "1.2.7"
+version = "1.2.8"
 description = "Courseware for Making With Code"
 authors = ["Chris Proctor <chris@chrisproctor.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/cproctor/making-with-code-courseware"
 
 [tool.poetry.dependencies]
```

### Comparing `making_with_code_cli-1.2.7/PKG-INFO` & `making_with_code_cli-1.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: making-with-code-cli
-Version: 1.2.7
+Version: 1.2.8
 Summary: Courseware for Making With Code
 Home-page: https://github.com/cproctor/making-with-code-courseware
 License: MIT
 Author: Chris Proctor
 Author-email: chris@chrisproctor.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

