# Comparing `tmp/jgp_report_creditos-0.0.12.tar.gz` & `tmp/jgp_report_creditos-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jgp_report_creditos-0.0.12.tar", last modified: Fri Jul 14 18:45:30 2023, max compression
+gzip compressed data, was "jgp_report_creditos-0.0.9.tar", last modified: Mon Jun  5 16:17:06 2023, max compression
```

## Comparing `jgp_report_creditos-0.0.12.tar` & `jgp_report_creditos-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,25 @@
-drwxrwxr-x   0 sistemas  (1000) sistemas  (1000)        0 2023-07-14 18:45:30.641753 jgp_report_creditos-0.0.12/
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)     1074 2023-06-15 20:54:52.000000 jgp_report_creditos-0.0.12/LICENSE
--rw-rw-r--   0 sistemas  (1000) sistemas  (1000)     6619 2023-07-14 18:45:30.641753 jgp_report_creditos-0.0.12/PKG-INFO
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)     6246 2023-06-15 20:54:52.000000 jgp_report_creditos-0.0.12/README.md
-drwxrwxr-x   0 sistemas  (1000) sistemas  (1000)        0 2023-07-14 18:45:30.621754 jgp_report_creditos-0.0.12/jgp_report_creditos/
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)       83 2023-06-15 20:54:52.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/__init__.py
-drwxrwxr-x   0 sistemas  (1000) sistemas  (1000)        0 2023-07-14 18:45:30.625753 jgp_report_creditos-0.0.12/jgp_report_creditos/core/
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)       56 2023-06-19 20:47:24.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/core/__init__.py
-drwxrwxr-x   0 sistemas  (1000) sistemas  (1000)        0 2023-07-14 18:45:30.625753 jgp_report_creditos-0.0.12/jgp_report_creditos/core/contrato/
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)        0 2023-06-15 20:54:52.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/core/contrato/__init__.py
-drwxrwxr-x   0 sistemas  (1000) sistemas  (1000)        0 2023-07-14 18:45:30.629753 jgp_report_creditos-0.0.12/jgp_report_creditos/core/contrato/v1/
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)     4711 2023-06-16 14:55:12.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/core/contrato/v1/Controlar tablas de firmas.py
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)        0 2023-06-15 20:54:52.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/core/contrato/v1/__init__.py
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)   146894 2023-07-14 18:30:12.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/core/contrato/v1/base.py
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)    20081 2023-06-24 15:53:30.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/core/contrato/v1/contratos.py
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)    36882 2023-07-13 16:07:41.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/core/deposito.py
-drwxrwxr-x   0 sistemas  (1000) sistemas  (1000)        0 2023-07-14 18:45:30.633753 jgp_report_creditos-0.0.12/jgp_report_creditos/core/exception/
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)       37 2023-06-15 20:54:52.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/core/exception/__init__.py
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)      309 2023-06-15 20:54:52.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/core/exception/exception.py
--rw-rw-r--   0 sistemas  (1000) sistemas  (1000)     6588 2023-07-13 18:43:01.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/core/rutas.py
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)    21940 2023-07-13 18:29:12.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/report.py
-drwxrwxr-x   0 sistemas  (1000) sistemas  (1000)        0 2023-07-14 18:45:30.617754 jgp_report_creditos-0.0.12/jgp_report_creditos/resources/
-drwxrwxr-x   0 sistemas  (1000) sistemas  (1000)        0 2023-07-14 18:45:30.633753 jgp_report_creditos-0.0.12/jgp_report_creditos/resources/img/
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)    57446 2023-06-15 20:54:52.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/resources/img/logo_jgp.png
-drwxrwxr-x   0 sistemas  (1000) sistemas  (1000)        0 2023-07-14 18:45:30.637753 jgp_report_creditos-0.0.12/jgp_report_creditos/template/
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)        0 2023-06-17 16:56:44.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/template/__init__.py
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)    22964 2023-07-12 19:53:27.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/template/components.py
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)      660 2023-06-17 16:08:06.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/template/template.py
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)      714 2023-06-15 21:23:54.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/test.py
-drwxrwxr-x   0 sistemas  (1000) sistemas  (1000)        0 2023-07-14 18:45:30.637753 jgp_report_creditos-0.0.12/jgp_report_creditos/tests/
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)        0 2023-06-17 16:57:48.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/tests/__init__.py
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)      952 2023-07-14 18:35:17.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/tests/test_contratos.py
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)    33149 2023-07-13 18:42:45.000000 jgp_report_creditos-0.0.12/jgp_report_creditos/tests/test_deposito.py
-drwxrwxr-x   0 sistemas  (1000) sistemas  (1000)        0 2023-07-14 18:45:30.621754 jgp_report_creditos-0.0.12/jgp_report_creditos.egg-info/
--rw-rw-r--   0 sistemas  (1000) sistemas  (1000)     6619 2023-07-14 18:45:30.000000 jgp_report_creditos-0.0.12/jgp_report_creditos.egg-info/PKG-INFO
--rw-rw-r--   0 sistemas  (1000) sistemas  (1000)     1045 2023-07-14 18:45:30.000000 jgp_report_creditos-0.0.12/jgp_report_creditos.egg-info/SOURCES.txt
--rw-rw-r--   0 sistemas  (1000) sistemas  (1000)        1 2023-07-14 18:45:30.000000 jgp_report_creditos-0.0.12/jgp_report_creditos.egg-info/dependency_links.txt
--rw-rw-r--   0 sistemas  (1000) sistemas  (1000)       20 2023-07-14 18:45:30.000000 jgp_report_creditos-0.0.12/jgp_report_creditos.egg-info/top_level.txt
--rw-rw-r--   0 sistemas  (1000) sistemas  (1000)       38 2023-07-14 18:45:30.641753 jgp_report_creditos-0.0.12/setup.cfg
--rw-r--r--   0 sistemas  (1000) sistemas  (1000)      977 2023-07-14 18:34:31.000000 jgp_report_creditos-0.0.12/setup.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-05 16:17:06.772341 jgp_report_creditos-0.0.9/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     7363 2023-06-05 16:17:06.772341 jgp_report_creditos-0.0.9/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)     6246 2023-06-05 15:25:25.000000 jgp_report_creditos-0.0.9/README.md
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-05 16:17:06.768340 jgp_report_creditos-0.0.9/jgp_report_creditos/
+-rw-rw-r--   0 axel      (1000) axel      (1000)       83 2023-05-15 21:24:18.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/__init__.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-05 16:17:06.772341 jgp_report_creditos-0.0.9/jgp_report_creditos/core/
+-rw-rw-r--   0 axel      (1000) axel      (1000)        0 2023-05-04 12:51:20.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/core/__init__.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-05 16:17:06.772341 jgp_report_creditos-0.0.9/jgp_report_creditos/core/contrato/
+-rw-rw-r--   0 axel      (1000) axel      (1000)        0 2023-05-08 15:26:09.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/core/contrato/__init__.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-05 16:17:06.772341 jgp_report_creditos-0.0.9/jgp_report_creditos/core/contrato/v1/
+-rw-rw-r--   0 axel      (1000) axel      (1000)        0 2023-05-08 15:26:09.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/core/contrato/v1/__init__.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)   145944 2023-06-05 16:03:31.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/core/contrato/v1/base.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)    19761 2023-05-16 19:16:33.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/core/contrato/v1/contratos.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-05 16:17:06.772341 jgp_report_creditos-0.0.9/jgp_report_creditos/core/exception/
+-rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-05-15 21:24:18.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/core/exception/__init__.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      309 2023-05-15 21:24:18.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/core/exception/exception.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     3791 2023-06-01 17:41:20.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/report.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      714 2023-06-01 17:41:20.000000 jgp_report_creditos-0.0.9/jgp_report_creditos/test.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-05 16:17:06.772341 jgp_report_creditos-0.0.9/jgp_report_creditos.egg-info/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     7363 2023-06-05 16:17:06.000000 jgp_report_creditos-0.0.9/jgp_report_creditos.egg-info/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)      602 2023-06-05 16:17:06.000000 jgp_report_creditos-0.0.9/jgp_report_creditos.egg-info/SOURCES.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-06-05 16:17:06.000000 jgp_report_creditos-0.0.9/jgp_report_creditos.egg-info/dependency_links.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       20 2023-06-05 16:17:06.000000 jgp_report_creditos-0.0.9/jgp_report_creditos.egg-info/top_level.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-06-05 16:17:06.772341 jgp_report_creditos-0.0.9/setup.cfg
+-rw-rw-r--   0 axel      (1000) axel      (1000)      976 2023-06-05 16:16:28.000000 jgp_report_creditos-0.0.9/setup.py
```

### Comparing `jgp_report_creditos-0.0.12/PKG-INFO` & `jgp_report_creditos-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,104 +1,104 @@
 Metadata-Version: 2.1
 Name: jgp_report_creditos
-Version: 0.0.12
+Version: 0.0.9
 Summary: Librería con funciones y herramientas útiles exclusivas para jgp
 Home-page: https://gitlab.com/develop-team-jdgp/jgp-report-creditos.git
 Author: JGP Dev
 Author-email: jgpdev20@gmail.com
 License: MIT
+Description: # jgp-report-creditos
+        
+        
+        
+        ## Getting started
+        
+        To make it easy for you to get started with GitLab, here's a list of recommended next steps.
+        
+        Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!
+        
+        ## Add your files
+        
+        - [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
+        - [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
+        
+        ```
+        cd existing_repo
+        git remote add origin https://gitlab.com/develop-team-jdgp/jgp-report-creditos.git
+        git branch -M main
+        git push -uf origin main
+        ```
+        
+        ## Integrate with your tools
+        
+        - [ ] [Set up project integrations](https://gitlab.com/develop-team-jdgp/jgp-report-creditos/-/settings/integrations)
+        
+        ## Collaborate with your team
+        
+        - [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
+        - [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
+        - [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
+        - [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
+        - [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)
+        
+        ## Test and Deploy
+        
+        Use the built-in continuous integration in GitLab.
+        
+        - [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
+        - [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
+        - [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
+        - [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
+        - [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)
+        
+        ***
+        
+        # Editing this README
+        
+        When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.
+        
+        ## Suggestions for a good README
+        Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.
+        
+        ## Name
+        Choose a self-explaining name for your project.
+        
+        ## Description
+        Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
+        
+        ## Badges
+        On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.
+        
+        ## Visuals
+        Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.
+        
+        ## Installation
+        Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.
+        
+        ## Usage
+        Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
+        
+        ## Support
+        Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.
+        
+        ## Roadmap
+        If you have ideas for releases in the future, it is a good idea to list them in the README.
+        
+        ## Contributing
+        State if you are open to contributions and what your requirements are for accepting them.
+        
+        For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.
+        
+        You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.
+        
+        ## Authors and acknowledgment
+        Show your appreciation to those who have contributed to the project.
+        
+        ## License
+        For open source projects, say how it is licensed.
+        
+        ## Project status
+        If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
+        
 Keywords: python,primer paquete jgp
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# jgp-report-creditos
-
-
-
-## Getting started
-
-To make it easy for you to get started with GitLab, here's a list of recommended next steps.
-
-Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!
-
-## Add your files
-
-- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
-- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
-
-```
-cd existing_repo
-git remote add origin https://gitlab.com/develop-team-jdgp/jgp-report-creditos.git
-git branch -M main
-git push -uf origin main
-```
-
-## Integrate with your tools
-
-- [ ] [Set up project integrations](https://gitlab.com/develop-team-jdgp/jgp-report-creditos/-/settings/integrations)
-
-## Collaborate with your team
-
-- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
-- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
-- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
-- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
-- [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)
-
-## Test and Deploy
-
-Use the built-in continuous integration in GitLab.
-
-- [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
-- [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
-- [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
-- [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
-- [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)
-
-***
-
-# Editing this README
-
-When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.
-
-## Suggestions for a good README
-Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.
-
-## Name
-Choose a self-explaining name for your project.
-
-## Description
-Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
-
-## Badges
-On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.
-
-## Visuals
-Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.
-
-## Installation
-Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.
-
-## Usage
-Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
-
-## Support
-Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.
-
-## Roadmap
-If you have ideas for releases in the future, it is a good idea to list them in the README.
-
-## Contributing
-State if you are open to contributions and what your requirements are for accepting them.
-
-For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.
-
-You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.
-
-## Authors and acknowledgment
-Show your appreciation to those who have contributed to the project.
-
-## License
-For open source projects, say how it is licensed.
-
-## Project status
-If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
```

### Comparing `jgp_report_creditos-0.0.12/README.md` & `jgp_report_creditos-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `jgp_report_creditos-0.0.12/jgp_report_creditos/core/contrato/v1/base.py` & `jgp_report_creditos-0.0.9/jgp_report_creditos/core/contrato/v1/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from reportlab.lib.pagesizes import A4
 from reportlab.lib.units import mm, inch, cm
 from reportlab.lib.enums import TA_JUSTIFY, TA_CENTER, TA_LEFT
 from reportlab.lib.pagesizes import letter
 from reportlab.platypus import SimpleDocTemplate, Paragraph, Spacer, ListFlowable
 from reportlab.lib.styles import getSampleStyleSheet, ParagraphStyle
 from reportlab.lib.units import inch
-from reportlab.platypus import (SimpleDocTemplate, Spacer, Paragraph, Table, PageBreak)
+from reportlab.platypus import (SimpleDocTemplate, Spacer, Paragraph, Table)
 from reportlab.lib.styles import getSampleStyleSheet
 from reportlab.lib import colors
 from io import BytesIO
 import datetime
 import os.path
 
 #Add styles
@@ -34,39 +34,36 @@
     return SimpleDocTemplate(nombre_document, pagesize=letter, rightMargin=10.1*mm, leftMargin=16*mm,
                             topMargin=24*mm, bottomMargin=17*mm)
 
 # -------------------PARRAFOS DE LOS CONTRATOS----------------------
 class BaseContrato :   
     _parrafos = []
     #creacion de cosntructores
-    def __init__(self, contrato, usuario):
+    def __init__(self, contrato):
         self.__contrato = contrato
-        self.usuario = usuario
     
     # footer and header
     def _encabezado(self,canvas,doc):
         """Header of page"""
         canvas.saveState()
         #tipo y tamaño de letra
-        canvas.setFont('Helvetica',5.8)
+        canvas.setFont('Helvetica',6)
         #obtengo la fecha actual
         x= datetime.datetime.now()
         #setting model of date
         formatoFecha= x.strftime("%d/%m/%Y")
+        usuario= "150"
         codigo_operacion=self.__contrato["codigo_operacion"]
-
+        usuario_actualizacion=self.__contrato["testimonio_poder"]["usuario_actualizacion"]
         
         #posicion del encabezado(x, y, texto)
-        canvas.drawString(0.68*inch, A4[1]-86, formatoFecha)
-        canvas.drawString(0.68*inch, A4[1]-94, str(self.usuario))
-        canvas.drawString(0.68*inch, A4[1]-103, codigo_operacion)
+        canvas.drawString(0.68*inch, A4[1]-78, formatoFecha)
+        canvas.drawString(0.68*inch, A4[1]-87, str(usuario_actualizacion))
+        canvas.drawString(0.68*inch, A4[1]-96, codigo_operacion)
         canvas.restoreState()
-
-
-        
         """footer of page"""
         canvas.saveState()
         canvas.setFont('Helvetica',7)
         #para colocar la posicion del pie de pagina (x, y, texto)
         canvas.drawString(4.2 *inch, 0.5 * inch, " %d" % doc.page)
         #ssetting only page 2k+1
         if(doc.page%2!=0):
@@ -127,15 +124,15 @@
         cargo = testimonio_poder["representante_legal"]["rol"]       
         numero_testimonio = testimonio_poder["numero_testimonio"]
         fecha_testimonio = Utils.get_fecha(self, testimonio_poder["fecha_testimonio"])
         numero_notaria = testimonio_poder["numero_notaria_publica"]
         responsable_notaria = testimonio_poder["nombre_notario_publico"]
         texto = f'<b><u>{numeral}</u>.- (PARTES CONTRATANTES)</b>.- Intervienen en la suscripción del presente contrato:'
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
-        a = f'<b>GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A.</b>, sociedad \
+        a = f'<b>GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.</b>, sociedad \
             legalmente constituida bajo las leyes del Estado Plurinacional de Bolivia, con Matrícula de \
             Comercio y Número de Identificación Tributaria 173788022, con domicilio en la \
             {domicilio_legal} de esta ciudad, representada legalmente por <b>{apoderado}</b>, con C.I. Nº {numero_ci_apoderado}, mayor de edad, hábil \
             por derecho y vecino(a) de esta ciudad, en su condición de {cargo} en mérito al \
             Testimonio Poder No. {numero_testimonio} de fecha {fecha_testimonio} otorgado por ante la \
             Notaría de Fe Pública Nº {numero_notaria} del Distrito Judicial de La Paz a cargo de(la) Dr(a).\
             {responsable_notaria}, quien en adelante se denominará <b>"EL ACREEDOR"</b>.'
@@ -212,26 +209,26 @@
         cargo = testimonio_poder["representante_legal"]["rol"]       
         numero_testimonio = testimonio_poder["numero_testimonio"]
         fecha_testimonio = Utils.get_fecha(self, testimonio_poder["fecha_testimonio"])
         numero_notaria = testimonio_poder["numero_notaria_publica"]
         responsable_notaria = testimonio_poder["nombre_notario_publico"]
         texto = f'<b><u>{numeral}</u>.- (PARTES CONTRATANTES)</b>.- Intervienen en la suscripción del presente contrato:'
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
-        a = f'<b>GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A.</b>, sociedad \
+        a = f'<b>GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.</b>, sociedad \
             legalmente constituida bajo las leyes del Estado Plurinacional de Bolivia, con Matrícula de \
             Comercio y Número de Identificación Tributaria 173788022, con domicilio en la \
             {domicilio_legal} de esta ciudad, representada legalmente por <b>{apoderado}</b>, con C.I. Nº {numero_ci_apoderado}, mayor de edad, hábil \
             por derecho y vecino(a) de esta ciudad, en su condición de {cargo} en mérito al \
             Testimonio Poder No. {numero_testimonio} de fecha {fecha_testimonio} otorgado por ante la \
             Notaría de Fe Pública Nº {numero_notaria} del Distrito Judicial de La Paz a cargo de(la) Dr(a).\
             {responsable_notaria}, quien en adelante se denominará <b>"EL ACREEDOR"</b>.'
-        # Insiso b)
         b = "El(la)(los) señor(a)(es) "
         deudores = self.get_deudores()
         i=0
+        #55555555555555555555555555555555555555
         for item in deudores:
             i+=1
             nombreDeudor = item['nombre_completo'].upper()
             numeroCiDeudor = item['ci']
             estadoCivilDeudor = self.get_estado_civil(item['estado_civil'],item['genero'])
             domicilioDeudor = item['direccion']
             domicilio_deudor = self.get_articulo_direccion(domicilioDeudor)
@@ -240,15 +237,15 @@
             b = b + aux
             if (i != len(deudores)-1):
                 b = b + ","+" "
             else:
                 b = b + " y"+" "
         aux1='mayor(es) de edad y hábil(es) por derecho, que en lo sucesivo se denominará(n) <b>"El(la)(los) DEUDOR(A)(ES)"</b>.'
         b=b+aux1
-        #Insiso c)
+        #para el inciso c
         fiadores = self.get_fiadores()
         c=""
         #5555555555555555555555555
         if(len(fiadores)>0):
             c = "El(la)(los) señor(a)(es) "
             j=0
             for item in fiadores:
@@ -280,15 +277,15 @@
             bulletFontName='Helvetica-Bold',
             bulletFontSize=9.1,
             bulletOffsetY=0,
             bulletDedent=20        
             )
             self._parrafos.append(incisos)
         else:   
-            raise ContratoError("Campo requerido", "El contrato requiere los Datos del(los) Garante(es)")
+            raise ContratoError("Campo requerido", "El contrato requiere los Datos de fiadores")
     
 
     def _objeto_del_contrato(self, numeral):
         monto1=float(self.__contrato["monto_aprobado"])
         monto = Utils.literalEnteroMontoPrestamo(monto1)
         motivo_prestamo = self.__contrato["motivo_prestamo"].upper()
         texto_objeto = f'<b><u>{numeral}</u>.- (OBJETO DEL CONTRATO, MONTO, MONEDA Y DESTINO DEL PRÉSTAMO)</b>.- \
@@ -508,26 +505,26 @@
         garantias=self.__contrato["garantias_reales"]
         sw=False
         for item in garantias:
             if(item['concepto']=="Descripcion"):
                 prendaria=item['detalle_garantia']  
                 sw=True
         if(sw==False):
-            raise ContratoError("Campo requerido", "El contrato requiere los Datos de la garantia por concepto de: Descripción")
+            raise ContratoError("Campo requerido", "El contrato requiere los Datos de concepto: Descripcion")
         return prendaria
 
     def get_direccion_g(self):
         garantias=self.__contrato["garantias_reales"]
         sw=False
         for item in garantias:
             if(item['concepto']=="Ubicacion"):
                 ubicacion=item['detalle_garantia']
                 sw=True 
         if(sw==False):
-            raise ContratoError("Campo requerido", "El contrato requiere los Datos de la garantia por concepto de: Ubicación")            
+            raise ContratoError("Campo requerido", "El contrato requiere los Datos de concepto: Ubicacion")            
         return ubicacion.upper()
         
     #METODOS PARA detalle_garantia
     def isNumeric(self,s):
         try:
             int(s)
             return True
@@ -578,15 +575,15 @@
             texto_10_2 = f' <b>10.2. "El(la)(los) DEUDOR(A)(ES)"</b> otorgará(n) al <b>ACREEDOR</b> como garantía {prendaria}, cuyas \
                 características se encuentran detalladas y descritas en el formulario <b>"Avalúo de Garantía Prendaria"</b>, misma \
                 que forma parte integrante de este contrato sin necesidad de ser transcrito, siendo aplicable para esta operación la \
                 normativa legal vigente consignada en los artículos 1403 y siguientes del Código Civil.<br/> \
                 A solicitud expresa del(la)(los) <b>DEPOSITARIO(S)</b> los bienes constituidos en prenda permanecerán en la <b>{direccion_garantia}</b>, bienes que quedarán en depósito y/o poder de '
             c=texto_10_2
         else:
-            raise ContratoError("Campo requerido", "El contrato requiere los Datos de la garantia real, revisar la garantia por concepto de: Ubicacion ó Descripcion")
+            raise ContratoError("Campo requerido", "El contrato requiere los Datos de al menos dos garantias reales")
 
         if(len(fiadores)>0):
             c = c+ '<b>"El(la)(los) GARANTE(S) DEPOSITARIO(S)"</b>'
             j=0
             for item in fiadores:
                 j+=1
                 nombreFiador = item['nombre_completo'].upper()
@@ -598,15 +595,15 @@
                 else:
                     c = c + " y"+" "
             aux3='quien(es) a la suscripción del presente documento se declara(n) en posesión física, material y real de los bienes otorgados en prenda, los mismos que se encuentran en perfecto estado de conservación y/o funcionamiento, con las obligaciones y responsabilidades correspondientes al depositario gratuito, quedando encargado(s) de su cuidado, guarda y conservación por su cuenta exclusiva, asumiendo solidariamente todas las obligaciones y responsabilidades civiles y penales propias a su(s) condición(es) de depositario(s) que establecen disposiciones relativas al depósito y prenda, facultando a <b>"EL ACREEDOR"</b> a exigir su permanente exhibición, debiendo <b>"El(la)(los) DEPOSITARIO(S)"</b> mantener informado a <b>"EL ACREEDOR"</b> del lugar donde se encuentra la prenda, sobre cualquier cambio que se produzca respecto de la conservación o cualquier riesgo que puedan sufrir los bienes otorgados en prenda, dicha información debe realizarse por escrito dentro de los quinde (15) días siguientes de ocurrido el hecho. Trasladar la prenda a donde y cuando lo disponga <b>"EL ACREEDOR"</b>. Los bienes dados en prenda, no podrán ser cambiados del lugar de ubicación salvo consentimiento expreso de <b>"EL ACREEDOR".</b><br/> \
             Sobre los bienes de la prenda no existen obligaciones ni restricciones de ninguna clase que pudieran reclamar terceros, según declaración expresa que hace <b>"El(la)(los) DEUDOR(A)(ES)".</b>'
 
             self._parrafos.append(Paragraph(c+aux3, estilos['Justify']))
         else:
-            raise ContratoError("Campo requerido", "El contrato requiere los Datos de al menos un Garante")
+            raise ContratoError("Campo requerido", "El contrato requiere los Datos de al menos dos garantias reales")
         
         
         #LLAMAMOS A LOS FIADORES
         texto_10_3 = "<b>10.3.</b> Con la Garantía personal, solidaria, mancomunada e indivisible del (la)(los) señor(a)(es)"
         fiadores = self.get_fiadores()
         i=0
         for item in fiadores:
@@ -659,19 +656,19 @@
             transcrito, bienes, mercaderías, muebles e inmuebles, futuros sin exclusión ni limitación alguna. <b>"El(la)(los) \
             DEUDOR(A)(ES)"</b> se obliga(n) a no vender, ceder, transferir, etc., bajo ningún título los bienes \
             descritos en el formulario de Declaración Patrimonial, mientras perdure la obligación con GESTION Y \
             SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.'
         self._parrafos.append(Paragraph(texto_10_1, estilos['Justify']))
         #Sacado 10.2 de convenio
         if(self.__contrato["convenio"]):
-            asociacion=self.__contrato["convenio"]["sindicato"].upper() 
-            convenio_con=self.__contrato["convenio"]["abreviatura"].upper()
+            asociacion=self.__contrato["convenio"][0]["sindicato"].upper() 
+            convenio_con=self.__contrato["convenio"][0]["abreviatura"].upper()
             texto_10_2 =f' <b>10.2.</b> En forma señalada, con la garantía del(los) <b>DERECHO(S) DE LINEA</b> que posee(n) como \
                 propietario(s) en <b>{asociacion}</b>, y que \
-                pone a disposición de GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A. de \
+                pone a disposición de GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A. de \
                 acuerdo al Convenio Interinstitucional suscrito con <b>{convenio_con}</b>. Consiguientemente la(s) acción(es) de \
                 línea se constituye(n) en forma incondicional e irrestricta en garantía(s), dispuestas a hacerse líquidas \
                 para cubrir de forma total o parcial las obligaciones producto del presente contrato de <b>"El(la)(los) \
                 DEUDOR(A)(ES)"</b> con <b>"EL ACREEDOR"</b>, sin reserva, ni limitación alguna. Obligándose <b>"El(la)(los) \
                 DEUDOR(A)(ES)"</b> a mantener dicha(s) línea(s) libre(s) de multas y obligaciones con su sindicato o \
                 cualquier otra persona natural o jurídica.' 
             self._parrafos.append(Paragraph(texto_10_2, estilos['Justify']))
@@ -739,22 +736,22 @@
             <b>"El(la)(los) DEUDOR(A)(ES)"</b>, limitando su accionar a comunicar dicha cesión al domicilio señalado en \
             la cláusula primera.'
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
     
     def _autorizacion(self, numeral):
         texto = f'<b><u>{numeral}</u>.- (AUTORIZACION DE INVESTIGACION DE ANTECEDENTES CREDITICIOS).- \
             "El(la)(los) DEUDOR(A)(ES)" y "El(la)(los) FIADOR(A)(ES) PERSONAL(ES)"</b>, autoriza(n) en forma \
-            expresa a GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A. a solicitar \
+            expresa a GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A. a solicitar \
             información sobre sus antecedentes crediticios y otras cuentas por pagar de carácter económico, \
             financiero y comercial registrados en el BI y la CIC de la Autoridad de Supervisión del Sistema \
             Financiero (ASFI), mientras dure su relación contractual con el citado usuario.<br/>\
             Asimismo, autoriza(n):'
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
         a = '<bullet></bullet> Incorporar los datos crediticios y de otras cuentas por pagar de carácter económico, financiero y \
-            comercial derivados de la relación con GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL \
+            comercial derivados de la relación con GESTION Y SOPORTE DE PROYECTOS JESUS DEL \
             GRAN PODER S.A., en la(s) base(s) de datos de propiedad de los Burós de Información que \
             cuenten con Licencia de Funcionamiento de ASFI y en la CIC.' 
         b = '<bullet></bullet> Al registro de sus datos crediticios en las bases de datos de INFOCENTER S.A, con licencia de \
             funcionamiento del Organismo de Supervisión, ASFI.' 
         incisos = ListFlowable(
         [
             Paragraph(a,estilos['Inciso']),
@@ -771,22 +768,22 @@
         )
         self._parrafos.append(incisos)
     
     #12
     def _autorizacion4(self, numeral):
         texto = f'<b><u>{numeral}</u>.- (AUTORIZACION DE INVESTIGACION DE ANTECEDENTES CREDITICIOS).- \
             "El(la)(los) DEUDOR(A)(ES)" y "El(la)(los) GARANTE(S) PERSONAL(ES)"</b>, autoriza(n) en forma \
-            expresa a GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A. a solicitar \
+            expresa a GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A. a solicitar \
             información sobre sus antecedentes crediticios y otras cuentas por pagar de carácter económico, \
             financiero y comercial registrados en el BI y la CIC de la Autoridad de Supervisión del Sistema \
             Financiero (ASFI), mientras dure su relación contractual con el citado usuario.<br/>\
             Asimismo, autoriza(n):'
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
         a = '<bullet></bullet> Incorporar los datos crediticios y de otras cuentas por pagar de carácter económico, financiero y \
-            comercial derivados de la relación con GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL \
+            comercial derivados de la relación con GESTION Y SOPORTE DE PROYECTOS JESUS DEL \
             GRAN PODER S.A., en la(s) base(s) de datos de propiedad de los Burós de Información que \
             cuenten con Licencia de Funcionamiento de ASFI y en la CIC.' 
         b = '<bullet></bullet> Al registro de sus datos crediticios en las bases de datos de INFOCENTER S.A, con licencia de \
             funcionamiento del Organismo de Supervisión, ASFI.' 
         incisos = ListFlowable(
         [
             Paragraph(a,estilos['Inciso']),
@@ -946,34 +943,31 @@
     #PRIMERA 2
     def nombreCompleto_repre(self):
         nombre = (self.__contrato["testimonio_poder"]["representante_legal"]["first_name"]+" "+self.__contrato["testimonio_poder"]["representante_legal"]["last_name"]).upper()
         return nombre
     
     def get_deudores(self):   
         deudores=self.__contrato["deudores"]     
-        if(len(deudores)>0):
-            deudores_ = [item for item in deudores if (item["tipo_obligado"]=="1A" or item["tipo_obligado"]=="4A" or item["tipo_obligado"]=="5A" or item["tipo_obligado"]=="1B")]
-            return deudores_
-        else:
-            raise ContratoError("Campo requerido", "El contrato requiere los dados del(los) Deudor(es)")
+        deudores_ = [item for item in deudores if (item["tipo_obligado"]=="1A" or item["tipo_obligado"]=="4A" or item["tipo_obligado"]=="5A" or item["tipo_obligado"]=="1B")]
+        return deudores_
     
     def get_estado_civil(self,_estado_civil, genero):
         #diccionario para comprobar
         estados_civiles = {"S": "solter","C": "casad","V": "viud","D": "divorciad", "N":"solter"}
         if(genero =="F"): 
             return estados_civiles.get(_estado_civil) +"a"
         else:
             return estados_civiles.get(_estado_civil) +"o"
 
     def get_articulo_direccion(self,direccion_dato):
         #diccionario para comprobar  
         direccion = direccion_dato.split(' ')
         direccion_uno= direccion[0].lower()
         articulo=""
-        if(direccion_uno =="avenida" or direccion_uno =="calle" or direccion_uno =="av." or direccion_uno =="av"): 
+        if(direccion_uno =="avenida" or direccion_uno =="calle" or direccion_uno =="av."): 
             articulo = "la "
         if(direccion_uno =="pasaje" or direccion_uno =="callejon" or direccion_uno =="psje." or direccion_uno =="pje."): 
             articulo = "el "
         
         return articulo + direccion_dato
         
     def _partes_contratantes2(self, numeral):
@@ -985,15 +979,15 @@
         cargo = testimonio_poder["representante_legal"]["rol"]       
         numero_testimonio = testimonio_poder["numero_testimonio"]
         fecha_testimonio = Utils.get_fecha(self, testimonio_poder["fecha_testimonio"])
         numero_notaria = testimonio_poder["numero_notaria_publica"]
         responsable_notaria = testimonio_poder["nombre_notario_publico"]
         texto = f'<b><u>{numeral}</u>.- (PARTES CONTRATANTES)</b>.- Intervienen en la suscripción del presente contrato:' 
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
-        a = f'<b>GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A.</b>, sociedad \
+        a = f'<b>GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.</b>, sociedad \
             legalmente constituida bajo las leyes del Estado Plurinacional de Bolivia, con Matrícula de \
             Comercio y Número de Identificación Tributaria 173788022, con domicilio en la \
             {domicilio_legal} de esta ciudad, representada legalmente por <b>{apoderado}</b>, con C.I. Nº {numero_ci_apoderado}, mayor de edad, hábil \
             por derecho y vecino(a) de esta ciudad, en su condición de {cargo} en mérito al \
             Testimonio Poder No. {numero_testimonio} de fecha {fecha_testimonio} otorgado por ante la \
             Notaría de Fe Pública Nº {numero_notaria} del Distrito Judicial de La Paz a cargo de(la) Dr(a).\
             {responsable_notaria}, quien en adelante se denominará <b>"EL ACREEDOR"</b>.'      
@@ -1045,15 +1039,15 @@
         cargo = testimonio_poder["representante_legal"]["rol"]       
         numero_testimonio = testimonio_poder["numero_testimonio"]
         fecha_testimonio = Utils.get_fecha(self, testimonio_poder["fecha_testimonio"])
         numero_notaria = testimonio_poder["numero_notaria_publica"]
         responsable_notaria = testimonio_poder["nombre_notario_publico"]
         texto = f'<b><u>{numeral}</u>.- (PARTES CONTRATANTES)</b>.- Intervienen en la suscripción del presente contrato:' 
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
-        a = f'<b>GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A.</b>, sociedad \
+        a = f'<b>GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.</b>, sociedad \
             legalmente constituida bajo las leyes del Estado Plurinacional de Bolivia, con Matrícula de \
             Comercio y Número de Identificación Tributaria 173788022, con domicilio en la \
             {domicilio_legal} de esta ciudad, representada legalmente por <b>{apoderado}</b>, con C.I. Nº {numero_ci_apoderado}, mayor de edad, hábil \
             por derecho y vecino(a) de esta ciudad, en su condición de {cargo} en mérito al \
             Testimonio Poder No. {numero_testimonio} de fecha {fecha_testimonio} otorgado por ante la \
             Notaría de Fe Pública Nº {numero_notaria} del Distrito Judicial de La Paz a cargo de(la) Dr(a).\
             {responsable_notaria}, quien en adelante se denominará <b>"EL ACREEDOR"</b>.'      
@@ -1270,15 +1264,15 @@
         # LA API(http://192.168.100.5:8000/api/v1/contratos/501231701701/) DEVUEVE UN DICCIONAIO PERO EN EL ADMI SE 
         # ALMACENA COMO UNA ARRAY, SE AJUSTO A LO QUE SE TIENE EN EL ADMI
         if(self.__contrato["convenio"]):
             asociacion=self.__contrato["convenio"][0]["sindicato"].upper() 
             convenio_con=self.__contrato["convenio"][0]["abreviatura"].upper()
             texto_10_2 =f' <b>10.2.</b> En forma señalada, con la garantía del(los) <b>DERECHO(S) DE LINEA</b> que posee(n) como \
                 propietario(s) en <b>{asociacion}</b>, y que \
-                pone a disposición de GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A. de \
+                pone a disposición de GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A. de \
                 acuerdo al Convenio Interinstitucional suscrito con <b>{convenio_con}</b>. Consiguientemente la(s) acción(es) de \
                 línea se constituye(n) en forma incondicional e irrestricta en garantía(s), dispuestas a hacerse líquidas \
                 para cubrir de forma total o parcial las obligaciones producto del presente contrato de <b>"El(la)(los) \
                 DEUDOR(A)(ES)"</b> con <b>"EL ACREEDOR"</b>, sin reserva, ni limitación alguna. Obligándose <b>"El(la)(los) \
                 DEUDOR(A)(ES)"</b> a mantener dicha(s) línea(s) libre(s) de multas y obligaciones con su sindicato o \
                 cualquier otra persona natural o jurídica.<br/>\
                 Queda establecido que mientras no se haga efectivo el pago total y definitivo de la deuda y demás \
@@ -1322,15 +1316,15 @@
             SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.'
         self._parrafos.append(Paragraph(texto_10_1, estilos['Justify']))
         if(self.__contrato["convenio"]):
             asociacion=self.__contrato["convenio"][0]["sindicato"].upper()
             convenio_con=self.__contrato["convenio"][0]["abreviatura"].upper()
             texto_10_2 = f' <b>10.2.</b> En forma señalada, con la garantía del(los) <b>DERECHO(S) DE LINEA</b> que posee(n) como \
                 propietario(s) en <b>{asociacion}</b>, y que \
-                pone a disposición de GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A. de \
+                pone a disposición de GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A. de \
                 acuerdo al Convenio Interinstitucional suscrito con <b>{convenio_con}</b>. Consiguientemente la(s) acción(es) de \
                 línea se constituye(n) en forma incondicional e irrestricta en garantía(s), dispuestas a hacerse líquidas \
                 para cubrir de forma total o parcial las obligaciones producto del presente contrato de <b>"El(la)(los) \
                 DEUDOR(A)(ES)"</b> con <b>"EL ACREEDOR"</b>, sin reserva, ni limitación alguna. Obligándose <b>"El(la)(los) \
                 DEUDOR(A)(ES)"</b> a mantener dicha(s) línea(s) libre(s) de multas y obligaciones con su sindicato o \
                 cualquier otra persona natural o jurídica' 
             self._parrafos.append(Paragraph(texto_10_2, estilos['Justify']))
@@ -1355,16 +1349,14 @@
         colWidths=[30,230,86], rowHeights=None
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
             ('ALIGN',(0,-1),(-1,-1),'CENTER'),
             ('VALIGN',(0,-1),(-1,-1),'MIDDLE'),
-            ('BOTTOMPADDING',(0,0),(-1,-1),1),
-            ('TOPPADDING',(0,0),(-1,-1),1),
         ])
         self._parrafos.append(t)
         estilo = getSampleStyleSheet()
         P1 = Paragraph('''El tux templario''', estilo["BodyText"])
         i=0
         t = Table(
             data=[                
@@ -1376,17 +1368,15 @@
                 #para modificar el ancho de las columnas
             ], 
             colWidths=[30,230,86], rowHeights=None           
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
-            ('VALIGN', (0,0), (-1, -1), 'TOP'),    
-            ('BOTTOMPADDING',(0,0),(-1,-1),0),
-            ('TOPPADDING',(0,0),(-1,-1),0),         
+            ('VALIGN', (0,0), (-1, -1), 'TOP'),            
         ])
         self._parrafos.append(t)
         linea=Table(data=[''],colWidths=12.2*cm,rowHeights=0.02*cm,style=[('LINEABOVE',(0, 0), (-1, 0),1,colors.black)])
         self._parrafos.append(linea)
         self._parrafos.append(Spacer(0, 10))
         texto_10_3_continue ='Documentos originales de propiedad de <b>"El(la)(los) DEUDOR(A)(ES)"</b> y depositados en las oficinas de <b>"EL \
             ACREEDOR"</b> bajo libre y espontánea voluntad y sin presión alguna por parte del(la)(los) propietario(a)(s).<br/> \
@@ -1416,15 +1406,15 @@
             SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.'
         self._parrafos.append(Paragraph(texto_10_1, estilos['Justify']))
         if(self.__contrato["convenio"]):
             asociacion=self.__contrato["convenio"][0]["sindicato"].upper()
             convenio_con=self.__contrato["convenio"][0]["abreviatura"].upper()
             texto_10_2 = f' <b>10.2.</b> En forma señalada, con la garantía del(los) <b>DERECHO(S) DE LINEA</b> que posee(n) como \
                 propietario(s) en <b>{asociacion}</b>, y que \
-                pone a disposición de GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A. de \
+                pone a disposición de GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A. de \
                 acuerdo al Convenio Interinstitucional suscrito con <b>{convenio_con}</b>. Consiguientemente la(s) acción(es) de \
                 línea se constituye(n) en forma incondicional e irrestricta en garantía(s), dispuestas a hacerse líquidas \
                 para cubrir de forma total o parcial las obligaciones producto del presente contrato de <b>"El(la)(los) \
                 DEUDOR(A)(ES)"</b> con <b>"EL ACREEDOR"</b>, sin reserva, ni limitación alguna. Obligándose <b>"El(la)(los) \
                 DEUDOR(A)(ES)"</b> a mantener dicha(s) línea(s) libre(s) de multas y obligaciones con su sindicato o \
                 cualquier otra persona natural o jurídica'
             self._parrafos.append(Paragraph(texto_10_2, estilos['Justify']))
@@ -1447,16 +1437,14 @@
         colWidths=[30,230,86], rowHeights=None
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
             ('ALIGN',(0,-1),(-1,-1),'CENTER'),
             ('VALIGN',(0,-1),(-1,-1),'MIDDLE'),
-            ('BOTTOMPADDING',(0,0),(-1,-1),1),
-            ('TOPPADDING',(0,0),(-1,-1),1),
         ])
         self._parrafos.append(t)
         estilo = getSampleStyleSheet()
         P1 = Paragraph('''El tux templario''', estilo["BodyText"])
         i=0
         t = Table(
             data=[                
@@ -1468,17 +1456,15 @@
                 #para modificar el ancho de las columnas
             ], 
             colWidths=[30,230,86], rowHeights=None           
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
-            ('VALIGN', (0,0), (-1, -1), 'TOP'),  
-            ('BOTTOMPADDING',(0,0),(-1,-1),0),
-            ('TOPPADDING',(0,0),(-1,-1),0),           
+            ('VALIGN', (0,0), (-1, -1), 'TOP'),            
         ])
         self._parrafos.append(t)
         linea=Table(data=[''],colWidths=12.2*cm,rowHeights=0.02*cm,style=[('LINEABOVE',(0, 0), (-1, 0),1,colors.black)])
         self._parrafos.append(linea)
         self._parrafos.append(Spacer(0, 10))
         texto_10_3_continue ='<br/>Documentos originales de propiedad de <b>"El(la)(los) DEUDOR(A)(ES)"</b> y depositados en las oficinas de <b>"EL \
             ACREEDOR"</b> bajo libre y espontánea voluntad y sin presión alguna por parte del(la)(los) propietario(a)(s).<br/>\
@@ -1542,18 +1528,15 @@
             descritos en el formulario de Declaración Patrimonial, mientras perdure la obligación con GESTION Y \
             SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.'
         self._parrafos.append(Paragraph(texto_10_1, estilos['Justify']))
         #eliminado matricula
         texto_10_3 =f' <b>10.2.</b> En especial y en forma señalada, con la(s) garantía(s) de <b>OTROS DOCUMENTOS EN CUSTODIA</b> \
             registrado(s) bajo el siguiente detalle: '
         self._parrafos.append(Paragraph(texto_10_3, estilos['Justify']))
-        #salto de pagina
-        a=self._parrafos.append
-        a(PageBreak()) 
-        #salto de pagina
+        #jalo al json
         datos_garantias = self.__contrato["garantias_reales"]=self.filtrar_datos()
         if(len(datos_garantias)>0):
             P0 = Paragraph('''
                 <b>Nº</b>''')
             P1 = Paragraph('''
                 <b>DETALLE DEL DOCUMENTO</b>''')
             P2 = Paragraph('''
@@ -1563,16 +1546,14 @@
             colWidths=[30,230,86], rowHeights=None
             )
             t.setStyle([
                 ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
                 ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
                 ('ALIGN',(0,-1),(-1,-1),'CENTER'),
                 ('VALIGN',(0,-1),(-1,-1),'MIDDLE'),
-                ('BOTTOMPADDING',(0,0),(-1,-1),1),
-                ('TOPPADDING',(0,0),(-1,-1),1),
             ])
             self._parrafos.append(t)
             estilo = getSampleStyleSheet()
             P1 = Paragraph('''El tux templario''', estilo["BodyText"])
             i=0
             t = Table(
                 data=[                
@@ -1584,23 +1565,20 @@
                     #para modificar el ancho de las columnas
                 ], 
                 colWidths=[30,230,86], rowHeights=None           
             )
             t.setStyle([
                 ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
                 ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
-                ('VALIGN', (0,0), (-1, -1), 'TOP'),  
-                ('BOTTOMPADDING',(0,0),(-1,-1),0),
-                ('TOPPADDING',(0,0),(-1,-1),0),           
+                ('VALIGN', (0,0), (-1, -1), 'TOP'),            
             ])
             self._parrafos.append(t)
             linea=Table(data=[''],colWidths=12.2*cm,rowHeights=0.02*cm,style=[('LINEABOVE',(0, 0), (-1, 0),1,colors.black)])
             self._parrafos.append(linea)
             self._parrafos.append(Spacer(0, 10))
-            
         else:
                 raise ContratoError("Campo requerido", "El contrato requiere los Datos de garantias reales")
 
         texto_10_3_continue ='Documentos originales de propiedad de <b>"El(la)(los) DEUDOR(A)(ES)"</b> y depositados en las oficinas de <b>"EL \
             ACREEDOR"</b> bajo libre y espontánea voluntad y sin presión alguna por parte del(la)(los) propietario(a)(s).<br/>\
             Consiguientemente los Documentos del Inmueble se constituye(n) en forma incondicional e irrestricta en \
             garantía(s), dispuesta(s) a hacerse liquida para cubrir de forma total o parcial las obligaciones producto del \
@@ -1644,16 +1622,14 @@
         colWidths=[30,230,86], rowHeights=None
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
             ('ALIGN',(0,-1),(-1,-1),'CENTER'),
             ('VALIGN',(0,-1),(-1,-1),'MIDDLE'),
-            ('BOTTOMPADDING',(0,0),(-1,-1),1),
-            ('TOPPADDING',(0,0),(-1,-1),1),
         ])
         self._parrafos.append(t)
         estilo = getSampleStyleSheet()
         P1 = Paragraph('''El tux templario''', estilo["BodyText"])
         i=0
         t = Table(
             data=[                
@@ -1665,17 +1641,15 @@
                 #para modificar el ancho de las columnas
             ], 
             colWidths=[30,230,86], rowHeights=None           
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
-            ('VALIGN', (0,0), (-1, -1), 'TOP'),     
-            ('BOTTOMPADDING',(0,0),(-1,-1),0),
-            ('TOPPADDING',(0,0),(-1,-1),0),        
+            ('VALIGN', (0,0), (-1, -1), 'TOP'),            
         ])
         self._parrafos.append(t)
         linea=Table(data=[''],colWidths=12.2*cm,rowHeights=0.02*cm,style=[('LINEABOVE',(0, 0), (-1, 0),1,colors.black)])
         self._parrafos.append(linea)
         self._parrafos.append(Spacer(0, 10))
         
         texto_10_3_continue ='Documentos originales de propiedad de <b>"El(la)(los) DEUDOR(A)(ES)"</b> y depositados en las oficinas de <b>"EL \
@@ -1773,16 +1747,14 @@
         colWidths=[30,230,86], rowHeights=None
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
             ('ALIGN',(0,-1),(-1,-1),'CENTER'),
             ('VALIGN',(0,-1),(-1,-1),'MIDDLE'),
-            ('BOTTOMPADDING',(0,0),(-1,-1),1),
-            ('TOPPADDING',(0,0),(-1,-1),1),
         ])
         self._parrafos.append(t)
         estilo = getSampleStyleSheet()
         P1 = Paragraph('''El tux templario''', estilo["BodyText"])
         i=0
         t = Table(
             data=[                
@@ -1794,17 +1766,15 @@
                 #para modificar el ancho de las columnas
             ], 
             colWidths=[30,230,86], rowHeights=None           
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
-            ('VALIGN', (0,0), (-1, -1), 'TOP'), 
-            ('BOTTOMPADDING',(0,0),(-1,-1),0),
-            ('TOPPADDING',(0,0),(-1,-1),0),            
+            ('VALIGN', (0,0), (-1, -1), 'TOP'),            
         ])
         self._parrafos.append(t)
         linea=Table(data=[''],colWidths=12.2*cm,rowHeights=0.02*cm,style=[('LINEABOVE',(0, 0), (-1, 0),1,colors.black)])
         self._parrafos.append(linea)
         self._parrafos.append(Spacer(0, 10))
         texto_10_3_continue ='Documentos originales de propiedad de <b>"El(la)(los) DEUDOR(A)(ES)"</b> y depositados en las oficinas de <b>"EL \
         ACREEDOR"</b> bajo libre y espontánea voluntad y sin presión alguna por parte del(la)(los) propietario(a)(s).<br/>\
@@ -1859,15 +1829,14 @@
             descritos en el formulario de Declaración Patrimonial, mientras perdure la obligación con GESTION Y \
             SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.'
         self._parrafos.append(Paragraph(texto_10_1, estilos['Justify']))
         placa=self.get_placa()
         texto_10_2 =f' <b>10.2.</b> En especial y en forma señalada, con la(s) garantía(s) de <b>DOCUMENTOS EN CUSTODIA DEL \
             VEHÍCULO</b> con <b>{placa}</b>, bajo el siguiente detalle: ' 
         self._parrafos.append(Paragraph(texto_10_2, estilos['Justify']))
-        self._parrafos.append(Spacer(0, 10))
 
         datos_garantias = self.__contrato["garantias_reales"]=self.filtrar_datos()
         
         P0 = Paragraph('''
             <b>Nº</b>''')
         P1 = Paragraph('''
             <b>DETALLE DEL DOCUMENTO</b>''')
@@ -1878,35 +1847,34 @@
         colWidths=[30,230,86], rowHeights=None
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
             ('ALIGN',(0,-1),(-1,-1),'CENTER'),
             ('VALIGN',(0,-1),(-1,-1),'MIDDLE'),
-            ('BOTTOMPADDING',(0,0),(-1,-1),1),
-            ('TOPPADDING',(0,0),(-1,-1),1),
         ])
         self._parrafos.append(t)
+        estilo = getSampleStyleSheet()
+        P1 = Paragraph('''El tux templario''', estilo["BodyText"])
+        i=0
         t = Table(
             data=[                
                 (
                     str(i)+".",                    
                     Paragraph(items["concepto"].upper()+" "+items["detalle_garantia"].upper(),estilos["left"]),
                     Paragraph(items["fojas"],estilos["left"])
                 ) for i,items in enumerate(datos_garantias,1)
                 #para modificar el ancho de las columnas
             ], 
             colWidths=[30,230,86], rowHeights=None          
         )
         t.setStyle([
             ('LINEABOVE', (0,0), (-1, 0), 1, colors.black),
             ('INNERGRID', (-10,-5), (-20,-13), 0.65, colors.black),
-            ('VALIGN', (0,0), (-1, -1), 'TOP'),   
-            ('BOTTOMPADDING',(0,0),(-1,-1),0),
-            ('TOPPADDING',(0,0),(-1,-1),0),         
+            ('VALIGN', (0,0), (-1, -1), 'TOP'),            
         ])
         self._parrafos.append(t)
         linea=Table(data=[''],colWidths=12.2*cm,rowHeights=0.02*cm,style=[('LINEABOVE',(0, 0), (-1, 0),1,colors.black)])
         self._parrafos.append(linea)
         self._parrafos.append(Spacer(0, 10))
         texto_10_2_continue ='Documentos originales de propiedad de <b>"El(la)(los) DEUDOR(A)(ES)"</b> y depositados en las oficinas de <b>"EL \
         ACREEDOR"</b> bajo libre y espontánea voluntad y sin presión alguna por parte del(la)(los) propietario(a)(s).<br/>\
@@ -1988,22 +1956,22 @@
             así como a no constituir sobre el(los) mismo(s) ningún otro derecho especial a favor de terceras personales naturales o jurídicas, sin la expresa autorización escrita de <b>“EL \
             ACREEDOR"</b>.'
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
     
     #DÉCIMA TERCERA 2 
     def _autorizacion2(self, numeral):
         texto = f'<b><u>{numeral}</u>.- (AUTORIZACION DE INVESTIGACION DE ANTECEDENTES CREDITICIOS).- "El(la)(los) \
-            DEUDOR(A)(ES)"</b> autoriza(n) en forma expresa a GESTIÓN Y SOPORTE DE PROYECTOS JESÚS \
+            DEUDOR(A)(ES)"</b> autoriza(n) en forma expresa a GESTION Y SOPORTE DE PROYECTOS JESUS \
             DEL GRAN PODER S.A. a solicitar información sobre sus antecedentes crediticios y otras cuentas por pagar \
             de carácter económico, financiero y comercial registrados en el BI y la CIC de la Autoridad de Supervisión \
             del Sistema Financiero (ASFI), mientras dure su relación contractual con el citado usuario.<br/>\
             Asimismo, autoriza(n):'
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
         a = 'Incorporar los datos crediticios y de otras cuentas por pagar de carácter económico, financiero y \
-            comercial derivados de la relación con GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL \
+            comercial derivados de la relación con GESTION Y SOPORTE DE PROYECTOS JESUS DEL \
             GRAN PODER S.A., en la(s) base(s) de datos de propiedad de los Burós de Información que \
             cuenten con Licencia de Funcionamiento de ASFI y en la CIC.' 
         b = 'Al registro de sus datos crediticios en las bases de datos de INFOCENTER S.A, con licencia de \
             funcionamiento del Organismo de Supervisión, ASFI.' 
         incisos = ListFlowable(
         [
             Paragraph(a, estilos['Inciso']),
@@ -2019,22 +1987,22 @@
         bulletDedent=20        
         )
         self._parrafos.append(incisos)
     
     #DÉCIMA TERCERA 3'''Personal y Documentos en Custodia de Vehículo'''
     def _autorizacion3(self, numeral):
         texto = f'<b><u>{numeral}</u>.- (AUTORIZACION DE INVESTIGACION DE ANTECEDENTES CREDITICIOS).- "El(la) \
-            (los) DEUDOR(A)(ES)"</b> y <b>"El(la)(los) FIADOR(A)(ES) PERSONAL(ES)"</b>, autoriza(n) en forma expresa a GESTIÓN Y SOPORTE DE PROYECTOS JESÚS \
+            (los) DEUDOR(A)(ES)"</b> y <b>"El(la)(los) FIADOR(A)(ES) PERSONAL(ES)"</b>, autoriza(n) en forma expresa a GESTION Y SOPORTE DE PROYECTOS JESUS \
             DEL GRAN PODER S.A. a solicitar información sobre sus antecedentes crediticios y otras cuentas por pagar \
             de carácter económico, financiero y comercial registrados en el BI y la CIC de la Autoridad de Supervisión \
             del Sistema Financiero (ASFI), mientras dure su relación contractual con el citado usuario.<br/>\
             Asimismo, autoriza(n):'
         self._parrafos.append(Paragraph(texto, estilos['Justify']))
         a = 'Incorporar los datos crediticios y de otras cuentas por pagar de carácter económico, financiero y \
-            comercial derivados de la relación con GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL \
+            comercial derivados de la relación con GESTION Y SOPORTE DE PROYECTOS JESUS DEL \
             GRAN PODER S.A., en la(s) base(s) de datos de propiedad de los Burós de Información que \
             cuenten con Licencia de Funcionamiento de ASFI y en la CIC.' 
         b = 'Al registro de sus datos crediticios en las bases de datos de INFOCENTER S.A, con licencia de \
             funcionamiento del Organismo de Supervisión, ASFI.' 
         incisos = ListFlowable(
         [
             Paragraph(a, estilos['Inciso']),
@@ -2081,51 +2049,28 @@
     def get_fiadores(self):   
         deudores = self.__contrato["deudores"]     
         fiadores = [item for item in deudores if item['tipo_obligado']=='2A']
         return fiadores
     
     # FIRMAS
     def _firmas(self):
-        tipo_garantia=self.__contrato["tipo_garantia"]["descripcion"]
-        print()
-        print("!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!111")
-        print(tipo_garantia)
-
-        # modificando -----------------------------
-        if(tipo_garantia=="Quirografaria"):
-            a=self._parrafos.append
-            a(PageBreak())
-            
-        # modificando -------------------------------
         fiadores= self.get_fiadores()
         deudores= self.get_deudores()
-        if(tipo_garantia!="Quirografaria"):
-            self._parrafos.append(Spacer(0,15))
-
+        self._parrafos.append(Spacer(0,15))
         texto= ('POR SI, COMO DEUDOR(A)(ES) o PRESTATARIO(A)(S):')
         self._parrafos.append(Paragraph(texto,style = estilos["Justify"]))        
         self._posicion_firmas(deudores)
         self._parrafos.append(Spacer(0,0.5*cm))
         if (len(fiadores) > 0):
             self._parrafos.append(Spacer(0,1))
-            if(tipo_garantia=="Prendaria y Personal"):
-                a=self._parrafos.append
-                a(PageBreak()) 
-                texto= ('Y COMO DEPOSITARIO(S) Y/O GARANTE(S) SOLIDARIO(A)(S), MANCOMUNADO(A)(S) E INDIVISIBLE(S): ')
-            if(tipo_garantia!="Prendaria y Personal"):
-                texto= ('Y COMO FIADOR(A)(ES) SOLIDARIO(A)(S), MANCOMUNADO(A)(S) E INDIVISIBLE(S): ')
+            texto= ('Y COMO FIADOR(A)(ES) SOLIDARIO(A)(S), MANCOMUNADO(A)(S) E INDIVISIBLE(S): ')
             self._parrafos.append(Paragraph(texto,style = estilos["Justify"]))            
             self._posicion_firmas(fiadores)
             self._parrafos.append(Spacer(0,0.5*cm))
-            #garantes mas de 3 en Convenio y Garantia personal
-            if(tipo_garantia=="Convenio y Garantia personal" and len(fiadores)>=3):
-                a=self._parrafos.append
-                a(PageBreak())
-            
-        texto= ('POR <b>GESTIÓN Y SOPORTE DE PROYECTOS JESÚS DEL GRAN PODER S.A.</b>')
+        texto= ('POR <b>GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.</b>')
         self._parrafos.append(Paragraph(texto,style = estilos["Justify"]))  
         self._parrafos.append(Spacer(0,2.3*cm))
         dato_nombre = self.nombreCompleto_repre()
         dato_cargo = self.__contrato["testimonio_poder"]["representante_legal"]["rol"]
         t_firmas=Table(
                     data=[[dato_nombre+'\n'+dato_cargo]],colWidths=8*cm,
                     style=[('ALIGN',(0,0),(-1,-1),'CENTER'),('FONT', (0,0), (-1,-1), 'Helvetica-Bold', 10),])
@@ -2153,13 +2098,39 @@
                 else:
                     if(len(dato)==1):
                         self._parrafos.append(Spacer(0,2.3*cm))
                         t_firmas=Table(
                             data=[[dato_1[0]+'\nC.I. N° '+dato_1[1]]],colWidths=8*cm,
                             style=[('ALIGN',(0,0),(-1,-1),'CENTER'),('FONT', (0,0), (-1,-1), 'Helvetica-Bold', 10)])
                         self._parrafos.append(t_firmas)
+    #FIRMAS GARANTE
+    # FIRMAS
+    def _firmas2(self):
+        fiadores= self.get_fiadores()
+        deudores= self.get_deudores()
+        self._parrafos.append(Spacer(0,15))
+        texto= ('POR SI, COMO DEUDOR(A)(ES) o PRESTATARIO(A)(S):')
+        self._parrafos.append(Paragraph(texto,style = estilos["Justify"]))        
+        self._posicion_firmas(deudores)
+        self._parrafos.append(Spacer(0,0.5*cm))
+        if (len(fiadores) > 0):
+            self._parrafos.append(Spacer(0,1))
+            texto= ('Y COMO GARANTE(S) SOLIDARIO(A)(S), MANCOMUNADO(A)(S) E INDIVISIBLE(S): ')
+            self._parrafos.append(Paragraph(texto,style = estilos["Justify"]))            
+            self._posicion_firmas(fiadores)
+            self._parrafos.append(Spacer(0,0.5*cm))
+        texto= ('POR <b>GESTION Y SOPORTE DE PROYECTOS JESUS DEL GRAN PODER S.A.</b>')
+        self._parrafos.append(Paragraph(texto,style = estilos["Justify"]))  
+        self._parrafos.append(Spacer(0,2.3*cm))
+        dato_nombre = self.nombreCompleto_repre()
+        dato_cargo = self.__contrato["testimonio_poder"]["representante_legal"]["rol"]
+        t_firmas=Table(
+                    data=[[dato_nombre+'\n'+dato_cargo]],colWidths=8*cm,
+                    style=[('ALIGN',(0,0),(-1,-1),'CENTER'),('FONT', (0,0), (-1,-1), 'Helvetica-Bold', 10),])
+        self._parrafos.append(t_firmas)
+
     
     def generar1(self):
         buffer = BytesIO()   
         documentos(buffer).build(self._parrafos, onFirstPage=self._encabezado,  onLaterPages=self._encabezado)
         return buffer
```

### Comparing `jgp_report_creditos-0.0.12/jgp_report_creditos/core/contrato/v1/contratos.py` & `jgp_report_creditos-0.0.9/jgp_report_creditos/core/contrato/v1/contratos.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from reportlab.pdfgen import canvas
 from jgp_report_creditos.core.exception.exception import ContratoError
 
 from .base import BaseContrato
 
 class ContratoPersonal (BaseContrato):
     
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, json_enviado):
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(json_enviado)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía Personal')
             self._partes_contratantes('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza('CUARTA')
             self._intereses('QUINTA')
             self._plazo('SEXTA')
@@ -36,17 +36,17 @@
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))  
         finally:
             print("TERMINADO")
 
 #11 CONVENIO Y GARANTIA PERSONAL
 class ContratoConvenioGarantiaPersonal (BaseContrato):
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, contrato):
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía de Derecho de Línea y garantía Personal')
             self._partes_contratantes('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza('CUARTA')
             self._intereses_pyv('QUINTA')#garantes
             self._plazo('SEXTA')
@@ -73,17 +73,17 @@
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))  
         finally:
             print("TERMINADO")
 
 # 12 GARANTE DEPOSITARIO
 class ContratoPrendariayPersonal(BaseContrato):
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, contrato):
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía Prendaria y Personal')
             self._partes_contratantes3('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza3('CUARTA')
             self._intereses3('QUINTA')
             self._plazo('SEXTA')
@@ -97,29 +97,29 @@
             self._cesion_obligacion('DÉCIMA TERCERA')
             self._autorizacion4('DÉCIMA CUARTA')
             self._titulo_ejecutivo('DÉCIMA QUINTA')
             self._gastos('DÉCIMA SEXTA')
             self._derechos_deudor('DÉCIMA SÉPTIMA')
             self._domicilio_especial('DÉCIMA OCTAVA')
             self._aceptacion3('DÉCIMA NOVENA')
-            self._firmas()
+            self._firmas2()
         except ContratoError as ex:
             p1, p2 = ex.args
             print("°°°°°°°°°°° ERROR PERSONALIZADO: °°°°°°°°°°")
             self._error_mensaje(p1,p2)
         except Exception as e:
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))   
         finally:
             print("TERMINADO")
 # CONVENIO
 class ContratoConvenio (BaseContrato):
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, contrato):    
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía de Derecho de Línea')
             self._partes_contratantes2('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza2('CUARTA')
             self._intereses2('QUINTA')
             self._plazo('SEXTA')
@@ -146,17 +146,17 @@
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))  
         finally:
             print("TERMINADO")
 
 # CONVENIO Y DOC. CUSTODIA DE INMUEBLE   -------------------------REVISADO 1-1
 class ContratoConvenioCustodiaInmueble (BaseContrato):
-    def __init__(self, json_enviado, usuario):
-        try:
-            super().__init__(json_enviado, usuario)
+    def __init__(self, contrato):
+        try:    
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía de Derecho de Línea y Garantía de Documentos en Custodia de Inmueble')        
             self._partes_contratantes2('PRIMERA')       
             self._objeto_del_contrato('SEGUNDA')       
             self._desembolso('TERCERA')       
             self._gestion_cobranza2('CUARTA')        
             self._intereses2('QUINTA')        
             self._plazo('SEXTA')        
@@ -183,17 +183,17 @@
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))   
         finally:
             print("TERMINADO")
 
 # CONVENIO Y DOC. CUSTODIA DE VEHÍCULO   
 class ContratoConvenioCustodiaVehiculo (BaseContrato):
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, contrato):
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía de Derecho de Línea y Garantía de Documentos en Custodia de Vehículo')
             self._partes_contratantes2('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza2('CUARTA')
             self._intereses2('QUINTA')
             self._plazo('SEXTA')
@@ -220,17 +220,17 @@
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e)) 
         finally:
             print("TERMINADO")
 
 # DOC. CUSTODIA DE INMUEBLE DE PAMPAHASI M
 class ContratoCustosiaInmueblePampahasi (BaseContrato):
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, contrato):
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía de Documentos en Custodia de Inmueble')
             self._partes_contratantes2('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza2('CUARTA')
             self._intereses2('QUINTA')
             self._plazo('SEXTA')
@@ -257,17 +257,17 @@
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))    
         finally:
             print("TERMINADO")
 
 # Documentos en Custodia de Vehículo M  ------EN REV
 class ContratoDocumentoCustodiaVehiculo (BaseContrato):
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, contrato):
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía de Documentos en Custodia de vehículo')
             self._partes_contratantes2('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza2('CUARTA')
             self._intereses2('QUINTA')
             self._plazo('SEXTA')
@@ -294,17 +294,17 @@
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))    
         finally:
             print("TERMINADO")
 
 # Otros Documentos en Custodia (patente) M
 class ContratoOtroDocumentoCustodiaPatente (BaseContrato):
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, contrato):
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía de Otros Documentos en Custodia')
             self._partes_contratantes2('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza2('CUARTA')
             self._intereses2('QUINTA')
             self._plazo('SEXTA')
@@ -330,17 +330,17 @@
         except Exception as e:
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))    
         finally:
             print("TERMINADO")
 # Personal y Documentos en Custodia de Vehículo M
 class ContratoPersonalDocumentosCustodiaVehiculo (BaseContrato):
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, contrato):
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía Personal y Documentos en Custodia de vehículo')
             self._partes_contratantes('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza('CUARTA')
             self._intereses_pyv('QUINTA')
             self._plazo('SEXTA')
@@ -366,17 +366,17 @@
         except Exception as e:
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))    
         finally:
             print("TERMINADO")
 # Quirografaria OFICINA EL CARMEN
 class ContratoQuirografariaOficinaElCarmen (BaseContrato):
-    def __init__(self, json_enviado, usuario):
-        try:
-            super().__init__(json_enviado, usuario)
+    def __init__(self, contrato):
+        try :
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía Quirografaria')
             self._partes_contratantes2('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza2('CUARTA')
             self._intereses2('QUINTA')
             self._plazo('SEXTA')
@@ -403,17 +403,17 @@
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))   
         finally:
             print("TERMINADO")
             
 # Solidario
 class ContratoSolidario (BaseContrato):
-    def __init__(self, json_enviado, usuario):
+    def __init__(self, contrato):
         try:
-            super().__init__(json_enviado, usuario)
+            super().__init__(contrato)
             self._tipo_contrato('PRESTAMO DE DINERO o MUTUO bajo garantía Solidaria')
             self._partes_contratantes2Soli('PRIMERA')
             self._objeto_del_contrato('SEGUNDA')
             self._desembolso('TERCERA')
             self._gestion_cobranza2('CUARTA')
             self._intereses2('QUINTA')
             self._plazo('SEXTA')
@@ -438,10 +438,10 @@
         except Exception as e:
             print("ERROR INESPERADO!!!!!") 
             self._error_mensaje("Error inesperado",repr(e))    
         finally:
             print("TERMINADO")
 # CONTRATO ERROR BASE
 class ContratoErrorBase(BaseContrato):
-    def __init__(self, json_enviado, usuario):
-        super().__init__(json_enviado, usuario)
+    def __init__(self, contrato):
+        super().__init__(contrato)
         self._error_mensaje("Error en el contrato","Tipo de garantia desconocido")
```

### Comparing `jgp_report_creditos-0.0.12/jgp_report_creditos/test.py` & `jgp_report_creditos-0.0.9/jgp_report_creditos/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 #from report import makeContato
 from jgp_report_creditos import makeContato
 
 if  __name__ == '__main__':     
     print(" ªªªªªªªªªªªªªªªªªªªªªªªªªªªªªªªªª test ªªªªªªªªªªªªªªªªªªªªªªªªªª")
-    parametros ="401211601714"
+    parametros ="501211601894"
     #datos_json= json.load(requests.get("http://190.181.25.202:8003/api/v1/cre/contrato/"+parametros).text)
     #http://192.168.100.5:8000/api/v1/contratos/501211601894/
     datos_json = requests.get("http://192.168.100.5:8000/api/v1/contratos/"+parametros).text
     print("ddddddddddddddddddddddddddddddddddddddd")
 
     #ESTA LLAMADA CREA EL PDF
     print(datos_json)
```

### Comparing `jgp_report_creditos-0.0.12/jgp_report_creditos.egg-info/PKG-INFO` & `jgp_report_creditos-0.0.9/jgp_report_creditos.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,104 +1,104 @@
 Metadata-Version: 2.1
 Name: jgp-report-creditos
-Version: 0.0.12
+Version: 0.0.9
 Summary: Librería con funciones y herramientas útiles exclusivas para jgp
 Home-page: https://gitlab.com/develop-team-jdgp/jgp-report-creditos.git
 Author: JGP Dev
 Author-email: jgpdev20@gmail.com
 License: MIT
+Description: # jgp-report-creditos
+        
+        
+        
+        ## Getting started
+        
+        To make it easy for you to get started with GitLab, here's a list of recommended next steps.
+        
+        Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!
+        
+        ## Add your files
+        
+        - [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
+        - [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
+        
+        ```
+        cd existing_repo
+        git remote add origin https://gitlab.com/develop-team-jdgp/jgp-report-creditos.git
+        git branch -M main
+        git push -uf origin main
+        ```
+        
+        ## Integrate with your tools
+        
+        - [ ] [Set up project integrations](https://gitlab.com/develop-team-jdgp/jgp-report-creditos/-/settings/integrations)
+        
+        ## Collaborate with your team
+        
+        - [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
+        - [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
+        - [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
+        - [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
+        - [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)
+        
+        ## Test and Deploy
+        
+        Use the built-in continuous integration in GitLab.
+        
+        - [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
+        - [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
+        - [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
+        - [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
+        - [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)
+        
+        ***
+        
+        # Editing this README
+        
+        When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.
+        
+        ## Suggestions for a good README
+        Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.
+        
+        ## Name
+        Choose a self-explaining name for your project.
+        
+        ## Description
+        Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
+        
+        ## Badges
+        On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.
+        
+        ## Visuals
+        Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.
+        
+        ## Installation
+        Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.
+        
+        ## Usage
+        Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
+        
+        ## Support
+        Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.
+        
+        ## Roadmap
+        If you have ideas for releases in the future, it is a good idea to list them in the README.
+        
+        ## Contributing
+        State if you are open to contributions and what your requirements are for accepting them.
+        
+        For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.
+        
+        You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.
+        
+        ## Authors and acknowledgment
+        Show your appreciation to those who have contributed to the project.
+        
+        ## License
+        For open source projects, say how it is licensed.
+        
+        ## Project status
+        If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
+        
 Keywords: python,primer paquete jgp
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# jgp-report-creditos
-
-
-
-## Getting started
-
-To make it easy for you to get started with GitLab, here's a list of recommended next steps.
-
-Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!
-
-## Add your files
-
-- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
-- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:
-
-```
-cd existing_repo
-git remote add origin https://gitlab.com/develop-team-jdgp/jgp-report-creditos.git
-git branch -M main
-git push -uf origin main
-```
-
-## Integrate with your tools
-
-- [ ] [Set up project integrations](https://gitlab.com/develop-team-jdgp/jgp-report-creditos/-/settings/integrations)
-
-## Collaborate with your team
-
-- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
-- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
-- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
-- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
-- [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)
-
-## Test and Deploy
-
-Use the built-in continuous integration in GitLab.
-
-- [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
-- [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
-- [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
-- [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
-- [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)
-
-***
-
-# Editing this README
-
-When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.
-
-## Suggestions for a good README
-Every project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.
-
-## Name
-Choose a self-explaining name for your project.
-
-## Description
-Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
-
-## Badges
-On some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.
-
-## Visuals
-Depending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.
-
-## Installation
-Within a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.
-
-## Usage
-Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
-
-## Support
-Tell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.
-
-## Roadmap
-If you have ideas for releases in the future, it is a good idea to list them in the README.
-
-## Contributing
-State if you are open to contributions and what your requirements are for accepting them.
-
-For people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.
-
-You can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.
-
-## Authors and acknowledgment
-Show your appreciation to those who have contributed to the project.
-
-## License
-For open source projects, say how it is licensed.
-
-## Project status
-If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
```

### Comparing `jgp_report_creditos-0.0.12/jgp_report_creditos.egg-info/SOURCES.txt` & `jgp_report_creditos-0.0.9/jgp_report_creditos.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,16 @@
-LICENSE
 README.md
 setup.py
 jgp_report_creditos/__init__.py
 jgp_report_creditos/report.py
 jgp_report_creditos/test.py
 jgp_report_creditos.egg-info/PKG-INFO
 jgp_report_creditos.egg-info/SOURCES.txt
 jgp_report_creditos.egg-info/dependency_links.txt
 jgp_report_creditos.egg-info/top_level.txt
 jgp_report_creditos/core/__init__.py
-jgp_report_creditos/core/deposito.py
-jgp_report_creditos/core/rutas.py
 jgp_report_creditos/core/contrato/__init__.py
-jgp_report_creditos/core/contrato/v1/Controlar tablas de firmas.py
 jgp_report_creditos/core/contrato/v1/__init__.py
 jgp_report_creditos/core/contrato/v1/base.py
 jgp_report_creditos/core/contrato/v1/contratos.py
 jgp_report_creditos/core/exception/__init__.py
-jgp_report_creditos/core/exception/exception.py
-jgp_report_creditos/resources/img/logo_jgp.png
-jgp_report_creditos/template/__init__.py
-jgp_report_creditos/template/components.py
-jgp_report_creditos/template/template.py
-jgp_report_creditos/tests/__init__.py
-jgp_report_creditos/tests/test_contratos.py
-jgp_report_creditos/tests/test_deposito.py
+jgp_report_creditos/core/exception/exception.py
```

### Comparing `jgp_report_creditos-0.0.12/setup.py` & `jgp_report_creditos-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.12' 
+VERSION = '0.0.9' 
 PACKAGE_NAME = 'jgp_report_creditos' 
 AUTHOR = 'JGP Dev' 
 AUTHOR_EMAIL = 'jgpdev20@gmail.com' 
 URL = 'https://gitlab.com/develop-team-jdgp/jgp-report-creditos.git'
 
 LICENSE = 'MIT' 
 DESCRIPTION = 'Librería con funciones y herramientas útiles exclusivas para jgp'
```
