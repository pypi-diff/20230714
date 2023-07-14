# Comparing `tmp/plinkliftover-0.3.0.tar.gz` & `tmp/plinkliftover-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plinkliftover-0.3.0.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `plinkliftover-0.3.0.tar` & `plinkliftover-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,38 @@
--rwxr-xr-x   0        0        0     1492 2021-11-11 22:13:52.936046 plinkliftover-0.3.0/LICENSE
--rwxr-xr-x   0        0        0     5912 2022-02-17 17:25:51.676487 plinkliftover-0.3.0/README.md
--rw-r--r--   0        0        0     3714 2022-02-17 17:28:15.156487 plinkliftover-0.3.0/pyproject.toml
--rwxr-xr-x   0        0        0      829 2022-02-17 17:25:04.406487 plinkliftover-0.3.0/src/plinkliftover/__init__.py
--rwxr-xr-x   0        0        0     4631 2022-02-17 17:25:04.396487 plinkliftover-0.3.0/src/plinkliftover/__main__.py
--rw-r--r--   0        0        0     1859 2022-02-17 17:25:04.406487 plinkliftover-0.3.0/src/plinkliftover/bed2map.py
--rwxr-xr-x   0        0        0     3994 2022-02-17 17:25:04.396487 plinkliftover-0.3.0/src/plinkliftover/liftover.py
--rwxr-xr-x   0        0        0     3140 2021-11-11 22:13:52.936046 plinkliftover-0.3.0/src/plinkliftover/logger.py
--rw-r--r--   0        0        0     1875 2022-02-17 17:25:04.406487 plinkliftover-0.3.0/src/plinkliftover/map2bed.py
--rwxr-xr-x   0        0        0        0 2021-11-11 22:13:52.936046 plinkliftover-0.3.0/src/plinkliftover/py.typed
--rw-r--r--   0        0        0     7174 2022-02-17 17:28:29.612195 plinkliftover-0.3.0/setup.py
--rw-r--r--   0        0        0     6880 2022-02-17 17:28:29.612568 plinkliftover-0.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0      332 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.dockerignore
+-rwxr-xr-x   0        0        0      424 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.editorconfig
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.flake8
+-rwxr-xr-x   0        0        0      744 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0     2346 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/CHANGELOG.md
+-rwxr-xr-x   0        0        0     3352 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0        0        0     1465 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     2889 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/Makefile
+-rwxr-xr-x   0        0        0     1175 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/SECURITY.md
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/cookiecutter-config-file.yml
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/renovate.json
+-rwxr-xr-x   0        0        0     1265 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/setup.cfg
+-rwxr-xr-x   0        0        0      684 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/.stale.yml
+-rwxr-xr-x   0        0        0     1206 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/PULL_REQUEST_TEMPLATE.md
+-rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/dependabot.yml
+-rwxr-xr-x   0        0        0      791 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/release-drafter.yml
+-rwxr-xr-x   0        0        0      744 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/ISSUE_TEMPLATE/config.yml
+-rwxr-xr-x   0        0        0      524 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rwxr-xr-x   0        0        0      508 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/workflows/greetings.yml
+-rwxr-xr-x   0        0        0      398 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.github/workflows/release-drafter.yml
+-rwxr-xr-x   0        0        0     1524 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.vscode/launch.json
+-rwxr-xr-x   0        0        0      733 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/docker/Dockerfile
+-rwxr-xr-x   0        0        0      776 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/docker/README.md
+-rwxr-xr-x   0        0        0     1292 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/src/plinkliftover/__init__.py
+-rwxr-xr-x   0        0        0     4767 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/src/plinkliftover/__main__.py
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/src/plinkliftover/bed2map.py
+-rwxr-xr-x   0        0        0     3888 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/src/plinkliftover/liftover.py
+-rwxr-xr-x   0        0        0      824 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/src/plinkliftover/logger.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/src/plinkliftover/map2bed.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/src/plinkliftover/py.typed
+-rwxr-xr-x   0        0        0    10552 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/.gitignore
+-rwxr-xr-x   0        0        0    34902 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/LICENSE.md
+-rwxr-xr-x   0        0        0     5912 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/README.md
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7515 2020-02-02 00:00:00.000000 plinkliftover-0.4.1/PKG-INFO
```

### Comparing `plinkliftover-0.3.0/README.md` & `plinkliftover-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 allowing one to update the coordinates from one genome reference version to
 another.
 
 
 ## Installation
 
 PLINKLiftOver requires
-* Python 3.8 
+* Python 3.10
 * The command line version of [liftOver](http://genome.ucsc.edu/cgi-bin/hgLiftOver),
 installed and on the system path
 * An appropriate [chain file](http://hgdownload.soe.ucsc.edu/downloads.html#liftover)
 * The [MAP file](https://zzz.bwh.harvard.edu/plink/data.shtml) from a PLINK
 dataset
 
 Install from [pypi](https://pypi.org/project/plinkliftover/)
```

### Comparing `plinkliftover-0.3.0/src/plinkliftover/__init__.py` & `plinkliftover-0.4.1/src/plinkliftover/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,53 @@
-# type: ignore[attr-defined]
-"""`plinkliftover` Converts genotype data stored in plink's PED+MAP format from one genome build to another, using liftOver"""
+"""
+`plinkliftover` Converts genotype data stored in plink's PED+MAP
+format from one genome build to another, using liftOver
+"""
 from importlib.metadata import PackageNotFoundError, version
+from typing import Annotated
+
+from loguru import logger
 
 try:
     __version__ = version(__name__)
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
 
 import typer
 from rich.console import Console
 
 console = Console()
+logger.disable("readcounts")
+
+app = typer.Typer(
+    name="plinkliftover",
+    help="Converts genotype data stored in plink's PED+MAP format from one genome build to another, using liftOver",
+    add_completion=False,
+)
+
+verbosity_level = 0
 
 
-def version_callback(value: bool):
+def version_callback(value: bool) -> None:  # noqa FBT001
     """Prints the version of the package."""
     if value:
-        console.print(
-            f"[yellow]plinkliftover[/] version: [bold blue]{__version__}[/]"
-        )
+        console.print(f"[yellow]plinkliftover[/] version: [bold blue]{__version__}[/]")
         raise typer.Exit()
 
 
-app = typer.Typer(
-    name="plinkliftover",
-    help="Converts genotype data stored in plink's PED+MAP format from one genome build to another, using liftOver",
-    add_completion=False,
-)
+@app.callback()
+def verbosity(
+    verbose: Annotated[
+        int,
+        typer.Option(
+            "-v",
+            "--verbose",
+            help="Control output verbosity. Pass this argument multiple times to increase the amount of output.",
+            count=True,
+        ),
+    ] = 0
+) -> None:
+    verbosity_level = verbose  # noqa: F841
+
+
+if __name__ == "main":
+    app()
```

### Comparing `plinkliftover-0.3.0/src/plinkliftover/__main__.py` & `plinkliftover-0.4.1/src/plinkliftover/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,91 +1,95 @@
-# type: ignore[attr-defined]
-from typing import Optional
-
 from distutils.spawn import find_executable
 from pathlib import Path
+from typing import Annotated, Optional
 
 import typer
+from loguru import logger
 
-from . import __version__, app, console, version_callback
-from .bed2map import bed2map
-from .liftover import liftBed, liftDat, liftPed
-from .logger import plo_logger as logger
-from .map2bed import map2bed
+from plinkliftover import app, console, verbosity_level, version_callback
+from plinkliftover.bed2map import bed2map
+from plinkliftover.liftover import lift_bed, lift_dat, lift_ped
+from plinkliftover.logger import init_logger
+from plinkliftover.map2bed import map2bed
 
 
-@app.command(name="")
+@app.command(name="liftover")
 def liftover(
-    mapfile: str = typer.Argument(
-        ..., help="The plink MAP file to `liftOver`."
-    ),
-    chainfile: str = typer.Argument(
-        ..., help="The location of the chain files to provide to `liftOver`."
-    ),
-    pedfile: Optional[str] = typer.Option(
-        None,
-        help='Optionally remove "unlifted SNPs" from the plink PED file after running `liftOver`.',
-        show_default=False,
-    ),
-    datfile: Optional[str] = typer.Option(
-        None,
-        help="Optionally remove 'unlifted SNPs' from a data file containing a list of SNPs (e.g. for  --exclude or --include in `plink`)",
-        show_default=False,
-    ),
-    prefix: Optional[str] = typer.Option(
-        None, help="The prefix to give to the output files.", show_default=False
-    ),
-    liftoverexecutable: Optional[str] = typer.Option(
-        None, help="The location of the `liftOver` executable."
-    ),
-    version: bool = typer.Option(
-        None,
-        "-v",
-        "--version",
-        callback=version_callback,
-        is_eager=True,
-        help="Prints the version of the plinkliftover package.",
-    ),
+    mapfile: Annotated[
+        Path,
+        typer.Argument(help="The plink MAP file to `liftOver`."),
+    ],
+    chainfile: Annotated[Path, typer.Argument(help="The location of the chain files to provide to `liftOver`.")],
+    pedfile: Annotated[
+        Optional[Path],  # noqa UP007
+        typer.Option(
+            help='Optionally remove "unlifted SNPs" from the plink PED file after running `liftOver`.',
+            show_default=False,
+        ),
+    ] = None,
+    datfile: Annotated[
+        Optional[Path],  # noqa UP007
+        typer.Option(
+            help=(
+                "Optionally remove 'unlifted SNPs' from a data file containing a list of SNPs "
+                "(e.g. for  --exclude or --include in `plink`)"
+            ),
+            show_default=False,
+        ),
+    ] = None,
+    prefix: Annotated[
+        Optional[str], typer.Option(help="The prefix to give to the output files.", show_default=False)  # noqa UP007
+    ] = None,
+    liftoverexecutable: Annotated[
+        Optional[str], typer.Option(help="The location of the `liftOver` executable.")  # noqa UP007
+    ] = None,
+    version: Annotated[  # noqa ARG007
+        bool,
+        typer.Option(
+            "-V",
+            "--version",
+            callback=version_callback,
+            is_eager=True,
+            help="Prints the version of the plinkliftover package.",
+        ),
+    ] = False,  # noqa FBT002
 ) -> None:
     """Converts genotype data stored in plink's PED+MAP format from one genome
     build to another, using liftOver.
     """
     # Show usage message if user hasn't provided any arguments, rather
     # than giving a non-descript error message with the usage()
 
-    mapfile = Path(mapfile)
+    init_logger(verbose=verbosity_level)
+
     oldbed = mapfile.with_suffix(".bed")
     map2bed(mapfile, oldbed)
 
     # If a location is not specified for the liftOver executable.
     # assume it is in the User's $PATH.
     if liftoverexecutable is None:
-        try:
-            liftOverPath = Path(find_executable("liftOver"))
-        except TypeError as e:
-            logger.exception(
-                "The `liftOver` executable was not found.  Please make sure it is installed and in the PATH"
-            )
-            logger.error(e)
+        if (lop := find_executable("liftOver")) is not None:
+            lift_over_path = Path(lop)
+            if not lift_over_path.exists():
+                msg = "The `liftOver` executable was not found.  Please make sure it is installed and in the PATH"
+                logger.exception(msg)
+                raise FileNotFoundError(msg)
     else:
-        liftOverPath = Path(liftoverexecutable)
-        if not liftOverPath.exists():
-            logger.exception(
-                "The `liftOver` executable was not found.  Please make sure it is installed and in the PATH"
-            )
-            raise FileNotFoundError(
-                "The `liftOver` executable was not found.  Please make sure it is installed and in the PATH"
-            )
+        lift_over_path = Path(liftoverexecutable)
+        if not lift_over_path.exists():
+            msg = "The `liftOver` executable was not found.  Please make sure it is installed and in the PATH"
+            logger.exception(msg)
+            raise FileNotFoundError(msg)
 
     newbed = Path(f"{mapfile}.bed")
-    lifted_set, unlifted_set, lb_status = liftBed(
+    lifted_set, unlifted_set, lb_status = lift_bed(
         fin=oldbed,
         fout=newbed,
         chainfile=chainfile,
-        liftOverPath=liftOverPath,
+        lift_over_path=lift_over_path,
     )
 
     if lb_status:
         console.print("lifting [purple]bed[/] file: [green bold]SUCCESS[/]")
         logger.info(f"lifting bed file: {newbed} - SUCCESS")
     else:
         console.print("lifting [purple]bed[/] file: [red bold]FAILED[/]")
@@ -95,43 +99,30 @@
     bed2map(newbed, newmap)
 
     if datfile is not None:
         datfile = Path(datfile)
         console.print(f"[pink]{datfile.name}[/]")
         newdat = Path(f"{prefix}.dat")
 
-        ld_status = liftDat(fin=datfile, fout=newdat, lifted_set=lifted_set)
-
-        if ld_status:
+        if lift_dat(fin=datfile, fout=newdat, lifted_set=lifted_set):
             console.print("lifting [purple]dat[/] file: [green]SUCCESS[/]")
             logger.info(f"lifting map file: {newmap} - SUCCESS")
         else:
             console.print("lifting [purple]dat[/] file: [red]FAILED[/]")
             logger.info(f"lifting map file: {newmap} - FAILED")
 
     if pedfile is not None:
         pedfile = Path(pedfile)
         console.print(f"[pink]{pedfile.name}[/]")
-        newPed = Path(f"{prefix}.ped")
-        lp_status = liftPed(
-            fin=pedfile, fout=newPed, fOldMap=mapfile, unlifted_set=unlifted_set
-        )
-
-        if lp_status:
-            console.print(
-                "lifting [dark_orange3]ped[/] file: [bold green]SUCCESS[/]"
-            )
+        new_ped = Path(f"{prefix}.ped")
+
+        if lift_ped(fin=pedfile, fout=new_ped, foldmap=mapfile, unlifted_set=unlifted_set):
+            console.print("lifting [dark_orange3]ped[/] file: [bold green]SUCCESS[/]")
             logger.info("lifting ped file: SUCCESS")
         else:
-            console.print(
-                "lifting [dark_orange3]ped[/] file: [bold red]FAILED[/]"
-            )
+            console.print("lifting [dark_orange3]ped[/] file: [bold red]FAILED[/]")
             logger.info("lifting ped file: FAILED")
 
     console.print("cleaning up BED files...")
     logger.info("cleaning up BED files...")
     newbed.unlink()
     oldbed.unlink()
-
-
-if __name__ == "__main__":
-    typer.run(main)
```

### Comparing `plinkliftover-0.3.0/src/plinkliftover/bed2map.py` & `plinkliftover-0.4.1/src/plinkliftover/bed2map.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,62 @@
-from typing import Optional
-
 from pathlib import Path
+from typing import Annotated, Optional
 
 import typer
+from loguru import logger
 
-from . import app, console, version_callback
-from .logger import plo_logger as logger
+from plinkliftover import app, console, verbosity_level, version_callback
+from plinkliftover.logger import init_logger
 
-# bed2mapapp = typer.Typer(
-#     name="bed2map",
-#     help="Converts BED files to PLINK MAP format",
-#     add_completion=False,
-# )
+BED_LINES_LENGTH: int = 4
 
 
 def bed2map(fin: Path, fout: Path) -> bool:
+    init_logger(verbosity_level)
     logger.info(f"fin: {fin}, fout: {fout}")
     console.print(
         f"Converting lifted [green]BED[/] [blue]{fin.name}[/] file back to [green]MAP[/] [yellow]{fout.name}[/]..."
     )
     lines = fin.read_text().split("\n")
-    output = list()
+    output = []
     with typer.progressbar(lines) as bed_lines:
         for line in bed_lines:
-            if len(x := line.split()) == 4:
+            if len(x := line.split()) == BED_LINES_LENGTH:
                 chrom, _, pos1, rs = x
                 chrom = chrom.replace("chr", "")
                 output.append(f"{chrom}\t{rs}\t0.0\t{pos1}")
     fout.write_text("\n".join(output))
     return True
 
 
 @app.command(name="bed2map")
 def bed2mapapp(
-    bedfile: Path = typer.Argument(..., help="A BED file."),
-    output: Optional[Path] = typer.Option(
-        None,
-        "-o",
-        "--output",
-        help=f"Location to save MAP file to.  If one is not provided, "
-        f"then it will be saved to where the BED file is.",
-        show_default=True,
-    ),
-    version: bool = typer.Option(
-        None,
-        "-v",
-        "--version",
-        callback=version_callback,
-        is_eager=True,
-        help="Prints the version of the plinkliftover package.",
-    ),
+    bedfile: Annotated[Path, typer.Argument(help="A BED file.")],
+    output: Annotated[
+        Optional[Path],  # noqa UP007
+        typer.Option(
+            "-o",
+            "--output",
+            help=(
+                "Location to save MAP file to.  If one is not provided, "
+                "then it will be saved to where the BED file is."
+            ),
+            show_default=True,
+        ),
+    ] = None,
+    version: Annotated[  # noqa ARG001
+        Optional[bool],  # noqa UP007
+        typer.Option(
+            "-v",
+            "--version",
+            callback=version_callback,
+            is_eager=True,
+            help="Prints the version of the plinkliftover package.",
+        ),
+    ] = None,
 ) -> None:
     """Convert genotype data stored in a PLINK MAP file into a BED file,
     allowing one to use the online version of liftOver should the local
     executable is unavailable
     """
 
     if output is None:
```

### Comparing `plinkliftover-0.3.0/src/plinkliftover/liftover.py` & `plinkliftover-0.4.1/src/plinkliftover/liftover.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,114 +10,99 @@
    the original developer's specific chain file.
  - to not rely the original developer's path to liftOver.
  - to provide helpful usage documentation.
  - to clean up the intermediary BED files to avoid confusion.
  - to generally be slightly more PEP compliant.
 
 Modified by Miles Smith:
- - Update to work with python >=3.7
+ - Update to work with python >= 3.10
 """
 
-from typing import Set, Tuple
-
 import sys
 from pathlib import Path
 from subprocess import check_output
 
+from loguru import logger
 from typer import progressbar
 
-from . import console
-from .logger import plo_logger as logger
+from plinkliftover import console
+
+DAT_LINE_LENGTH: int = 2
 
 
-def liftBed(
+def lift_bed(
     fin: Path,
     fout: Path,
     chainfile: Path,
-    liftOverPath: Path,
-) -> Tuple[Set[str]]:
+    lift_over_path: Path,
+) -> tuple[set[str], set[str], bool]:
     console.print(f"Lifting [green]BED[/] file [blue]{fin.name}[/]...")
-    params = {
-        "LIFTOVER_BIN": liftOverPath.resolve(),
+    params: dict[str, str | Path] = {
+        "LIFTOVER_BIN": lift_over_path.resolve(),
         "OLD": fin,
         "CHAIN": chainfile,
         "NEW": fout,
         "UNLIFTED": f"{fout}.unlifted",
     }
 
-    check_output(params.values())
+    check_output([str(params[_]) for _ in params])  # noqa: S603
     # record lifted/unliftd rs
     unlifted_lines = Path(params["UNLIFTED"]).read_text().split("\n")
     console.print(f"Processing [red]unlifted[/] {fout.name}.unlifted")
     with progressbar(unlifted_lines) as unlifted:
-        unlifted_set = {
-            ln.strip().split()[-1]
-            for ln in unlifted
-            if len(ln) > 0 and ln[0] != "#"
-        }
+        unlifted_set = {ln.strip().split()[-1] for ln in unlifted if len(ln) > 0 and ln[0] != "#"}
 
     console.print(f"Processing [red]new[/] {fout.name}")
     new_bed_lines = Path(params["NEW"]).read_text().split("\n")
     with progressbar(new_bed_lines) as new_bed:
-        lifted_set = {
-            ln.strip().split()[-1]
-            for ln in new_bed
-            if len(ln) != 0 and ln[0] != "#"
-        }
+        lifted_set = {ln.strip().split()[-1] for ln in new_bed if len(ln) != 0 and ln[0] != "#"}
 
     return lifted_set, unlifted_set, True
 
 
-def liftDat(fin: Path, fout: Path, lifted_set: Set[str]) -> bool:
+def lift_dat(fin: Path, fout: Path, lifted_set: set[str]) -> bool:
     console.print(f"Updating [green]DAT[/] file [pink]{fin.name}[/]...")
     lines = fin.read_text().split("\n")
-    output = list()
+    output = []
     with progressbar(lines) as dat_lines:
         for ln in dat_lines:
             if len(ln) == 0 or ln[0] != "M":
                 output.append(ln)
-            else:
-                if len(thing := ln.strip().split()) == 2:
-                    _, rs = thing
-                    if rs in lifted_set:
-                        output.append(ln)
+            elif len(thing := ln.strip().split()) == DAT_LINE_LENGTH:
+                _, rs = thing
+                if rs in lifted_set:
+                    output.append(ln)
     console.print(f"Writing [green]new DAT[/] file [pink]{fout.name}[/]...")
 
     return True
 
 
-def liftPed(
-    fin: Path, fout: Path, fOldMap: Path, unlifted_set: Set[str]
-) -> bool:
+def lift_ped(fin: Path, fout: Path, foldmap: Path, unlifted_set: set[str]) -> bool:
     # two ways to do it:
     # 1. write unlifted snp list
     #    use PLINK to do this job using --exclude
     # 2. alternatively, we can write our own method
     # we will use method 2
-    marker = [i.strip().split()[1] for i in open(fOldMap)]
+    marker = [i.strip().split()[1] for i in open(foldmap)]
     flag = [(x not in unlifted_set) for x in marker]
 
     console.print(f"Updating [green]PED[/] file [orange]{fin.resolve()}[/]...")
     lines = fin.read_text().split("\n")
-    output = list()
+    output = []
     with progressbar(lines) as liftped_lines:
         for ln in liftped_lines:
             if ln.strip() != "":
                 f = ln.strip().split()
-                f = f[:6] + [
-                    f[i * 2] + " " + f[i * 2 + 1] for i in range(3, len(f) // 2)
-                ]
+                f = f[:6] + [f"{f[i * 2]} {f[i * 2 + 1]}" for i in range(3, len(f) // 2)]
                 if len(f[6:]) != len(flag):
                     logger.error("Inconsistent length of ped and map files")
                     logger.error(f"{len(f[6:])} vs {len(flag)}")
                     sys.exit(-1)
                 newmarker = [m for i, m in enumerate(f[6:]) if flag[i]]
 
                 a = "\t".join(f[:6])
                 b = "\t".join(newmarker)
                 output.append(f"{a}\t{b}\n")
-    console.print(
-        f"Writing new [green]PED[/] data to [light_slate_blue]{fout.resolve()}[/]"
-    )
+    console.print(f"Writing new [green]PED[/] data to [light_slate_blue]{fout.resolve()}[/]")
     with open(fout, "w") as fo:
         fo.writelines(output)
     return True
```

### Comparing `plinkliftover-0.3.0/src/plinkliftover/map2bed.py` & `plinkliftover-0.4.1/src/plinkliftover/map2bed.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,61 @@
-from typing import Optional
-
 from pathlib import Path
+from typing import Annotated, Optional
 
 import typer
+from loguru import logger
 
-from . import app, console, version_callback
-from .logger import plo_logger as logger
+from plinkliftover import app, console, verbosity_level, version_callback
+from plinkliftover.logger import init_logger
 
-# map2bedapp = typer.Typer(
-#     name="map2bed",
-#     help="Converts PLINK MAP files into BED format",
-#     add_completion=False,
-# )
+MAP_LINE_LENGTH: int = 4
 
 
 def map2bed(fin: Path, fout: Path) -> bool:
     logger.info(f"fin: {fin}, fout: {fout}")
     console.print(
         f"Converting [green]MAP[/] file [yellow]{fin.name}[/] file to [green]UCSC BED[/] file [blue]{fout.name}[/]..."
     )
+    init_logger(verbosity_level)
     lines = fin.read_text().split("\n")
-    output = list()
+    output = []
     with typer.progressbar(lines) as map_lines:
         for line in map_lines:
-            if len(x := line.split()) == 4:
+            if len(x := line.split()) == MAP_LINE_LENGTH:
                 chrom, rs, _, pos = x
                 output.append(f"chr{chrom}\t{int(pos)-1}\t{int(pos)}\t{rs}")
-            else:
-                pass
     fout.write_text("\n".join(output))
     return True
 
 
 @app.command(name="map2bed")
 def map2bedapp(
-    mapfile: Path = typer.Argument(..., help="A PLINK MAP file."),
-    output: Optional[Path] = typer.Option(
-        None,
-        "-o",
-        "--output",
-        help=f"Location to save BED file to.  If one is not provided, "
-        f"then it will be saved to where the MAP file is.",
-        show_default=True,
-    ),
-    version: bool = typer.Option(
-        None,
-        "-v",
-        "--version",
-        callback=version_callback,
-        is_eager=True,
-        help="Prints the version of the plinkliftover package.",
-    ),
+    mapfile: Annotated[Path, typer.Argument(help="A PLINK MAP file.")],
+    output: Annotated[
+        Optional[Path],  # noqa UP007
+        typer.Option(
+            "-o",
+            "--output",
+            help=(
+                "Location to save BED file to.  If one is not provided, "
+                "then it will be saved to where the MAP file is."
+            ),
+            show_default=True,
+        ),
+    ] = None,
+    version: Annotated[  # noqa ARG001
+        bool,
+        typer.Option(
+            "-v",
+            "--version",
+            callback=version_callback,
+            is_eager=True,
+            help="Prints the version of the plinkliftover package.",
+        ),
+    ] = False,  # noqa FBT007
 ) -> None:
     """Convert genotype data stored in a PLINK MAP file into a BED file,
     allowing one to use the online version of liftOver should the local
     executable is unavailable
     """
 
     if output is None:
```

### Comparing `plinkliftover-0.3.0/setup.py` & `plinkliftover-0.4.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,192 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-package_dir = \
-{'': 'src'}
-
-packages = \
-['plinkliftover']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['psutil>=5.8.0,<6.0.0', 'rich>=10.2.1,<11.0.0', 'typer>=0.4.0,<0.5.0']
-
-entry_points = \
-{'console_scripts': ['bed2map = plinkliftover.bed2map:bed2mapapp',
-                     'map2bed = plinkliftover.map2bed:map2bedapp',
-                     'plinkliftover = plinkliftover.__main__:app']}
-
-setup_kwargs = {
-    'name': 'plinkliftover',
-    'version': '0.3.0',
-    'description': "Converts genotype data stored in plink's PED+MAP format from one genome build to another, using liftOver",
-    'long_description': '# PLINKLiftOver\n\n[![Build status](https://github.com/milescsmith/plinkliftover/workflows/build/badge.svg?branch=master&event=push)](https://github.com/milescsmith/plinkliftover/actions?query=workflow%3Abuild)\n[![Python Version](https://img.shields.io/pypi/pyversions/plinkliftover.svg)](https://pypi.org/project/plinkliftover/)\n[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/milescsmith/plinkliftover/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)\n[![Semantic Versions](https://img.shields.io/badge/%F0%9F%9A%80-semantic%20versions-informational.svg)](https://github.com/milescsmith/plinkliftover/releases)\n[![License](https://img.shields.io/github/license/milescsmith/plinkliftover)](https://github.com/milescsmith/plinkliftover/blob/master/LICENSE)\n![Alt](https://repobeats.axiom.co/api/embed/8d9c682229fb45f45eef3f300367eb33a44bd347.svg "Repobeats analytics image")\n\n**PLINKLiftOver** is a utility enabling [liftOver](http://genome.ucsc.edu/cgi-bin/hgLiftOver)\nto work on genomics files from [PLINK](https://www.cog-genomics.org/plink/),\nallowing one to update the coordinates from one genome reference version to\nanother.\n\n\n## Installation\n\nPLINKLiftOver requires\n* Python 3.8 \n* The command line version of [liftOver](http://genome.ucsc.edu/cgi-bin/hgLiftOver),\ninstalled and on the system path\n* An appropriate [chain file](http://hgdownload.soe.ucsc.edu/downloads.html#liftover)\n* The [MAP file](https://zzz.bwh.harvard.edu/plink/data.shtml) from a PLINK\ndataset\n\nInstall from [pypi](https://pypi.org/project/plinkliftover/)\n```bash\npip install -U plinkliftover\n```\n\nor install the development version with\n\n```bash\npip install -U git+https://github.com/milescsmith/plinkliftover.git\n```\n\n## Usage\n\nplinkliftover has three subcommands:\n* liftover: Fully convert the genomic coordinates from one version to another \nin a PLINK file\n* map2bed: Convert a PLINK MAP file to a BED file\n* bed2map: Convert a BED file to a MAP file\n\nThe latter two subcommands are most useful in situations where it is not \npossible to run the liftOver executable locally (i.e. you are on Windows) but \ncan use [UCSC\'s online version](https://genome.ucsc.edu/cgi-bin/hgLiftOver) \nor you otherwise need/want a BED file.\n\n\n### liftover:\n\n```bash\nUsage: plinkliftover liftover [OPTIONS] MAPFILE CHAINFILE\n\n  Converts genotype data stored in the PLINK PED+MAP format from one genome\n  build to another, using liftOver.\n\nArguments:\n  MAPFILE    The plink MAP file to `liftOver`.  [required]\n  CHAINFILE  The location of the chain files to provide to `liftOver`.\n             [required]\n\nOptions:\n  --pedfile TEXT             Optionally remove "unlifted SNPs" from the plink\n                             PED file after running `liftOver`.\n  --datfile TEXT             Optionally remove \'unlifted SNPs\' from a data\n                             file containing a list of SNPs (e.g. for\n                             --exclude or --include in `plink`)\n  --prefix TEXT              The prefix to give to the output files.\n  --liftoverexecutable TEXT  The location of the `liftOver` executable.\n  -v, --version              Prints the version of the plinkliftover package.\n  --help                     Show this message and exit.\n```\n\nFor example\n\n```bash\nplinkliftover liftover updating.map hg19ToHg38.over.chain.gz --prefix updated\n```\n\n### map2bed:\n\n```bash\nUsage: plinkliftover map2bed [OPTIONS] MAPFILE\n\n  Convert genotype data stored in a PLINK MAP file into a BED file, allowing\n  one to use the online version of liftOver should the local executable is\n  unavailable\n\nArguments:\n  MAPFILE  A PLINK MAP file.  [required]\n\nOptions:\n  -o, --output PATH  Location to save BED file to.  If one is not provided,\n                     then it will be saved to where the MAP file is.\n  -v, --version      Prints the version of the plinkliftover package.\n  --help             Show this message and exit.\n```\n\n### bed2map:\n\n```bash\nUsage: plinkliftover bed2map [OPTIONS] BEDFILE\n\n  Convert genotype data stored in a PLINK MAP file into a BED file, allowing\n  one to use the online version of liftOver should the local executable is\n  unavailable\n\nArguments:\n  BEDFILE  A BED file.  [required]\n\nOptions:\n  -o, --output PATH  Location to save MAP file to.  If one is not provided,\n                     then it will be saved to where the BED file is.\n  -v, --version      Prints the version of the plinkliftover package.\n  --help             Show this message and exit.\n```\n\n### Note!\n\nBy default, [PLINK 2.0](https://www.cog-genomics.org/plink/2.0/) does not \nuse/create the required MAP file.  It can be generated using PLINK 1.9 by\n\n```bash\nplink --bfile original --recode --out to_update\n```\n\nwhere `original` is the prefix for the bed/bim/fam files and `to_update` is the prefix to give the new files.\n\n## 🛡 License\n\n[![License](https://img.shields.io/github/license/milescsmith/plinkliftover)](https://github.com/milescsmith/plinkliftover/blob/master/LICENSE)\n\nThis project is licensed under the terms of the `GNU GPL v3.0` license. See [LICENSE](https://github.com/milescsmith/plinkliftover/blob/master/LICENSE) for more details.\n\n## 📃 Citation\n\n```\n@misc{plinkliftover,\n  author = {Miles Smith <miles-smith@omrf.org>},\n  title = {Awesome `plinkliftover` is a Python cli/package created with https://github.com/TezRomacH/python-package-template},\n  year = {2021},\n  publisher = {GitHub},\n  journal = {GitHub repository},\n  howpublished = {\\url{https://github.com/milescsmith/plinkliftover}}\n}\n```\n\n## Credits\n\nThis project was generated with [`python-package-template`](https://github.com/TezRomacH/python-package-template).\n',
-    'author': 'Miles Smith',
-    'author_email': 'miles-smith@omrf.org',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/milescsmith/plinkliftover',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8.3,<4.0',
+Metadata-Version: 2.1
+Name: plinkliftover
+Version: 0.4.1
+Summary: Converts genotype data stored in plink's PED+MAP format from one genome build to another, using liftOver
+Project-URL: repository, https://github.com/milescsmith/plinkliftover
+Project-URL: homepage, https://github.com/milescsmith/plinkliftover
+Author-email: Miles Smith <miles-smith@omrf.org>
+License-File: LICENSE.md
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: loguru==0.7.0
+Requires-Dist: psutil==5.9.5
+Requires-Dist: rich==13.4.2
+Requires-Dist: typer==0.9.0
+Provides-Extra: dev
+Requires-Dist: bandit==1.7.5; extra == 'dev'
+Requires-Dist: black==23.7.0; extra == 'dev'
+Requires-Dist: build==0.10.0; extra == 'dev'
+Requires-Dist: darglint==1.8.1; extra == 'dev'
+Requires-Dist: flakehell==0.9.0; extra == 'dev'
+Requires-Dist: isort==5.12.0; extra == 'dev'
+Requires-Dist: jupyterlab==4.0.3; extra == 'dev'
+Requires-Dist: mypy==1.4.1; extra == 'dev'
+Requires-Dist: nox==2023.4.22; extra == 'dev'
+Requires-Dist: pre-commit==3.3.3; extra == 'dev'
+Requires-Dist: pycodestyle==2.10.0; extra == 'dev'
+Requires-Dist: pydocstyle==6.3.0; extra == 'dev'
+Requires-Dist: pyflakes==3.0.1; extra == 'dev'
+Requires-Dist: pylint==2.17.4; extra == 'dev'
+Requires-Dist: pytest==7.4.0; extra == 'dev'
+Requires-Dist: pyupgrade==3.9.0; extra == 'dev'
+Requires-Dist: safety==2.3.4; extra == 'dev'
+Requires-Dist: twine==4.0.2; extra == 'dev'
+Description-Content-Type: text/markdown
+
+# PLINKLiftOver
+
+[![Build status](https://github.com/milescsmith/plinkliftover/workflows/build/badge.svg?branch=master&event=push)](https://github.com/milescsmith/plinkliftover/actions?query=workflow%3Abuild)
+[![Python Version](https://img.shields.io/pypi/pyversions/plinkliftover.svg)](https://pypi.org/project/plinkliftover/)
+[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/milescsmith/plinkliftover/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
+[![Semantic Versions](https://img.shields.io/badge/%F0%9F%9A%80-semantic%20versions-informational.svg)](https://github.com/milescsmith/plinkliftover/releases)
+[![License](https://img.shields.io/github/license/milescsmith/plinkliftover)](https://github.com/milescsmith/plinkliftover/blob/master/LICENSE)
+![Alt](https://repobeats.axiom.co/api/embed/8d9c682229fb45f45eef3f300367eb33a44bd347.svg "Repobeats analytics image")
+
+**PLINKLiftOver** is a utility enabling [liftOver](http://genome.ucsc.edu/cgi-bin/hgLiftOver)
+to work on genomics files from [PLINK](https://www.cog-genomics.org/plink/),
+allowing one to update the coordinates from one genome reference version to
+another.
+
+
+## Installation
+
+PLINKLiftOver requires
+* Python 3.10
+* The command line version of [liftOver](http://genome.ucsc.edu/cgi-bin/hgLiftOver),
+installed and on the system path
+* An appropriate [chain file](http://hgdownload.soe.ucsc.edu/downloads.html#liftover)
+* The [MAP file](https://zzz.bwh.harvard.edu/plink/data.shtml) from a PLINK
+dataset
+
+Install from [pypi](https://pypi.org/project/plinkliftover/)
+```bash
+pip install -U plinkliftover
+```
+
+or install the development version with
+
+```bash
+pip install -U git+https://github.com/milescsmith/plinkliftover.git
+```
+
+## Usage
+
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
+```bash
+Usage: plinkliftover liftover [OPTIONS] MAPFILE CHAINFILE
+
+  Converts genotype data stored in the PLINK PED+MAP format from one genome
+  build to another, using liftOver.
+
+Arguments:
+  MAPFILE    The plink MAP file to `liftOver`.  [required]
+  CHAINFILE  The location of the chain files to provide to `liftOver`.
+             [required]
+
+Options:
+  --pedfile TEXT             Optionally remove "unlifted SNPs" from the plink
+                             PED file after running `liftOver`.
+  --datfile TEXT             Optionally remove 'unlifted SNPs' from a data
+                             file containing a list of SNPs (e.g. for
+                             --exclude or --include in `plink`)
+  --prefix TEXT              The prefix to give to the output files.
+  --liftoverexecutable TEXT  The location of the `liftOver` executable.
+  -v, --version              Prints the version of the plinkliftover package.
+  --help                     Show this message and exit.
+```
+
+For example
+
+```bash
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
+```
+
+### Note!
+
+By default, [PLINK 2.0](https://www.cog-genomics.org/plink/2.0/) does not 
+use/create the required MAP file.  It can be generated using PLINK 1.9 by
+
+```bash
+plink --bfile original --recode --out to_update
+```
+
+where `original` is the prefix for the bed/bim/fam files and `to_update` is the prefix to give the new files.
+
+## 🛡 License
+
+[![License](https://img.shields.io/github/license/milescsmith/plinkliftover)](https://github.com/milescsmith/plinkliftover/blob/master/LICENSE)
+
+This project is licensed under the terms of the `GNU GPL v3.0` license. See [LICENSE](https://github.com/milescsmith/plinkliftover/blob/master/LICENSE) for more details.
+
+## 📃 Citation
+
+```
+@misc{plinkliftover,
+  author = {Miles Smith <miles-smith@omrf.org>},
+  title = {Awesome `plinkliftover` is a Python cli/package created with https://github.com/TezRomacH/python-package-template},
+  year = {2021},
+  publisher = {GitHub},
+  journal = {GitHub repository},
+  howpublished = {\url{https://github.com/milescsmith/plinkliftover}}
 }
+```
 
+## Credits
 
-setup(**setup_kwargs)
+This project was generated with [`python-package-template`](https://github.com/TezRomacH/python-package-template).
```

