# Comparing `tmp/gocept.country-2.1.tar.gz` & `tmp/gocept.country-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gocept.country-2.1.tar", last modified: Mon Sep 30 12:21:47 2019, max compression
+gzip compressed data, was "gocept.country-3.0.tar", last modified: Fri Jul 14 12:46:36 2023, max compression
```

## Comparing `gocept.country-2.1.tar` & `gocept.country-3.0.tar`

### file list

```diff
@@ -1,35 +1,33 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2019-09-30 12:21:47.000000 gocept.country-2.1/
--rw-r--r--   0 mac        (501) staff       (20)      187 2019-09-30 12:21:46.000000 gocept.country-2.1/.coveragerc
--rw-r--r--   0 mac        (501) staff       (20)      148 2019-09-30 12:21:46.000000 gocept.country-2.1/.gitignore
--rw-r--r--   0 mac        (501) staff       (20)      957 2019-09-30 12:21:46.000000 gocept.country-2.1/.travis.yml
--rw-r--r--   0 mac        (501) staff       (20)     2255 2019-09-30 12:21:46.000000 gocept.country-2.1/CHANGES.rst
--rw-r--r--   0 mac        (501) staff       (20)      449 2019-09-30 12:21:46.000000 gocept.country-2.1/COPYRIGHT.txt
--rw-r--r--   0 mac        (501) staff       (20)     2071 2019-09-30 12:21:46.000000 gocept.country-2.1/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)    19851 2019-09-30 12:21:47.000000 gocept.country-2.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      685 2019-09-30 12:21:46.000000 gocept.country-2.1/README.rst
--rw-r--r--   0 mac        (501) staff       (20)       23 2019-09-30 12:21:46.000000 gocept.country-2.1/pytest.ini
--rw-r--r--   0 mac        (501) staff       (20)       38 2019-09-30 12:21:47.000000 gocept.country-2.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     2199 2019-09-30 12:21:46.000000 gocept.country-2.1/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2019-09-30 12:21:47.000000 gocept.country-2.1/src/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2019-09-30 12:21:47.000000 gocept.country-2.1/src/gocept/
--rw-r--r--   0 mac        (501) staff       (20)       56 2019-09-30 12:21:46.000000 gocept.country-2.1/src/gocept/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2019-09-30 12:21:47.000000 gocept.country-2.1/src/gocept/country/
--rw-r--r--   0 mac        (501) staff       (20)    10812 2019-09-30 12:21:46.000000 gocept.country-2.1/src/gocept/country/README.txt
--rw-r--r--   0 mac        (501) staff       (20)      460 2019-09-30 12:21:46.000000 gocept.country-2.1/src/gocept/country/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      712 2019-09-30 12:21:46.000000 gocept.country-2.1/src/gocept/country/configure.zcml
--rw-r--r--   0 mac        (501) staff       (20)     2340 2019-09-30 12:21:46.000000 gocept.country-2.1/src/gocept/country/db.py
--rw-r--r--   0 mac        (501) staff       (20)      271 2019-09-30 12:21:46.000000 gocept.country-2.1/src/gocept/country/ftesting.zcml
--rw-r--r--   0 mac        (501) staff       (20)      303 2019-09-30 12:21:46.000000 gocept.country-2.1/src/gocept/country/interfaces.py
--rw-r--r--   0 mac        (501) staff       (20)     3240 2019-09-30 12:21:46.000000 gocept.country-2.1/src/gocept/country/sources.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2019-09-30 12:21:47.000000 gocept.country-2.1/src/gocept/country/tests/
--rw-r--r--   0 mac        (501) staff       (20)      222 2019-09-30 12:21:46.000000 gocept.country-2.1/src/gocept/country/tests/test_db.py
--rw-r--r--   0 mac        (501) staff       (20)      445 2019-09-30 12:21:46.000000 gocept.country-2.1/src/gocept/country/tests/test_doctest.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2019-09-30 12:21:47.000000 gocept.country-2.1/src/gocept.country.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)    19851 2019-09-30 12:21:47.000000 gocept.country-2.1/src/gocept.country.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      728 2019-09-30 12:21:47.000000 gocept.country-2.1/src/gocept.country.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2019-09-30 12:21:47.000000 gocept.country-2.1/src/gocept.country.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)        7 2019-09-30 12:21:47.000000 gocept.country-2.1/src/gocept.country.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2019-09-30 12:21:47.000000 gocept.country-2.1/src/gocept.country.egg-info/not-zip-safe
--rw-r--r--   0 mac        (501) staff       (20)      162 2019-09-30 12:21:47.000000 gocept.country-2.1/src/gocept.country.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        7 2019-09-30 12:21:47.000000 gocept.country-2.1/src/gocept.country.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)      688 2019-09-30 12:21:46.000000 gocept.country-2.1/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-14 12:46:36.921338 gocept.country-3.0/
+-rw-r--r--   0 mac        (513) staff       (20)      115 2023-07-14 12:46:36.000000 gocept.country-3.0/.coveragerc
+-rw-r--r--   0 mac        (513) staff       (20)     2383 2023-07-14 12:46:36.000000 gocept.country-3.0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      449 2023-07-14 12:46:36.000000 gocept.country-3.0/COPYRIGHT.txt
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-07-14 12:46:36.000000 gocept.country-3.0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)    15637 2023-07-14 12:46:36.921519 gocept.country-3.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      759 2023-07-14 12:46:36.000000 gocept.country-3.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)       23 2023-07-14 12:46:36.000000 gocept.country-3.0/pytest.ini
+-rw-r--r--   0 mac        (513) staff       (20)      213 2023-07-14 12:46:36.922083 gocept.country-3.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     2187 2023-07-14 12:46:36.000000 gocept.country-3.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-14 12:46:36.912698 gocept.country-3.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-14 12:46:36.916039 gocept.country-3.0/src/gocept/
+-rw-r--r--   0 mac        (513) staff       (20)       56 2023-07-14 12:46:36.000000 gocept.country-3.0/src/gocept/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-14 12:46:36.920434 gocept.country-3.0/src/gocept/country/
+-rw-r--r--   0 mac        (513) staff       (20)    10792 2023-07-14 12:46:36.000000 gocept.country-3.0/src/gocept/country/README.txt
+-rw-r--r--   0 mac        (513) staff       (20)      435 2023-07-14 12:46:36.000000 gocept.country-3.0/src/gocept/country/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)      712 2023-07-14 12:46:36.000000 gocept.country-3.0/src/gocept/country/configure.zcml
+-rw-r--r--   0 mac        (513) staff       (20)     2306 2023-07-14 12:46:36.000000 gocept.country-3.0/src/gocept/country/db.py
+-rw-r--r--   0 mac        (513) staff       (20)      271 2023-07-14 12:46:36.000000 gocept.country-3.0/src/gocept/country/ftesting.zcml
+-rw-r--r--   0 mac        (513) staff       (20)      277 2023-07-14 12:46:36.000000 gocept.country-3.0/src/gocept/country/interfaces.py
+-rw-r--r--   0 mac        (513) staff       (20)     3197 2023-07-14 12:46:36.000000 gocept.country-3.0/src/gocept/country/sources.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-14 12:46:36.921052 gocept.country-3.0/src/gocept/country/tests/
+-rw-r--r--   0 mac        (513) staff       (20)      206 2023-07-14 12:46:36.000000 gocept.country-3.0/src/gocept/country/tests/test_db.py
+-rw-r--r--   0 mac        (513) staff       (20)      326 2023-07-14 12:46:36.000000 gocept.country-3.0/src/gocept/country/tests/test_doctest.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-14 12:46:36.918231 gocept.country-3.0/src/gocept.country.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)    15637 2023-07-14 12:46:36.000000 gocept.country-3.0/src/gocept.country.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      715 2023-07-14 12:46:36.000000 gocept.country-3.0/src/gocept.country.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-07-14 12:46:36.000000 gocept.country-3.0/src/gocept.country.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        7 2023-07-14 12:46:36.000000 gocept.country-3.0/src/gocept.country.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-07-14 12:46:36.000000 gocept.country-3.0/src/gocept.country.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)      162 2023-07-14 12:46:36.000000 gocept.country-3.0/src/gocept.country.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        7 2023-07-14 12:46:36.000000 gocept.country-3.0/src/gocept.country.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)      530 2023-07-14 12:46:36.000000 gocept.country-3.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gocept.country-2.1/CHANGES.rst` & `gocept.country-3.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 Changes
 =======
 
+3.0 (2023-07-14)
+----------------
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.9, 3.10, 3.11.
+
+
 2.1 (2019-09-30)
 ----------------
 
-- Support Python 3.5 up to 3.8, PyPy and PyPy3.
+- Add support for Python 3.5 up to 3.8, PyPy and PyPy3.
 
 - Replace test dependency on `zope.app.testing` by `zope.app.wsgi[testlayer]`.
 
 - Migrate to Github.
 
 
 2.0 (2017-01-21)
@@ -109,8 +117,7 @@
 
 - initial release
 
 Contributors
 ============
 
 - Michael Howitz <mh at gocept dot com>
-
```

### Comparing `gocept.country-2.1/LICENSE.txt` & `gocept.country-3.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,8 +37,7 @@
 EVENT SHALL THE COPYRIGHT HOLDERS BE LIABLE FOR ANY DIRECT, INDIRECT,
 INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
 PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
```

### Comparing `gocept.country-2.1/PKG-INFO` & `gocept.country-3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,576 +1,584 @@
 Metadata-Version: 2.1
 Name: gocept.country
-Version: 2.1
+Version: 3.0
 Summary: Zope 3 sources for pycountry databases
 Home-page: https://github.com/gocept/gocept.country
 Author: gocept gmbh & co. kg
 Author-email: mail@gocept.com
 License: ZPL 2.1
-Description: Copyright (c) 2008-2015 gocept gmbh & co. kg
-        
-        All Rights Reserved.
-        
-        This software is subject to the provisions of the Zope Public License,
-        Version 2.1 (ZPL). A copy of the ZPL should accompany this distribution.
-        THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
-        WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-        WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
-        FOR A PARTICULAR PURPOSE.
-        
-        
-        .. image:: https://travis-ci.com/gocept/gocept.country.svg?branch=master
-            :target: https://travis-ci.com/gocept/gocept.country
-            
-        .. image:: https://coveralls.io/repos/github/gocept/gocept.country/badge.svg?branch=master
-            :target: https://coveralls.io/github/gocept/gocept.country?branch=master
-        
-        
-        This package lets you use the `pycountry database
-        <http://pypi.python.org/pypi/pycountry/>`_ within Zope 3.
-        
-        
-        In practice, this means e.g., that you can easily get a zope.schema.Choice
-        field to provide a full list of iso 3166 country codes.
-        
-        For more information about the database please refer to the
-        `pycountry product <http://pypi.python.org/pypi/pycountry/>`_.
-        
-        .. contents::
-        
-        
-        ==============
-        gocept.country
-        ==============
-        
-        
-        `gocept.country` provides Zope 3 sources for the pycountry databases. You can
-        use it e.g. to get a ``zope.schema.Choice`` field with all ISO 3166 countries.
-        
-          >>> import gocept.country
-          >>> import gocept.country.db
-          >>> import zope.schema
-        
-        
-        ISO 3166 Countries
-        ==================
-        
-        To get a list of ISO 3166 countries in a web form, you can use the
-        ``zope.schema.Choice`` field and provide the gocept.country.countries as
-        source:
-        
-          >>> countries_field = zope.schema.Choice(title=u'Country',
-          ...                            source=gocept.country.countries)
-          >>> countries_field
-          <zope.schema._field.Choice object at 0x...>
-          >>> countries = iter(countries_field.source)
-        
-        
-        The ``gocept.country.countries`` source factory returns Country objects as
-        values, which use the values from pycountry:
-        
-          >>> aruba = next(countries)
-          >>> afghanistan = next(countries)
-          >>> afghanistan
-          <gocept.country.db.Country object at 0x...>
-          >>> print(afghanistan.name)
-          Afghanistan
-        
-        
-        Calling ``next()`` again returns the next country from the source:
-        
-          >>> angola = next(countries)
-          >>> print(angola.name)
-          Angola
-        
-        
-        There are all information available, which you can get from pycountry:
-        
-          >>> print(afghanistan.alpha_2)
-          AF
-          >>> print(afghanistan.alpha_3)
-          AFG
-          >>> print(afghanistan.numeric)
-          004
-          >>> print(afghanistan.official_name)
-          Islamic Republic of Afghanistan
-        
-        
-        To reduce the amount of results you can provide a list or tuple of countries
-        you like to have in your source:
-        
-          >>> countries = gocept.country.CountrySource(alpha_2=['DE', 'US'])
-          >>> print(*[countries.factory.getTitle(x) for x in countries], sep=', ')
-          Germany, United States
-          >>> print(*[countries.factory.getToken(x) for x in countries], sep=', ')
-          DE, US
-        
-        Please note, that the result items are sorted by *alpha_2* code. Please also
-        note, that you can provide alpha_3 and numeric codes and names resp.
-        official_names to reduce the amount of result items, too:
-        
-          >>> len(list(gocept.country.CountrySource())) > 200
-          True
-          >>> len(list(gocept.country.CountrySource(alpha_2=['DE', 'US', 'GB'])))
-          3
-          >>> len(list(gocept.country.CountrySource(alpha_3=['DEU', 'USA'])))
-          2
-          >>> len(list(gocept.country.CountrySource(numeric=['276', ])))
-          1
-          >>> countries_list = ['Germany', 'Italy', 'Poland', 'France']
-          >>> len(list(gocept.country.CountrySource(name=countries_list)))
-          4
-        
-        
-        Providing codes, which are not present, does not result in an exception but
-        in an empty list:
-        
-          >>> len(list(gocept.country.CountrySource(capital=['Berlin', 'Paris'])))
-          0
-        
-        ISO 3166-2 Country subdivisions
-        ===============================
-        
-        Context free source
-        -------------------
-        
-        Country subdivisions are similar to countries:
-        
-          >>> subdivisions_field = zope.schema.Choice(
-          ...     title=u'Country subdivisions', source=gocept.country.subdivisions)
-          >>> subdivisions = iter(subdivisions_field.source)
-        
-          >>> canillo = next(subdivisions)
-          >>> print(canillo.name)
-          Canillo
-          >>> print(canillo.code)
-          AD-02
-        
-          >>> encamp = next(subdivisions)
-          >>> print(encamp.name)
-          Encamp
-          >>> print(encamp.code)
-          AD-03
-          >>> print(gocept.country.subdivisions.factory.getToken(encamp))
-          AD-03
-        
-        Please note, that the result items are sorted by their *code*. Please
-        also note, that you can provide names and numeric codes to reduce the
-        amount of result items, too.
-        
-          >>> len(list(gocept.country.SubdivisionSource())) > 4000
-          True
-          >>> len(list(gocept.country.SubdivisionSource(code=['DE-ST', 'US-WA'])))
-          2
-          >>> len(list(gocept.country.SubdivisionSource(country_code=['DE'])))
-          16
-          >>> print(*[x.name
-          ...         for x in gocept.country.SubdivisionSource(country_code=['DE'])][3:5],
-          ...       sep=', ')
-          Bayern, Bremen
-          >>> len(list(gocept.country.SubdivisionSource(name=[u'Bayern', u'Bremen'])))
-          2
-        
-        Contextual source
-        -----------------
-        
-        There is also a contextual source for country subdivisions which
-        depends on a country. Let's set up a context object first:
-        
-          >>> import zope.interface
-          >>> class IAddress(zope.interface.Interface):
-          ...     country = zope.interface.Attribute("The country of the address.")
-          ...     subdivision = zope.schema.Choice(
-          ...         title=u'Country subdivisions',
-          ...         source=gocept.country.contextual_subdivisions)
-        
-          >>> @zope.interface.implementer(IAddress)
-          ... class Address(object):
-          ...     pass
-          >>> address = Address()
-          >>> address.country = gocept.country.db.Country('DE')
-        
-        The contextual source expects an adapter between the context and
-        ``gocept.country.interfaces.ICountry``:
-        
-          >>> import zope.component
-          >>> import gocept.country.interfaces
-          >>> def get_country(context):
-          ...     return context.country
-          >>> zope.component.provideAdapter(
-          ...    get_country, (IAddress, ), gocept.country.interfaces.ICountry)
-        
-          >>> print(gocept.country.interfaces.ICountry(address).name)
-          Germany
-        
-        So the source contains only the country subdivisions belonging to the
-        country:
-        
-          >>> len(list(iter(gocept.country.contextual_subdivisions(address))))
-          16
-          >>> print(*[x.name
-          ...         for x in iter(gocept.country.contextual_subdivisions(address))][3:5],
-          ...       sep=', ')
-          Bayern, Bremen
-        
-        Changing the country changes also the subdivisions:
-        
-          >>> address.country = gocept.country.db.Country('CH')
-          >>> len(list(iter(gocept.country.contextual_subdivisions(address))))
-          26
-          >>> print(*[x.name
-          ...         for x in iter(gocept.country.contextual_subdivisions(address))],
-          ...       sep=', ')
-          Aargau, Appenzell Innerrhoden, ...
-          >>> print(*[x.code
-          ...         for x in iter(gocept.country.contextual_subdivisions(address))],
-          ...       sep=', ')
-          CH-AG, CH-AI, ...
-          >>> print(*[gocept.country.contextual_subdivisions.factory.getToken(address, x)
-          ...         for x in iter(gocept.country.contextual_subdivisions(address))],
-          ...       sep=', ')
-          CH-AG, CH-AI, ...
-        
-          >>> print(gocept.country.contextual_subdivisions.factory.getTitle(
-          ...     address, gocept.country.db.Subdivision('CH-AG')))
-          Aargau
-        
-        If the country is not set there are no subdivisions:
-        
-          >>> address.country = None
-          >>> len(list(iter(gocept.country.contextual_subdivisions(address))))
-          0
-          >>> list(iter(gocept.country.contextual_subdivisions(address)))
-          []
-        
-        
-        ISO 15924 Scripts
-        =================
-        
-        Scripts are similar to countries:
-        
-          >>> scripts_field = zope.schema.Choice(title=u'Script',
-          ...                            source=gocept.country.scripts)
-          >>> scripts = iter(scripts_field.source)
-        
-        
-          >>> adlam = next(scripts)
-          >>> print(adlam.name)
-          Adlam
-        
-          >>> afaka = next(scripts)
-          >>> print(afaka.name)
-          Afaka
-          >>> print(gocept.country.scripts.factory.getToken(afaka))
-          Afak
-        
-        
-        Please note, that the result items are sorted by *alpha_4* code. Please also
-        note, that you can provide names and numeric codes to smaller the amount of
-        result items, too.
-        
-          >>> len(list(gocept.country.ScriptSource())) > 130
-          True
-          >>> len(list(gocept.country.ScriptSource(alpha_4=['Arab', 'Latn'])))
-          2
-          >>> len(list(gocept.country.ScriptSource(numeric=['215', ])))
-          1
-          >>> len(list(gocept.country.ScriptSource(name=['Arabic', 'Latin'])))
-          2
-        
-        
-        ISO 4217 Currencies
-        ===================
-        
-        Currencies are similar to the ones before:
-        
-          >>> currencies_field = zope.schema.Choice(title=u'Currency',
-          ...                            source=gocept.country.currencies)
-        
-          >>> currencies = iter(currencies_field.source)
-        
-          >>> dirham = next(currencies)
-          >>> print(dirham.name)
-          UAE Dirham
-        
-          >>> afghani = next(currencies)
-          >>> print(afghani.name)
-          Afghani
-          >>> print(gocept.country.currencies.factory.getToken(afghani))
-          AFN
-        
-        Please note, that the result items are sorted by *alpha_3* code. Please also
-        note, that you can provide names and numeric codes to reduce the amount of
-        result items, too.
-        
-          >>> len(list(gocept.country.CurrencySource())) >= 170
-          True
-          >>> len(list(gocept.country.CurrencySource(alpha_3=['ARS', 'AED', 'AFN'])))
-          3
-          >>> len(list(gocept.country.CurrencySource(numeric=['032', '784'])))
-          2
-          >>> len(list(gocept.country.CurrencySource(name=['Afghani', ])))
-          1
-        
-        
-        ISO 639 Languages
-        =================
-        
-        Languages are similar, too:
-        
-          >>> languages_field = zope.schema.Choice(title=u'Language',
-          ...                            source=gocept.country.languages)
-        
-          >>> languages = iter(languages_field.source)
-        
-          >>> ghotuo = next(languages)
-          >>> print(ghotuo.name)
-          Ghotuo
-        
-          >>> alumu_tesu = next(languages)
-          >>> print(alumu_tesu.name)
-          Alumu-Tesu
-          >>> print(gocept.country.languages.factory.getToken(alumu_tesu))
-          aab
-        
-        Please note, that the result items are sorted by *alpha_3*. Please also
-        note, that you can provide names to reduce the amount of result items, too.
-        
-          >>> len(list(gocept.country.LanguageSource())) > 480
-          True
-          >>> len(list(gocept.country.LanguageSource(alpha_3=['eng', 'deu'])))
-          2
-          >>> len(list(gocept.country.LanguageSource(name=['English', 'German'])))
-          2
-        
-        
-        Translations
-        ============
-        
-        
-        First we fetch a specific country:
-        
-          >>> countries = list(iter(countries_field.source))
-          >>> germany = [x for x in countries if x.name == u'Germany'][0]
-        
-        
-        The i18n translate method translates 'Germany' into German:
-        
-          >>> print(zope.i18n.translate(germany.name, target_language='de'))
-          Deutschland
-        
-        
-        There are also translations for scripts, currencies and languages.
-        
-        
-        Comparison
-        ==========
-        
-        
-        Countries, scripts, currencies and languages can be compared to equality. To
-        test this, we will need another country object ``afghanistan``, which is not
-        the *same* object as retrieved before:
-        
-        
-          >>> afghanistan = next(iter(gocept.country.CountrySource(alpha_2=['AF'])))
-          >>> afghanistan2 = next(iter(gocept.country.CountrySource(alpha_2=['AF'])))
-        
-          >>> str(afghanistan) == str(afghanistan2)
-          False
-        
-        
-        Comparing them will get the token for each and compare it:
-        
-          >>> afghanistan == afghanistan2
-          True
-          >>> afghanistan != afghanistan2
-          False
-          >>> afghanistan != germany
-          True
-          >>> afghanistan == germany
-          False
-        
-        
-        Comparing with an instance of another class always returns False:
-        
-          >>> afghanistan == None
-          False
-          >>> afghanistan != None
-          True
-          >>> afghanistan == object()
-          False
-          >>> afghanistan != object()
-          True
-        
-        
-        Pickling and unpickling
-        =======================
-        
-        
-        It should be possible to store "proxy objects" in a database (like the ZODB).
-        Therefore, they have to be pickleable:
-        
-          >>> from io import BytesIO
-          >>> import pickle
-          >>> f = BytesIO(b'')
-        
-        Pickling a country should never raise an error...
-        
-          >>> pickle.dump(afghanistan, f)
-        
-        
-        ... and results in storing the token in the pickle:
-        
-          >>> ignored = f.seek(0)
-          >>> b'AF' in f.read()
-          True
-        
-        
-        Reading the pickle again will return the same country which was pickled
-        before:
-        
-          >>> ignored = f.seek(0)
-          >>> afghanistan2 = pickle.load(f)
-          >>> afghanistan2 == afghanistan
-          True
-          >>> print(afghanistan2.name)
-          Afghanistan
-        
-        
-        Changes
-        =======
-        
-        2.1 (2019-09-30)
-        ----------------
-        
-        - Support Python 3.5 up to 3.8, PyPy and PyPy3.
-        
-        - Replace test dependency on `zope.app.testing` by `zope.app.wsgi[testlayer]`.
-        
-        - Migrate to Github.
-        
-        
-        2.0 (2017-01-21)
-        ----------------
-        
-        - Update to ``pycountry >= 16.x``.
-        
-        - Drop support for Python 2.6.
-        
-        - Bring test coverage to 100 %.
-        
-        - Change testrunner to py.test.
-        
-        
-        1.0 (2015-08-05)
-        ----------------
-        
-        - Update to ``pycountry 1.12`` thus adding support for ISO 639 3, dropping the
-          old ISO 639 support.
-        
-        
-        0.6.5 (2015-08-05)
-        ------------------
-        
-        - Move repos to https://bitbucket.org/gocept/gocept.country
-        
-        0.6.4 (2008-10-21)
-        ------------------
-        
-        - Bugfix: declared namespace package in setup.py
-        
-        0.6.3 (2008-10-14)
-        ------------------
-        
-        - Bugfix: added not-equal compare method for db objects
-        
-        0.6.2 (2008-10-13)
-        ------------------
-        
-        - Added security declarations for token.
-        - Bugfix in comparison of db objects, where `isinstance` returns False
-          for objects of the same type
-        
-        0.6.1 (2008-09-13)
-        ------------------
-        
-        - Bugfix in countextual subdivision source: parameters of some methods
-          where in wrong order.
-        
-        0.6 (2008-09-12)
-        ----------------
-        
-        - Added contextual country subdivision source, so country subdivisions
-          can depend on the country.
-        
-        
-        0.5 (2008-09-11)
-        ----------------
-        
-        - Added support for country subdivisions.
-        
-        0.4.2 (2008-09-10)
-        ------------------
-        
-        - Added security declarations for tokens.
-        
-        0.4.1 (2008-09-10)
-        ------------------
-        
-        - Fixed bug in token comparison.
-        
-        0.4 (2008-06-10)
-        ----------------
-        
-        - added possibility to smaller the amount of results generated by the
-          sourcefactory
-        
-        
-        0.3 (2008-05-21)
-        ----------------
-        
-        - added test for comparing the returned countries to equality
-        - added __reduce__ to data objects so that they can be pickled
-        - added tests for pickling and unpickling data objects
-        
-        
-        0.2 (2008-05-20)
-        ----------------
-        
-        - gocept.country now returns special data objects instead of pycountry
-          objects for a better object-oriented purpose and flexibility in handling the
-          result
-        - improved configure.zcml and added functional tests for the i18n translations
-        - improved test cases in general
-        
-        0.1 (2008-05-20)
-        ----------------
-        
-        - initial release
-        
-        Contributors
-        ============
-        
-        - Michael Howitz <mh at gocept dot com>
-        
-        
 Keywords: country subdivision language currency iso 3166 639 4217 15924 3166-2 zope pycountry
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
+Requires-Python: >=3.7
 Provides-Extra: test
+License-File: LICENSE.txt
+
+Copyright (c) 2008-2015 gocept gmbh & co. kg
+
+All Rights Reserved.
+
+This software is subject to the provisions of the Zope Public License,
+Version 2.1 (ZPL). A copy of the ZPL should accompany this distribution.
+THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
+WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
+FOR A PARTICULAR PURPOSE.
+
+
+==============
+gocept.country
+==============
+
+.. image:: https://github.com/gocept/gocept.country/workflows/tests/badge.svg
+    :target: https://github.com/gocept/gocept.country/actions?query=workflow%3Atests
+.. image:: https://coveralls.io/repos/github/gocept/gocept.country/badge.svg?branch=master
+    :target: https://coveralls.io/github/gocept/gocept.country?branch=master
+
+
+This package lets you use the `pycountry database
+<http://pypi.python.org/pypi/pycountry/>`_ within Zope 3.
+
+
+In practice, this means e.g., that you can easily get a zope.schema.Choice
+field to provide a full list of iso 3166 country codes.
+
+For more information about the database please refer to the
+`pycountry product <http://pypi.python.org/pypi/pycountry/>`_.
+
+.. contents::
+
+
+Introduction
+============
+
+`gocept.country` provides Zope 3 sources for the pycountry databases. You can
+use it e.g. to get a ``zope.schema.Choice`` field with all ISO 3166 countries.
+
+  >>> import gocept.country
+  >>> import gocept.country.db
+  >>> import zope.schema
+
+
+ISO 3166 Countries
+==================
+
+To get a list of ISO 3166 countries in a web form, you can use the
+``zope.schema.Choice`` field and provide the gocept.country.countries as
+source:
+
+  >>> countries_field = zope.schema.Choice(title=u'Country',
+  ...                            source=gocept.country.countries)
+  >>> countries_field
+  <zope.schema._field.Choice object at 0x...>
+  >>> countries = iter(countries_field.source)
+
+
+The ``gocept.country.countries`` source factory returns Country objects as
+values, which use the values from pycountry:
+
+  >>> aruba = next(countries)
+  >>> afghanistan = next(countries)
+  >>> afghanistan
+  <gocept.country.db.Country object at 0x...>
+  >>> print(afghanistan.name)
+  Afghanistan
+
+
+Calling ``next()`` again returns the next country from the source:
+
+  >>> angola = next(countries)
+  >>> print(angola.name)
+  Angola
+
+
+There are all information available, which you can get from pycountry:
+
+  >>> print(afghanistan.alpha_2)
+  AF
+  >>> print(afghanistan.alpha_3)
+  AFG
+  >>> print(afghanistan.numeric)
+  004
+  >>> print(afghanistan.official_name)
+  Islamic Republic of Afghanistan
+
+
+To reduce the amount of results you can provide a list or tuple of countries
+you like to have in your source:
+
+  >>> countries = gocept.country.CountrySource(alpha_2=['DE', 'US'])
+  >>> print(*[countries.factory.getTitle(x) for x in countries], sep=', ')
+  Germany, United States
+  >>> print(*[countries.factory.getToken(x) for x in countries], sep=', ')
+  DE, US
+
+Please note, that the result items are sorted by *alpha_2* code. Please also
+note, that you can provide alpha_3 and numeric codes and names resp.
+official_names to reduce the amount of result items, too:
+
+  >>> len(list(gocept.country.CountrySource())) > 200
+  True
+  >>> len(list(gocept.country.CountrySource(alpha_2=['DE', 'US', 'GB'])))
+  3
+  >>> len(list(gocept.country.CountrySource(alpha_3=['DEU', 'USA'])))
+  2
+  >>> len(list(gocept.country.CountrySource(numeric=['276', ])))
+  1
+  >>> countries_list = ['Germany', 'Italy', 'Poland', 'France']
+  >>> len(list(gocept.country.CountrySource(name=countries_list)))
+  4
+
+
+Providing codes, which are not present, does not result in an exception but
+in an empty list:
+
+  >>> len(list(gocept.country.CountrySource(capital=['Berlin', 'Paris'])))
+  0
+
+ISO 3166-2 Country subdivisions
+===============================
+
+Context free source
+-------------------
+
+Country subdivisions are similar to countries:
+
+  >>> subdivisions_field = zope.schema.Choice(
+  ...     title=u'Country subdivisions', source=gocept.country.subdivisions)
+  >>> subdivisions = iter(subdivisions_field.source)
+
+  >>> canillo = next(subdivisions)
+  >>> print(canillo.name)
+  Canillo
+  >>> print(canillo.code)
+  AD-02
+
+  >>> encamp = next(subdivisions)
+  >>> print(encamp.name)
+  Encamp
+  >>> print(encamp.code)
+  AD-03
+  >>> print(gocept.country.subdivisions.factory.getToken(encamp))
+  AD-03
+
+Please note, that the result items are sorted by their *code*. Please
+also note, that you can provide names and numeric codes to reduce the
+amount of result items, too.
+
+  >>> len(list(gocept.country.SubdivisionSource())) > 4000
+  True
+  >>> len(list(gocept.country.SubdivisionSource(code=['DE-ST', 'US-WA'])))
+  2
+  >>> len(list(gocept.country.SubdivisionSource(country_code=['DE'])))
+  16
+  >>> print(*[x.name
+  ...         for x in gocept.country.SubdivisionSource(country_code=['DE'])][3:5],
+  ...       sep=', ')
+  Bayern, Bremen
+  >>> len(list(gocept.country.SubdivisionSource(name=[u'Bayern', u'Bremen'])))
+  2
+
+Contextual source
+-----------------
+
+There is also a contextual source for country subdivisions which
+depends on a country. Let's set up a context object first:
+
+  >>> import zope.interface
+  >>> class IAddress(zope.interface.Interface):
+  ...     country = zope.interface.Attribute("The country of the address.")
+  ...     subdivision = zope.schema.Choice(
+  ...         title=u'Country subdivisions',
+  ...         source=gocept.country.contextual_subdivisions)
+
+  >>> @zope.interface.implementer(IAddress)
+  ... class Address(object):
+  ...     pass
+  >>> address = Address()
+  >>> address.country = gocept.country.db.Country('DE')
+
+The contextual source expects an adapter between the context and
+``gocept.country.interfaces.ICountry``:
+
+  >>> import zope.component
+  >>> import gocept.country.interfaces
+  >>> def get_country(context):
+  ...     return context.country
+  >>> zope.component.provideAdapter(
+  ...    get_country, (IAddress, ), gocept.country.interfaces.ICountry)
+
+  >>> print(gocept.country.interfaces.ICountry(address).name)
+  Germany
+
+So the source contains only the country subdivisions belonging to the
+country:
+
+  >>> len(list(iter(gocept.country.contextual_subdivisions(address))))
+  16
+  >>> print(*[x.name
+  ...         for x in iter(gocept.country.contextual_subdivisions(address))][3:5],
+  ...       sep=', ')
+  Bayern, Bremen
+
+Changing the country changes also the subdivisions:
+
+  >>> address.country = gocept.country.db.Country('CH')
+  >>> len(list(iter(gocept.country.contextual_subdivisions(address))))
+  26
+  >>> print(*[x.name
+  ...         for x in iter(gocept.country.contextual_subdivisions(address))],
+  ...       sep=', ')
+  Aargau, Appenzell Innerrhoden, ...
+  >>> print(*[x.code
+  ...         for x in iter(gocept.country.contextual_subdivisions(address))],
+  ...       sep=', ')
+  CH-AG, CH-AI, ...
+  >>> print(*[gocept.country.contextual_subdivisions.factory.getToken(address, x)
+  ...         for x in iter(gocept.country.contextual_subdivisions(address))],
+  ...       sep=', ')
+  CH-AG, CH-AI, ...
+
+  >>> print(gocept.country.contextual_subdivisions.factory.getTitle(
+  ...     address, gocept.country.db.Subdivision('CH-AG')))
+  Aargau
+
+If the country is not set there are no subdivisions:
+
+  >>> address.country = None
+  >>> len(list(iter(gocept.country.contextual_subdivisions(address))))
+  0
+  >>> list(iter(gocept.country.contextual_subdivisions(address)))
+  []
+
+
+ISO 15924 Scripts
+=================
+
+Scripts are similar to countries:
+
+  >>> scripts_field = zope.schema.Choice(title=u'Script',
+  ...                            source=gocept.country.scripts)
+  >>> scripts = iter(scripts_field.source)
+
+
+  >>> adlam = next(scripts)
+  >>> print(adlam.name)
+  Adlam
+
+  >>> afaka = next(scripts)
+  >>> print(afaka.name)
+  Afaka
+  >>> print(gocept.country.scripts.factory.getToken(afaka))
+  Afak
+
+
+Please note, that the result items are sorted by *alpha_4* code. Please also
+note, that you can provide names and numeric codes to smaller the amount of
+result items, too.
+
+  >>> len(list(gocept.country.ScriptSource())) > 130
+  True
+  >>> len(list(gocept.country.ScriptSource(alpha_4=['Arab', 'Latn'])))
+  2
+  >>> len(list(gocept.country.ScriptSource(numeric=['215', ])))
+  1
+  >>> len(list(gocept.country.ScriptSource(name=['Arabic', 'Latin'])))
+  2
+
+
+ISO 4217 Currencies
+===================
+
+Currencies are similar to the ones before:
+
+  >>> currencies_field = zope.schema.Choice(title=u'Currency',
+  ...                            source=gocept.country.currencies)
+
+  >>> currencies = iter(currencies_field.source)
+
+  >>> dirham = next(currencies)
+  >>> print(dirham.name)
+  UAE Dirham
+
+  >>> afghani = next(currencies)
+  >>> print(afghani.name)
+  Afghani
+  >>> print(gocept.country.currencies.factory.getToken(afghani))
+  AFN
+
+Please note, that the result items are sorted by *alpha_3* code. Please also
+note, that you can provide names and numeric codes to reduce the amount of
+result items, too.
+
+  >>> len(list(gocept.country.CurrencySource())) >= 170
+  True
+  >>> len(list(gocept.country.CurrencySource(alpha_3=['ARS', 'AED', 'AFN'])))
+  3
+  >>> len(list(gocept.country.CurrencySource(numeric=['032', '784'])))
+  2
+  >>> len(list(gocept.country.CurrencySource(name=['Afghani', ])))
+  1
+
+
+ISO 639 Languages
+=================
+
+Languages are similar, too:
+
+  >>> languages_field = zope.schema.Choice(title=u'Language',
+  ...                            source=gocept.country.languages)
+
+  >>> languages = iter(languages_field.source)
+
+  >>> ghotuo = next(languages)
+  >>> print(ghotuo.name)
+  Ghotuo
+
+  >>> alumu_tesu = next(languages)
+  >>> print(alumu_tesu.name)
+  Alumu-Tesu
+  >>> print(gocept.country.languages.factory.getToken(alumu_tesu))
+  aab
+
+Please note, that the result items are sorted by *alpha_3*. Please also
+note, that you can provide names to reduce the amount of result items, too.
+
+  >>> len(list(gocept.country.LanguageSource())) > 480
+  True
+  >>> len(list(gocept.country.LanguageSource(alpha_3=['eng', 'deu'])))
+  2
+  >>> len(list(gocept.country.LanguageSource(name=['English', 'German'])))
+  2
+
+
+Translations
+============
+
+
+First we fetch a specific country:
+
+  >>> countries = list(iter(countries_field.source))
+  >>> germany = [x for x in countries if x.name == u'Germany'][0]
+
+
+The i18n translate method translates 'Germany' into German:
+
+  >>> print(zope.i18n.translate(germany.name, target_language='de'))
+  Deutschland
+
+
+There are also translations for scripts, currencies and languages.
+
+
+Comparison
+==========
+
+
+Countries, scripts, currencies and languages can be compared to equality. To
+test this, we will need another country object ``afghanistan``, which is not
+the *same* object as retrieved before:
+
+
+  >>> afghanistan = next(iter(gocept.country.CountrySource(alpha_2=['AF'])))
+  >>> afghanistan2 = next(iter(gocept.country.CountrySource(alpha_2=['AF'])))
+
+  >>> str(afghanistan) == str(afghanistan2)
+  False
+
+
+Comparing them will get the token for each and compare it:
+
+  >>> afghanistan == afghanistan2
+  True
+  >>> afghanistan != afghanistan2
+  False
+  >>> afghanistan != germany
+  True
+  >>> afghanistan == germany
+  False
+
+
+Comparing with an instance of another class always returns False:
+
+  >>> afghanistan == None
+  False
+  >>> afghanistan != None
+  True
+  >>> afghanistan == object()
+  False
+  >>> afghanistan != object()
+  True
+
+
+Pickling and unpickling
+=======================
+
+
+It should be possible to store "proxy objects" in a database (like the ZODB).
+Therefore, they have to be pickleable:
+
+  >>> from io import BytesIO
+  >>> import pickle
+  >>> f = BytesIO(b'')
+
+Pickling a country should never raise an error...
+
+  >>> pickle.dump(afghanistan, f)
+
+
+... and results in storing the token in the pickle:
+
+  >>> ignored = f.seek(0)
+  >>> b'AF' in f.read()
+  True
+
+
+Reading the pickle again will return the same country which was pickled
+before:
+
+  >>> ignored = f.seek(0)
+  >>> afghanistan2 = pickle.load(f)
+  >>> afghanistan2 == afghanistan
+  True
+  >>> print(afghanistan2.name)
+  Afghanistan
+
+
+Changes
+=======
+
+3.0 (2023-07-14)
+----------------
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.9, 3.10, 3.11.
+
+
+2.1 (2019-09-30)
+----------------
+
+- Add support for Python 3.5 up to 3.8, PyPy and PyPy3.
+
+- Replace test dependency on `zope.app.testing` by `zope.app.wsgi[testlayer]`.
+
+- Migrate to Github.
+
+
+2.0 (2017-01-21)
+----------------
+
+- Update to ``pycountry >= 16.x``.
+
+- Drop support for Python 2.6.
+
+- Bring test coverage to 100 %.
+
+- Change testrunner to py.test.
+
+
+1.0 (2015-08-05)
+----------------
+
+- Update to ``pycountry 1.12`` thus adding support for ISO 639 3, dropping the
+  old ISO 639 support.
+
+
+0.6.5 (2015-08-05)
+------------------
+
+- Move repos to https://bitbucket.org/gocept/gocept.country
+
+0.6.4 (2008-10-21)
+------------------
+
+- Bugfix: declared namespace package in setup.py
+
+0.6.3 (2008-10-14)
+------------------
+
+- Bugfix: added not-equal compare method for db objects
+
+0.6.2 (2008-10-13)
+------------------
+
+- Added security declarations for token.
+- Bugfix in comparison of db objects, where `isinstance` returns False
+  for objects of the same type
+
+0.6.1 (2008-09-13)
+------------------
+
+- Bugfix in countextual subdivision source: parameters of some methods
+  where in wrong order.
+
+0.6 (2008-09-12)
+----------------
+
+- Added contextual country subdivision source, so country subdivisions
+  can depend on the country.
+
+
+0.5 (2008-09-11)
+----------------
+
+- Added support for country subdivisions.
+
+0.4.2 (2008-09-10)
+------------------
+
+- Added security declarations for tokens.
+
+0.4.1 (2008-09-10)
+------------------
+
+- Fixed bug in token comparison.
+
+0.4 (2008-06-10)
+----------------
+
+- added possibility to smaller the amount of results generated by the
+  sourcefactory
+
+
+0.3 (2008-05-21)
+----------------
+
+- added test for comparing the returned countries to equality
+- added __reduce__ to data objects so that they can be pickled
+- added tests for pickling and unpickling data objects
+
+
+0.2 (2008-05-20)
+----------------
+
+- gocept.country now returns special data objects instead of pycountry
+  objects for a better object-oriented purpose and flexibility in handling the
+  result
+- improved configure.zcml and added functional tests for the i18n translations
+- improved test cases in general
+
+0.1 (2008-05-20)
+----------------
+
+- initial release
+
+Contributors
+============
+
+- Michael Howitz <mh at gocept dot com>
```

### Comparing `gocept.country-2.1/README.rst` & `gocept.country-3.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-.. image:: https://travis-ci.com/gocept/gocept.country.svg?branch=master
-    :target: https://travis-ci.com/gocept/gocept.country
-    
+==============
+gocept.country
+==============
+
+.. image:: https://github.com/gocept/gocept.country/workflows/tests/badge.svg
+    :target: https://github.com/gocept/gocept.country/actions?query=workflow%3Atests
 .. image:: https://coveralls.io/repos/github/gocept/gocept.country/badge.svg?branch=master
     :target: https://coveralls.io/github/gocept/gocept.country?branch=master
 
 
 This package lets you use the `pycountry database
 <http://pypi.python.org/pypi/pycountry/>`_ within Zope 3.
```

### Comparing `gocept.country-2.1/setup.py` & `gocept.country-3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# vim:fileencoding=utf-8
+from setuptools import find_packages
+from setuptools import setup
 import os.path
-from setuptools import setup, find_packages
 
 
 def read(*rnames):
     """Read a file from a path."""
     with open(os.path.join(os.curdir, *rnames)) as f:
         return f.read()
 
+
 setup(
     name='gocept.country',
-    version='2.1',
+    version='3.0',
     author='gocept gmbh & co. kg',
     author_email='mail@gocept.com',
     description='Zope 3 sources for pycountry databases',
     long_description='\n\n'.join([
         read('COPYRIGHT.txt'),
         read('README.rst'),
         read('src', 'gocept', 'country', 'README.txt'),
@@ -27,30 +28,31 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Natural Language :: English',
         'Operating System :: OS Independent',
-        'Topic :: Internet :: WWW/HTTP'],
+        'Topic :: Internet :: WWW/HTTP',
+    ],
     url='https://github.com/gocept/gocept.country',
     packages=find_packages('src'),
     include_package_data=True,
     package_dir={'': 'src'},
+    python_requires='>=3.7',
     install_requires=['setuptools',
                       'pycountry >= 16.0',
                       'zope.i18nmessageid',
                       'zc.sourcefactory>=0.3.3',
                       'zope.deferredimport'],
     extras_require=dict(
         test=['zope.testing',
```

### Comparing `gocept.country-2.1/src/gocept/country/README.txt` & `gocept.country-3.0/src/gocept/country/README.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-==============
-gocept.country
-==============
-
+Introduction
+============
 
 `gocept.country` provides Zope 3 sources for the pycountry databases. You can
 use it e.g. to get a ``zope.schema.Choice`` field with all ISO 3166 countries.
 
   >>> import gocept.country
   >>> import gocept.country.db
   >>> import zope.schema
```

### Comparing `gocept.country-2.1/src/gocept/country/configure.zcml` & `gocept.country-3.0/src/gocept/country/configure.zcml`

 * *Files identical despite different names*

### Comparing `gocept.country-2.1/src/gocept/country/db.py` & `gocept.country-3.0/src/gocept/country/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: latin-1 -*-
 # Copyright (c) 2008-2009 gocept gmbh & co. kg
 # See also LICENSE.txt
 # $Id$
 
 import gocept.country.interfaces
 import pycountry
 import zope.i18nmessageid
@@ -12,15 +11,15 @@
 iso3166msg = zope.i18nmessageid.MessageFactory('iso3166')
 iso3166_2msg = zope.i18nmessageid.MessageFactory('iso3166_2')
 iso15924msg = zope.i18nmessageid.MessageFactory('iso15924')
 iso4217msg = zope.i18nmessageid.MessageFactory('iso4217')
 iso639msg = zope.i18nmessageid.MessageFactory('iso639')
 
 
-class Data(object):
+class Data:
     """ """
 
     def __init__(self, token):
         self.token = token
 
     def __eq__(self, other):
         if not other:
```

### Comparing `gocept.country-2.1/src/gocept/country/sources.py` & `gocept.country-3.0/src/gocept/country/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# -*- coding: latin-1 -*-
 import gocept.country.db
 import gocept.country.interfaces
 import pycountry
 import zc.sourcefactory.basic
 import zc.sourcefactory.contextual
 import zope.component
 
 
 class BasicSource(zc.sourcefactory.basic.BasicSourceFactory):
     """A basic source for countries, scripts, languages and currencies."""
 
     def __init__(self, **kw):
-        super(BasicSource, self).__init__()
+        super().__init__()
         self.filter = kw
 
     def __contains__(self, item):
         for token, values in self.filter.items():
             if (getattr(item, token, None) not in values):
                 return False
         return True
```

### Comparing `gocept.country-2.1/src/gocept.country.egg-info/PKG-INFO` & `gocept.country-3.0/src/gocept.country.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,576 +1,584 @@
 Metadata-Version: 2.1
 Name: gocept.country
-Version: 2.1
+Version: 3.0
 Summary: Zope 3 sources for pycountry databases
 Home-page: https://github.com/gocept/gocept.country
 Author: gocept gmbh & co. kg
 Author-email: mail@gocept.com
 License: ZPL 2.1
-Description: Copyright (c) 2008-2015 gocept gmbh & co. kg
-        
-        All Rights Reserved.
-        
-        This software is subject to the provisions of the Zope Public License,
-        Version 2.1 (ZPL). A copy of the ZPL should accompany this distribution.
-        THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
-        WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-        WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
-        FOR A PARTICULAR PURPOSE.
-        
-        
-        .. image:: https://travis-ci.com/gocept/gocept.country.svg?branch=master
-            :target: https://travis-ci.com/gocept/gocept.country
-            
-        .. image:: https://coveralls.io/repos/github/gocept/gocept.country/badge.svg?branch=master
-            :target: https://coveralls.io/github/gocept/gocept.country?branch=master
-        
-        
-        This package lets you use the `pycountry database
-        <http://pypi.python.org/pypi/pycountry/>`_ within Zope 3.
-        
-        
-        In practice, this means e.g., that you can easily get a zope.schema.Choice
-        field to provide a full list of iso 3166 country codes.
-        
-        For more information about the database please refer to the
-        `pycountry product <http://pypi.python.org/pypi/pycountry/>`_.
-        
-        .. contents::
-        
-        
-        ==============
-        gocept.country
-        ==============
-        
-        
-        `gocept.country` provides Zope 3 sources for the pycountry databases. You can
-        use it e.g. to get a ``zope.schema.Choice`` field with all ISO 3166 countries.
-        
-          >>> import gocept.country
-          >>> import gocept.country.db
-          >>> import zope.schema
-        
-        
-        ISO 3166 Countries
-        ==================
-        
-        To get a list of ISO 3166 countries in a web form, you can use the
-        ``zope.schema.Choice`` field and provide the gocept.country.countries as
-        source:
-        
-          >>> countries_field = zope.schema.Choice(title=u'Country',
-          ...                            source=gocept.country.countries)
-          >>> countries_field
-          <zope.schema._field.Choice object at 0x...>
-          >>> countries = iter(countries_field.source)
-        
-        
-        The ``gocept.country.countries`` source factory returns Country objects as
-        values, which use the values from pycountry:
-        
-          >>> aruba = next(countries)
-          >>> afghanistan = next(countries)
-          >>> afghanistan
-          <gocept.country.db.Country object at 0x...>
-          >>> print(afghanistan.name)
-          Afghanistan
-        
-        
-        Calling ``next()`` again returns the next country from the source:
-        
-          >>> angola = next(countries)
-          >>> print(angola.name)
-          Angola
-        
-        
-        There are all information available, which you can get from pycountry:
-        
-          >>> print(afghanistan.alpha_2)
-          AF
-          >>> print(afghanistan.alpha_3)
-          AFG
-          >>> print(afghanistan.numeric)
-          004
-          >>> print(afghanistan.official_name)
-          Islamic Republic of Afghanistan
-        
-        
-        To reduce the amount of results you can provide a list or tuple of countries
-        you like to have in your source:
-        
-          >>> countries = gocept.country.CountrySource(alpha_2=['DE', 'US'])
-          >>> print(*[countries.factory.getTitle(x) for x in countries], sep=', ')
-          Germany, United States
-          >>> print(*[countries.factory.getToken(x) for x in countries], sep=', ')
-          DE, US
-        
-        Please note, that the result items are sorted by *alpha_2* code. Please also
-        note, that you can provide alpha_3 and numeric codes and names resp.
-        official_names to reduce the amount of result items, too:
-        
-          >>> len(list(gocept.country.CountrySource())) > 200
-          True
-          >>> len(list(gocept.country.CountrySource(alpha_2=['DE', 'US', 'GB'])))
-          3
-          >>> len(list(gocept.country.CountrySource(alpha_3=['DEU', 'USA'])))
-          2
-          >>> len(list(gocept.country.CountrySource(numeric=['276', ])))
-          1
-          >>> countries_list = ['Germany', 'Italy', 'Poland', 'France']
-          >>> len(list(gocept.country.CountrySource(name=countries_list)))
-          4
-        
-        
-        Providing codes, which are not present, does not result in an exception but
-        in an empty list:
-        
-          >>> len(list(gocept.country.CountrySource(capital=['Berlin', 'Paris'])))
-          0
-        
-        ISO 3166-2 Country subdivisions
-        ===============================
-        
-        Context free source
-        -------------------
-        
-        Country subdivisions are similar to countries:
-        
-          >>> subdivisions_field = zope.schema.Choice(
-          ...     title=u'Country subdivisions', source=gocept.country.subdivisions)
-          >>> subdivisions = iter(subdivisions_field.source)
-        
-          >>> canillo = next(subdivisions)
-          >>> print(canillo.name)
-          Canillo
-          >>> print(canillo.code)
-          AD-02
-        
-          >>> encamp = next(subdivisions)
-          >>> print(encamp.name)
-          Encamp
-          >>> print(encamp.code)
-          AD-03
-          >>> print(gocept.country.subdivisions.factory.getToken(encamp))
-          AD-03
-        
-        Please note, that the result items are sorted by their *code*. Please
-        also note, that you can provide names and numeric codes to reduce the
-        amount of result items, too.
-        
-          >>> len(list(gocept.country.SubdivisionSource())) > 4000
-          True
-          >>> len(list(gocept.country.SubdivisionSource(code=['DE-ST', 'US-WA'])))
-          2
-          >>> len(list(gocept.country.SubdivisionSource(country_code=['DE'])))
-          16
-          >>> print(*[x.name
-          ...         for x in gocept.country.SubdivisionSource(country_code=['DE'])][3:5],
-          ...       sep=', ')
-          Bayern, Bremen
-          >>> len(list(gocept.country.SubdivisionSource(name=[u'Bayern', u'Bremen'])))
-          2
-        
-        Contextual source
-        -----------------
-        
-        There is also a contextual source for country subdivisions which
-        depends on a country. Let's set up a context object first:
-        
-          >>> import zope.interface
-          >>> class IAddress(zope.interface.Interface):
-          ...     country = zope.interface.Attribute("The country of the address.")
-          ...     subdivision = zope.schema.Choice(
-          ...         title=u'Country subdivisions',
-          ...         source=gocept.country.contextual_subdivisions)
-        
-          >>> @zope.interface.implementer(IAddress)
-          ... class Address(object):
-          ...     pass
-          >>> address = Address()
-          >>> address.country = gocept.country.db.Country('DE')
-        
-        The contextual source expects an adapter between the context and
-        ``gocept.country.interfaces.ICountry``:
-        
-          >>> import zope.component
-          >>> import gocept.country.interfaces
-          >>> def get_country(context):
-          ...     return context.country
-          >>> zope.component.provideAdapter(
-          ...    get_country, (IAddress, ), gocept.country.interfaces.ICountry)
-        
-          >>> print(gocept.country.interfaces.ICountry(address).name)
-          Germany
-        
-        So the source contains only the country subdivisions belonging to the
-        country:
-        
-          >>> len(list(iter(gocept.country.contextual_subdivisions(address))))
-          16
-          >>> print(*[x.name
-          ...         for x in iter(gocept.country.contextual_subdivisions(address))][3:5],
-          ...       sep=', ')
-          Bayern, Bremen
-        
-        Changing the country changes also the subdivisions:
-        
-          >>> address.country = gocept.country.db.Country('CH')
-          >>> len(list(iter(gocept.country.contextual_subdivisions(address))))
-          26
-          >>> print(*[x.name
-          ...         for x in iter(gocept.country.contextual_subdivisions(address))],
-          ...       sep=', ')
-          Aargau, Appenzell Innerrhoden, ...
-          >>> print(*[x.code
-          ...         for x in iter(gocept.country.contextual_subdivisions(address))],
-          ...       sep=', ')
-          CH-AG, CH-AI, ...
-          >>> print(*[gocept.country.contextual_subdivisions.factory.getToken(address, x)
-          ...         for x in iter(gocept.country.contextual_subdivisions(address))],
-          ...       sep=', ')
-          CH-AG, CH-AI, ...
-        
-          >>> print(gocept.country.contextual_subdivisions.factory.getTitle(
-          ...     address, gocept.country.db.Subdivision('CH-AG')))
-          Aargau
-        
-        If the country is not set there are no subdivisions:
-        
-          >>> address.country = None
-          >>> len(list(iter(gocept.country.contextual_subdivisions(address))))
-          0
-          >>> list(iter(gocept.country.contextual_subdivisions(address)))
-          []
-        
-        
-        ISO 15924 Scripts
-        =================
-        
-        Scripts are similar to countries:
-        
-          >>> scripts_field = zope.schema.Choice(title=u'Script',
-          ...                            source=gocept.country.scripts)
-          >>> scripts = iter(scripts_field.source)
-        
-        
-          >>> adlam = next(scripts)
-          >>> print(adlam.name)
-          Adlam
-        
-          >>> afaka = next(scripts)
-          >>> print(afaka.name)
-          Afaka
-          >>> print(gocept.country.scripts.factory.getToken(afaka))
-          Afak
-        
-        
-        Please note, that the result items are sorted by *alpha_4* code. Please also
-        note, that you can provide names and numeric codes to smaller the amount of
-        result items, too.
-        
-          >>> len(list(gocept.country.ScriptSource())) > 130
-          True
-          >>> len(list(gocept.country.ScriptSource(alpha_4=['Arab', 'Latn'])))
-          2
-          >>> len(list(gocept.country.ScriptSource(numeric=['215', ])))
-          1
-          >>> len(list(gocept.country.ScriptSource(name=['Arabic', 'Latin'])))
-          2
-        
-        
-        ISO 4217 Currencies
-        ===================
-        
-        Currencies are similar to the ones before:
-        
-          >>> currencies_field = zope.schema.Choice(title=u'Currency',
-          ...                            source=gocept.country.currencies)
-        
-          >>> currencies = iter(currencies_field.source)
-        
-          >>> dirham = next(currencies)
-          >>> print(dirham.name)
-          UAE Dirham
-        
-          >>> afghani = next(currencies)
-          >>> print(afghani.name)
-          Afghani
-          >>> print(gocept.country.currencies.factory.getToken(afghani))
-          AFN
-        
-        Please note, that the result items are sorted by *alpha_3* code. Please also
-        note, that you can provide names and numeric codes to reduce the amount of
-        result items, too.
-        
-          >>> len(list(gocept.country.CurrencySource())) >= 170
-          True
-          >>> len(list(gocept.country.CurrencySource(alpha_3=['ARS', 'AED', 'AFN'])))
-          3
-          >>> len(list(gocept.country.CurrencySource(numeric=['032', '784'])))
-          2
-          >>> len(list(gocept.country.CurrencySource(name=['Afghani', ])))
-          1
-        
-        
-        ISO 639 Languages
-        =================
-        
-        Languages are similar, too:
-        
-          >>> languages_field = zope.schema.Choice(title=u'Language',
-          ...                            source=gocept.country.languages)
-        
-          >>> languages = iter(languages_field.source)
-        
-          >>> ghotuo = next(languages)
-          >>> print(ghotuo.name)
-          Ghotuo
-        
-          >>> alumu_tesu = next(languages)
-          >>> print(alumu_tesu.name)
-          Alumu-Tesu
-          >>> print(gocept.country.languages.factory.getToken(alumu_tesu))
-          aab
-        
-        Please note, that the result items are sorted by *alpha_3*. Please also
-        note, that you can provide names to reduce the amount of result items, too.
-        
-          >>> len(list(gocept.country.LanguageSource())) > 480
-          True
-          >>> len(list(gocept.country.LanguageSource(alpha_3=['eng', 'deu'])))
-          2
-          >>> len(list(gocept.country.LanguageSource(name=['English', 'German'])))
-          2
-        
-        
-        Translations
-        ============
-        
-        
-        First we fetch a specific country:
-        
-          >>> countries = list(iter(countries_field.source))
-          >>> germany = [x for x in countries if x.name == u'Germany'][0]
-        
-        
-        The i18n translate method translates 'Germany' into German:
-        
-          >>> print(zope.i18n.translate(germany.name, target_language='de'))
-          Deutschland
-        
-        
-        There are also translations for scripts, currencies and languages.
-        
-        
-        Comparison
-        ==========
-        
-        
-        Countries, scripts, currencies and languages can be compared to equality. To
-        test this, we will need another country object ``afghanistan``, which is not
-        the *same* object as retrieved before:
-        
-        
-          >>> afghanistan = next(iter(gocept.country.CountrySource(alpha_2=['AF'])))
-          >>> afghanistan2 = next(iter(gocept.country.CountrySource(alpha_2=['AF'])))
-        
-          >>> str(afghanistan) == str(afghanistan2)
-          False
-        
-        
-        Comparing them will get the token for each and compare it:
-        
-          >>> afghanistan == afghanistan2
-          True
-          >>> afghanistan != afghanistan2
-          False
-          >>> afghanistan != germany
-          True
-          >>> afghanistan == germany
-          False
-        
-        
-        Comparing with an instance of another class always returns False:
-        
-          >>> afghanistan == None
-          False
-          >>> afghanistan != None
-          True
-          >>> afghanistan == object()
-          False
-          >>> afghanistan != object()
-          True
-        
-        
-        Pickling and unpickling
-        =======================
-        
-        
-        It should be possible to store "proxy objects" in a database (like the ZODB).
-        Therefore, they have to be pickleable:
-        
-          >>> from io import BytesIO
-          >>> import pickle
-          >>> f = BytesIO(b'')
-        
-        Pickling a country should never raise an error...
-        
-          >>> pickle.dump(afghanistan, f)
-        
-        
-        ... and results in storing the token in the pickle:
-        
-          >>> ignored = f.seek(0)
-          >>> b'AF' in f.read()
-          True
-        
-        
-        Reading the pickle again will return the same country which was pickled
-        before:
-        
-          >>> ignored = f.seek(0)
-          >>> afghanistan2 = pickle.load(f)
-          >>> afghanistan2 == afghanistan
-          True
-          >>> print(afghanistan2.name)
-          Afghanistan
-        
-        
-        Changes
-        =======
-        
-        2.1 (2019-09-30)
-        ----------------
-        
-        - Support Python 3.5 up to 3.8, PyPy and PyPy3.
-        
-        - Replace test dependency on `zope.app.testing` by `zope.app.wsgi[testlayer]`.
-        
-        - Migrate to Github.
-        
-        
-        2.0 (2017-01-21)
-        ----------------
-        
-        - Update to ``pycountry >= 16.x``.
-        
-        - Drop support for Python 2.6.
-        
-        - Bring test coverage to 100 %.
-        
-        - Change testrunner to py.test.
-        
-        
-        1.0 (2015-08-05)
-        ----------------
-        
-        - Update to ``pycountry 1.12`` thus adding support for ISO 639 3, dropping the
-          old ISO 639 support.
-        
-        
-        0.6.5 (2015-08-05)
-        ------------------
-        
-        - Move repos to https://bitbucket.org/gocept/gocept.country
-        
-        0.6.4 (2008-10-21)
-        ------------------
-        
-        - Bugfix: declared namespace package in setup.py
-        
-        0.6.3 (2008-10-14)
-        ------------------
-        
-        - Bugfix: added not-equal compare method for db objects
-        
-        0.6.2 (2008-10-13)
-        ------------------
-        
-        - Added security declarations for token.
-        - Bugfix in comparison of db objects, where `isinstance` returns False
-          for objects of the same type
-        
-        0.6.1 (2008-09-13)
-        ------------------
-        
-        - Bugfix in countextual subdivision source: parameters of some methods
-          where in wrong order.
-        
-        0.6 (2008-09-12)
-        ----------------
-        
-        - Added contextual country subdivision source, so country subdivisions
-          can depend on the country.
-        
-        
-        0.5 (2008-09-11)
-        ----------------
-        
-        - Added support for country subdivisions.
-        
-        0.4.2 (2008-09-10)
-        ------------------
-        
-        - Added security declarations for tokens.
-        
-        0.4.1 (2008-09-10)
-        ------------------
-        
-        - Fixed bug in token comparison.
-        
-        0.4 (2008-06-10)
-        ----------------
-        
-        - added possibility to smaller the amount of results generated by the
-          sourcefactory
-        
-        
-        0.3 (2008-05-21)
-        ----------------
-        
-        - added test for comparing the returned countries to equality
-        - added __reduce__ to data objects so that they can be pickled
-        - added tests for pickling and unpickling data objects
-        
-        
-        0.2 (2008-05-20)
-        ----------------
-        
-        - gocept.country now returns special data objects instead of pycountry
-          objects for a better object-oriented purpose and flexibility in handling the
-          result
-        - improved configure.zcml and added functional tests for the i18n translations
-        - improved test cases in general
-        
-        0.1 (2008-05-20)
-        ----------------
-        
-        - initial release
-        
-        Contributors
-        ============
-        
-        - Michael Howitz <mh at gocept dot com>
-        
-        
 Keywords: country subdivision language currency iso 3166 639 4217 15924 3166-2 zope pycountry
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
+Requires-Python: >=3.7
 Provides-Extra: test
+License-File: LICENSE.txt
+
+Copyright (c) 2008-2015 gocept gmbh & co. kg
+
+All Rights Reserved.
+
+This software is subject to the provisions of the Zope Public License,
+Version 2.1 (ZPL). A copy of the ZPL should accompany this distribution.
+THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
+WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
+FOR A PARTICULAR PURPOSE.
+
+
+==============
+gocept.country
+==============
+
+.. image:: https://github.com/gocept/gocept.country/workflows/tests/badge.svg
+    :target: https://github.com/gocept/gocept.country/actions?query=workflow%3Atests
+.. image:: https://coveralls.io/repos/github/gocept/gocept.country/badge.svg?branch=master
+    :target: https://coveralls.io/github/gocept/gocept.country?branch=master
+
+
+This package lets you use the `pycountry database
+<http://pypi.python.org/pypi/pycountry/>`_ within Zope 3.
+
+
+In practice, this means e.g., that you can easily get a zope.schema.Choice
+field to provide a full list of iso 3166 country codes.
+
+For more information about the database please refer to the
+`pycountry product <http://pypi.python.org/pypi/pycountry/>`_.
+
+.. contents::
+
+
+Introduction
+============
+
+`gocept.country` provides Zope 3 sources for the pycountry databases. You can
+use it e.g. to get a ``zope.schema.Choice`` field with all ISO 3166 countries.
+
+  >>> import gocept.country
+  >>> import gocept.country.db
+  >>> import zope.schema
+
+
+ISO 3166 Countries
+==================
+
+To get a list of ISO 3166 countries in a web form, you can use the
+``zope.schema.Choice`` field and provide the gocept.country.countries as
+source:
+
+  >>> countries_field = zope.schema.Choice(title=u'Country',
+  ...                            source=gocept.country.countries)
+  >>> countries_field
+  <zope.schema._field.Choice object at 0x...>
+  >>> countries = iter(countries_field.source)
+
+
+The ``gocept.country.countries`` source factory returns Country objects as
+values, which use the values from pycountry:
+
+  >>> aruba = next(countries)
+  >>> afghanistan = next(countries)
+  >>> afghanistan
+  <gocept.country.db.Country object at 0x...>
+  >>> print(afghanistan.name)
+  Afghanistan
+
+
+Calling ``next()`` again returns the next country from the source:
+
+  >>> angola = next(countries)
+  >>> print(angola.name)
+  Angola
+
+
+There are all information available, which you can get from pycountry:
+
+  >>> print(afghanistan.alpha_2)
+  AF
+  >>> print(afghanistan.alpha_3)
+  AFG
+  >>> print(afghanistan.numeric)
+  004
+  >>> print(afghanistan.official_name)
+  Islamic Republic of Afghanistan
+
+
+To reduce the amount of results you can provide a list or tuple of countries
+you like to have in your source:
+
+  >>> countries = gocept.country.CountrySource(alpha_2=['DE', 'US'])
+  >>> print(*[countries.factory.getTitle(x) for x in countries], sep=', ')
+  Germany, United States
+  >>> print(*[countries.factory.getToken(x) for x in countries], sep=', ')
+  DE, US
+
+Please note, that the result items are sorted by *alpha_2* code. Please also
+note, that you can provide alpha_3 and numeric codes and names resp.
+official_names to reduce the amount of result items, too:
+
+  >>> len(list(gocept.country.CountrySource())) > 200
+  True
+  >>> len(list(gocept.country.CountrySource(alpha_2=['DE', 'US', 'GB'])))
+  3
+  >>> len(list(gocept.country.CountrySource(alpha_3=['DEU', 'USA'])))
+  2
+  >>> len(list(gocept.country.CountrySource(numeric=['276', ])))
+  1
+  >>> countries_list = ['Germany', 'Italy', 'Poland', 'France']
+  >>> len(list(gocept.country.CountrySource(name=countries_list)))
+  4
+
+
+Providing codes, which are not present, does not result in an exception but
+in an empty list:
+
+  >>> len(list(gocept.country.CountrySource(capital=['Berlin', 'Paris'])))
+  0
+
+ISO 3166-2 Country subdivisions
+===============================
+
+Context free source
+-------------------
+
+Country subdivisions are similar to countries:
+
+  >>> subdivisions_field = zope.schema.Choice(
+  ...     title=u'Country subdivisions', source=gocept.country.subdivisions)
+  >>> subdivisions = iter(subdivisions_field.source)
+
+  >>> canillo = next(subdivisions)
+  >>> print(canillo.name)
+  Canillo
+  >>> print(canillo.code)
+  AD-02
+
+  >>> encamp = next(subdivisions)
+  >>> print(encamp.name)
+  Encamp
+  >>> print(encamp.code)
+  AD-03
+  >>> print(gocept.country.subdivisions.factory.getToken(encamp))
+  AD-03
+
+Please note, that the result items are sorted by their *code*. Please
+also note, that you can provide names and numeric codes to reduce the
+amount of result items, too.
+
+  >>> len(list(gocept.country.SubdivisionSource())) > 4000
+  True
+  >>> len(list(gocept.country.SubdivisionSource(code=['DE-ST', 'US-WA'])))
+  2
+  >>> len(list(gocept.country.SubdivisionSource(country_code=['DE'])))
+  16
+  >>> print(*[x.name
+  ...         for x in gocept.country.SubdivisionSource(country_code=['DE'])][3:5],
+  ...       sep=', ')
+  Bayern, Bremen
+  >>> len(list(gocept.country.SubdivisionSource(name=[u'Bayern', u'Bremen'])))
+  2
+
+Contextual source
+-----------------
+
+There is also a contextual source for country subdivisions which
+depends on a country. Let's set up a context object first:
+
+  >>> import zope.interface
+  >>> class IAddress(zope.interface.Interface):
+  ...     country = zope.interface.Attribute("The country of the address.")
+  ...     subdivision = zope.schema.Choice(
+  ...         title=u'Country subdivisions',
+  ...         source=gocept.country.contextual_subdivisions)
+
+  >>> @zope.interface.implementer(IAddress)
+  ... class Address(object):
+  ...     pass
+  >>> address = Address()
+  >>> address.country = gocept.country.db.Country('DE')
+
+The contextual source expects an adapter between the context and
+``gocept.country.interfaces.ICountry``:
+
+  >>> import zope.component
+  >>> import gocept.country.interfaces
+  >>> def get_country(context):
+  ...     return context.country
+  >>> zope.component.provideAdapter(
+  ...    get_country, (IAddress, ), gocept.country.interfaces.ICountry)
+
+  >>> print(gocept.country.interfaces.ICountry(address).name)
+  Germany
+
+So the source contains only the country subdivisions belonging to the
+country:
+
+  >>> len(list(iter(gocept.country.contextual_subdivisions(address))))
+  16
+  >>> print(*[x.name
+  ...         for x in iter(gocept.country.contextual_subdivisions(address))][3:5],
+  ...       sep=', ')
+  Bayern, Bremen
+
+Changing the country changes also the subdivisions:
+
+  >>> address.country = gocept.country.db.Country('CH')
+  >>> len(list(iter(gocept.country.contextual_subdivisions(address))))
+  26
+  >>> print(*[x.name
+  ...         for x in iter(gocept.country.contextual_subdivisions(address))],
+  ...       sep=', ')
+  Aargau, Appenzell Innerrhoden, ...
+  >>> print(*[x.code
+  ...         for x in iter(gocept.country.contextual_subdivisions(address))],
+  ...       sep=', ')
+  CH-AG, CH-AI, ...
+  >>> print(*[gocept.country.contextual_subdivisions.factory.getToken(address, x)
+  ...         for x in iter(gocept.country.contextual_subdivisions(address))],
+  ...       sep=', ')
+  CH-AG, CH-AI, ...
+
+  >>> print(gocept.country.contextual_subdivisions.factory.getTitle(
+  ...     address, gocept.country.db.Subdivision('CH-AG')))
+  Aargau
+
+If the country is not set there are no subdivisions:
+
+  >>> address.country = None
+  >>> len(list(iter(gocept.country.contextual_subdivisions(address))))
+  0
+  >>> list(iter(gocept.country.contextual_subdivisions(address)))
+  []
+
+
+ISO 15924 Scripts
+=================
+
+Scripts are similar to countries:
+
+  >>> scripts_field = zope.schema.Choice(title=u'Script',
+  ...                            source=gocept.country.scripts)
+  >>> scripts = iter(scripts_field.source)
+
+
+  >>> adlam = next(scripts)
+  >>> print(adlam.name)
+  Adlam
+
+  >>> afaka = next(scripts)
+  >>> print(afaka.name)
+  Afaka
+  >>> print(gocept.country.scripts.factory.getToken(afaka))
+  Afak
+
+
+Please note, that the result items are sorted by *alpha_4* code. Please also
+note, that you can provide names and numeric codes to smaller the amount of
+result items, too.
+
+  >>> len(list(gocept.country.ScriptSource())) > 130
+  True
+  >>> len(list(gocept.country.ScriptSource(alpha_4=['Arab', 'Latn'])))
+  2
+  >>> len(list(gocept.country.ScriptSource(numeric=['215', ])))
+  1
+  >>> len(list(gocept.country.ScriptSource(name=['Arabic', 'Latin'])))
+  2
+
+
+ISO 4217 Currencies
+===================
+
+Currencies are similar to the ones before:
+
+  >>> currencies_field = zope.schema.Choice(title=u'Currency',
+  ...                            source=gocept.country.currencies)
+
+  >>> currencies = iter(currencies_field.source)
+
+  >>> dirham = next(currencies)
+  >>> print(dirham.name)
+  UAE Dirham
+
+  >>> afghani = next(currencies)
+  >>> print(afghani.name)
+  Afghani
+  >>> print(gocept.country.currencies.factory.getToken(afghani))
+  AFN
+
+Please note, that the result items are sorted by *alpha_3* code. Please also
+note, that you can provide names and numeric codes to reduce the amount of
+result items, too.
+
+  >>> len(list(gocept.country.CurrencySource())) >= 170
+  True
+  >>> len(list(gocept.country.CurrencySource(alpha_3=['ARS', 'AED', 'AFN'])))
+  3
+  >>> len(list(gocept.country.CurrencySource(numeric=['032', '784'])))
+  2
+  >>> len(list(gocept.country.CurrencySource(name=['Afghani', ])))
+  1
+
+
+ISO 639 Languages
+=================
+
+Languages are similar, too:
+
+  >>> languages_field = zope.schema.Choice(title=u'Language',
+  ...                            source=gocept.country.languages)
+
+  >>> languages = iter(languages_field.source)
+
+  >>> ghotuo = next(languages)
+  >>> print(ghotuo.name)
+  Ghotuo
+
+  >>> alumu_tesu = next(languages)
+  >>> print(alumu_tesu.name)
+  Alumu-Tesu
+  >>> print(gocept.country.languages.factory.getToken(alumu_tesu))
+  aab
+
+Please note, that the result items are sorted by *alpha_3*. Please also
+note, that you can provide names to reduce the amount of result items, too.
+
+  >>> len(list(gocept.country.LanguageSource())) > 480
+  True
+  >>> len(list(gocept.country.LanguageSource(alpha_3=['eng', 'deu'])))
+  2
+  >>> len(list(gocept.country.LanguageSource(name=['English', 'German'])))
+  2
+
+
+Translations
+============
+
+
+First we fetch a specific country:
+
+  >>> countries = list(iter(countries_field.source))
+  >>> germany = [x for x in countries if x.name == u'Germany'][0]
+
+
+The i18n translate method translates 'Germany' into German:
+
+  >>> print(zope.i18n.translate(germany.name, target_language='de'))
+  Deutschland
+
+
+There are also translations for scripts, currencies and languages.
+
+
+Comparison
+==========
+
+
+Countries, scripts, currencies and languages can be compared to equality. To
+test this, we will need another country object ``afghanistan``, which is not
+the *same* object as retrieved before:
+
+
+  >>> afghanistan = next(iter(gocept.country.CountrySource(alpha_2=['AF'])))
+  >>> afghanistan2 = next(iter(gocept.country.CountrySource(alpha_2=['AF'])))
+
+  >>> str(afghanistan) == str(afghanistan2)
+  False
+
+
+Comparing them will get the token for each and compare it:
+
+  >>> afghanistan == afghanistan2
+  True
+  >>> afghanistan != afghanistan2
+  False
+  >>> afghanistan != germany
+  True
+  >>> afghanistan == germany
+  False
+
+
+Comparing with an instance of another class always returns False:
+
+  >>> afghanistan == None
+  False
+  >>> afghanistan != None
+  True
+  >>> afghanistan == object()
+  False
+  >>> afghanistan != object()
+  True
+
+
+Pickling and unpickling
+=======================
+
+
+It should be possible to store "proxy objects" in a database (like the ZODB).
+Therefore, they have to be pickleable:
+
+  >>> from io import BytesIO
+  >>> import pickle
+  >>> f = BytesIO(b'')
+
+Pickling a country should never raise an error...
+
+  >>> pickle.dump(afghanistan, f)
+
+
+... and results in storing the token in the pickle:
+
+  >>> ignored = f.seek(0)
+  >>> b'AF' in f.read()
+  True
+
+
+Reading the pickle again will return the same country which was pickled
+before:
+
+  >>> ignored = f.seek(0)
+  >>> afghanistan2 = pickle.load(f)
+  >>> afghanistan2 == afghanistan
+  True
+  >>> print(afghanistan2.name)
+  Afghanistan
+
+
+Changes
+=======
+
+3.0 (2023-07-14)
+----------------
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.9, 3.10, 3.11.
+
+
+2.1 (2019-09-30)
+----------------
+
+- Add support for Python 3.5 up to 3.8, PyPy and PyPy3.
+
+- Replace test dependency on `zope.app.testing` by `zope.app.wsgi[testlayer]`.
+
+- Migrate to Github.
+
+
+2.0 (2017-01-21)
+----------------
+
+- Update to ``pycountry >= 16.x``.
+
+- Drop support for Python 2.6.
+
+- Bring test coverage to 100 %.
+
+- Change testrunner to py.test.
+
+
+1.0 (2015-08-05)
+----------------
+
+- Update to ``pycountry 1.12`` thus adding support for ISO 639 3, dropping the
+  old ISO 639 support.
+
+
+0.6.5 (2015-08-05)
+------------------
+
+- Move repos to https://bitbucket.org/gocept/gocept.country
+
+0.6.4 (2008-10-21)
+------------------
+
+- Bugfix: declared namespace package in setup.py
+
+0.6.3 (2008-10-14)
+------------------
+
+- Bugfix: added not-equal compare method for db objects
+
+0.6.2 (2008-10-13)
+------------------
+
+- Added security declarations for token.
+- Bugfix in comparison of db objects, where `isinstance` returns False
+  for objects of the same type
+
+0.6.1 (2008-09-13)
+------------------
+
+- Bugfix in countextual subdivision source: parameters of some methods
+  where in wrong order.
+
+0.6 (2008-09-12)
+----------------
+
+- Added contextual country subdivision source, so country subdivisions
+  can depend on the country.
+
+
+0.5 (2008-09-11)
+----------------
+
+- Added support for country subdivisions.
+
+0.4.2 (2008-09-10)
+------------------
+
+- Added security declarations for tokens.
+
+0.4.1 (2008-09-10)
+------------------
+
+- Fixed bug in token comparison.
+
+0.4 (2008-06-10)
+----------------
+
+- added possibility to smaller the amount of results generated by the
+  sourcefactory
+
+
+0.3 (2008-05-21)
+----------------
+
+- added test for comparing the returned countries to equality
+- added __reduce__ to data objects so that they can be pickled
+- added tests for pickling and unpickling data objects
+
+
+0.2 (2008-05-20)
+----------------
+
+- gocept.country now returns special data objects instead of pycountry
+  objects for a better object-oriented purpose and flexibility in handling the
+  result
+- improved configure.zcml and added functional tests for the i18n translations
+- improved test cases in general
+
+0.1 (2008-05-20)
+----------------
+
+- initial release
+
+Contributors
+============
+
+- Michael Howitz <mh at gocept dot com>
```

### Comparing `gocept.country-2.1/src/gocept.country.egg-info/SOURCES.txt` & `gocept.country-3.0/src/gocept.country.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .coveragerc
-.gitignore
-.travis.yml
 CHANGES.rst
 COPYRIGHT.txt
 LICENSE.txt
 README.rst
 pytest.ini
+setup.cfg
 setup.py
 tox.ini
 src/gocept/__init__.py
 src/gocept.country.egg-info/PKG-INFO
 src/gocept.country.egg-info/SOURCES.txt
 src/gocept.country.egg-info/dependency_links.txt
 src/gocept.country.egg-info/namespace_packages.txt
```

