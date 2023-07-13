# Comparing `tmp/bopforge-0.0.3.tar.gz` & `tmp/bopforge-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bopforge-0.0.3.tar", last modified: Thu Jun 15 23:35:03 2023, max compression
+gzip compressed data, was "bopforge-0.0.4.tar", last modified: Thu Jul 13 22:27:32 2023, max compression
```

## Comparing `bopforge-0.0.3.tar` & `bopforge-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:35:03.404027 bopforge-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-15 23:34:07.000000 bopforge-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-15 23:35:03.404027 bopforge-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 23:34:07.000000 bopforge-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-15 23:34:07.000000 bopforge-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 23:35:03.404027 bopforge-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:35:03.400027 bopforge-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:35:03.404027 bopforge-0.0.3/src/bopforge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 23:34:07.000000 bopforge-0.0.3/src/bopforge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:35:03.404027 bopforge-0.0.3/src/bopforge/continuous_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 23:34:07.000000 bopforge-0.0.3/src/bopforge/continuous_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-15 23:34:07.000000 bopforge-0.0.3/src/bopforge/continuous_pipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22868 2023-06-15 23:34:07.000000 bopforge-0.0.3/src/bopforge/continuous_pipeline/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:35:03.404027 bopforge-0.0.3/src/bopforge/dichotomous_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 23:34:07.000000 bopforge-0.0.3/src/bopforge/dichotomous_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-06-15 23:34:07.000000 bopforge-0.0.3/src/bopforge/dichotomous_pipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-06-15 23:34:07.000000 bopforge-0.0.3/src/bopforge/dichotomous_pipeline/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-15 23:34:07.000000 bopforge-0.0.3/src/bopforge/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:35:03.404027 bopforge-0.0.3/src/bopforge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-15 23:35:03.000000 bopforge-0.0.3/src/bopforge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-15 23:35:03.000000 bopforge-0.0.3/src/bopforge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 23:35:03.000000 bopforge-0.0.3/src/bopforge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-15 23:35:03.000000 bopforge-0.0.3/src/bopforge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-15 23:35:03.000000 bopforge-0.0.3/src/bopforge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 23:35:03.000000 bopforge-0.0.3/src/bopforge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 23:35:03.404027 bopforge-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 23:34:07.000000 bopforge-0.0.3/tests/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:27:32.292618 bopforge-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-13 22:26:31.000000 bopforge-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-13 22:27:32.292618 bopforge-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 22:26:31.000000 bopforge-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-13 22:26:31.000000 bopforge-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 22:27:32.292618 bopforge-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:27:32.292618 bopforge-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:27:32.292618 bopforge-0.0.4/src/bopforge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 22:26:31.000000 bopforge-0.0.4/src/bopforge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:27:32.292618 bopforge-0.0.4/src/bopforge/continuous_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 22:26:31.000000 bopforge-0.0.4/src/bopforge/continuous_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-07-13 22:26:31.000000 bopforge-0.0.4/src/bopforge/continuous_pipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22868 2023-07-13 22:26:31.000000 bopforge-0.0.4/src/bopforge/continuous_pipeline/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:27:32.292618 bopforge-0.0.4/src/bopforge/dichotomous_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 22:26:31.000000 bopforge-0.0.4/src/bopforge/dichotomous_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-07-13 22:26:31.000000 bopforge-0.0.4/src/bopforge/dichotomous_pipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-07-13 22:26:31.000000 bopforge-0.0.4/src/bopforge/dichotomous_pipeline/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-07-13 22:26:31.000000 bopforge-0.0.4/src/bopforge/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:27:32.292618 bopforge-0.0.4/src/bopforge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-13 22:27:32.000000 bopforge-0.0.4/src/bopforge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-13 22:27:32.000000 bopforge-0.0.4/src/bopforge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 22:27:32.000000 bopforge-0.0.4/src/bopforge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-13 22:27:32.000000 bopforge-0.0.4/src/bopforge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-13 22:27:32.000000 bopforge-0.0.4/src/bopforge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 22:27:32.000000 bopforge-0.0.4/src/bopforge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:27:32.292618 bopforge-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-13 22:26:31.000000 bopforge-0.0.4/tests/test_dummy.py
```

### Comparing `bopforge-0.0.3/LICENSE` & `bopforge-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bopforge-0.0.3/PKG-INFO` & `bopforge-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bopforge
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pipelines for Burden of Proof (BoP) analyses
 Author-email: IHME Math Sciences <ihme.math.sciences@gmail.com>
 License: BSD 2-Clause License
         
         Copyright (c) 2023, IHME Math Sciences
         All rights reserved.
```

### Comparing `bopforge-0.0.3/pyproject.toml` & `bopforge-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bopforge"
-version = "0.0.3"
+version = "0.0.4"
 description = "Pipelines for Burden of Proof (BoP) analyses"
 readme = "REDME.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
 authors = [
     { name = "IHME Math Sciences", email = "ihme.math.sciences@gmail.com" },
 ]
@@ -25,8 +25,8 @@
 continuous_pipeline = "bopforge.continuous_pipeline.__main__:main"
 dichotomous_pipeline = "bopforge.dichotomous_pipeline.__main__:main"
 
 [tool.sphinx]
 project = "modrover"
 author = "IHME Math Sciences"
 copyright = "2023, IHME Math Sciences"
-version = "0.0.3"
+version = "0.0.4"
```

### Comparing `bopforge-0.0.3/src/bopforge/continuous_pipeline/__main__.py` & `bopforge-0.0.4/src/bopforge/continuous_pipeline/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import os
 import shutil
 import warnings
 from argparse import ArgumentParser
 from pathlib import Path
 
 import bopforge.continuous_pipeline.functions as functions
 import numpy as np
-from bopforge.utils import fill_dict
+from bopforge.utils import fill_dict, ParseKwargs
 from pplkit.data.interface import DataInterface
 
 warnings.filterwarnings("ignore")
 
 
 def pre_processing(dataif: DataInterface) -> None:
     name = dataif.result.name
@@ -159,15 +160,21 @@
     dataif.dump_result(df_inner_draws, "inner_draws.csv")
     dataif.dump_result(df_outer_draws, "outer_draws.csv")
     dataif.dump_result(df_inner_quantiles, "inner_quantiles.csv")
     dataif.dump_result(df_outer_quantiles, "outer_quantiles.csv")
     fig.savefig(dataif.result / "linear_model.pdf", bbox_inches="tight")
 
 
-def run(i_dir: str, o_dir: str, pairs: list[str], actions: list[str]) -> None:
+def run(
+    i_dir: str,
+    o_dir: str,
+    pairs: list[str],
+    actions: list[str],
+    metadata: dict,
+) -> None:
     i_dir, o_dir = Path(i_dir), Path(o_dir)
 
     # check the input and output folders
     if not i_dir.exists():
         raise FileNotFoundError("input data folder not found")
 
     o_dir.mkdir(parents=True, exist_ok=True)
@@ -198,30 +205,35 @@
 
         shutil.copy(i_dir / f"{pair}.csv", pair_o_dir / f"raw-{pair}.csv")
 
         if pair not in settings:
             pair_settings = settings["default"]
         else:
             pair_settings = fill_dict(settings[pair], settings["default"])
+        pair_settings["metadata"] = metadata
         dataif.dump_o_dir(pair_settings, pair, "settings.yaml")
 
         np.random.seed(pair_settings["seed"])
         pair_dataif = DataInterface(result=pair_o_dir)
         pre_processing(pair_dataif)
         for action in actions:
             globals()[action](pair_dataif)
 
 
 def main(args=None) -> None:
     parser = ArgumentParser(description="Continuous burden of proof pipeline.")
     parser.add_argument(
-        "-i", "--input", type=str, required=True, help="Input data folder"
+        "-i", "--input", type=os.path.abspath, required=True, help="Input data folder"
     )
     parser.add_argument(
-        "-o", "--output", type=str, required=True, help="Output result folder"
+        "-o",
+        "--output",
+        type=os.path.abspath,
+        required=True,
+        help="Output result folder",
     )
     parser.add_argument(
         "-p",
         "--pairs",
         required=False,
         default=None,
         nargs="+",
@@ -231,13 +243,22 @@
         "-a",
         "--actions",
         choices=["fit_signal_model", "select_bias_covs", "fit_linear_model"],
         default=None,
         nargs="+",
         help="Included actions, default all actions",
     )
+    parser.add_argument(
+        "-m",
+        "--metadata",
+        nargs="*",
+        required=False,
+        default={},
+        action=ParseKwargs,
+        help="User defined metadata",
+    )
     args = parser.parse_args(args)
-    run(args.input, args.output, args.pairs, args.actions)
-    
+    run(args.input, args.output, args.pairs, args.actions, args.metadata)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `bopforge-0.0.3/src/bopforge/continuous_pipeline/functions.py` & `bopforge-0.0.4/src/bopforge/continuous_pipeline/functions.py`

 * *Files identical despite different names*

### Comparing `bopforge-0.0.3/src/bopforge/dichotomous_pipeline/__main__.py` & `bopforge-0.0.4/src/bopforge/dichotomous_pipeline/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import os
 import shutil
 import warnings
 from argparse import ArgumentParser
 from pathlib import Path
 
 import bopforge.dichotomous_pipeline.functions as functions
 import numpy as np
-from bopforge.utils import fill_dict
+from bopforge.utils import fill_dict, ParseKwargs
 from pplkit.data.interface import DataInterface
 
 warnings.filterwarnings("ignore")
 
 
 def pre_processing(result_folder: Path) -> None:
     dataif = DataInterface(result=result_folder)
@@ -138,30 +139,34 @@
     linear_model = functions.get_linear_model(df_train, cov_finder_result)
     linear_model.fit_model()
 
     summary = functions.get_linear_model_summary(summary, df, linear_model)
 
     df_inner_draws, df_outer_draws = functions.get_draws(settings, summary)
 
-    df_inner_quantiles, df_outer_quantiles = functions.get_quantiles(
-        settings, summary
-    )
+    df_inner_quantiles, df_outer_quantiles = functions.get_quantiles(settings, summary)
 
     fig = functions.plot_linear_model(summary, df)
 
     dataif.dump_result(linear_model, "linear_model.pkl")
     dataif.dump_result(summary, "summary.yaml")
     dataif.dump_result(df_inner_draws, "inner_draws.csv")
     dataif.dump_result(df_outer_draws, "outer_draws.csv")
     dataif.dump_result(df_inner_quantiles, "inner_quantiles.csv")
     dataif.dump_result(df_outer_quantiles, "outer_quantiles.csv")
     fig.savefig(dataif.result / "linear_model.pdf", bbox_inches="tight")
 
 
-def run(i_dir: str, o_dir: str, pairs: list[str], actions: list[str]) -> None:
+def run(
+    i_dir: str,
+    o_dir: str,
+    pairs: list[str],
+    actions: list[str],
+    metadata: dict,
+) -> None:
     i_dir, o_dir = Path(i_dir), Path(o_dir)
     # check the input and output folders
     if not i_dir.exists():
         raise FileNotFoundError("input data folder not found")
 
     o_dir.mkdir(parents=True, exist_ok=True)
 
@@ -191,29 +196,34 @@
 
         shutil.copy(i_dir / f"{pair}.csv", pair_o_dir / f"raw-{pair}.csv")
 
         if pair not in settings:
             pair_settings = settings["default"]
         else:
             pair_settings = fill_dict(settings[pair], settings["default"])
+        pair_settings["metadata"] = metadata
         dataif.dump_o_dir(pair_settings, pair, "settings.yaml")
 
         np.random.seed(pair_settings["seed"])
         pre_processing(pair_o_dir)
         for action in actions:
             globals()[action](pair_o_dir)
 
 
 def main(args=None) -> None:
     parser = ArgumentParser(description="Dichotomous burden of proof pipeline.")
     parser.add_argument(
-        "-i", "--input", type=str, required=True, help="Input data folder"
+        "-i", "--input", type=os.path.abspath, required=True, help="Input data folder"
     )
     parser.add_argument(
-        "-o", "--output", type=str, required=True, help="Output result folder"
+        "-o",
+        "--output",
+        type=os.path.abspath,
+        required=True,
+        help="Output result folder",
     )
     parser.add_argument(
         "-p",
         "--pairs",
         required=False,
         default=None,
         nargs="+",
@@ -223,14 +233,23 @@
         "-a",
         "--actions",
         choices=["fit_signal_model", "select_bias_covs", "fit_linear_model"],
         default=None,
         nargs="+",
         help="Included actions, default all actions",
     )
+    parser.add_argument(
+        "-m",
+        "--metadata",
+        nargs="*",
+        required=False,
+        default={},
+        action=ParseKwargs,
+        help="User defined metadata",
+    )
     args = parser.parse_args(args)
 
-    run(args.input, args.output, args.pairs, args.actions)    
+    run(args.input, args.output, args.pairs, args.actions, args.metadata)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `bopforge-0.0.3/src/bopforge/dichotomous_pipeline/functions.py` & `bopforge-0.0.4/src/bopforge/dichotomous_pipeline/functions.py`

 * *Files identical despite different names*

### Comparing `bopforge-0.0.3/src/bopforge/utils.py` & `bopforge-0.0.4/src/bopforge/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Ultility functions
 """
-from typing import Dict, Tuple
+import argparse
+from typing import Any, Dict, Tuple, Optional
 
 import numpy as np
 from mrtool import MRBRT, MRBeRT, MRData
 
 
 def fill_dict(des_dict: Dict, default_dict: Dict) -> Dict:
     """Fill given dictionary by the default dictionary.
@@ -26,16 +27,15 @@
         if key not in des_dict:
             des_dict[key] = value
         elif isinstance(value, dict):
             des_dict[key] = fill_dict(des_dict[key], value)
     return des_dict
 
 
-def get_beta_info(model: MRBRT,
-                  cov_name: str = "signal") -> Tuple[float, float]:
+def get_beta_info(model: MRBRT, cov_name: str = "signal") -> Tuple[float, float]:
     """Get the posterior information of beta.
 
     Parameters
     ----------
     model : MRBRT
         MRBRT model, preferably is a simple linear mixed effects model.
     cov_name : str, optional
@@ -45,15 +45,15 @@
     -------
     Tuple[float, float]
         Return the mean and standard deviation of the corresponding beta.
     """
     lt = model.lt
     index = model.cov_names.index(cov_name)
     beta = model.beta_soln[index]
-    beta_hessian = lt.hessian(lt.soln)[:lt.k_beta, :lt.k_beta]
+    beta_hessian = lt.hessian(lt.soln)[: lt.k_beta, : lt.k_beta]
     beta_sd = 1.0 / np.sqrt(beta_hessian[index, index])
     return (beta, beta_sd)
 
 
 def get_gamma_info(model: MRBRT) -> Tuple[float, float]:
     """Get the posterior information of gamma.
 
@@ -67,27 +67,72 @@
     -------
     Tuple[float, float]
         Return the mean and standard deviation of the corresponding gamma.
     """
     lt = model.lt
     gamma = model.gamma_soln[0]
     gamma_fisher = lt.get_gamma_fisher(lt.gamma)
-    gamma_sd = 1.0/np.sqrt(gamma_fisher[0, 0])
+    gamma_sd = 1.0 / np.sqrt(gamma_fisher[0, 0])
     return (gamma, gamma_sd)
 
 
 def get_signal(signal_model: MRBeRT, risk: np.ndarray) -> np.ndarray:
     """Get signal from signal_model
 
     Parameters
     ----------
     signal_model : MRBeRT
         Signal model object.
     risk : np.ndarray
         Risk exposures that we want to create signal on.
     """
-    return signal_model.predict(MRData(covs={
-        "ref_risk_lower": np.repeat(risk.min(), len(risk)),
-        "ref_risk_upper": np.repeat(risk.min(), len(risk)),
-        "alt_risk_lower": risk,
-        "alt_risk_upper": risk
-    }))
+    return signal_model.predict(
+        MRData(
+            covs={
+                "ref_risk_lower": np.repeat(risk.min(), len(risk)),
+                "ref_risk_upper": np.repeat(risk.min(), len(risk)),
+                "alt_risk_lower": risk,
+                "alt_risk_upper": risk,
+            }
+        )
+    )
+
+
+class ParseKwargs(argparse.Action):
+    def __call__(
+        self,
+        parser: argparse.ArgumentParser,
+        namespace: argparse.Namespace,
+        values: list[str],
+        option_string: Optional[str] = None,
+    ):
+        """Parse keyword arguments into a dictionary. Be sure to set `nargs='*'`
+        in the ArgumentParser to parse the input as a list of strings, otherwise
+        this function will break. If provided string does not the form of
+        '{key}={value}', an error will be raised.
+
+        Example
+        -------
+
+        .. code-block:: python
+
+            parser = ArgumentParser()
+            parser.add_argument(
+                "-m",
+                "--metadata",
+                nargs="*",
+                required=False,
+                default={},
+                action=ParseKwargs,
+            )
+
+        """
+        data = dict()
+        for value in values:
+            data_key, _, data_value = value.partition("=")
+            if (not data_key) or (not data_value):
+                raise ValueError(
+                    "please provide kwargs in the form of {key}={value}, "
+                    f"current input is '{value}'"
+                )
+            data[data_key] = data_value
+        setattr(namespace, self.dest, data)
```

### Comparing `bopforge-0.0.3/src/bopforge.egg-info/PKG-INFO` & `bopforge-0.0.4/src/bopforge.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bopforge
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pipelines for Burden of Proof (BoP) analyses
 Author-email: IHME Math Sciences <ihme.math.sciences@gmail.com>
 License: BSD 2-Clause License
         
         Copyright (c) 2023, IHME Math Sciences
         All rights reserved.
```

### Comparing `bopforge-0.0.3/src/bopforge.egg-info/SOURCES.txt` & `bopforge-0.0.4/src/bopforge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

