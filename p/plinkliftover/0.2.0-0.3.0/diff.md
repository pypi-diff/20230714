# Comparing `tmp/plinkliftover-0.2.0.tar.gz` & `tmp/plinkliftover-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plinkliftover-0.2.0.tar", max compression
+gzip compressed data, was "plinkliftover-0.3.0.tar", max compression
```

## Comparing `plinkliftover-0.2.0.tar` & `plinkliftover-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rwxr-xr-x   0        0        0     1492 2022-02-02 21:22:09.324801 plinkliftover-0.2.0/LICENSE
--rwxr-xr-x   0        0        0     4207 2022-02-03 03:39:15.809127 plinkliftover-0.2.0/README.md
--rw-r--r--   0        0        0     3622 2022-02-03 04:57:15.471078 plinkliftover-0.2.0/pyproject.toml
--rwxr-xr-x   0        0        0      336 2022-02-03 03:35:23.195430 plinkliftover-0.2.0/src/plinkliftover/__init__.py
--rwxr-xr-x   0        0        0     5031 2022-02-03 04:53:51.783096 plinkliftover-0.2.0/src/plinkliftover/__main__.py
--rwxr-xr-x   0        0        0     5244 2022-02-03 04:57:03.564934 plinkliftover-0.2.0/src/plinkliftover/liftover.py
--rwxr-xr-x   0        0        0     3140 2022-02-02 21:22:09.334765 plinkliftover-0.2.0/src/plinkliftover/logger.py
--rwxr-xr-x   0        0        0        0 2022-02-02 21:22:09.334878 plinkliftover-0.2.0/src/plinkliftover/py.typed
--rw-r--r--   0        0        0     5284 2022-02-03 04:58:25.719801 plinkliftover-0.2.0/setup.py
--rw-r--r--   0        0        0     5175 2022-02-03 04:58:25.720469 plinkliftover-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1492 2021-11-11 22:13:52.936046 plinkliftover-0.3.0/LICENSE
+-rwxr-xr-x   0        0        0     5912 2022-02-17 17:25:51.676487 plinkliftover-0.3.0/README.md
+-rw-r--r--   0        0        0     3714 2022-02-17 17:28:15.156487 plinkliftover-0.3.0/pyproject.toml
+-rwxr-xr-x   0        0        0      829 2022-02-17 17:25:04.406487 plinkliftover-0.3.0/src/plinkliftover/__init__.py
+-rwxr-xr-x   0        0        0     4631 2022-02-17 17:25:04.396487 plinkliftover-0.3.0/src/plinkliftover/__main__.py
+-rw-r--r--   0        0        0     1859 2022-02-17 17:25:04.406487 plinkliftover-0.3.0/src/plinkliftover/bed2map.py
+-rwxr-xr-x   0        0        0     3994 2022-02-17 17:25:04.396487 plinkliftover-0.3.0/src/plinkliftover/liftover.py
+-rwxr-xr-x   0        0        0     3140 2021-11-11 22:13:52.936046 plinkliftover-0.3.0/src/plinkliftover/logger.py
+-rw-r--r--   0        0        0     1875 2022-02-17 17:25:04.406487 plinkliftover-0.3.0/src/plinkliftover/map2bed.py
+-rwxr-xr-x   0        0        0        0 2021-11-11 22:13:52.936046 plinkliftover-0.3.0/src/plinkliftover/py.typed
+-rw-r--r--   0        0        0     7174 2022-02-17 17:28:29.612195 plinkliftover-0.3.0/setup.py
+-rw-r--r--   0        0        0     6880 2022-02-17 17:28:29.612568 plinkliftover-0.3.0/PKG-INFO
```

### Comparing `plinkliftover-0.2.0/LICENSE` & `plinkliftover-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.2.0/README.md` & `plinkliftover-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # PLINKLiftOver
 
-<div align="justified">
-
 [![Build status](https://github.com/milescsmith/plinkliftover/workflows/build/badge.svg?branch=master&event=push)](https://github.com/milescsmith/plinkliftover/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/plinkliftover.svg)](https://pypi.org/project/plinkliftover/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/milescsmith/plinkliftover/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Semantic Versions](https://img.shields.io/badge/%F0%9F%9A%80-semantic%20versions-informational.svg)](https://github.com/milescsmith/plinkliftover/releases)
@@ -13,41 +11,56 @@
 ![Alt](https://repobeats.axiom.co/api/embed/8d9c682229fb45f45eef3f300367eb33a44bd347.svg "Repobeats analytics image")
 
 **PLINKLiftOver** is a utility enabling [liftOver](http://genome.ucsc.edu/cgi-bin/hgLiftOver)
 to work on genomics files from [PLINK](https://www.cog-genomics.org/plink/),
 allowing one to update the coordinates from one genome reference version to
 another.
 
-</div>
+
 ## Installation
 
 PLINKLiftOver requires
 * Python 3.8 
 * The command line version of [liftOver](http://genome.ucsc.edu/cgi-bin/hgLiftOver),
 installed and on the system path
 * An appropriate [chain file](http://hgdownload.soe.ucsc.edu/downloads.html#liftover)
 * The [MAP file](https://zzz.bwh.harvard.edu/plink/data.shtml) from a PLINK
 dataset
 
+Install from [pypi](https://pypi.org/project/plinkliftover/)
 ```bash
 pip install -U plinkliftover
 ```
 
-or install with the development version with
+or install the development version with
 
 ```bash
 pip install -U git+https://github.com/milescsmith/plinkliftover.git
 ```
 
 ## Usage
 
+plinkliftover has three subcommands:
+* liftover: Fully convert the genomic coordinates from one version to another 
+in a PLINK file
+* map2bed: Convert a PLINK MAP file to a BED file
+* bed2map: Convert a BED file to a MAP file
+
+The latter two subcommands are most useful in situations where it is not 
+possible to run the liftOver executable locally (i.e. you are on Windows) but 
+can use [UCSC's online version](https://genome.ucsc.edu/cgi-bin/hgLiftOver) 
+or you otherwise need/want a BED file.
+
+
+### liftover:
+
 ```bash
-Usage: plinkliftover [OPTIONS] MAPFILE CHAINFILE
+Usage: plinkliftover liftover [OPTIONS] MAPFILE CHAINFILE
 
-  Converts genotype data stored in plink's PED+MAP format from one genome
+  Converts genotype data stored in the PLINK PED+MAP format from one genome
   build to another, using liftOver.
 
 Arguments:
   MAPFILE    The plink MAP file to `liftOver`.  [required]
   CHAINFILE  The location of the chain files to provide to `liftOver`.
              [required]
 
@@ -62,15 +75,53 @@
   -v, --version              Prints the version of the plinkliftover package.
   --help                     Show this message and exit.
 ```
 
 For example
 
 ```bash
-plinkliftover updating.map hg19ToHg38.over.chain.gz
+plinkliftover liftover updating.map hg19ToHg38.over.chain.gz --prefix updated
+```
+
+### map2bed:
+
+```bash
+Usage: plinkliftover map2bed [OPTIONS] MAPFILE
+
+  Convert genotype data stored in a PLINK MAP file into a BED file, allowing
+  one to use the online version of liftOver should the local executable is
+  unavailable
+
+Arguments:
+  MAPFILE  A PLINK MAP file.  [required]
+
+Options:
+  -o, --output PATH  Location to save BED file to.  If one is not provided,
+                     then it will be saved to where the MAP file is.
+  -v, --version      Prints the version of the plinkliftover package.
+  --help             Show this message and exit.
+```
+
+### bed2map:
+
+```bash
+Usage: plinkliftover bed2map [OPTIONS] BEDFILE
+
+  Convert genotype data stored in a PLINK MAP file into a BED file, allowing
+  one to use the online version of liftOver should the local executable is
+  unavailable
+
+Arguments:
+  BEDFILE  A BED file.  [required]
+
+Options:
+  -o, --output PATH  Location to save MAP file to.  If one is not provided,
+                     then it will be saved to where the BED file is.
+  -v, --version      Prints the version of the plinkliftover package.
+  --help             Show this message and exit.
 ```
 
 ### Note!
 
 By default, [PLINK 2.0](https://www.cog-genomics.org/plink/2.0/) does not 
 use/create the required MAP file.  It can be generated using PLINK 1.9 by
```

### Comparing `plinkliftover-0.2.0/pyproject.toml` & `plinkliftover-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["poetry>=1.0"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "plinkliftover"
-version = "0.2.0"
+version = "0.3.0"
 description = "Converts genotype data stored in plink's PED+MAP format from one genome build to another, using liftOver"
 readme = "README.md"
 authors = [
   "Miles Smith <miles-smith@omrf.org>"
 ]
 license = "GNU GPL v3.0"
 repository = "https://github.com/milescsmith/plinkliftover"
@@ -26,14 +26,16 @@
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.scripts]
 # Entry points for the package https://python-poetry.org/docs/pyproject/#scripts
 "plinkliftover" = "plinkliftover.__main__:app"
+"map2bed"= "plinkliftover.map2bed:map2bedapp"
+"bed2map"= "plinkliftover.bed2map:bed2mapapp"
 
 [tool.poetry.dependencies]
 python = ">=3.8.3,<4.0"
 typer = "^0.4.0"
 rich = "^10.2.1"
 psutil = "^5.8.0"
```

### Comparing `plinkliftover-0.2.0/src/plinkliftover/__main__.py` & `plinkliftover-0.3.0/src/plinkliftover/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,24 @@
 # type: ignore[attr-defined]
 from typing import Optional
 
 from distutils.spawn import find_executable
 from pathlib import Path
 
 import typer
-from . import __version__
-from .liftover import bed2map, liftBed, liftDat, liftPed, map2bed
-from .logger import plo_logger as logger
-from rich.console import Console
-
-app = typer.Typer(
-    name="plinkliftover",
-    help="Converts genotype data stored in plink's PED+MAP format from one genome build to another, using liftOver",
-    add_completion=False,
-)
-console = Console()
 
-
-def version_callback(value: bool):
-    """Prints the version of the package."""
-    if value:
-        console.print(
-            f"[yellow]plinkliftover[/] version: [bold blue]{__version__}[/]"
-        )
-        raise typer.Exit()
+from . import __version__, app, console, version_callback
+from .bed2map import bed2map
+from .liftover import liftBed, liftDat, liftPed
+from .logger import plo_logger as logger
+from .map2bed import map2bed
 
 
 @app.command(name="")
-def main(
+def liftover(
     mapfile: str = typer.Argument(
         ..., help="The plink MAP file to `liftOver`."
     ),
     chainfile: str = typer.Argument(
         ..., help="The location of the chain files to provide to `liftOver`."
     ),
     pedfile: Optional[str] = typer.Option(
```

### Comparing `plinkliftover-0.2.0/src/plinkliftover/logger.py` & `plinkliftover-0.3.0/src/plinkliftover/logger.py`

 * *Files identical despite different names*

### Comparing `plinkliftover-0.2.0/PKG-INFO` & `plinkliftover-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plinkliftover
-Version: 0.2.0
+Version: 0.3.0
 Summary: Converts genotype data stored in plink's PED+MAP format from one genome build to another, using liftOver
 Home-page: https://github.com/milescsmith/plinkliftover
 License: GNU GPL v3.0
 Author: Miles Smith
 Author-email: miles-smith@omrf.org
 Requires-Python: >=3.8.3,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -19,16 +19,14 @@
 Requires-Dist: rich (>=10.2.1,<11.0.0)
 Requires-Dist: typer (>=0.4.0,<0.5.0)
 Project-URL: Repository, https://github.com/milescsmith/plinkliftover
 Description-Content-Type: text/markdown
 
 # PLINKLiftOver
 
-<div align="justified">
-
 [![Build status](https://github.com/milescsmith/plinkliftover/workflows/build/badge.svg?branch=master&event=push)](https://github.com/milescsmith/plinkliftover/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/plinkliftover.svg)](https://pypi.org/project/plinkliftover/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/milescsmith/plinkliftover/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Semantic Versions](https://img.shields.io/badge/%F0%9F%9A%80-semantic%20versions-informational.svg)](https://github.com/milescsmith/plinkliftover/releases)
@@ -36,41 +34,56 @@
 ![Alt](https://repobeats.axiom.co/api/embed/8d9c682229fb45f45eef3f300367eb33a44bd347.svg "Repobeats analytics image")
 
 **PLINKLiftOver** is a utility enabling [liftOver](http://genome.ucsc.edu/cgi-bin/hgLiftOver)
 to work on genomics files from [PLINK](https://www.cog-genomics.org/plink/),
 allowing one to update the coordinates from one genome reference version to
 another.
 
-</div>
+
 ## Installation
 
 PLINKLiftOver requires
 * Python 3.8 
 * The command line version of [liftOver](http://genome.ucsc.edu/cgi-bin/hgLiftOver),
 installed and on the system path
 * An appropriate [chain file](http://hgdownload.soe.ucsc.edu/downloads.html#liftover)
 * The [MAP file](https://zzz.bwh.harvard.edu/plink/data.shtml) from a PLINK
 dataset
 
+Install from [pypi](https://pypi.org/project/plinkliftover/)
 ```bash
 pip install -U plinkliftover
 ```
 
-or install with the development version with
+or install the development version with
 
 ```bash
 pip install -U git+https://github.com/milescsmith/plinkliftover.git
 ```
 
 ## Usage
 
+plinkliftover has three subcommands:
+* liftover: Fully convert the genomic coordinates from one version to another 
+in a PLINK file
+* map2bed: Convert a PLINK MAP file to a BED file
+* bed2map: Convert a BED file to a MAP file
+
+The latter two subcommands are most useful in situations where it is not 
+possible to run the liftOver executable locally (i.e. you are on Windows) but 
+can use [UCSC's online version](https://genome.ucsc.edu/cgi-bin/hgLiftOver) 
+or you otherwise need/want a BED file.
+
+
+### liftover:
+
 ```bash
-Usage: plinkliftover [OPTIONS] MAPFILE CHAINFILE
+Usage: plinkliftover liftover [OPTIONS] MAPFILE CHAINFILE
 
-  Converts genotype data stored in plink's PED+MAP format from one genome
+  Converts genotype data stored in the PLINK PED+MAP format from one genome
   build to another, using liftOver.
 
 Arguments:
   MAPFILE    The plink MAP file to `liftOver`.  [required]
   CHAINFILE  The location of the chain files to provide to `liftOver`.
              [required]
 
@@ -85,15 +98,53 @@
   -v, --version              Prints the version of the plinkliftover package.
   --help                     Show this message and exit.
 ```
 
 For example
 
 ```bash
-plinkliftover updating.map hg19ToHg38.over.chain.gz
+plinkliftover liftover updating.map hg19ToHg38.over.chain.gz --prefix updated
+```
+
+### map2bed:
+
+```bash
+Usage: plinkliftover map2bed [OPTIONS] MAPFILE
+
+  Convert genotype data stored in a PLINK MAP file into a BED file, allowing
+  one to use the online version of liftOver should the local executable is
+  unavailable
+
+Arguments:
+  MAPFILE  A PLINK MAP file.  [required]
+
+Options:
+  -o, --output PATH  Location to save BED file to.  If one is not provided,
+                     then it will be saved to where the MAP file is.
+  -v, --version      Prints the version of the plinkliftover package.
+  --help             Show this message and exit.
+```
+
+### bed2map:
+
+```bash
+Usage: plinkliftover bed2map [OPTIONS] BEDFILE
+
+  Convert genotype data stored in a PLINK MAP file into a BED file, allowing
+  one to use the online version of liftOver should the local executable is
+  unavailable
+
+Arguments:
+  BEDFILE  A BED file.  [required]
+
+Options:
+  -o, --output PATH  Location to save MAP file to.  If one is not provided,
+                     then it will be saved to where the BED file is.
+  -v, --version      Prints the version of the plinkliftover package.
+  --help             Show this message and exit.
 ```
 
 ### Note!
 
 By default, [PLINK 2.0](https://www.cog-genomics.org/plink/2.0/) does not 
 use/create the required MAP file.  It can be generated using PLINK 1.9 by
```

