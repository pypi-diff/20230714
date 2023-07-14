# Comparing `tmp/grokcore.startup-3.0.1.tar.gz` & `tmp/grokcore.startup-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grokcore.startup-3.0.1.tar", last modified: Fri Jan 12 13:28:17 2018, max compression
+gzip compressed data, was "grokcore.startup-4.0.tar", last modified: Fri Jul 14 06:14:17 2023, max compression
```

## Comparing `grokcore.startup-3.0.1.tar` & `grokcore.startup-4.0.tar`

### file list

```diff
@@ -1,34 +1,32 @@
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:28:17.000000 grokcore.startup-3.0.1/
--rw-r--r--   0 jw         (501) staff       (20)      357 2018-01-12 13:28:16.000000 grokcore.startup-3.0.1/.travis.yml
--rw-r--r--   0 jw         (501) staff       (20)     6158 2018-01-12 13:28:16.000000 grokcore.startup-3.0.1/bootstrap.py
--rw-r--r--   0 jw         (501) staff       (20)      373 2018-01-12 13:28:16.000000 grokcore.startup-3.0.1/buildout.cfg
--rw-r--r--   0 jw         (501) staff       (20)     2614 2018-01-12 13:28:16.000000 grokcore.startup-3.0.1/CHANGES.txt
--rw-r--r--   0 jw         (501) staff       (20)       32 2018-01-12 13:28:16.000000 grokcore.startup-3.0.1/COPYRIGHT.txt
--rw-r--r--   0 jw         (501) staff       (20)      145 2018-01-12 13:28:16.000000 grokcore.startup-3.0.1/CREDITS.txt
--rw-r--r--   0 jw         (501) staff       (20)     2070 2018-01-12 13:28:16.000000 grokcore.startup-3.0.1/LICENSE.txt
--rw-r--r--   0 jw         (501) staff       (20)      143 2018-01-12 13:28:16.000000 grokcore.startup-3.0.1/MANIFEST.in
--rw-r--r--   0 jw         (501) staff       (20)    20664 2018-01-12 13:28:17.000000 grokcore.startup-3.0.1/PKG-INFO
--rw-r--r--   0 jw         (501) staff       (20)      515 2018-01-12 13:28:16.000000 grokcore.startup-3.0.1/README.txt
--rw-r--r--   0 jw         (501) staff       (20)      124 2018-01-12 13:28:16.000000 grokcore.startup-3.0.1/requirements.txt
--rw-r--r--   0 jw         (501) staff       (20)       38 2018-01-12 13:28:17.000000 grokcore.startup-3.0.1/setup.cfg
--rw-r--r--   0 jw         (501) staff       (20)     2281 2018-01-12 13:28:16.000000 grokcore.startup-3.0.1/setup.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:28:17.000000 grokcore.startup-3.0.1/src/
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:28:17.000000 grokcore.startup-3.0.1/src/grokcore/
--rw-r--r--   0 jw         (501) staff       (20)      200 2018-01-12 13:28:16.000000 grokcore.startup-3.0.1/src/grokcore/__init__.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:28:17.000000 grokcore.startup-3.0.1/src/grokcore/startup/
--rw-r--r--   0 jw         (501) staff       (20)      795 2018-01-12 13:28:16.000000 grokcore.startup-3.0.1/src/grokcore/startup/__init__.py
--rw-r--r--   0 jw         (501) staff       (20)     5861 2018-01-12 13:28:16.000000 grokcore.startup-3.0.1/src/grokcore/startup/debug.py
--rw-r--r--   0 jw         (501) staff       (20)    12454 2018-01-12 13:28:16.000000 grokcore.startup-3.0.1/src/grokcore/startup/README.txt
--rw-r--r--   0 jw         (501) staff       (20)     2821 2018-01-12 13:28:16.000000 grokcore.startup-3.0.1/src/grokcore/startup/startup.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:28:17.000000 grokcore.startup-3.0.1/src/grokcore/startup/tests/
--rw-r--r--   0 jw         (501) staff       (20)       23 2018-01-12 13:28:16.000000 grokcore.startup-3.0.1/src/grokcore/startup/tests/__init__.py
--rw-r--r--   0 jw         (501) staff       (20)      923 2018-01-12 13:28:16.000000 grokcore.startup-3.0.1/src/grokcore/startup/tests/test_grokcorestartup.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 13:28:17.000000 grokcore.startup-3.0.1/src/grokcore.startup.egg-info/
--rw-r--r--   0 jw         (501) staff       (20)        1 2018-01-12 13:28:17.000000 grokcore.startup-3.0.1/src/grokcore.startup.egg-info/dependency_links.txt
--rw-r--r--   0 jw         (501) staff       (20)      116 2018-01-12 13:28:17.000000 grokcore.startup-3.0.1/src/grokcore.startup.egg-info/entry_points.txt
--rw-r--r--   0 jw         (501) staff       (20)        9 2018-01-12 13:28:17.000000 grokcore.startup-3.0.1/src/grokcore.startup.egg-info/namespace_packages.txt
--rw-r--r--   0 jw         (501) staff       (20)        1 2018-01-12 13:28:17.000000 grokcore.startup-3.0.1/src/grokcore.startup.egg-info/not-zip-safe
--rw-r--r--   0 jw         (501) staff       (20)    20664 2018-01-12 13:28:17.000000 grokcore.startup-3.0.1/src/grokcore.startup.egg-info/PKG-INFO
--rw-r--r--   0 jw         (501) staff       (20)      206 2018-01-12 13:28:17.000000 grokcore.startup-3.0.1/src/grokcore.startup.egg-info/requires.txt
--rw-r--r--   0 jw         (501) staff       (20)      740 2018-01-12 13:28:17.000000 grokcore.startup-3.0.1/src/grokcore.startup.egg-info/SOURCES.txt
--rw-r--r--   0 jw         (501) staff       (20)        9 2018-01-12 13:28:17.000000 grokcore.startup-3.0.1/src/grokcore.startup.egg-info/top_level.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-14 06:14:17.187892 grokcore.startup-4.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2806 2023-07-14 06:14:16.000000 grokcore.startup-4.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-14 06:14:16.000000 grokcore.startup-4.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-14 06:14:16.000000 grokcore.startup-4.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      145 2023-07-14 06:14:16.000000 grokcore.startup-4.0/CREDITS.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-14 06:14:16.000000 grokcore.startup-4.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      224 2023-07-14 06:14:16.000000 grokcore.startup-4.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)    16878 2023-07-14 06:14:17.187973 grokcore.startup-4.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      515 2023-07-14 06:14:16.000000 grokcore.startup-4.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      478 2023-07-14 06:14:17.188246 grokcore.startup-4.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2270 2023-07-14 06:14:16.000000 grokcore.startup-4.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-14 06:14:17.183980 grokcore.startup-4.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-14 06:14:17.185682 grokcore.startup-4.0/src/grokcore/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       56 2023-07-14 06:14:16.000000 grokcore.startup-4.0/src/grokcore/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-14 06:14:17.187472 grokcore.startup-4.0/src/grokcore/startup/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    12454 2023-07-14 06:14:16.000000 grokcore.startup-4.0/src/grokcore/startup/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      823 2023-07-14 06:14:16.000000 grokcore.startup-4.0/src/grokcore/startup/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5906 2023-07-14 06:14:16.000000 grokcore.startup-4.0/src/grokcore/startup/debug.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2912 2023-07-14 06:14:16.000000 grokcore.startup-4.0/src/grokcore/startup/startup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-14 06:14:17.187756 grokcore.startup-4.0/src/grokcore/startup/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       23 2023-07-14 06:14:16.000000 grokcore.startup-4.0/src/grokcore/startup/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      421 2023-07-14 06:14:16.000000 grokcore.startup-4.0/src/grokcore/startup/tests/test_grokcorestartup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-14 06:14:17.186882 grokcore.startup-4.0/src/grokcore.startup.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    16878 2023-07-14 06:14:17.000000 grokcore.startup-4.0/src/grokcore.startup.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      719 2023-07-14 06:14:17.000000 grokcore.startup-4.0/src/grokcore.startup.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-14 06:14:17.000000 grokcore.startup-4.0/src/grokcore.startup.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      115 2023-07-14 06:14:17.000000 grokcore.startup-4.0/src/grokcore.startup.egg-info/entry_points.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        9 2023-07-14 06:14:17.000000 grokcore.startup-4.0/src/grokcore.startup.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-14 06:14:17.000000 grokcore.startup-4.0/src/grokcore.startup.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      222 2023-07-14 06:14:17.000000 grokcore.startup-4.0/src/grokcore.startup.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        9 2023-07-14 06:14:17.000000 grokcore.startup-4.0/src/grokcore.startup.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1434 2023-07-14 06:14:16.000000 grokcore.startup-4.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `grokcore.startup-3.0.1/CHANGES.txt` & `grokcore.startup-4.0/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 Changes
 *******
 
+4.0 (2023-07-14)
+================
+
+- Add support for Python 3.10, 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.7, 3.8 and 3.9.
+
+- Drop support for Python 3.4.
+
+
 3.0.1 (2018-01-12)
 ==================
 
 - Rearrange tests such that Travis CI can pick up all functional tests too.
 
 3.0.0 (2018-01-10)
 ==================
```

### Comparing `grokcore.startup-3.0.1/LICENSE.txt` & `grokcore.startup-4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grokcore.startup-3.0.1/PKG-INFO` & `grokcore.startup-4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,528 +1,542 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: grokcore.startup
-Version: 3.0.1
+Version: 4.0
 Summary: Paster support for Grok projects.
-Home-page: http://grok.zope.org
+Home-page: https://github.com/zopefoundation/grokcore.startup
 Author: Grok Team
-Author-email: grok-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL
-Download-URL: http://pypi.python.org/pypi/grokcore.startup
-Description: grokcore.startup
-        ****************
-        
-        This package provides elements for starting a `Grok`_ project with
-        `paster`_ and `WSGI`_.
-        
-        .. contents::
-        
-        Setting up ``grokcore.startup``
-        ===============================
-        
-        There is nothing special to setup this package.
-        
-        All you have to do is, to make this package available during runtime.
-        
-        With `zc.buildout`_ or other `setuptools`_-related setups this can be
-        done by simply adding the package name ``grokcore.startup`` to the
-        required packages of your project in ``setup.py``.
-        
-        
-        Detailed Description
-        ********************
-        
-        Setting up Grok projects as ``paster`` served WSGI applications
-        ===============================================================
-        
-        The main target of this package is to provide support for enabling
-        `Grok`_ applications to be run as `paster`_ served `WSGI`_
-        applications. To make this working some configuration files have to be
-        set up.
-        
-        Setting up a project with ``grokproject``
-        -----------------------------------------
-        
-        The most convenient way to setup a `Grok`_ project is using
-        `grokproject`_. Once installed, you can a project like this::
-        
-          $ grokproject Sample
-        
-        which will generate all configuration files for you.
-        
-        .. note:: Older versions of `grokproject`_ need an update
-        
-          As older versions of `grokproject`_ do not support
-          `grokcore.startup`, you might want to update your existing
-          `grokproject`_ installation by running::
-        
-            $ easy_install -U grokproject
-        
-        
-        Setting up a project manually
-        -----------------------------
-        
-        Before we can make use of ``grokcore.startup``, we have to setup
-        several configuration files in the project root:
-        
-        * ``setup.py``
-        
-        * ``buildout.cfg`` (optional)
-        
-        * ``zope.conf`` (normally found in the ``parts/etc/`` subdirectory of your
-          `Grok`_ project)
-        
-        * ``site.zcml`` (normally found in the ``parts/etc/`` subdirectory of your
-          `Grok`_ project)
-        
-        * ``deploy.ini`` (or any other .ini-file; normally found in the
-          ``parts/etc/`` subdirectory of your `Grok`_ project)
-        
-        
-        When we want to setup a Zope instance as `paster`_ served `WSGI`_
-        application, then we have to set a ``paste.app_factory`` entry point
-        in ``setup.py``. A minimal setup could look like this::
-        
-          # setup.py
-          from setuptools import setup, find_packages
-        
-          setup(name='sampleproject',
-                version='0.1dev',
-                description="A sample project",
-                long_description="""Without a long description.""",
-                classifiers=[],
-                keywords="",
-                author="U.N.Owen",
-                author_email="",
-                url="",
-                license="",
-                package_dir={'': 'src'},
-                packages=find_packages('src'),
-                include_package_data=True,
-                zip_safe=False,
-                install_requires=['setuptools',],
-                entry_points = """
-                [paste.app_factory]
-                main = grokcore.startup:application_factory
-                """,
-                )
-        
-        Here the `paste.app_factory` entry point pointing to
-        `grokcore.startup:application_factory` is important.
-        
-        Furthermore we need at least a minimal ``buildout.cfg`` which enables
-        `zc.buildout`_ to create the control scripts for our instance::
-        
-          [buildout]
-          develop = .
-          parts = app
-        
-          [app]
-          recipe = zc.recipe.egg
-          eggs = sampleproject
-                 grokcore.startup
-                 Paste
-                 PasteScript
-                 PasteDeploy
-        
-        Here an egg-entry for ``grokcore.startup`` **might** be important, if
-        it is not required otherwise by your application. Projects generated
-        by `grokproject`_ will automatically include such a dependency and
-        upcoming versions of `Grok`_ will pull in ``grokcore.startup`` anyway,
-        so that ``grokcore.startup`` would not be required in this list of
-        eggs any more.
-        
-        Next we need ``site.zcml`` and ``zope.conf`` files to define the
-        Zope instance. These configurations are completely independent from
-        being served by `Paste`_ or not. If you are upgrading an old `Grok`_
-        project, you can use ``site.zcml`` and ``zope.conf`` of those project
-        as-is. You only have to take care of the maybe changed
-        ``site-definition`` entry in ``zope.conf`` (see below).
-        
-        The file ``site.zcml`` can be quite
-        short, but for real projects you certainly want to have some useful
-        content in here::
-        
-          <configure />
-        
-        A short ``zope.conf`` file for use in tests could look like this::
-        
-          site-definition site.zcml
-        
-          <zodb>
-            <mappingstorage />
-          </zodb>
-        
-          <eventlog>
-            <logfile>
-              path STDOUT
-             </logfile>
-          </eventlog>
-        
-        where the ``site-definition`` entry should point to the location of
-        the file ``site.zcml``. In regular Grok projects those files are put
-        into the ``etc/`` subdirectory of your project root.
-        
-        Finally we have to provide a ``deploy.ini`` (or another .ini-file),
-        which tells paster where to find the pieces. This is also put into the
-        ``etc/`` subdirectory of your project root in regular Grok projects
-        created by `grokproject`_::
-        
-          [app:main]
-          use = egg:sampleproject
-        
-          [server:main]
-          use = egg:Paste#http
-          host = 127.0.0.1
-          port = 8080
-        
-          [DEFAULT]
-          zope_conf = %(here)s/zope.conf
-        
-        
-        
-        API Documentation
-        =================
-        
-        ``application_factory(global_conf, **local_conf)``
-        --------------------------------------------------
-        
-          ``grokcore.startup`` provides a function ``application_factory``
-          which delivers a `WSGIPublisherApplication`_ instance when called
-          with an appropriate configuration. See the `zope.app.wsgi
-          documentation
-          <http://apidoc.zope.org/++apidoc++/Code/zope/app/wsgi/README.txt/index.html>`_
-          to learn more about Zope objects supporting `WSGI`_.
-        
-          A call to this function is normally required as entry point in
-          `setuptools`_-driven `paster`_ environments  (see
-          http://pythonpaste.org/deploy/#paste-app-factory).
-        
-          We have to create our own site definition file -- which will simply
-          be empty -- to provide a minimal test::
-        
-            >>> import os, tempfile
-            >>> temp_dir = tempfile.mkdtemp()
-            >>> sitezcml = os.path.join(temp_dir, 'site.zcml')
-            >>> out = open(sitezcml, 'w')
-            >>> _ = out.write('<configure />')
-            >>> out.close()
-        
-          Furthermore we create a Zope configuration file, which is also quite
-          plain::
-        
-            >>> zope_conf = os.path.join(temp_dir, 'zope.conf')
-            >>> out = open(zope_conf, 'w')
-            >>> _ = out.write('''
-            ... site-definition %s
-            ...
-            ... <zodb>
-            ...   <mappingstorage />
-            ... </zodb>
-            ...
-            ... <eventlog>
-            ...   <logfile>
-            ...     path STDOUT
-            ...   </logfile>
-            ... </eventlog>
-            ... ''' % sitezcml)
-            >>> out.close()
-        
-          Now we can call ``application_factory`` to get a WSGI application::
-        
-            >>> from grokcore.startup import application_factory
-            >>> app_factory = application_factory({'zope_conf': zope_conf})
-            >>> app_factory
-            <zope.app.wsgi.WSGIPublisherApplication object at 0x...>
-        
-        ``debug_application_factory(global_conf, **local_conf)``
-        --------------------------------------------------------
-        
-          There's a second application factory that can be used when debugging
-          the application, especially when using the ``z3c.evalexception`` middleware.
-        
-          When debugging zope is instructed not to handle any raised exceptions
-          itself. The ``z3c.evalexception`` middleware then catches the exceptions
-          and provides an user interfaces for debugging in the webbrowser.
-        
-          As a result also the IUnauthorized execption would not be handled by zope
-          and the authentication mechanisms of zope are not triggered. As a result,
-          when debugging one cannot login.
-        
-          The ``debug_application_factory`` function accepts the "exempt-exceptions"
-          configuration option. The value for this option should be a comma seperated
-          list of dotted names for each of the execptions that should *still* be
-          handled by zope and not re-raised to be catched by the middleware.
-        
-            >>> from grokcore.startup import debug_application_factory
-            >>> app_factory = debug_application_factory({'zope_conf': zope_conf})
-            >>> app_factory
-            <zope.app.wsgi.WSGIPublisherApplication object at 0x...>
-        
-            >>> from zope.interface import implementer
-            >>> from zope.security.interfaces import IUnauthorized
-            >>> @implementer(IUnauthorized)
-            ... class UnauthorizedException(object):
-            ...     pass
-            >>>
-            >>> from zope.component import queryAdapter
-            >>> from zope.publisher.interfaces import IReRaiseException
-        
-          Since the ``exempt-execptions`` configuration option was not passed,
-          there's no IReRaiseException adapter registered for any type of exceptions
-          including IUnauthorized:
-        
-            >>> error = UnauthorizedException()
-            >>> reraise = queryAdapter(error, IReRaiseException, default=None)
-            >>> reraise is None
-            True
-        
-          When the option is passed, the adapter will be registered. Calling this
-          adapter yields ``False``, telling zope not to reraise this particular
-          exception.
-        
-            >>> app_factory = debug_application_factory(
-            ...     {'zope_conf': zope_conf},
-            ...     **{'exempt-exceptions': 'zope.security.interfaces.IUnauthorized'})
-            >>>
-            >>> reraise = queryAdapter(error, IReRaiseException, default=None)
-            >>> reraise is None
-            False
-            >>> reraise()
-            False
-        
-          Clean up the temp_dir
-        
-            >>> import shutil
-            >>> shutil.rmtree(temp_dir)
-        
-        ``interactive_debug_prompt(zope_conf_path)``
-        --------------------------------------------
-        
-          Get an interactive console with a debugging shell started.
-        
-          `grokcore.startup` provides two different debuggers currently: a
-          plain one based on `zope.app.debug` and a more powerful `IPython`_
-          debugger. The IPython debugger is automatically enabled if you have
-          IPython available in the environment.
-        
-          You can explicitly enable the IPython_ debugger by stating::
-        
-            grokcore.startup [debug]
-        
-          in the install requirements of your `setup.py`, probably adding only
-          ``[debug]`` to an already existing entry for
-          `grokcore.startup`. Don't forget to rerun `buildout` afterwards.
-        
-          You can explicitly require one or the other debugger by calling::
-        
-            grokcore.startup.startup.interactive_debug_prompt(zope_conf)
-        
-          or::
-        
-            grokcore.startup.debug.ipython_debug_prompt(zope_conf)
-        
-          in the ``[interactive_debugger]`` section of your ``buildout.cfg``.
-        
-            >>> import zope.app.appsetup.appsetup
-            >>> zope.app.appsetup.appsetup._configured = False
-        
-            >>> temp_dir = tempfile.mkdtemp()
-        
-            >>> sitezcml = os.path.join(temp_dir, 'site.zcml')
-            >>> out = open(sitezcml, 'w')
-            >>> _ = out.write(
-            ...    """<configure xmlns="http://namespaces.zope.org/zope">
-            ...   <include package="zope.component" file="meta.zcml"/>
-            ...   <include package="zope.component"/>
-            ...   <include package="zope.traversing"/>
-            ...   <include package="zope.security" file="meta.zcml"/>
-            ...   <include package="zope.security"/>
-            ...   <include package="zope.container"/>
-            ...   <include package="zope.site"/>
-            ...   <include package="zope.app.appsetup"/>
-            ... </configure>""")
-            >>> out.close()
-            >>>
-            >>> zopeconf = os.path.join(temp_dir, 'zope.conf')
-            >>> out = open(zopeconf, 'w')
-            >>> _ = out.write("""
-            ...     site-definition %s
-            ...     <zodb>
-            ...       <filestorage>
-            ...         path %s
-            ...       </filestorage>
-            ...     </zodb>
-            ...     <eventlog>
-            ...       <logfile>
-            ...         path STDOUT
-            ...         formatter zope.exceptions.log.Formatter
-            ...       </logfile>
-            ...     </eventlog>
-            ...     """ % (sitezcml, os.path.join(temp_dir, 'Data.fs')))
-            >>> out.close()
-            >>>
-            >>> import sys
-            >>> old_argv = sys.argv[:]
-            >>>
-            >>> script = os.path.join(temp_dir, 'script.py')
-            >>> out = open(script, 'w')
-            >>> _ = out.write(
-            ...    """import sys
-            ... from pprint import pprint
-            ... pprint(debugger)
-            ... pprint(app)
-            ... pprint(root)
-            ... pprint(sys.argv)
-            ... pprint(__file__)
-            ... pprint(__name__)""")
-            >>>
-            >>> out.close()
-            >>>
-            >>> sys.argv = ['interactive_debugger', script]
-            >>> from grokcore.startup import interactive_debug_prompt
-            >>> try:
-            ...     interactive_debug_prompt(zopeconf)
-            ... except SystemExit:
-            ...     # Catch the exit from the interactive prompt as it would
-            ...     # exit this test as well.
-            ...     pass
-            ------
-            ...WARNING zope.app.appsetup Security policy is not configured.
-            Please make sure that securitypolicy.zcml is included in site.zcml
-            immediately before principals.zcml
-            ...
-            <zope.app.debug.debug.Debugger object at ...>
-            <zope.app.debug.debug.Debugger object at ...>
-            <zope.site.folder.Folder object at ...>
-            ['...script.py']
-            '...script.py'
-            '__main__'
-        
-          Clean up the temp_dir
-        
-            >>> sys.argv = old_argv
-            >>> import shutil
-            >>> shutil.rmtree(temp_dir)
-        
-        .. _grok: http://pypi.python.org/pypi/grok
-        .. _grokproject: http://pypi.python.org/pypi/grokproject
-        .. _Paste: http://pythonpaste.org/
-        .. _paster: Paste_
-        .. _setuptools: http://pypi.python.org/pypi/setuptools
-        .. _WSGI: http://www.wsgi.org/wsgi/
-        .. _WSGIPublisherApplication: http://apidoc.zope.org/++apidoc++/Code/zope/app/wsgi/WSGIPublisherApplication/index.html
-        .. _zc.buildout: http://pypi.python.org/pypi/zc.buildout
-        .. _ipython: http://ipython.org/
-        
-        Changes
-        *******
-        
-        3.0.1 (2018-01-12)
-        ==================
-        
-        - Rearrange tests such that Travis CI can pick up all functional tests too.
-        
-        3.0.0 (2018-01-10)
-        ==================
-        
-        - Python 3 compatibility.
-        
-        1.2.1 (2016-02-15)
-        ==================
-        
-        - Update tests.
-        
-        1.2 (2012-05-02)
-        ================
-        
-        - Added new IPython-based interactive debugger which is used
-          automatically when IPython is available. Otherwise the gdb-style
-          debugger is provided.
-        
-        1.1 (2010-10-26)
-        ================
-        
-        - Drop zdaemon support.
-        
-        - Close the database explicitely when execing a script through the
-          ``interactive_debug_prompt``. This came to light in tests on Windows, as the
-          tests would try to delete the temp directory it created with the still
-          unclosed database file in there.
-        
-        1.0.2 (2010-10-05)
-        ==================
-        
-        - Somehow the intended fix in 1.0.1 did not actually get included in that
-          release. We make the fix again.
-        
-        1.0.1 (2010-08-18)
-        ==================
-        
-        - When passing a script to the interactive_debug_prompt command, one would
-          expect to be able to do: `if __name__ == '__main__':`, however __name__ would
-          be "__builtin__". This is fixed.
-        
-        1.0 (2010-05-20)
-        ================
-        
-        - Amend the interactive_debug_prompt function to behave more or less like the
-          "old" zopectl command. Whenever there's commandline arguments passed to the
-          command, the first one is assumed to be a python script that is 'execfile'd.
-          This allows ad hoc scripts to run against the setup application.
-        
-        - Make package comply to zope.org repository policy.
-        
-        - The upgrade notes will be moved to the Grok upgrade notes.
-        
-        - Define entry points for main and debug application factories in
-          grokcore.startup.
-        
-        - Use the groktoolkit.
-        
-        0.4 (2009-10-06)
-        ================
-        
-        - Fix documentation bugs.
-        
-        0.3 (2009-10-02)
-        ================
-        
-        * Add a ``debug_application_factory`` function that allows for the
-          ``exempt-exceptions`` configuration option. The value for this option
-          should be a comma seperated list of dotted names for each of the exceptions
-          that should not be re-raised during debugging.
-        
-          This for one allow the IUnauthorized exception to still be handled by zope
-          and thus have the normal authentication mechanisms still work.
-        
-        * Bring versions.cfg in line with current grok versions.cfg.
-        
-        0.2 (2009-02-21)
-        ================
-        
-        * Made main functions available package wide.
-        
-        0.1 (2009-01-15)
-        ================
-        
-        * Added support for local ``zope_conf`` parameter.
-          Fix bug https://bugs.launchpad.net/grok/+bug/320644
-        
-        * Created ``grokcore.startup`` in January 2009 by factoring paster
-          related application code out of grokcore templates.
-        
 Keywords: zope zope3 grok grokproject WSGI Paste paster
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
+Classifier: Framework :: Zope :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Framework :: Zope3
+Requires-Python: >=3.7
+Provides-Extra: test
+Provides-Extra: debug
+License-File: LICENSE.txt
+
+grokcore.startup
+****************
+
+This package provides elements for starting a `Grok`_ project with
+`paster`_ and `WSGI`_.
+
+.. contents::
+
+Setting up ``grokcore.startup``
+===============================
+
+There is nothing special to setup this package.
+
+All you have to do is, to make this package available during runtime.
+
+With `zc.buildout`_ or other `setuptools`_-related setups this can be
+done by simply adding the package name ``grokcore.startup`` to the
+required packages of your project in ``setup.py``.
+
+
+Detailed Description
+********************
+
+Setting up Grok projects as ``paster`` served WSGI applications
+===============================================================
+
+The main target of this package is to provide support for enabling
+`Grok`_ applications to be run as `paster`_ served `WSGI`_
+applications. To make this working some configuration files have to be
+set up.
+
+Setting up a project with ``grokproject``
+-----------------------------------------
+
+The most convenient way to setup a `Grok`_ project is using
+`grokproject`_. Once installed, you can a project like this::
+
+  $ grokproject Sample
+
+which will generate all configuration files for you.
+
+.. note:: Older versions of `grokproject`_ need an update
+
+  As older versions of `grokproject`_ do not support
+  `grokcore.startup`, you might want to update your existing
+  `grokproject`_ installation by running::
+
+    $ easy_install -U grokproject
+
+
+Setting up a project manually
+-----------------------------
+
+Before we can make use of ``grokcore.startup``, we have to setup
+several configuration files in the project root:
+
+* ``setup.py``
+
+* ``buildout.cfg`` (optional)
+
+* ``zope.conf`` (normally found in the ``parts/etc/`` subdirectory of your
+  `Grok`_ project)
+
+* ``site.zcml`` (normally found in the ``parts/etc/`` subdirectory of your
+  `Grok`_ project)
+
+* ``deploy.ini`` (or any other .ini-file; normally found in the
+  ``parts/etc/`` subdirectory of your `Grok`_ project)
+
+
+When we want to setup a Zope instance as `paster`_ served `WSGI`_
+application, then we have to set a ``paste.app_factory`` entry point
+in ``setup.py``. A minimal setup could look like this::
+
+  # setup.py
+  from setuptools import setup, find_packages
+
+  setup(name='sampleproject',
+        version='0.1dev',
+        description="A sample project",
+        long_description="""Without a long description.""",
+        classifiers=[],
+        keywords="",
+        author="U.N.Owen",
+        author_email="",
+        url="",
+        license="",
+        package_dir={'': 'src'},
+        packages=find_packages('src'),
+        include_package_data=True,
+        zip_safe=False,
+        install_requires=['setuptools',],
+        entry_points = """
+        [paste.app_factory]
+        main = grokcore.startup:application_factory
+        """,
+        )
+
+Here the `paste.app_factory` entry point pointing to
+`grokcore.startup:application_factory` is important.
+
+Furthermore we need at least a minimal ``buildout.cfg`` which enables
+`zc.buildout`_ to create the control scripts for our instance::
+
+  [buildout]
+  develop = .
+  parts = app
+
+  [app]
+  recipe = zc.recipe.egg
+  eggs = sampleproject
+         grokcore.startup
+         Paste
+         PasteScript
+         PasteDeploy
+
+Here an egg-entry for ``grokcore.startup`` **might** be important, if
+it is not required otherwise by your application. Projects generated
+by `grokproject`_ will automatically include such a dependency and
+upcoming versions of `Grok`_ will pull in ``grokcore.startup`` anyway,
+so that ``grokcore.startup`` would not be required in this list of
+eggs any more.
+
+Next we need ``site.zcml`` and ``zope.conf`` files to define the
+Zope instance. These configurations are completely independent from
+being served by `Paste`_ or not. If you are upgrading an old `Grok`_
+project, you can use ``site.zcml`` and ``zope.conf`` of those project
+as-is. You only have to take care of the maybe changed
+``site-definition`` entry in ``zope.conf`` (see below).
+
+The file ``site.zcml`` can be quite
+short, but for real projects you certainly want to have some useful
+content in here::
+
+  <configure />
+
+A short ``zope.conf`` file for use in tests could look like this::
+
+  site-definition site.zcml
+
+  <zodb>
+    <mappingstorage />
+  </zodb>
+
+  <eventlog>
+    <logfile>
+      path STDOUT
+     </logfile>
+  </eventlog>
+
+where the ``site-definition`` entry should point to the location of
+the file ``site.zcml``. In regular Grok projects those files are put
+into the ``etc/`` subdirectory of your project root.
+
+Finally we have to provide a ``deploy.ini`` (or another .ini-file),
+which tells paster where to find the pieces. This is also put into the
+``etc/`` subdirectory of your project root in regular Grok projects
+created by `grokproject`_::
+
+  [app:main]
+  use = egg:sampleproject
+
+  [server:main]
+  use = egg:Paste#http
+  host = 127.0.0.1
+  port = 8080
+
+  [DEFAULT]
+  zope_conf = %(here)s/zope.conf
+
+
+
+API Documentation
+=================
+
+``application_factory(global_conf, **local_conf)``
+--------------------------------------------------
+
+  ``grokcore.startup`` provides a function ``application_factory``
+  which delivers a `WSGIPublisherApplication`_ instance when called
+  with an appropriate configuration. See the `zope.app.wsgi
+  documentation
+  <http://apidoc.zope.org/++apidoc++/Code/zope/app/wsgi/README.txt/index.html>`_
+  to learn more about Zope objects supporting `WSGI`_.
+
+  A call to this function is normally required as entry point in
+  `setuptools`_-driven `paster`_ environments  (see
+  http://pythonpaste.org/deploy/#paste-app-factory).
+
+  We have to create our own site definition file -- which will simply
+  be empty -- to provide a minimal test::
+
+    >>> import os, tempfile
+    >>> temp_dir = tempfile.mkdtemp()
+    >>> sitezcml = os.path.join(temp_dir, 'site.zcml')
+    >>> out = open(sitezcml, 'w')
+    >>> _ = out.write('<configure />')
+    >>> out.close()
+
+  Furthermore we create a Zope configuration file, which is also quite
+  plain::
+
+    >>> zope_conf = os.path.join(temp_dir, 'zope.conf')
+    >>> out = open(zope_conf, 'w')
+    >>> _ = out.write('''
+    ... site-definition %s
+    ...
+    ... <zodb>
+    ...   <mappingstorage />
+    ... </zodb>
+    ...
+    ... <eventlog>
+    ...   <logfile>
+    ...     path STDOUT
+    ...   </logfile>
+    ... </eventlog>
+    ... ''' % sitezcml)
+    >>> out.close()
+
+  Now we can call ``application_factory`` to get a WSGI application::
+
+    >>> from grokcore.startup import application_factory
+    >>> app_factory = application_factory({'zope_conf': zope_conf})
+    >>> app_factory
+    <zope.app.wsgi.WSGIPublisherApplication object at 0x...>
+
+``debug_application_factory(global_conf, **local_conf)``
+--------------------------------------------------------
+
+  There's a second application factory that can be used when debugging
+  the application, especially when using the ``z3c.evalexception`` middleware.
+
+  When debugging zope is instructed not to handle any raised exceptions
+  itself. The ``z3c.evalexception`` middleware then catches the exceptions
+  and provides an user interfaces for debugging in the webbrowser.
+
+  As a result also the IUnauthorized execption would not be handled by zope
+  and the authentication mechanisms of zope are not triggered. As a result,
+  when debugging one cannot login.
+
+  The ``debug_application_factory`` function accepts the "exempt-exceptions"
+  configuration option. The value for this option should be a comma seperated
+  list of dotted names for each of the execptions that should *still* be
+  handled by zope and not re-raised to be catched by the middleware.
+
+    >>> from grokcore.startup import debug_application_factory
+    >>> app_factory = debug_application_factory({'zope_conf': zope_conf})
+    >>> app_factory
+    <zope.app.wsgi.WSGIPublisherApplication object at 0x...>
+
+    >>> from zope.interface import implementer
+    >>> from zope.security.interfaces import IUnauthorized
+    >>> @implementer(IUnauthorized)
+    ... class UnauthorizedException(object):
+    ...     pass
+    >>>
+    >>> from zope.component import queryAdapter
+    >>> from zope.publisher.interfaces import IReRaiseException
+
+  Since the ``exempt-execptions`` configuration option was not passed,
+  there's no IReRaiseException adapter registered for any type of exceptions
+  including IUnauthorized:
+
+    >>> error = UnauthorizedException()
+    >>> reraise = queryAdapter(error, IReRaiseException, default=None)
+    >>> reraise is None
+    True
+
+  When the option is passed, the adapter will be registered. Calling this
+  adapter yields ``False``, telling zope not to reraise this particular
+  exception.
+
+    >>> app_factory = debug_application_factory(
+    ...     {'zope_conf': zope_conf},
+    ...     **{'exempt-exceptions': 'zope.security.interfaces.IUnauthorized'})
+    >>>
+    >>> reraise = queryAdapter(error, IReRaiseException, default=None)
+    >>> reraise is None
+    False
+    >>> reraise()
+    False
+
+  Clean up the temp_dir
+
+    >>> import shutil
+    >>> shutil.rmtree(temp_dir)
+
+``interactive_debug_prompt(zope_conf_path)``
+--------------------------------------------
+
+  Get an interactive console with a debugging shell started.
+
+  `grokcore.startup` provides two different debuggers currently: a
+  plain one based on `zope.app.debug` and a more powerful `IPython`_
+  debugger. The IPython debugger is automatically enabled if you have
+  IPython available in the environment.
+
+  You can explicitly enable the IPython_ debugger by stating::
+
+    grokcore.startup [debug]
+
+  in the install requirements of your `setup.py`, probably adding only
+  ``[debug]`` to an already existing entry for
+  `grokcore.startup`. Don't forget to rerun `buildout` afterwards.
+
+  You can explicitly require one or the other debugger by calling::
+
+    grokcore.startup.startup.interactive_debug_prompt(zope_conf)
+
+  or::
+
+    grokcore.startup.debug.ipython_debug_prompt(zope_conf)
+
+  in the ``[interactive_debugger]`` section of your ``buildout.cfg``.
+
+    >>> import zope.app.appsetup.appsetup
+    >>> zope.app.appsetup.appsetup._configured = False
+
+    >>> temp_dir = tempfile.mkdtemp()
+
+    >>> sitezcml = os.path.join(temp_dir, 'site.zcml')
+    >>> out = open(sitezcml, 'w')
+    >>> _ = out.write(
+    ...    """<configure xmlns="http://namespaces.zope.org/zope">
+    ...   <include package="zope.component" file="meta.zcml"/>
+    ...   <include package="zope.component"/>
+    ...   <include package="zope.traversing"/>
+    ...   <include package="zope.security" file="meta.zcml"/>
+    ...   <include package="zope.security"/>
+    ...   <include package="zope.container"/>
+    ...   <include package="zope.site"/>
+    ...   <include package="zope.app.appsetup"/>
+    ... </configure>""")
+    >>> out.close()
+    >>>
+    >>> zopeconf = os.path.join(temp_dir, 'zope.conf')
+    >>> out = open(zopeconf, 'w')
+    >>> _ = out.write("""
+    ...     site-definition %s
+    ...     <zodb>
+    ...       <filestorage>
+    ...         path %s
+    ...       </filestorage>
+    ...     </zodb>
+    ...     <eventlog>
+    ...       <logfile>
+    ...         path STDOUT
+    ...         formatter zope.exceptions.log.Formatter
+    ...       </logfile>
+    ...     </eventlog>
+    ...     """ % (sitezcml, os.path.join(temp_dir, 'Data.fs')))
+    >>> out.close()
+    >>>
+    >>> import sys
+    >>> old_argv = sys.argv[:]
+    >>>
+    >>> script = os.path.join(temp_dir, 'script.py')
+    >>> out = open(script, 'w')
+    >>> _ = out.write(
+    ...    """import sys
+    ... from pprint import pprint
+    ... pprint(debugger)
+    ... pprint(app)
+    ... pprint(root)
+    ... pprint(sys.argv)
+    ... pprint(__file__)
+    ... pprint(__name__)""")
+    >>>
+    >>> out.close()
+    >>>
+    >>> sys.argv = ['interactive_debugger', script]
+    >>> from grokcore.startup import interactive_debug_prompt
+    >>> try:
+    ...     interactive_debug_prompt(zopeconf)
+    ... except SystemExit:
+    ...     # Catch the exit from the interactive prompt as it would
+    ...     # exit this test as well.
+    ...     pass
+    ------
+    ...WARNING zope.app.appsetup Security policy is not configured.
+    Please make sure that securitypolicy.zcml is included in site.zcml
+    immediately before principals.zcml
+    ...
+    <zope.app.debug.debug.Debugger object at ...>
+    <zope.app.debug.debug.Debugger object at ...>
+    <zope.site.folder.Folder object at ...>
+    ['...script.py']
+    '...script.py'
+    '__main__'
+
+  Clean up the temp_dir
+
+    >>> sys.argv = old_argv
+    >>> import shutil
+    >>> shutil.rmtree(temp_dir)
+
+.. _grok: http://pypi.python.org/pypi/grok
+.. _grokproject: http://pypi.python.org/pypi/grokproject
+.. _Paste: http://pythonpaste.org/
+.. _paster: Paste_
+.. _setuptools: http://pypi.python.org/pypi/setuptools
+.. _WSGI: http://www.wsgi.org/wsgi/
+.. _WSGIPublisherApplication: http://apidoc.zope.org/++apidoc++/Code/zope/app/wsgi/WSGIPublisherApplication/index.html
+.. _zc.buildout: http://pypi.python.org/pypi/zc.buildout
+.. _ipython: http://ipython.org/
+
+Changes
+*******
+
+4.0 (2023-07-14)
+================
+
+- Add support for Python 3.10, 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.7, 3.8 and 3.9.
+
+- Drop support for Python 3.4.
+
+
+3.0.1 (2018-01-12)
+==================
+
+- Rearrange tests such that Travis CI can pick up all functional tests too.
+
+3.0.0 (2018-01-10)
+==================
+
+- Python 3 compatibility.
+
+1.2.1 (2016-02-15)
+==================
+
+- Update tests.
+
+1.2 (2012-05-02)
+================
+
+- Added new IPython-based interactive debugger which is used
+  automatically when IPython is available. Otherwise the gdb-style
+  debugger is provided.
+
+1.1 (2010-10-26)
+================
+
+- Drop zdaemon support.
+
+- Close the database explicitely when execing a script through the
+  ``interactive_debug_prompt``. This came to light in tests on Windows, as the
+  tests would try to delete the temp directory it created with the still
+  unclosed database file in there.
+
+1.0.2 (2010-10-05)
+==================
+
+- Somehow the intended fix in 1.0.1 did not actually get included in that
+  release. We make the fix again.
+
+1.0.1 (2010-08-18)
+==================
+
+- When passing a script to the interactive_debug_prompt command, one would
+  expect to be able to do: `if __name__ == '__main__':`, however __name__ would
+  be "__builtin__". This is fixed.
+
+1.0 (2010-05-20)
+================
+
+- Amend the interactive_debug_prompt function to behave more or less like the
+  "old" zopectl command. Whenever there's commandline arguments passed to the
+  command, the first one is assumed to be a python script that is 'execfile'd.
+  This allows ad hoc scripts to run against the setup application.
+
+- Make package comply to zope.org repository policy.
+
+- The upgrade notes will be moved to the Grok upgrade notes.
+
+- Define entry points for main and debug application factories in
+  grokcore.startup.
+
+- Use the groktoolkit.
+
+0.4 (2009-10-06)
+================
+
+- Fix documentation bugs.
+
+0.3 (2009-10-02)
+================
+
+* Add a ``debug_application_factory`` function that allows for the
+  ``exempt-exceptions`` configuration option. The value for this option
+  should be a comma seperated list of dotted names for each of the exceptions
+  that should not be re-raised during debugging.
+
+  This for one allow the IUnauthorized exception to still be handled by zope
+  and thus have the normal authentication mechanisms still work.
+
+* Bring versions.cfg in line with current grok versions.cfg.
+
+0.2 (2009-02-21)
+================
+
+* Made main functions available package wide.
+
+0.1 (2009-01-15)
+================
+
+* Added support for local ``zope_conf`` parameter.
+  Fix bug https://bugs.launchpad.net/grok/+bug/320644
+
+* Created ``grokcore.startup`` in January 2009 by factoring paster
+  related application code out of grokcore templates.
```

### Comparing `grokcore.startup-3.0.1/README.txt` & `grokcore.startup-4.0/README.rst`

 * *Files identical despite different names*

### Comparing `grokcore.startup-3.0.1/setup.py` & `grokcore.startup-4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,80 +1,82 @@
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
 long_description = (
-    read('README.txt')
+    read('README.rst')
     + '\n' +
-    read(os.path.join('src', 'grokcore', 'startup', 'README.txt'))
+    read(os.path.join('src', 'grokcore', 'startup', 'README.rst'))
     + '\n' +
-    read('CHANGES.txt')
-    )
+    read('CHANGES.rst')
+)
 
 
 tests_require = [
     'zope.app.appsetup',
     'zope.component',
     'zope.interface',
     'zope.security',
     'zope.securitypolicy',
     'zope.testing',
-    ]
+    'zope.testrunner',
+]
 
 
 debug_requires = [
     'IPython',
-    ]
+]
 
 setup(
     name='grokcore.startup',
-    version='3.0.1',
+    version='4.0',
     author='Grok Team',
-    author_email='grok-dev@zope.org',
-    url='http://grok.zope.org',
-    download_url='http://pypi.python.org/pypi/grokcore.startup',
+    author_email='zope-dev@zope.dev',
+    url='https://github.com/zopefoundation/grokcore.startup',
     description='Paster support for Grok projects.',
     long_description=long_description,
     license='ZPL',
     keywords='zope zope3 grok grokproject WSGI Paste paster',
     classifiers=[
         'Environment :: Web Environment',
+        'Framework :: Zope :: 3',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
-        'Framework :: Zope3',
-        ],
+    ],
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['grokcore'],
     include_package_data=True,
     zip_safe=False,
+    python_requires='>=3.7',
     install_requires=[
         'setuptools',
         'zope.app.debug',
         'zope.app.wsgi',
         'zope.component',
         'zope.dottedname',
         'zope.publisher',
-        ],
-    tests_require=tests_require,
+    ],
     extras_require=dict(test=tests_require, debug=debug_requires),
     entry_points={
         'paste.app_factory': [
             'main = grokcore.startup:application_factory',
             'debug = grokcore.startup:debug_application_factory',
-            ]
+        ]
     },
 )
```

### Comparing `grokcore.startup-3.0.1/src/grokcore/startup/debug.py` & `grokcore.startup-4.0/src/grokcore/startup/debug.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,32 +7,34 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
-import sys
 import os.path
 import textwrap
+from pprint import pprint
 
 import transaction
-import zope.app.wsgi
 import zope.app.debug
-from pprint import pprint
+import zope.app.wsgi
+from IPython.frontend.terminal.embed import InteractiveShellEmbed
+from zope.component import getMultiAdapter
+from zope.component import getUtility
 from zope.securitypolicy.zopepolicy import settingsForObject
-from zope.component import getUtility, getMultiAdapter
 
-from IPython.frontend.terminal.embed import InteractiveShellEmbed
+
 shell = InteractiveShellEmbed()
 
 
 PATH_SEP = '/'
 
-class GrokDebug(object):
+
+class GrokDebug:
 
     def __init__(self, debugger):
         debugger = debugger
         self.app = debugger
         self.root = debugger.root()
         self.context = self.root
 
@@ -92,15 +94,14 @@
         """
         if path is None:
             return self._get_object_names(self.context)
 
         context = get_context_by_path(self.get_start_context(path), path)
         return self._get_object_names(context)
 
-
     def cd(self, path):
         """cd to specified path.
 
         Bound to `cdg` in IPython shell.
         `path` can be relative or absolute.
 
         To use autocompletion of path command should be invoked
@@ -149,36 +150,38 @@
         return self.context
 
     def providedBy(self, obj=None):
         if not obj:
             obj = self.ctx
         return list(zope.interface.providedBy(obj))
 
+
 def get_context_by_path(context, path):
     for name in (p for p in path.split(PATH_SEP) if p):
         context = context[name]
     return context
 
+
 def path_completer(self, event):
     """TAB path completer for `cdg` and `lsg` commands."""
     relpath = event.symbol
 
-    context = grokd.get_start_context(relpath)
+    context = grokd.get_start_context(relpath)  # noqa: F821 undefined name
 
     # ends with '/'
     if relpath.endswith(PATH_SEP):
         context = get_context_by_path(context, relpath)
-        return [relpath+obj.__name__ for obj in context.values()]
+        return [relpath + obj.__name__ for obj in context.values()]
 
     head, tail = os.path.split(relpath)
     if head and not head.endswith(PATH_SEP):
         head += PATH_SEP
     context = get_context_by_path(context, head)
 
-    return [head+obj.__name__ for obj in context.values()
+    return [head + obj.__name__ for obj in context.values()
             if obj.__name__.startswith(tail)]
 
 
 def ipython_debug_prompt(debugger):
     grokd = GrokDebug(debugger)
     banner = textwrap.dedent(
         """\
@@ -199,10 +202,10 @@
           pby (providedBy)
           pwdg
           sync
           commit
         """)
 
     shell.user_ns.update(grokd.ns())
-    shell.banner2=banner
+    shell.banner2 = banner
     shell.set_hook('complete_command', path_completer, re_key='.*cdg|.*lsg')
     shell(local_ns=grokd.ns())
```

### Comparing `grokcore.startup-3.0.1/src/grokcore/startup/README.txt` & `grokcore.startup-4.0/src/grokcore/startup/README.rst`

 * *Files identical despite different names*

### Comparing `grokcore.startup-3.0.1/src/grokcore/startup/startup.py` & `grokcore.startup-4.0/src/grokcore/startup/startup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,65 @@
+import code
 import os.path
 import sys
-import code
-import zope.app.wsgi
-import zope.app.debug
 
+import zope.app.debug
+import zope.app.wsgi
 from zope.component import provideAdapter
-from zope.publisher.interfaces import IReRaiseException
 from zope.dottedname.resolve import resolve
+from zope.publisher.interfaces import IReRaiseException
+
 
 def application_factory(global_conf, **local_conf):
-    zope_conf = local_conf.get('zope_conf', global_conf.get(
-            'zope_conf', os.path.join('parts', 'etc', 'zope.conf')))
+    zope_conf = local_conf.get(
+        'zope_conf',
+        global_conf.get('zope_conf',
+                        os.path.join('parts', 'etc', 'zope.conf')))
     return zope.app.wsgi.getWSGIApplication(zope_conf)
 
 
 def debug_application_factory(global_conf, **local_conf):
     # First create the application itself
     app = application_factory(global_conf, **local_conf)
     # Then register the IReRaiseException adaptation for
     # various types of exceptions that are exempt from being
     # raised by the publisher.
+
     def do_not_reraise_exception(context):
-        return lambda : False
+        return lambda: False
     iface_names = local_conf.get('exempt-exceptions', '').split(',')
     for name in iface_names:
         name = name.strip()
         if not name:
             continue
         iface = resolve(name)
         provideAdapter(do_not_reraise_exception, (iface, ), IReRaiseException)
     # Return the created application
     return app
 
+
 def _classic_debug_prompt(debugger):
     globals_ = {
         'debugger': debugger,
         'app': debugger,
         'root': debugger.root()}
     # Invoke an interactive interpreter prompt
     banner = (
         "Welcome to the interactive debug prompt.\n"
         "The 'root' variable contains the ZODB root folder.\n"
         "The 'app' variable contains the Debugger, 'app.publish(path)' "
         "simulates a request.")
     code.interact(banner=banner, local=globals_)
 
+
 def _ipython_debug_prompt(debugger):
     from grokcore.startup.debug import ipython_debug_prompt
     return ipython_debug_prompt(debugger)
 
+
 def interactive_debug_prompt(zope_conf):
     db = zope.app.wsgi.config(zope_conf)
     debugger = zope.app.debug.Debugger.fromDatabase(db)
     if len(sys.argv) > 1:
         # There're arguments passed to the command. We replicate the
         # "old" zopectl run command behaviour that would execfile()
         # the second argument.
@@ -62,17 +69,18 @@
             'root': debugger.root()}
         # The current first argument is the interactive_debugger command
         # itself. Pop it from the args list and as a result, the script
         # to run is the first argument.
         del sys.argv[0]
         globals_['__name__'] = '__main__'
         globals_['__file__'] = sys.argv[0]
-        exec(open(sys.argv[0]).read(), globals_)
+        with open(sys.argv[0]) as f:
+            exec(f.read(), globals_)
         # Housekeeping.
         db.close()
         sys.exit()
     # Start the interpreter.
     try:
-        import IPython
+        import IPython  # noqa: F401 imported but unused
     except ImportError:
         return _classic_debug_prompt(debugger)
     return _ipython_debug_prompt(debugger)
```

### Comparing `grokcore.startup-3.0.1/src/grokcore.startup.egg-info/PKG-INFO` & `grokcore.startup-4.0/src/grokcore.startup.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,528 +1,542 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: grokcore.startup
-Version: 3.0.1
+Version: 4.0
 Summary: Paster support for Grok projects.
-Home-page: http://grok.zope.org
+Home-page: https://github.com/zopefoundation/grokcore.startup
 Author: Grok Team
-Author-email: grok-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL
-Download-URL: http://pypi.python.org/pypi/grokcore.startup
-Description: grokcore.startup
-        ****************
-        
-        This package provides elements for starting a `Grok`_ project with
-        `paster`_ and `WSGI`_.
-        
-        .. contents::
-        
-        Setting up ``grokcore.startup``
-        ===============================
-        
-        There is nothing special to setup this package.
-        
-        All you have to do is, to make this package available during runtime.
-        
-        With `zc.buildout`_ or other `setuptools`_-related setups this can be
-        done by simply adding the package name ``grokcore.startup`` to the
-        required packages of your project in ``setup.py``.
-        
-        
-        Detailed Description
-        ********************
-        
-        Setting up Grok projects as ``paster`` served WSGI applications
-        ===============================================================
-        
-        The main target of this package is to provide support for enabling
-        `Grok`_ applications to be run as `paster`_ served `WSGI`_
-        applications. To make this working some configuration files have to be
-        set up.
-        
-        Setting up a project with ``grokproject``
-        -----------------------------------------
-        
-        The most convenient way to setup a `Grok`_ project is using
-        `grokproject`_. Once installed, you can a project like this::
-        
-          $ grokproject Sample
-        
-        which will generate all configuration files for you.
-        
-        .. note:: Older versions of `grokproject`_ need an update
-        
-          As older versions of `grokproject`_ do not support
-          `grokcore.startup`, you might want to update your existing
-          `grokproject`_ installation by running::
-        
-            $ easy_install -U grokproject
-        
-        
-        Setting up a project manually
-        -----------------------------
-        
-        Before we can make use of ``grokcore.startup``, we have to setup
-        several configuration files in the project root:
-        
-        * ``setup.py``
-        
-        * ``buildout.cfg`` (optional)
-        
-        * ``zope.conf`` (normally found in the ``parts/etc/`` subdirectory of your
-          `Grok`_ project)
-        
-        * ``site.zcml`` (normally found in the ``parts/etc/`` subdirectory of your
-          `Grok`_ project)
-        
-        * ``deploy.ini`` (or any other .ini-file; normally found in the
-          ``parts/etc/`` subdirectory of your `Grok`_ project)
-        
-        
-        When we want to setup a Zope instance as `paster`_ served `WSGI`_
-        application, then we have to set a ``paste.app_factory`` entry point
-        in ``setup.py``. A minimal setup could look like this::
-        
-          # setup.py
-          from setuptools import setup, find_packages
-        
-          setup(name='sampleproject',
-                version='0.1dev',
-                description="A sample project",
-                long_description="""Without a long description.""",
-                classifiers=[],
-                keywords="",
-                author="U.N.Owen",
-                author_email="",
-                url="",
-                license="",
-                package_dir={'': 'src'},
-                packages=find_packages('src'),
-                include_package_data=True,
-                zip_safe=False,
-                install_requires=['setuptools',],
-                entry_points = """
-                [paste.app_factory]
-                main = grokcore.startup:application_factory
-                """,
-                )
-        
-        Here the `paste.app_factory` entry point pointing to
-        `grokcore.startup:application_factory` is important.
-        
-        Furthermore we need at least a minimal ``buildout.cfg`` which enables
-        `zc.buildout`_ to create the control scripts for our instance::
-        
-          [buildout]
-          develop = .
-          parts = app
-        
-          [app]
-          recipe = zc.recipe.egg
-          eggs = sampleproject
-                 grokcore.startup
-                 Paste
-                 PasteScript
-                 PasteDeploy
-        
-        Here an egg-entry for ``grokcore.startup`` **might** be important, if
-        it is not required otherwise by your application. Projects generated
-        by `grokproject`_ will automatically include such a dependency and
-        upcoming versions of `Grok`_ will pull in ``grokcore.startup`` anyway,
-        so that ``grokcore.startup`` would not be required in this list of
-        eggs any more.
-        
-        Next we need ``site.zcml`` and ``zope.conf`` files to define the
-        Zope instance. These configurations are completely independent from
-        being served by `Paste`_ or not. If you are upgrading an old `Grok`_
-        project, you can use ``site.zcml`` and ``zope.conf`` of those project
-        as-is. You only have to take care of the maybe changed
-        ``site-definition`` entry in ``zope.conf`` (see below).
-        
-        The file ``site.zcml`` can be quite
-        short, but for real projects you certainly want to have some useful
-        content in here::
-        
-          <configure />
-        
-        A short ``zope.conf`` file for use in tests could look like this::
-        
-          site-definition site.zcml
-        
-          <zodb>
-            <mappingstorage />
-          </zodb>
-        
-          <eventlog>
-            <logfile>
-              path STDOUT
-             </logfile>
-          </eventlog>
-        
-        where the ``site-definition`` entry should point to the location of
-        the file ``site.zcml``. In regular Grok projects those files are put
-        into the ``etc/`` subdirectory of your project root.
-        
-        Finally we have to provide a ``deploy.ini`` (or another .ini-file),
-        which tells paster where to find the pieces. This is also put into the
-        ``etc/`` subdirectory of your project root in regular Grok projects
-        created by `grokproject`_::
-        
-          [app:main]
-          use = egg:sampleproject
-        
-          [server:main]
-          use = egg:Paste#http
-          host = 127.0.0.1
-          port = 8080
-        
-          [DEFAULT]
-          zope_conf = %(here)s/zope.conf
-        
-        
-        
-        API Documentation
-        =================
-        
-        ``application_factory(global_conf, **local_conf)``
-        --------------------------------------------------
-        
-          ``grokcore.startup`` provides a function ``application_factory``
-          which delivers a `WSGIPublisherApplication`_ instance when called
-          with an appropriate configuration. See the `zope.app.wsgi
-          documentation
-          <http://apidoc.zope.org/++apidoc++/Code/zope/app/wsgi/README.txt/index.html>`_
-          to learn more about Zope objects supporting `WSGI`_.
-        
-          A call to this function is normally required as entry point in
-          `setuptools`_-driven `paster`_ environments  (see
-          http://pythonpaste.org/deploy/#paste-app-factory).
-        
-          We have to create our own site definition file -- which will simply
-          be empty -- to provide a minimal test::
-        
-            >>> import os, tempfile
-            >>> temp_dir = tempfile.mkdtemp()
-            >>> sitezcml = os.path.join(temp_dir, 'site.zcml')
-            >>> out = open(sitezcml, 'w')
-            >>> _ = out.write('<configure />')
-            >>> out.close()
-        
-          Furthermore we create a Zope configuration file, which is also quite
-          plain::
-        
-            >>> zope_conf = os.path.join(temp_dir, 'zope.conf')
-            >>> out = open(zope_conf, 'w')
-            >>> _ = out.write('''
-            ... site-definition %s
-            ...
-            ... <zodb>
-            ...   <mappingstorage />
-            ... </zodb>
-            ...
-            ... <eventlog>
-            ...   <logfile>
-            ...     path STDOUT
-            ...   </logfile>
-            ... </eventlog>
-            ... ''' % sitezcml)
-            >>> out.close()
-        
-          Now we can call ``application_factory`` to get a WSGI application::
-        
-            >>> from grokcore.startup import application_factory
-            >>> app_factory = application_factory({'zope_conf': zope_conf})
-            >>> app_factory
-            <zope.app.wsgi.WSGIPublisherApplication object at 0x...>
-        
-        ``debug_application_factory(global_conf, **local_conf)``
-        --------------------------------------------------------
-        
-          There's a second application factory that can be used when debugging
-          the application, especially when using the ``z3c.evalexception`` middleware.
-        
-          When debugging zope is instructed not to handle any raised exceptions
-          itself. The ``z3c.evalexception`` middleware then catches the exceptions
-          and provides an user interfaces for debugging in the webbrowser.
-        
-          As a result also the IUnauthorized execption would not be handled by zope
-          and the authentication mechanisms of zope are not triggered. As a result,
-          when debugging one cannot login.
-        
-          The ``debug_application_factory`` function accepts the "exempt-exceptions"
-          configuration option. The value for this option should be a comma seperated
-          list of dotted names for each of the execptions that should *still* be
-          handled by zope and not re-raised to be catched by the middleware.
-        
-            >>> from grokcore.startup import debug_application_factory
-            >>> app_factory = debug_application_factory({'zope_conf': zope_conf})
-            >>> app_factory
-            <zope.app.wsgi.WSGIPublisherApplication object at 0x...>
-        
-            >>> from zope.interface import implementer
-            >>> from zope.security.interfaces import IUnauthorized
-            >>> @implementer(IUnauthorized)
-            ... class UnauthorizedException(object):
-            ...     pass
-            >>>
-            >>> from zope.component import queryAdapter
-            >>> from zope.publisher.interfaces import IReRaiseException
-        
-          Since the ``exempt-execptions`` configuration option was not passed,
-          there's no IReRaiseException adapter registered for any type of exceptions
-          including IUnauthorized:
-        
-            >>> error = UnauthorizedException()
-            >>> reraise = queryAdapter(error, IReRaiseException, default=None)
-            >>> reraise is None
-            True
-        
-          When the option is passed, the adapter will be registered. Calling this
-          adapter yields ``False``, telling zope not to reraise this particular
-          exception.
-        
-            >>> app_factory = debug_application_factory(
-            ...     {'zope_conf': zope_conf},
-            ...     **{'exempt-exceptions': 'zope.security.interfaces.IUnauthorized'})
-            >>>
-            >>> reraise = queryAdapter(error, IReRaiseException, default=None)
-            >>> reraise is None
-            False
-            >>> reraise()
-            False
-        
-          Clean up the temp_dir
-        
-            >>> import shutil
-            >>> shutil.rmtree(temp_dir)
-        
-        ``interactive_debug_prompt(zope_conf_path)``
-        --------------------------------------------
-        
-          Get an interactive console with a debugging shell started.
-        
-          `grokcore.startup` provides two different debuggers currently: a
-          plain one based on `zope.app.debug` and a more powerful `IPython`_
-          debugger. The IPython debugger is automatically enabled if you have
-          IPython available in the environment.
-        
-          You can explicitly enable the IPython_ debugger by stating::
-        
-            grokcore.startup [debug]
-        
-          in the install requirements of your `setup.py`, probably adding only
-          ``[debug]`` to an already existing entry for
-          `grokcore.startup`. Don't forget to rerun `buildout` afterwards.
-        
-          You can explicitly require one or the other debugger by calling::
-        
-            grokcore.startup.startup.interactive_debug_prompt(zope_conf)
-        
-          or::
-        
-            grokcore.startup.debug.ipython_debug_prompt(zope_conf)
-        
-          in the ``[interactive_debugger]`` section of your ``buildout.cfg``.
-        
-            >>> import zope.app.appsetup.appsetup
-            >>> zope.app.appsetup.appsetup._configured = False
-        
-            >>> temp_dir = tempfile.mkdtemp()
-        
-            >>> sitezcml = os.path.join(temp_dir, 'site.zcml')
-            >>> out = open(sitezcml, 'w')
-            >>> _ = out.write(
-            ...    """<configure xmlns="http://namespaces.zope.org/zope">
-            ...   <include package="zope.component" file="meta.zcml"/>
-            ...   <include package="zope.component"/>
-            ...   <include package="zope.traversing"/>
-            ...   <include package="zope.security" file="meta.zcml"/>
-            ...   <include package="zope.security"/>
-            ...   <include package="zope.container"/>
-            ...   <include package="zope.site"/>
-            ...   <include package="zope.app.appsetup"/>
-            ... </configure>""")
-            >>> out.close()
-            >>>
-            >>> zopeconf = os.path.join(temp_dir, 'zope.conf')
-            >>> out = open(zopeconf, 'w')
-            >>> _ = out.write("""
-            ...     site-definition %s
-            ...     <zodb>
-            ...       <filestorage>
-            ...         path %s
-            ...       </filestorage>
-            ...     </zodb>
-            ...     <eventlog>
-            ...       <logfile>
-            ...         path STDOUT
-            ...         formatter zope.exceptions.log.Formatter
-            ...       </logfile>
-            ...     </eventlog>
-            ...     """ % (sitezcml, os.path.join(temp_dir, 'Data.fs')))
-            >>> out.close()
-            >>>
-            >>> import sys
-            >>> old_argv = sys.argv[:]
-            >>>
-            >>> script = os.path.join(temp_dir, 'script.py')
-            >>> out = open(script, 'w')
-            >>> _ = out.write(
-            ...    """import sys
-            ... from pprint import pprint
-            ... pprint(debugger)
-            ... pprint(app)
-            ... pprint(root)
-            ... pprint(sys.argv)
-            ... pprint(__file__)
-            ... pprint(__name__)""")
-            >>>
-            >>> out.close()
-            >>>
-            >>> sys.argv = ['interactive_debugger', script]
-            >>> from grokcore.startup import interactive_debug_prompt
-            >>> try:
-            ...     interactive_debug_prompt(zopeconf)
-            ... except SystemExit:
-            ...     # Catch the exit from the interactive prompt as it would
-            ...     # exit this test as well.
-            ...     pass
-            ------
-            ...WARNING zope.app.appsetup Security policy is not configured.
-            Please make sure that securitypolicy.zcml is included in site.zcml
-            immediately before principals.zcml
-            ...
-            <zope.app.debug.debug.Debugger object at ...>
-            <zope.app.debug.debug.Debugger object at ...>
-            <zope.site.folder.Folder object at ...>
-            ['...script.py']
-            '...script.py'
-            '__main__'
-        
-          Clean up the temp_dir
-        
-            >>> sys.argv = old_argv
-            >>> import shutil
-            >>> shutil.rmtree(temp_dir)
-        
-        .. _grok: http://pypi.python.org/pypi/grok
-        .. _grokproject: http://pypi.python.org/pypi/grokproject
-        .. _Paste: http://pythonpaste.org/
-        .. _paster: Paste_
-        .. _setuptools: http://pypi.python.org/pypi/setuptools
-        .. _WSGI: http://www.wsgi.org/wsgi/
-        .. _WSGIPublisherApplication: http://apidoc.zope.org/++apidoc++/Code/zope/app/wsgi/WSGIPublisherApplication/index.html
-        .. _zc.buildout: http://pypi.python.org/pypi/zc.buildout
-        .. _ipython: http://ipython.org/
-        
-        Changes
-        *******
-        
-        3.0.1 (2018-01-12)
-        ==================
-        
-        - Rearrange tests such that Travis CI can pick up all functional tests too.
-        
-        3.0.0 (2018-01-10)
-        ==================
-        
-        - Python 3 compatibility.
-        
-        1.2.1 (2016-02-15)
-        ==================
-        
-        - Update tests.
-        
-        1.2 (2012-05-02)
-        ================
-        
-        - Added new IPython-based interactive debugger which is used
-          automatically when IPython is available. Otherwise the gdb-style
-          debugger is provided.
-        
-        1.1 (2010-10-26)
-        ================
-        
-        - Drop zdaemon support.
-        
-        - Close the database explicitely when execing a script through the
-          ``interactive_debug_prompt``. This came to light in tests on Windows, as the
-          tests would try to delete the temp directory it created with the still
-          unclosed database file in there.
-        
-        1.0.2 (2010-10-05)
-        ==================
-        
-        - Somehow the intended fix in 1.0.1 did not actually get included in that
-          release. We make the fix again.
-        
-        1.0.1 (2010-08-18)
-        ==================
-        
-        - When passing a script to the interactive_debug_prompt command, one would
-          expect to be able to do: `if __name__ == '__main__':`, however __name__ would
-          be "__builtin__". This is fixed.
-        
-        1.0 (2010-05-20)
-        ================
-        
-        - Amend the interactive_debug_prompt function to behave more or less like the
-          "old" zopectl command. Whenever there's commandline arguments passed to the
-          command, the first one is assumed to be a python script that is 'execfile'd.
-          This allows ad hoc scripts to run against the setup application.
-        
-        - Make package comply to zope.org repository policy.
-        
-        - The upgrade notes will be moved to the Grok upgrade notes.
-        
-        - Define entry points for main and debug application factories in
-          grokcore.startup.
-        
-        - Use the groktoolkit.
-        
-        0.4 (2009-10-06)
-        ================
-        
-        - Fix documentation bugs.
-        
-        0.3 (2009-10-02)
-        ================
-        
-        * Add a ``debug_application_factory`` function that allows for the
-          ``exempt-exceptions`` configuration option. The value for this option
-          should be a comma seperated list of dotted names for each of the exceptions
-          that should not be re-raised during debugging.
-        
-          This for one allow the IUnauthorized exception to still be handled by zope
-          and thus have the normal authentication mechanisms still work.
-        
-        * Bring versions.cfg in line with current grok versions.cfg.
-        
-        0.2 (2009-02-21)
-        ================
-        
-        * Made main functions available package wide.
-        
-        0.1 (2009-01-15)
-        ================
-        
-        * Added support for local ``zope_conf`` parameter.
-          Fix bug https://bugs.launchpad.net/grok/+bug/320644
-        
-        * Created ``grokcore.startup`` in January 2009 by factoring paster
-          related application code out of grokcore templates.
-        
 Keywords: zope zope3 grok grokproject WSGI Paste paster
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
+Classifier: Framework :: Zope :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Framework :: Zope3
+Requires-Python: >=3.7
+Provides-Extra: test
+Provides-Extra: debug
+License-File: LICENSE.txt
+
+grokcore.startup
+****************
+
+This package provides elements for starting a `Grok`_ project with
+`paster`_ and `WSGI`_.
+
+.. contents::
+
+Setting up ``grokcore.startup``
+===============================
+
+There is nothing special to setup this package.
+
+All you have to do is, to make this package available during runtime.
+
+With `zc.buildout`_ or other `setuptools`_-related setups this can be
+done by simply adding the package name ``grokcore.startup`` to the
+required packages of your project in ``setup.py``.
+
+
+Detailed Description
+********************
+
+Setting up Grok projects as ``paster`` served WSGI applications
+===============================================================
+
+The main target of this package is to provide support for enabling
+`Grok`_ applications to be run as `paster`_ served `WSGI`_
+applications. To make this working some configuration files have to be
+set up.
+
+Setting up a project with ``grokproject``
+-----------------------------------------
+
+The most convenient way to setup a `Grok`_ project is using
+`grokproject`_. Once installed, you can a project like this::
+
+  $ grokproject Sample
+
+which will generate all configuration files for you.
+
+.. note:: Older versions of `grokproject`_ need an update
+
+  As older versions of `grokproject`_ do not support
+  `grokcore.startup`, you might want to update your existing
+  `grokproject`_ installation by running::
+
+    $ easy_install -U grokproject
+
+
+Setting up a project manually
+-----------------------------
+
+Before we can make use of ``grokcore.startup``, we have to setup
+several configuration files in the project root:
+
+* ``setup.py``
+
+* ``buildout.cfg`` (optional)
+
+* ``zope.conf`` (normally found in the ``parts/etc/`` subdirectory of your
+  `Grok`_ project)
+
+* ``site.zcml`` (normally found in the ``parts/etc/`` subdirectory of your
+  `Grok`_ project)
+
+* ``deploy.ini`` (or any other .ini-file; normally found in the
+  ``parts/etc/`` subdirectory of your `Grok`_ project)
+
+
+When we want to setup a Zope instance as `paster`_ served `WSGI`_
+application, then we have to set a ``paste.app_factory`` entry point
+in ``setup.py``. A minimal setup could look like this::
+
+  # setup.py
+  from setuptools import setup, find_packages
+
+  setup(name='sampleproject',
+        version='0.1dev',
+        description="A sample project",
+        long_description="""Without a long description.""",
+        classifiers=[],
+        keywords="",
+        author="U.N.Owen",
+        author_email="",
+        url="",
+        license="",
+        package_dir={'': 'src'},
+        packages=find_packages('src'),
+        include_package_data=True,
+        zip_safe=False,
+        install_requires=['setuptools',],
+        entry_points = """
+        [paste.app_factory]
+        main = grokcore.startup:application_factory
+        """,
+        )
+
+Here the `paste.app_factory` entry point pointing to
+`grokcore.startup:application_factory` is important.
+
+Furthermore we need at least a minimal ``buildout.cfg`` which enables
+`zc.buildout`_ to create the control scripts for our instance::
+
+  [buildout]
+  develop = .
+  parts = app
+
+  [app]
+  recipe = zc.recipe.egg
+  eggs = sampleproject
+         grokcore.startup
+         Paste
+         PasteScript
+         PasteDeploy
+
+Here an egg-entry for ``grokcore.startup`` **might** be important, if
+it is not required otherwise by your application. Projects generated
+by `grokproject`_ will automatically include such a dependency and
+upcoming versions of `Grok`_ will pull in ``grokcore.startup`` anyway,
+so that ``grokcore.startup`` would not be required in this list of
+eggs any more.
+
+Next we need ``site.zcml`` and ``zope.conf`` files to define the
+Zope instance. These configurations are completely independent from
+being served by `Paste`_ or not. If you are upgrading an old `Grok`_
+project, you can use ``site.zcml`` and ``zope.conf`` of those project
+as-is. You only have to take care of the maybe changed
+``site-definition`` entry in ``zope.conf`` (see below).
+
+The file ``site.zcml`` can be quite
+short, but for real projects you certainly want to have some useful
+content in here::
+
+  <configure />
+
+A short ``zope.conf`` file for use in tests could look like this::
+
+  site-definition site.zcml
+
+  <zodb>
+    <mappingstorage />
+  </zodb>
+
+  <eventlog>
+    <logfile>
+      path STDOUT
+     </logfile>
+  </eventlog>
+
+where the ``site-definition`` entry should point to the location of
+the file ``site.zcml``. In regular Grok projects those files are put
+into the ``etc/`` subdirectory of your project root.
+
+Finally we have to provide a ``deploy.ini`` (or another .ini-file),
+which tells paster where to find the pieces. This is also put into the
+``etc/`` subdirectory of your project root in regular Grok projects
+created by `grokproject`_::
+
+  [app:main]
+  use = egg:sampleproject
+
+  [server:main]
+  use = egg:Paste#http
+  host = 127.0.0.1
+  port = 8080
+
+  [DEFAULT]
+  zope_conf = %(here)s/zope.conf
+
+
+
+API Documentation
+=================
+
+``application_factory(global_conf, **local_conf)``
+--------------------------------------------------
+
+  ``grokcore.startup`` provides a function ``application_factory``
+  which delivers a `WSGIPublisherApplication`_ instance when called
+  with an appropriate configuration. See the `zope.app.wsgi
+  documentation
+  <http://apidoc.zope.org/++apidoc++/Code/zope/app/wsgi/README.txt/index.html>`_
+  to learn more about Zope objects supporting `WSGI`_.
+
+  A call to this function is normally required as entry point in
+  `setuptools`_-driven `paster`_ environments  (see
+  http://pythonpaste.org/deploy/#paste-app-factory).
+
+  We have to create our own site definition file -- which will simply
+  be empty -- to provide a minimal test::
+
+    >>> import os, tempfile
+    >>> temp_dir = tempfile.mkdtemp()
+    >>> sitezcml = os.path.join(temp_dir, 'site.zcml')
+    >>> out = open(sitezcml, 'w')
+    >>> _ = out.write('<configure />')
+    >>> out.close()
+
+  Furthermore we create a Zope configuration file, which is also quite
+  plain::
+
+    >>> zope_conf = os.path.join(temp_dir, 'zope.conf')
+    >>> out = open(zope_conf, 'w')
+    >>> _ = out.write('''
+    ... site-definition %s
+    ...
+    ... <zodb>
+    ...   <mappingstorage />
+    ... </zodb>
+    ...
+    ... <eventlog>
+    ...   <logfile>
+    ...     path STDOUT
+    ...   </logfile>
+    ... </eventlog>
+    ... ''' % sitezcml)
+    >>> out.close()
+
+  Now we can call ``application_factory`` to get a WSGI application::
+
+    >>> from grokcore.startup import application_factory
+    >>> app_factory = application_factory({'zope_conf': zope_conf})
+    >>> app_factory
+    <zope.app.wsgi.WSGIPublisherApplication object at 0x...>
+
+``debug_application_factory(global_conf, **local_conf)``
+--------------------------------------------------------
+
+  There's a second application factory that can be used when debugging
+  the application, especially when using the ``z3c.evalexception`` middleware.
+
+  When debugging zope is instructed not to handle any raised exceptions
+  itself. The ``z3c.evalexception`` middleware then catches the exceptions
+  and provides an user interfaces for debugging in the webbrowser.
+
+  As a result also the IUnauthorized execption would not be handled by zope
+  and the authentication mechanisms of zope are not triggered. As a result,
+  when debugging one cannot login.
+
+  The ``debug_application_factory`` function accepts the "exempt-exceptions"
+  configuration option. The value for this option should be a comma seperated
+  list of dotted names for each of the execptions that should *still* be
+  handled by zope and not re-raised to be catched by the middleware.
+
+    >>> from grokcore.startup import debug_application_factory
+    >>> app_factory = debug_application_factory({'zope_conf': zope_conf})
+    >>> app_factory
+    <zope.app.wsgi.WSGIPublisherApplication object at 0x...>
+
+    >>> from zope.interface import implementer
+    >>> from zope.security.interfaces import IUnauthorized
+    >>> @implementer(IUnauthorized)
+    ... class UnauthorizedException(object):
+    ...     pass
+    >>>
+    >>> from zope.component import queryAdapter
+    >>> from zope.publisher.interfaces import IReRaiseException
+
+  Since the ``exempt-execptions`` configuration option was not passed,
+  there's no IReRaiseException adapter registered for any type of exceptions
+  including IUnauthorized:
+
+    >>> error = UnauthorizedException()
+    >>> reraise = queryAdapter(error, IReRaiseException, default=None)
+    >>> reraise is None
+    True
+
+  When the option is passed, the adapter will be registered. Calling this
+  adapter yields ``False``, telling zope not to reraise this particular
+  exception.
+
+    >>> app_factory = debug_application_factory(
+    ...     {'zope_conf': zope_conf},
+    ...     **{'exempt-exceptions': 'zope.security.interfaces.IUnauthorized'})
+    >>>
+    >>> reraise = queryAdapter(error, IReRaiseException, default=None)
+    >>> reraise is None
+    False
+    >>> reraise()
+    False
+
+  Clean up the temp_dir
+
+    >>> import shutil
+    >>> shutil.rmtree(temp_dir)
+
+``interactive_debug_prompt(zope_conf_path)``
+--------------------------------------------
+
+  Get an interactive console with a debugging shell started.
+
+  `grokcore.startup` provides two different debuggers currently: a
+  plain one based on `zope.app.debug` and a more powerful `IPython`_
+  debugger. The IPython debugger is automatically enabled if you have
+  IPython available in the environment.
+
+  You can explicitly enable the IPython_ debugger by stating::
+
+    grokcore.startup [debug]
+
+  in the install requirements of your `setup.py`, probably adding only
+  ``[debug]`` to an already existing entry for
+  `grokcore.startup`. Don't forget to rerun `buildout` afterwards.
+
+  You can explicitly require one or the other debugger by calling::
+
+    grokcore.startup.startup.interactive_debug_prompt(zope_conf)
+
+  or::
+
+    grokcore.startup.debug.ipython_debug_prompt(zope_conf)
+
+  in the ``[interactive_debugger]`` section of your ``buildout.cfg``.
+
+    >>> import zope.app.appsetup.appsetup
+    >>> zope.app.appsetup.appsetup._configured = False
+
+    >>> temp_dir = tempfile.mkdtemp()
+
+    >>> sitezcml = os.path.join(temp_dir, 'site.zcml')
+    >>> out = open(sitezcml, 'w')
+    >>> _ = out.write(
+    ...    """<configure xmlns="http://namespaces.zope.org/zope">
+    ...   <include package="zope.component" file="meta.zcml"/>
+    ...   <include package="zope.component"/>
+    ...   <include package="zope.traversing"/>
+    ...   <include package="zope.security" file="meta.zcml"/>
+    ...   <include package="zope.security"/>
+    ...   <include package="zope.container"/>
+    ...   <include package="zope.site"/>
+    ...   <include package="zope.app.appsetup"/>
+    ... </configure>""")
+    >>> out.close()
+    >>>
+    >>> zopeconf = os.path.join(temp_dir, 'zope.conf')
+    >>> out = open(zopeconf, 'w')
+    >>> _ = out.write("""
+    ...     site-definition %s
+    ...     <zodb>
+    ...       <filestorage>
+    ...         path %s
+    ...       </filestorage>
+    ...     </zodb>
+    ...     <eventlog>
+    ...       <logfile>
+    ...         path STDOUT
+    ...         formatter zope.exceptions.log.Formatter
+    ...       </logfile>
+    ...     </eventlog>
+    ...     """ % (sitezcml, os.path.join(temp_dir, 'Data.fs')))
+    >>> out.close()
+    >>>
+    >>> import sys
+    >>> old_argv = sys.argv[:]
+    >>>
+    >>> script = os.path.join(temp_dir, 'script.py')
+    >>> out = open(script, 'w')
+    >>> _ = out.write(
+    ...    """import sys
+    ... from pprint import pprint
+    ... pprint(debugger)
+    ... pprint(app)
+    ... pprint(root)
+    ... pprint(sys.argv)
+    ... pprint(__file__)
+    ... pprint(__name__)""")
+    >>>
+    >>> out.close()
+    >>>
+    >>> sys.argv = ['interactive_debugger', script]
+    >>> from grokcore.startup import interactive_debug_prompt
+    >>> try:
+    ...     interactive_debug_prompt(zopeconf)
+    ... except SystemExit:
+    ...     # Catch the exit from the interactive prompt as it would
+    ...     # exit this test as well.
+    ...     pass
+    ------
+    ...WARNING zope.app.appsetup Security policy is not configured.
+    Please make sure that securitypolicy.zcml is included in site.zcml
+    immediately before principals.zcml
+    ...
+    <zope.app.debug.debug.Debugger object at ...>
+    <zope.app.debug.debug.Debugger object at ...>
+    <zope.site.folder.Folder object at ...>
+    ['...script.py']
+    '...script.py'
+    '__main__'
+
+  Clean up the temp_dir
+
+    >>> sys.argv = old_argv
+    >>> import shutil
+    >>> shutil.rmtree(temp_dir)
+
+.. _grok: http://pypi.python.org/pypi/grok
+.. _grokproject: http://pypi.python.org/pypi/grokproject
+.. _Paste: http://pythonpaste.org/
+.. _paster: Paste_
+.. _setuptools: http://pypi.python.org/pypi/setuptools
+.. _WSGI: http://www.wsgi.org/wsgi/
+.. _WSGIPublisherApplication: http://apidoc.zope.org/++apidoc++/Code/zope/app/wsgi/WSGIPublisherApplication/index.html
+.. _zc.buildout: http://pypi.python.org/pypi/zc.buildout
+.. _ipython: http://ipython.org/
+
+Changes
+*******
+
+4.0 (2023-07-14)
+================
+
+- Add support for Python 3.10, 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.7, 3.8 and 3.9.
+
+- Drop support for Python 3.4.
+
+
+3.0.1 (2018-01-12)
+==================
+
+- Rearrange tests such that Travis CI can pick up all functional tests too.
+
+3.0.0 (2018-01-10)
+==================
+
+- Python 3 compatibility.
+
+1.2.1 (2016-02-15)
+==================
+
+- Update tests.
+
+1.2 (2012-05-02)
+================
+
+- Added new IPython-based interactive debugger which is used
+  automatically when IPython is available. Otherwise the gdb-style
+  debugger is provided.
+
+1.1 (2010-10-26)
+================
+
+- Drop zdaemon support.
+
+- Close the database explicitely when execing a script through the
+  ``interactive_debug_prompt``. This came to light in tests on Windows, as the
+  tests would try to delete the temp directory it created with the still
+  unclosed database file in there.
+
+1.0.2 (2010-10-05)
+==================
+
+- Somehow the intended fix in 1.0.1 did not actually get included in that
+  release. We make the fix again.
+
+1.0.1 (2010-08-18)
+==================
+
+- When passing a script to the interactive_debug_prompt command, one would
+  expect to be able to do: `if __name__ == '__main__':`, however __name__ would
+  be "__builtin__". This is fixed.
+
+1.0 (2010-05-20)
+================
+
+- Amend the interactive_debug_prompt function to behave more or less like the
+  "old" zopectl command. Whenever there's commandline arguments passed to the
+  command, the first one is assumed to be a python script that is 'execfile'd.
+  This allows ad hoc scripts to run against the setup application.
+
+- Make package comply to zope.org repository policy.
+
+- The upgrade notes will be moved to the Grok upgrade notes.
+
+- Define entry points for main and debug application factories in
+  grokcore.startup.
+
+- Use the groktoolkit.
+
+0.4 (2009-10-06)
+================
+
+- Fix documentation bugs.
+
+0.3 (2009-10-02)
+================
+
+* Add a ``debug_application_factory`` function that allows for the
+  ``exempt-exceptions`` configuration option. The value for this option
+  should be a comma seperated list of dotted names for each of the exceptions
+  that should not be re-raised during debugging.
+
+  This for one allow the IUnauthorized exception to still be handled by zope
+  and thus have the normal authentication mechanisms still work.
+
+* Bring versions.cfg in line with current grok versions.cfg.
+
+0.2 (2009-02-21)
+================
+
+* Made main functions available package wide.
+
+0.1 (2009-01-15)
+================
+
+* Added support for local ``zope_conf`` parameter.
+  Fix bug https://bugs.launchpad.net/grok/+bug/320644
+
+* Created ``grokcore.startup`` in January 2009 by factoring paster
+  related application code out of grokcore templates.
```

### Comparing `grokcore.startup-3.0.1/src/grokcore.startup.egg-info/SOURCES.txt` & `grokcore.startup-4.0/src/grokcore.startup.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-.travis.yml
-CHANGES.txt
+CHANGES.rst
+CONTRIBUTING.md
 COPYRIGHT.txt
 CREDITS.txt
 LICENSE.txt
 MANIFEST.in
-README.txt
-bootstrap.py
-buildout.cfg
-requirements.txt
+README.rst
+setup.cfg
 setup.py
+tox.ini
 src/grokcore/__init__.py
 src/grokcore.startup.egg-info/PKG-INFO
 src/grokcore.startup.egg-info/SOURCES.txt
 src/grokcore.startup.egg-info/dependency_links.txt
 src/grokcore.startup.egg-info/entry_points.txt
 src/grokcore.startup.egg-info/namespace_packages.txt
 src/grokcore.startup.egg-info/not-zip-safe
 src/grokcore.startup.egg-info/requires.txt
 src/grokcore.startup.egg-info/top_level.txt
-src/grokcore/startup/README.txt
+src/grokcore/startup/README.rst
 src/grokcore/startup/__init__.py
 src/grokcore/startup/debug.py
 src/grokcore/startup/startup.py
 src/grokcore/startup/tests/__init__.py
 src/grokcore/startup/tests/test_grokcorestartup.py
```

