# Comparing `tmp/plone.app.robotframework-2.0.1.tar.gz` & `tmp/plone.app.robotframework-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.robotframework-2.0.1.tar", last modified: Wed Feb 22 17:38:59 2023, max compression
+gzip compressed data, was "plone.app.robotframework-2.1.0.tar", last modified: Fri Jul 14 09:57:08 2023, max compression
```

## Comparing `plone.app.robotframework-2.0.1.tar` & `plone.app.robotframework-2.1.0.tar`

### file list

```diff
@@ -1,129 +1,131 @@
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:38:59.980787 plone.app.robotframework-2.0.1/
--rw-r--r--   0 gil       (1000) gil       (1000)    20951 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/CHANGES.rst
--rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/CONTRIBUTING.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      493 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/CONTRIBUTORS.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      116 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/MANIFEST.in
--rw-r--r--   0 gil       (1000) gil       (1000)    22940 2023-02-22 17:38:59.980787 plone.app.robotframework-2.0.1/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)      574 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/README.rst
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:38:59.969787 plone.app.robotframework-2.0.1/docs/
--rw-r--r--   0 gil       (1000) gil       (1000)    18092 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/LICENSE.GPL
--rw-r--r--   0 gil       (1000) gil       (1000)      733 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/LICENSE.txt
--rwxr-xr-x   0 gil       (1000) gil       (1000)     1844 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/libdoc.sh
--rw-r--r--   0 gil       (1000) gil       (1000)      142 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/requirements.txt
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:38:59.971787 plone.app.robotframework-2.0.1/docs/source/
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:38:59.971787 plone.app.robotframework-2.0.1/docs/source/_static/
--rw-r--r--   0 gil       (1000) gil       (1000)       23 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/_static/README
--rw-r--r--   0 gil       (1000) gil       (1000)      640 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/bdd.txt
--rw-r--r--   0 gil       (1000) gil       (1000)     8072 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/conf.py
--rw-r--r--   0 gil       (1000) gil       (1000)     3191 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/debugging.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     1031 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/examples.rst
--rw-r--r--   0 gil       (1000) gil       (1000)    12859 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/happy.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     5220 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/index.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     3218 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/keywords.rst
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:38:59.974787 plone.app.robotframework-2.0.1/docs/source/libdoc/
--rw-r--r--   0 gil       (1000) gil       (1000)   128197 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/libdoc/python_debugging.html
--rw-r--r--   0 gil       (1000) gil       (1000)   128191 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/libdoc/python_layoutmath.html
--rw-r--r--   0 gil       (1000) gil       (1000)   128179 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/libdoc/python_saucelabs.html
--rw-r--r--   0 gil       (1000) gil       (1000)   129496 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/libdoc/python_zope2server.html
--rw-r--r--   0 gil       (1000) gil       (1000)   129773 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/libdoc/remote_autologin.html
--rw-r--r--   0 gil       (1000) gil       (1000)   130080 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/libdoc/remote_content.html
--rw-r--r--   0 gil       (1000) gil       (1000)   128563 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/libdoc/remote_genericsetup.html
--rw-r--r--   0 gil       (1000) gil       (1000)   128845 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/libdoc/remote_i18n.html
--rw-r--r--   0 gil       (1000) gil       (1000)   129081 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/libdoc/remote_mockmailhost.html
--rw-r--r--   0 gil       (1000) gil       (1000)   129106 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/libdoc/remote_quickinstaller.html
--rw-r--r--   0 gil       (1000) gil       (1000)   128612 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/libdoc/remote_users.html
--rw-r--r--   0 gil       (1000) gil       (1000)   128522 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/libdoc/remote_zope2server.html
--rw-r--r--   0 gil       (1000) gil       (1000)   109491 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/libdoc/selenium.html
--rw-r--r--   0 gil       (1000) gil       (1000)   136653 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/libdoc/user_keywords.html
--rw-r--r--   0 gil       (1000) gil       (1000)   128668 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/libdoc/user_saucelabs.html
--rw-r--r--   0 gil       (1000) gil       (1000)   130665 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/libdoc/user_selenium.html
--rw-r--r--   0 gil       (1000) gil       (1000)   128392 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/libdoc/user_server.html
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:38:59.974787 plone.app.robotframework-2.0.1/docs/source/plone-keywords/
--rw-r--r--   0 gil       (1000) gil       (1000)      864 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/plone-keywords/browser.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     2032 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/plone-keywords/content.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      291 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/plone-keywords/edit-wizard-tabs.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      303 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/plone-keywords/generic.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      241 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/plone-keywords/history.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     2896 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/plone-keywords/index.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      351 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/plone-keywords/login.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      902 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/reload.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     1453 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/remote.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      917 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/ride.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     6102 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/robot.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     3981 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/saucelabs.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     1086 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/server.rst
--rw-r--r--   0 gil       (1000) gil       (1000)    13988 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/templer.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     1655 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/travis-ci.rst
--rw-r--r--   0 gil       (1000) gil       (1000)    10381 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/docs/source/tutorial.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      397 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/pyproject.toml
--rw-r--r--   0 gil       (1000) gil       (1000)      225 2023-02-22 17:38:59.981787 plone.app.robotframework-2.0.1/setup.cfg
--rw-r--r--   0 gil       (1000) gil       (1000)     3806 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/setup.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:38:59.968787 plone.app.robotframework-2.0.1/src/
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:38:59.975787 plone.app.robotframework-2.0.1/src/plone/
--rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:38:59.975787 plone.app.robotframework-2.0.1/src/plone/app/
--rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:38:59.979787 plone.app.robotframework-2.0.1/src/plone/app/robotframework/
--rw-r--r--   0 gil       (1000) gil       (1000)     1223 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)      430 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/_variables.robot
--rw-r--r--   0 gil       (1000) gil       (1000)      493 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/annotate.py
--rw-r--r--   0 gil       (1000) gil       (1000)    12936 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/annotate.robot
--rw-r--r--   0 gil       (1000) gil       (1000)     2172 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/autologin.py
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/config.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:38:59.979787 plone.app.robotframework-2.0.1/src/plone/app/robotframework/content/
--rw-r--r--   0 gil       (1000) gil       (1000)    74429 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/content/file.pdf
--rw-r--r--   0 gil       (1000) gil       (1000)     5131 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/content/image.jpg
--rw-r--r--   0 gil       (1000) gil       (1000)    10684 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/content.py
--rw-r--r--   0 gil       (1000) gil       (1000)      449 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/genericsetup.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2068 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/i18n.py
--rw-r--r--   0 gil       (1000) gil       (1000)      607 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/keywords.py
--rw-r--r--   0 gil       (1000) gil       (1000)    10047 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/keywords.robot
--rw-r--r--   0 gil       (1000) gil       (1000)      138 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/keywords.txt
--rw-r--r--   0 gil       (1000) gil       (1000)      505 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/mailhost.py
--rw-r--r--   0 gil       (1000) gil       (1000)      715 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/patches.py
--rw-r--r--   0 gil       (1000) gil       (1000)      945 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/pybabel.py
--rw-r--r--   0 gil       (1000) gil       (1000)      830 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/quickinstaller.py
--rw-r--r--   0 gil       (1000) gil       (1000)     8887 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/reload.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2385 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/remote.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2903 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/robotentrypoints.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1396 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/saucelabs.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1528 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/saucelabs.robot
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:38:59.979787 plone.app.robotframework-2.0.1/src/plone/app/robotframework/selectors/
--rw-r--r--   0 gil       (1000) gil       (1000)      154 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/selectors/cmfplone43.robot
--rw-r--r--   0 gil       (1000) gil       (1000)      154 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/selectors/cmfplone50.robot
--rw-r--r--   0 gil       (1000) gil       (1000)      142 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/selectors/cmfplone60.robot
--rw-r--r--   0 gil       (1000) gil       (1000)     6331 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/selenium.robot
--rw-r--r--   0 gil       (1000) gil       (1000)    14069 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/server.py
--rw-r--r--   0 gil       (1000) gil       (1000)      853 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/server.robot
--rw-r--r--   0 gil       (1000) gil       (1000)      134 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/server.txt
--rw-r--r--   0 gil       (1000) gil       (1000)      584 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/speak.robot
--rw-r--r--   0 gil       (1000) gil       (1000)    11376 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/testing.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:38:59.980787 plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:38:59.980787 plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/docs/
--rw-r--r--   0 gil       (1000) gil       (1000)      347 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/docs/test_hello.robot
--rw-r--r--   0 gil       (1000) gil       (1000)      934 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/docs/test_keywords.robot
--rw-r--r--   0 gil       (1000) gil       (1000)     3248 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/test_autologin_library.robot
--rw-r--r--   0 gil       (1000) gil       (1000)     2603 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/test_content.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2407 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/test_content_library.robot
--rw-r--r--   0 gil       (1000) gil       (1000)      439 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/test_i18n_library.robot
--rw-r--r--   0 gil       (1000) gil       (1000)      434 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/test_quickinstaller_library.robot
--rw-r--r--   0 gil       (1000) gil       (1000)     1999 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/test_robot.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1271 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/test_robotfixture.py
--rw-r--r--   0 gil       (1000) gil       (1000)      410 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/test_robotfixture.robot
--rw-r--r--   0 gil       (1000) gil       (1000)     3650 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/test_speakjs_library.robot
--rw-r--r--   0 gil       (1000) gil       (1000)     1205 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/test_users_library.robot
--rw-r--r--   0 gil       (1000) gil       (1000)      955 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/user.robot
--rw-r--r--   0 gil       (1000) gil       (1000)     1821 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/users.py
--rw-r--r--   0 gil       (1000) gil       (1000)      228 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/utils.py
--rw-r--r--   0 gil       (1000) gil       (1000)      510 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/variables.py
--rw-r--r--   0 gil       (1000) gil       (1000)      163 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone/app/robotframework/variables.robot
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-02-22 17:38:59.975787 plone.app.robotframework-2.0.1/src/plone.app.robotframework.egg-info/
--rw-r--r--   0 gil       (1000) gil       (1000)    22940 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone.app.robotframework.egg-info/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)     4355 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone.app.robotframework.egg-info/SOURCES.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone.app.robotframework.egg-info/dependency_links.txt
--rw-r--r--   0 gil       (1000) gil       (1000)      424 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone.app.robotframework.egg-info/entry_points.txt
--rw-r--r--   0 gil       (1000) gil       (1000)       16 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone.app.robotframework.egg-info/namespace_packages.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone.app.robotframework.egg-info/not-zip-safe
--rw-r--r--   0 gil       (1000) gil       (1000)      583 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone.app.robotframework.egg-info/requires.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-02-22 17:38:59.000000 plone.app.robotframework-2.0.1/src/plone.app.robotframework.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 09:57:08.927214 plone.app.robotframework-2.1.0/
+-rw-r--r--   0 maurits    (501) staff       (20)    21202 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      493 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/CONTRIBUTORS.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      116 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    23191 2023-07-14 09:57:08.927368 plone.app.robotframework-2.1.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      574 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 09:57:08.892222 plone.app.robotframework-2.1.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    18092 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      733 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/LICENSE.txt
+-rwxr-xr-x   0 maurits    (501) staff       (20)     1844 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/libdoc.sh
+-rw-r--r--   0 maurits    (501) staff       (20)      142 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/requirements.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 09:57:08.897171 plone.app.robotframework-2.1.0/docs/source/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 09:57:08.897422 plone.app.robotframework-2.1.0/docs/source/_static/
+-rw-r--r--   0 maurits    (501) staff       (20)       23 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/_static/README
+-rw-r--r--   0 maurits    (501) staff       (20)      640 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/bdd.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     8072 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3191 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/debugging.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1031 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/examples.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    12859 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/happy.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5220 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3218 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/keywords.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 09:57:08.905935 plone.app.robotframework-2.1.0/docs/source/libdoc/
+-rw-r--r--   0 maurits    (501) staff       (20)   128197 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/libdoc/python_debugging.html
+-rw-r--r--   0 maurits    (501) staff       (20)   128191 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/libdoc/python_layoutmath.html
+-rw-r--r--   0 maurits    (501) staff       (20)   128179 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/libdoc/python_saucelabs.html
+-rw-r--r--   0 maurits    (501) staff       (20)   129496 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/libdoc/python_zope2server.html
+-rw-r--r--   0 maurits    (501) staff       (20)   129773 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/libdoc/remote_autologin.html
+-rw-r--r--   0 maurits    (501) staff       (20)   130080 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/libdoc/remote_content.html
+-rw-r--r--   0 maurits    (501) staff       (20)   128563 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/libdoc/remote_genericsetup.html
+-rw-r--r--   0 maurits    (501) staff       (20)   128845 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/libdoc/remote_i18n.html
+-rw-r--r--   0 maurits    (501) staff       (20)   129081 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/libdoc/remote_mockmailhost.html
+-rw-r--r--   0 maurits    (501) staff       (20)   129106 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/libdoc/remote_quickinstaller.html
+-rw-r--r--   0 maurits    (501) staff       (20)   128612 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/libdoc/remote_users.html
+-rw-r--r--   0 maurits    (501) staff       (20)   128522 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/libdoc/remote_zope2server.html
+-rw-r--r--   0 maurits    (501) staff       (20)   109491 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/libdoc/selenium.html
+-rw-r--r--   0 maurits    (501) staff       (20)   136653 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/libdoc/user_keywords.html
+-rw-r--r--   0 maurits    (501) staff       (20)   128668 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/libdoc/user_saucelabs.html
+-rw-r--r--   0 maurits    (501) staff       (20)   130665 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/libdoc/user_selenium.html
+-rw-r--r--   0 maurits    (501) staff       (20)   128392 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/libdoc/user_server.html
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 09:57:08.908428 plone.app.robotframework-2.1.0/docs/source/plone-keywords/
+-rw-r--r--   0 maurits    (501) staff       (20)      864 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/plone-keywords/browser.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2032 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/plone-keywords/content.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      291 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/plone-keywords/edit-wizard-tabs.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      303 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/plone-keywords/generic.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      241 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/plone-keywords/history.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2896 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/plone-keywords/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      351 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/plone-keywords/login.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      902 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/reload.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1453 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/remote.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      917 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/ride.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6102 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/robot.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3981 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/saucelabs.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1086 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/server.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    13988 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/templer.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1655 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/travis-ci.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    10381 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/docs/source/tutorial.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      397 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      225 2023-07-14 09:57:08.927962 plone.app.robotframework-2.1.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     3836 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 09:57:08.887440 plone.app.robotframework-2.1.0/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 09:57:08.908712 plone.app.robotframework-2.1.0/src/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 09:57:08.911496 plone.app.robotframework-2.1.0/src/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 09:57:08.920863 plone.app.robotframework-2.1.0/src/plone/app/robotframework/
+-rw-r--r--   0 maurits    (501) staff       (20)     1223 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      430 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/_variables.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      493 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/annotate.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12936 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/annotate.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2172 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/autologin.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3187 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/browser.robot
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/config.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 09:57:08.921725 plone.app.robotframework-2.1.0/src/plone/app/robotframework/content/
+-rw-r--r--   0 maurits    (501) staff       (20)    74429 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/content/file.pdf
+-rw-r--r--   0 maurits    (501) staff       (20)     5131 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/content/image.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)    10684 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/content.py
+-rw-r--r--   0 maurits    (501) staff       (20)      449 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/genericsetup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2068 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/i18n.py
+-rw-r--r--   0 maurits    (501) staff       (20)      607 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/keywords.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9712 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/keywords.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      138 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/keywords.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      505 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/mailhost.py
+-rw-r--r--   0 maurits    (501) staff       (20)      715 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/patches.py
+-rw-r--r--   0 maurits    (501) staff       (20)      945 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/pybabel.py
+-rw-r--r--   0 maurits    (501) staff       (20)      830 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/quickinstaller.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8887 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/reload.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2385 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/remote.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2903 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/robotentrypoints.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1396 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/saucelabs.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1528 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/saucelabs.robot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 09:57:08.922783 plone.app.robotframework-2.1.0/src/plone/app/robotframework/selectors/
+-rw-r--r--   0 maurits    (501) staff       (20)      154 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/selectors/cmfplone43.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      154 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/selectors/cmfplone50.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      142 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/selectors/cmfplone60.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     6331 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/selenium.robot
+-rw-r--r--   0 maurits    (501) staff       (20)    14069 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/server.py
+-rw-r--r--   0 maurits    (501) staff       (20)      853 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/server.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      134 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/server.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      584 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/speak.robot
+-rw-r--r--   0 maurits    (501) staff       (20)    11376 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 09:57:08.926375 plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 09:57:08.927002 plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)      347 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/docs/test_hello.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      934 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/docs/test_keywords.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     3248 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/test_autologin_library.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      535 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/test_browser_library.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2603 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/test_content.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2407 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/test_content_library.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      439 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/test_i18n_library.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      434 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/test_quickinstaller_library.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2164 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1271 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/test_robotfixture.py
+-rw-r--r--   0 maurits    (501) staff       (20)      410 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/test_robotfixture.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     3650 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/test_speakjs_library.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1205 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/test_users_library.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      955 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/user.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1821 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/users.py
+-rw-r--r--   0 maurits    (501) staff       (20)      228 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)      510 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/variables.py
+-rw-r--r--   0 maurits    (501) staff       (20)      163 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone/app/robotframework/variables.robot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 09:57:08.911254 plone.app.robotframework-2.1.0/src/plone.app.robotframework.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    23191 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone.app.robotframework.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4460 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone.app.robotframework.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone.app.robotframework.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      424 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone.app.robotframework.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone.app.robotframework.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone.app.robotframework.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      606 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone.app.robotframework.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-07-14 09:57:08.000000 plone.app.robotframework-2.1.0/src/plone.app.robotframework.egg-info/top_level.txt
```

### Comparing `plone.app.robotframework-2.0.1/CHANGES.rst` & `plone.app.robotframework-2.1.0/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.1.0 (2023-07-14)
+------------------
+
+New features:
+
+
+- Add support for `playwright`-based tests via `robotframework-browser`.
+  [datakurre] (#3813)
+
+
+Bug fixes:
+
+
+- Remove unused and empty keyword that was displaying an error.
+  [gforcada] (#147)
+
+
 2.0.1 (2023-02-22)
 ------------------
 
 Bug fixes:
 
 
 - Fix deprecation warnings (#142)
```

### Comparing `plone.app.robotframework-2.0.1/PKG-INFO` & `plone.app.robotframework-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.robotframework
-Version: 2.0.1
+Version: 2.1.0
 Summary: Robot Framework testing resources for Plone
 Home-page: https://github.com/plone/plone.app.robotframework/
 Author: Asko Soukka
 Author-email: asko.soukka@iki.fi
 License: GPL
 Keywords: robot automatic browser testing Plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -77,14 +77,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.1.0 (2023-07-14)
+------------------
+
+New features:
+
+
+- Add support for `playwright`-based tests via `robotframework-browser`.
+  [datakurre] (#3813)
+
+
+Bug fixes:
+
+
+- Remove unused and empty keyword that was displaying an error.
+  [gforcada] (#147)
+
+
 2.0.1 (2023-02-22)
 ------------------
 
 Bug fixes:
 
 
 - Fix deprecation warnings (#142)
```

### Comparing `plone.app.robotframework-2.0.1/README.rst` & `plone.app.robotframework-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/LICENSE.GPL` & `plone.app.robotframework-2.1.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/LICENSE.txt` & `plone.app.robotframework-2.1.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/libdoc.sh` & `plone.app.robotframework-2.1.0/docs/libdoc.sh`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/bdd.txt` & `plone.app.robotframework-2.1.0/docs/source/bdd.txt`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/conf.py` & `plone.app.robotframework-2.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/debugging.rst` & `plone.app.robotframework-2.1.0/docs/source/debugging.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/examples.rst` & `plone.app.robotframework-2.1.0/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/happy.rst` & `plone.app.robotframework-2.1.0/docs/source/happy.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/index.rst` & `plone.app.robotframework-2.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/keywords.rst` & `plone.app.robotframework-2.1.0/docs/source/keywords.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/libdoc/python_debugging.html` & `plone.app.robotframework-2.1.0/docs/source/libdoc/python_debugging.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/libdoc/python_layoutmath.html` & `plone.app.robotframework-2.1.0/docs/source/libdoc/python_layoutmath.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/libdoc/python_saucelabs.html` & `plone.app.robotframework-2.1.0/docs/source/libdoc/python_saucelabs.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/libdoc/python_zope2server.html` & `plone.app.robotframework-2.1.0/docs/source/libdoc/python_zope2server.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/libdoc/remote_autologin.html` & `plone.app.robotframework-2.1.0/docs/source/libdoc/remote_autologin.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/libdoc/remote_content.html` & `plone.app.robotframework-2.1.0/docs/source/libdoc/remote_content.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/libdoc/remote_genericsetup.html` & `plone.app.robotframework-2.1.0/docs/source/libdoc/remote_genericsetup.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/libdoc/remote_i18n.html` & `plone.app.robotframework-2.1.0/docs/source/libdoc/remote_i18n.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/libdoc/remote_mockmailhost.html` & `plone.app.robotframework-2.1.0/docs/source/libdoc/remote_mockmailhost.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/libdoc/remote_quickinstaller.html` & `plone.app.robotframework-2.1.0/docs/source/libdoc/remote_quickinstaller.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/libdoc/remote_users.html` & `plone.app.robotframework-2.1.0/docs/source/libdoc/remote_users.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/libdoc/remote_zope2server.html` & `plone.app.robotframework-2.1.0/docs/source/libdoc/remote_zope2server.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/libdoc/selenium.html` & `plone.app.robotframework-2.1.0/docs/source/libdoc/selenium.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/libdoc/user_keywords.html` & `plone.app.robotframework-2.1.0/docs/source/libdoc/user_keywords.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/libdoc/user_saucelabs.html` & `plone.app.robotframework-2.1.0/docs/source/libdoc/user_saucelabs.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/libdoc/user_selenium.html` & `plone.app.robotframework-2.1.0/docs/source/libdoc/user_selenium.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/libdoc/user_server.html` & `plone.app.robotframework-2.1.0/docs/source/libdoc/user_server.html`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/plone-keywords/browser.rst` & `plone.app.robotframework-2.1.0/docs/source/plone-keywords/browser.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/plone-keywords/content.rst` & `plone.app.robotframework-2.1.0/docs/source/plone-keywords/content.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/plone-keywords/index.rst` & `plone.app.robotframework-2.1.0/docs/source/plone-keywords/index.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/reload.rst` & `plone.app.robotframework-2.1.0/docs/source/reload.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/remote.rst` & `plone.app.robotframework-2.1.0/docs/source/remote.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/ride.rst` & `plone.app.robotframework-2.1.0/docs/source/ride.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/robot.rst` & `plone.app.robotframework-2.1.0/docs/source/robot.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/saucelabs.rst` & `plone.app.robotframework-2.1.0/docs/source/saucelabs.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/server.rst` & `plone.app.robotframework-2.1.0/docs/source/server.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/templer.rst` & `plone.app.robotframework-2.1.0/docs/source/templer.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/travis-ci.rst` & `plone.app.robotframework-2.1.0/docs/source/travis-ci.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/docs/source/tutorial.rst` & `plone.app.robotframework-2.1.0/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/setup.py` & `plone.app.robotframework-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "2.0.1"
+version = "2.1.0"
 
 
 def indented(filename):
     return "".join([indent(line) for line in open(filename)])
 
 
 def indent(line):
@@ -58,14 +58,15 @@
     "plone.app.testing",
     "plone.base",
     "plone.testing",
     "plone.uuid",
     "robotframework",
     "robotframework-selenium2library",
     "robotframework-seleniumtestability",
+    "robotframework-browser",
     "robotsuite",  # not a direct dependency, but required for convenience
     "selenium",
     "setuptools",
     "zope.component",
     "zope.configuration",
     "zope.i18n",
     "zope.schema",
```

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/__init__.py` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/annotate.robot` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/annotate.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/autologin.py` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/autologin.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/content/file.pdf` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/content/file.pdf`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/content/image.jpg` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/content/image.jpg`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/content.py` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/content.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/i18n.py` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/i18n.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/keywords.py` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/keywords.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/keywords.robot` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/keywords.robot`

 * *Files 3% similar despite different names*

```diff
@@ -77,24 +77,14 @@
     Log in  ${TEST_USER_NAME}  ${TEST_USER_PASSWORD}
 
 Log in as site owner
     [Documentation]  Log in as the SITE_OWNER provided by plone.app.testing,
     ...              with all the rights and privileges of that user.
     Log in  ${SITE_OWNER_NAME}  ${SITE_OWNER_PASSWORD}
 
-Log in as test user with role
-    [Arguments]  ${usrid}  ${role}
-
-    # We need a generic way to login with a user that has one or more roles.
-
-    # Do we need to be able to assign multiple roles at once?
-
-    # Do we need to assign roles to arbitray users or is it sufficient if we
-    # always assign those roles to the test user?
-
 Log out
     Go to  ${PLONE_URL}/logout
     Page Should Contain Element  css=#login-form
 
 
 # ----------------------------------------------------------------------------
 # Overlays
```

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/patches.py` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/patches.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/pybabel.py` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/pybabel.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/quickinstaller.py` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/quickinstaller.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/reload.py` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/reload.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/remote.py` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/remote.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/robotentrypoints.py` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/robotentrypoints.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/saucelabs.py` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/saucelabs.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/saucelabs.robot` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/saucelabs.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/selenium.robot` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/selenium.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/server.py` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/server.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/server.robot` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/server.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/speak.robot` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/speak.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/testing.py` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/docs/test_keywords.robot` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/docs/test_keywords.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/test_autologin_library.robot` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/test_autologin_library.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/test_content.py` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/test_content.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/test_content_library.robot` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/test_content_library.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/test_robot.py` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/test_robot.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 
 
 def test_suite():
     suite = unittest.TestSuite()
     suite.addTests(
         [
             layered(
+                robotsuite.RobotTestSuite("test_browser_library.robot"),
+                layer=SIMPLE_PUBLICATION_ROBOT_TESTING,
+            ),
+            layered(
                 robotsuite.RobotTestSuite("test_autologin_library.robot"),
                 layer=SIMPLE_PUBLICATION_ROBOT_TESTING,
             ),
             layered(
                 robotsuite.RobotTestSuite("test_content_library.robot"),
                 layer=SIMPLE_PUBLICATION_ROBOT_TESTING,
             ),
```

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/test_robotfixture.py` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/test_robotfixture.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/test_speakjs_library.robot` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/test_speakjs_library.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/tests/test_users_library.robot` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/tests/test_users_library.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/user.robot` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/user.robot`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone/app/robotframework/users.py` & `plone.app.robotframework-2.1.0/src/plone/app/robotframework/users.py`

 * *Files identical despite different names*

### Comparing `plone.app.robotframework-2.0.1/src/plone.app.robotframework.egg-info/PKG-INFO` & `plone.app.robotframework-2.1.0/src/plone.app.robotframework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.robotframework
-Version: 2.0.1
+Version: 2.1.0
 Summary: Robot Framework testing resources for Plone
 Home-page: https://github.com/plone/plone.app.robotframework/
 Author: Asko Soukka
 Author-email: asko.soukka@iki.fi
 License: GPL
 Keywords: robot automatic browser testing Plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -77,14 +77,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.1.0 (2023-07-14)
+------------------
+
+New features:
+
+
+- Add support for `playwright`-based tests via `robotframework-browser`.
+  [datakurre] (#3813)
+
+
+Bug fixes:
+
+
+- Remove unused and empty keyword that was displaying an error.
+  [gforcada] (#147)
+
+
 2.0.1 (2023-02-22)
 ------------------
 
 Bug fixes:
 
 
 - Fix deprecation warnings (#142)
```

### Comparing `plone.app.robotframework-2.0.1/src/plone.app.robotframework.egg-info/SOURCES.txt` & `plone.app.robotframework-2.1.0/src/plone.app.robotframework.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 src/plone.app.robotframework.egg-info/top_level.txt
 src/plone/app/__init__.py
 src/plone/app/robotframework/__init__.py
 src/plone/app/robotframework/_variables.robot
 src/plone/app/robotframework/annotate.py
 src/plone/app/robotframework/annotate.robot
 src/plone/app/robotframework/autologin.py
+src/plone/app/robotframework/browser.robot
 src/plone/app/robotframework/config.py
 src/plone/app/robotframework/content.py
 src/plone/app/robotframework/genericsetup.py
 src/plone/app/robotframework/i18n.py
 src/plone/app/robotframework/keywords.py
 src/plone/app/robotframework/keywords.robot
 src/plone/app/robotframework/keywords.txt
@@ -96,14 +97,15 @@
 src/plone/app/robotframework/content/file.pdf
 src/plone/app/robotframework/content/image.jpg
 src/plone/app/robotframework/selectors/cmfplone43.robot
 src/plone/app/robotframework/selectors/cmfplone50.robot
 src/plone/app/robotframework/selectors/cmfplone60.robot
 src/plone/app/robotframework/tests/__init__.py
 src/plone/app/robotframework/tests/test_autologin_library.robot
+src/plone/app/robotframework/tests/test_browser_library.robot
 src/plone/app/robotframework/tests/test_content.py
 src/plone/app/robotframework/tests/test_content_library.robot
 src/plone/app/robotframework/tests/test_i18n_library.robot
 src/plone/app/robotframework/tests/test_quickinstaller_library.robot
 src/plone/app/robotframework/tests/test_robot.py
 src/plone/app/robotframework/tests/test_robotfixture.py
 src/plone/app/robotframework/tests/test_robotfixture.robot
```

### Comparing `plone.app.robotframework-2.0.1/src/plone.app.robotframework.egg-info/requires.txt` & `plone.app.robotframework-2.1.0/src/plone.app.robotframework.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 plone.app.testing
 plone.base
 plone.testing
 plone.uuid
 robotframework
 robotframework-selenium2library
 robotframework-seleniumtestability
+robotframework-browser
 robotsuite
 selenium
 setuptools
 zope.component
 zope.configuration
 zope.i18n
 zope.schema
```

