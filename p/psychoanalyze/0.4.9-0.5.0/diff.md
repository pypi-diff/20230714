# Comparing `tmp/psychoanalyze-0.4.9.tar.gz` & `tmp/psychoanalyze-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoanalyze-0.4.9.tar", max compression
+gzip compressed data, was "psychoanalyze-0.5.0.tar", max compression
```

## Comparing `psychoanalyze-0.4.9.tar` & `psychoanalyze-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35149 2023-07-09 20:02:37.718055 psychoanalyze-0.4.9/LICENSE
--rw-r--r--   0        0        0     1184 2023-07-09 20:02:37.718055 psychoanalyze-0.4.9/README.md
--rw-r--r--   0        0        0     1350 2023-07-09 20:04:14.410827 psychoanalyze-0.4.9/psychoanalyze/__init__.py
--rw-r--r--   0        0        0      749 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/analysis/__init__.py
--rw-r--r--   0        0        0     1281 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/analysis/bayes.py
--rw-r--r--   0        0        0     1113 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/analysis/ecdf.py
--rw-r--r--   0        0        0     2294 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/analysis/strength_duration.py
--rw-r--r--   0        0        0     2366 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/analysis/weber.py
--rw-r--r--   0        0        0     1643 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/data/__init__.py
--rw-r--r--   0        0        0     8278 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/data/blocks.py
--rw-r--r--   0        0        0     7903 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/data/points.py
--rw-r--r--   0        0        0     2861 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/data/sessions.py
--rw-r--r--   0        0        0      834 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/data/stimulus.py
--rw-r--r--   0        0        0     1671 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/data/subjects.py
--rw-r--r--   0        0        0     4936 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/data/trials.py
--rw-r--r--   0        0        0     3462 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/data/types.py
--rw-r--r--   0        0        0     1582 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/plot.py
--rw-r--r--   0        0        0     1511 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/sigmoids.py
--rw-r--r--   0        0        0     1985 2023-07-09 20:04:14.410827 psychoanalyze-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     2796 1970-01-01 00:00:00.000000 psychoanalyze-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-14 03:05:50.334003 psychoanalyze-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1105 2023-07-14 03:05:50.334003 psychoanalyze-0.5.0/README.md
+-rw-r--r--   0        0        0     1357 2023-07-14 03:07:52.912887 psychoanalyze-0.5.0/psychoanalyze/__init__.py
+-rw-r--r--   0        0        0      756 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/analysis/__init__.py
+-rw-r--r--   0        0        0     1288 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/analysis/bayes.py
+-rw-r--r--   0        0        0     1120 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/analysis/ecdf.py
+-rw-r--r--   0        0        0     2302 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/analysis/strength_duration.py
+-rw-r--r--   0        0        0     2373 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/analysis/weber.py
+-rw-r--r--   0        0        0     1639 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/data/__init__.py
+-rw-r--r--   0        0        0     8559 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/data/blocks.py
+-rw-r--r--   0        0        0     8048 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/data/points.py
+-rw-r--r--   0        0        0     2868 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/data/sessions.py
+-rw-r--r--   0        0        0      841 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/data/stimulus.py
+-rw-r--r--   0        0        0     1678 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/data/subjects.py
+-rw-r--r--   0        0        0     5256 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/data/trials.py
+-rw-r--r--   0        0        0     2938 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/data/types.py
+-rw-r--r--   0        0        0     1589 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/plot.py
+-rw-r--r--   0        0        0     1518 2023-07-14 03:05:50.410002 psychoanalyze-0.5.0/psychoanalyze/sigmoids.py
+-rw-r--r--   0        0        0     1963 2023-07-14 03:07:52.912887 psychoanalyze-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2839 1970-01-01 00:00:00.000000 psychoanalyze-0.5.0/PKG-INFO
```

### Comparing `psychoanalyze-0.4.9/LICENSE` & `psychoanalyze-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.9/README.md` & `psychoanalyze-0.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # PsychoAnalyze
 
 Psychophysics analysis in Python.
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/psychoanalyze)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]()
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 [![Open in Remote - Containers](https://img.shields.io/static/v1?label=Remote%20-%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/psychoanalyze/psychoanalyze)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/psychoanalyze/psychoanalyze/main.svg)](https://results.pre-commit.ci/latest/github/psychoanalyze/psychoanalyze/main)
 
 
 
 ## Installation
```

### Comparing `psychoanalyze-0.4.9/psychoanalyze/__init__.py` & `psychoanalyze-0.5.0/psychoanalyze/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 
 # PsychoAnalyze is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
-# You should have received a copy of the GNU General Public License along with Foobar.
-# If not, see <https://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
 """Top-level package for `psychoanalyze`.
 
 Modules:
 
 - [`plot`][psychoanalyze.plot]: Global plot settings and generic plot utilities.
 - [`sigmoids`][psychoanalyze.sigmoids]: Implementations of psychometric sigmoid
```

### Comparing `psychoanalyze-0.4.9/psychoanalyze/analysis/__init__.py` & `psychoanalyze-0.5.0/psychoanalyze/analysis/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 
 # PsychoAnalyze is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
-# You should have received a copy of the GNU General Public License along with Foobar.
-# If not, see <https://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
 """Data structures and manipulation methods."""
```

### Comparing `psychoanalyze-0.4.9/psychoanalyze/analysis/bayes.py` & `psychoanalyze-0.5.0/psychoanalyze/analysis/bayes.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 
 # PsychoAnalyze is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
-# You should have received a copy of the GNU General Public License along with Foobar.
-# If not, see <https://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
 """Bayesian analysis of psychophysical data."""
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
```

### Comparing `psychoanalyze-0.4.9/psychoanalyze/analysis/ecdf.py` & `psychoanalyze-0.5.0/psychoanalyze/analysis/ecdf.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 
 # PsychoAnalyze is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
-# You should have received a copy of the GNU General Public License along with Foobar.
-# If not, see <https://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
 """Empirical Distribution Functions (eCDF)."""
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
```

### Comparing `psychoanalyze-0.4.9/psychoanalyze/analysis/strength_duration.py` & `psychoanalyze-0.5.0/psychoanalyze/analysis/strength_duration.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 
 # PsychoAnalyze is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
-# You should have received a copy of the GNU General Public License along with Foobar.
-# If not, see <https://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
 """Strength-duration analysis.
 
 Contains functions assessing the relationship
 between the amplitude and the time course of the stimulus.
 """
 import pandas as pd
@@ -33,14 +33,15 @@
         ylabel = "Fixed Amplitude (μA)"
         xlabel = "Threshold Pulse Width (μs)"
 
     blocks[ylabel] = blocks["Threshold"]
     blocks[xlabel] = blocks["Fixed Magnitude"]
     return blocks.drop(columns=["Threshold", "Fixed Magnitude"])
 
+
 def plot(
     blocks: pd.DataFrame,
     dim: str,
     x_data: list[float],
     y_data: list[float],
 ) -> go.Figure:
     """Plot strength-duration curve given detection data."""
```

### Comparing `psychoanalyze-0.4.9/psychoanalyze/analysis/weber.py` & `psychoanalyze-0.5.0/psychoanalyze/analysis/weber.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 
 # PsychoAnalyze is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
-# You should have received a copy of the GNU General Public License along with Foobar.
-# If not, see <https://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
 """Test functions related to Weber's Law analysis.
 
 Contains functions assessing how discriminability of two stimuli
 relates to the baseline intensities of the stimuli according to Weber's Law.
 """
 from pathlib import Path
```

### Comparing `psychoanalyze-0.4.9/psychoanalyze/data/__init__.py` & `psychoanalyze-0.5.0/psychoanalyze/data/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 
 # PsychoAnalyze is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
-# You should have received a copy of the GNU General Public License along with Foobar.
-# If not, see <https://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
 """Data modules and general-purpose data transformation utilities.
 
 Functions:
 
 - [`psychoanalyze.data.load`][psychoanalyze.data.load]
 
@@ -38,9 +38,9 @@
     data_dir: Path = Path("data"),
 ) -> dict[str, pd.DataFrame]:
     """Load all tables into dict."""
     return {
         "Sessions": sessions.load(data_dir),
         "Subjects": subjects.load(data_dir),
         "Blocks": blocks.load(data_dir),
-        "Points": points.load(data_dir).to_frame(),
+        "Points": points.load(data_dir),
     }
```

### Comparing `psychoanalyze-0.4.9/psychoanalyze/data/blocks.py` & `psychoanalyze-0.5.0/psychoanalyze/data/blocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,35 +5,34 @@
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 
 # PsychoAnalyze is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
-# You should have received a copy of the GNU General Public License along with Foobar.
-# If not, see <https://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
 """Block-level data utilities.
 
 **Blocks** are the most analytically significant objects in the PsychoAnalyze
 data hierarchy. They represent a specific set of experimental conditions and generally
 correspond to a single fit of the psychometric function.
 """
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 from pandera.typing import DataFrame
-from scipy.special import expit
+from scipy.special import expit, logit
 from scipy.stats import logistic as scipy_logistic
 from sklearn.linear_model import LogisticRegression
 
-from psychoanalyze import data
 from psychoanalyze.data import (
     points,
     sessions,
     stimulus,
     subjects,
     trials,
     types,
@@ -207,15 +206,15 @@
     Args:
         blocks: Block-level DataFrame.
 
     Returns:
         A plotly Graph Object.
     """
     return px.scatter(
-        data.blocks.transform_errors(blocks),
+        transform_errors(blocks),
         x="Block",
         y="50%",
         error_y="err+",
         error_y_minus="err-",
         color="Subject",
         color_discrete_map={"U": "#e41a1c", "Y": "#377eb8", "Z": "#4daf4a"},
         template=template,
@@ -238,21 +237,29 @@
     ]
     param_fits = transform_errors(param_fits)
     param_fits = param_fits.rename(columns={"50%": y})
     param_fits.index = x
     return param_fits
 
 
-def logistic(
-    threshold: float = 0.0,
-    scale: float = 1.0,
-    gamma: float = 0.0,
-    lambda_: float = 0.0,
-) -> pd.Series:
-    """Generate logistic curves from parameters."""
-    x = np.linspace(scipy_logistic.ppf(0.01), scipy_logistic.ppf(0.99), 100)
-    index = pd.Index(x, name="x")
-    return pd.Series(
-        gamma + (1 - gamma - lambda_) * scipy_logistic.cdf(x, threshold, scale),
+def logistic(params: dict[str, float]) -> pd.DataFrame:
+    """Generate logistic function from parameters."""
+    x = np.linspace(
+        scipy_logistic.ppf(0.01) + params["Threshold"],
+        scipy_logistic.ppf(0.99) + params["Threshold"],
+        100,
+    )
+    y = params["Guess Rate"] + (
+        1 - params["Guess Rate"] - params["Lapse Rate"]
+    ) * scipy_logistic.cdf(x, params["Threshold"], params["Slope"])
+    index = pd.Index(x, name="Intensity")
+    logistic_points = pd.Series(
+        y,
         index=index,
         name="Hit Rate",
     )
+    logit_hit_rate = pd.Series(
+        logit(logistic_points),
+        index=logistic_points.index,
+        name="logit(Hit Rate)",
+    )
+    return pd.concat([logistic_points, logit_hit_rate], axis=1)
```

### Comparing `psychoanalyze-0.4.9/psychoanalyze/data/points.py` & `psychoanalyze-0.5.0/psychoanalyze/data/points.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,52 +5,57 @@
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 
 # PsychoAnalyze is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
-# You should have received a copy of the GNU General Public License along with Foobar.
-# If not, see <https://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
 """Utilities for points-level data.
 
 **Points** correspond to the aggregate measures of method-of-constant-stimuli
 experiments at each stimulus level measured. For example, a block that samples 8
 stimulus intensity levels would have 8 corresponding points.
 """
 from pathlib import Path
 
 import cmdstanpy as stan
 import numpy as np
 import pandas as pd
 import plotly.express as px
 from dash import dash_table
+from pandera import check_io, check_output
 from plotly import graph_objects as go
 from scipy.special import logit
 from scipy.stats import logistic
 
-from psychoanalyze.data import trials
+from psychoanalyze.data import trials as pa_trials
+from psychoanalyze.data import types
 
 index_levels = ["Amp1", "Width1", "Freq1", "Dur1"]
 
 
-def from_trials(_trials: pd.DataFrame) -> pd.Series:
+@check_io(trials=types.trials, out=types.points)
+def from_trials(trials: pd.DataFrame) -> pd.DataFrame:
     """Aggregate point-level measures from trial data."""
-    return (
-        _trials.groupby("Intensity")[["Result"]]
-        .agg(["count", "sum"])
-        .rename(columns={"count": "n", "sum": "Hits"})
-    )["Result"]
+    points = trials.groupby("Intensity").agg(["count", "sum"])
+    points.columns = points.columns.droplevel()
+    points = points.rename(columns={"count": "n", "sum": "Hits"})
+    points["Hit Rate"] = points["Hits"] / points["n"]
+    points["logit(Hit Rate)"] = logit(points["Hit Rate"])
+    return points
 
 
-def load(data_path: Path) -> pd.Series:
+@check_output(types.points)
+def load(data_path: Path) -> pd.DataFrame:
     """Load points data from csv."""
-    _trials = trials.load(data_path)
-    return from_trials(_trials)
+    trials = pa_trials.load(data_path)
+    return from_trials(trials)
 
 
 def dimension(points: pd.DataFrame) -> str:
     """Determine modulated dimension from point-level data."""
     amp1, width1 = (
         points.index.get_level_values(param) for param in ["Amp1", "Width1"]
     )
@@ -75,100 +80,75 @@
 
 
 def model() -> stan.CmdStanModel:
     """Instantiate Stan binomial regression model."""
     return stan.CmdStanModel(stan_file="models/binomial_regression.stan")
 
 
-# def fit(ready_for_fit: pd.DataFrame) -> pd.DataFrame:
-
-
 def fit(
     points: pd.DataFrame,
-    save_to: Path | None = None,
-    block: pd.DataFrame | None = None,
 ) -> pd.DataFrame:
     """Fit psychometric curve to points."""
-    points = points[["x", "Hits", "n"]]
     if len(points):
-        data = points
-        _fit = trials.fit(data)
-        _fit = pd.DataFrame(
+        fit = pa_trials.fit(points[["x", "Hits", "n"]])
+        return pd.DataFrame(
             {
-                "Threshold": [_fit["Fit"][0]],
-                "width": [_fit["Fit"][1]],
-                "gamma": [_fit["Fit"][2]],
-                "lambda": [_fit["Fit"][3]],
-                "err+": [None],
-                "err-": [None],
+                "Threshold": [fit["Threshold"]],
+                "Slope": [fit["Slope"]],
             },
-            index=pd.MultiIndex.from_tuples(
-                [block],
-                names=[
-                    "Monkey",
-                    "Date",
-                    "Amp2",
-                    "Width2",
-                    "Freq2",
-                    "Dur2",
-                    "Active Channels",
-                    "Return Channels",
-                ],
-            ),
         )
-        if save_to:
-            _fit.to_csv(save_to)
-        return _fit
     return pd.DataFrame(
         {
             "Threshold": [],
             "width": [],
             "lambda": [],
             "gamma": [],
             "err+": [],
             "err-": [],
         },
     )
 
 
 def hits(
     n: pd.Series,
-    threshold: float = 0.0,
-    scale: float = 1.0,
-    guess_rate: float = 0.0,
-    lapse_rate: float = 0.0,
+    params: dict[str, float],
 ) -> pd.Series:
     """Sample list of n hits from a list of intensity values."""
-    p = logistic.cdf(n.index.to_numpy(), threshold, scale)
-    psi = guess_rate + (1.0 - guess_rate - lapse_rate) * p
+    p = logistic.cdf(n.index.to_numpy(), params["Threshold"], params["Slope"])
+    psi = params["Guess Rate"] + (1.0 - params["Guess Rate"] - params["Lapse Rate"]) * p
     return pd.Series(
         np.random.default_rng().binomial(
             n,
             psi,
             len(n),
         ),
         index=n.index,
         name="Hits",
     )
 
 
-def generate(  # noqa: PLR0913
+def generate(
     n_trials: int,
-    options: list[float],
-    threshold: float = 0.0,
-    slope: float = 1.0,
-    guess_rate: float = 0.0,
-    lapse_rate: float = 0.0,
+    options: pd.Index,
+    params: dict[str, float],
 ) -> pd.DataFrame:
     """Generate points-level data."""
     n = generate_n(n_trials, options)
-    _hits = hits(n, threshold, slope, guess_rate, lapse_rate)
+    _hits = hits(
+        n,
+        params,
+    )
     points = pd.concat([n, _hits], axis=1)
     _hit_rate = hit_rate(points)
-    return pd.concat([points, _hit_rate], axis=1)
+    logit_hit_rate = pd.Series(
+        logit(_hit_rate),
+        name="logit(Hit Rate)",
+        index=n.index,
+    )
+    return pd.concat([points, _hit_rate, logit_hit_rate], axis=1)
 
 
 def generate_point(n: int, p: float) -> int:
     """Sample n hits from n trials and probability p from binomial dist."""
     return np.random.default_rng().binomial(n, p)
 
 
@@ -203,31 +183,31 @@
         ],
         id="experiment-psych-table",
     )
 
 
 def from_store(store_data: str) -> pd.DataFrame:
     """Get points-level measures from trials-level data store."""
-    _trials = trials.from_store(store_data)
-    return from_trials(_trials).to_frame()
+    trials = pa_trials.from_store(store_data)
+    return from_trials(trials)
 
 
 def combine_plots(fig1: go.Figure, fig2: go.Figure) -> go.Figure:
     """Combine two points-level plots. Possible duplicate."""
     return go.Figure(data=fig1.data + fig2.data)
 
 
 def n(trials: pd.Series) -> pd.Series:
     """Count trials at each point."""
     return pd.Series(trials.value_counts(), name="n")
 
 
-def generate_n(n_trials: int, options: list[float]) -> pd.Series:
+def generate_n(n_trials: int, options: pd.Index) -> pd.Series:
     """Simulate how many trials were performed per intensity level."""
-    return n(trials.generate_n(n_trials, options))
+    return n(pa_trials.generate_trial_index(n_trials, options))
 
 
 def to_block(points: pd.DataFrame) -> pd.DataFrame:
     """Aggregate to block-level measures from points-level data."""
     return points.groupby(level="Block").sum()
 
 
@@ -240,26 +220,45 @@
 ) -> float:
     """Calculate psi for an array of intensity levels x."""
     return gamma + (1 - gamma - lambda_) / (
         1 + np.exp(-gamma * (x - threshold) / width) ** lambda_
     )
 
 
-def plot(points: pd.DataFrame) -> go.Figure:
+def plot(points: pd.DataFrame, y: str) -> go.Figure:
     """Plot the psychometric function."""
     return px.scatter(
         points.reset_index(),
         x="Intensity",
-        y="Hit Rate",
+        y=y,
         size="n",
         template="plotly_white",
     )
 
 
 def hit_rate(df: pd.DataFrame) -> pd.Series:
     """Calculate hit rate from hits and number of trials."""
     return pd.Series(df["Hits"] / df["n"], name="Hit Rate")
 
 
 def transform(hit_rate: float, y: str) -> float:
     """Logit transform hit rate."""
     return logit(hit_rate) if y == "alpha" else hit_rate
+
+
+def plot_logistic(logistic: pd.DataFrame, y: str, name: str, color: str) -> go.Scatter:
+    """Plot a smooth logistic function."""
+    logistic = logistic.reset_index()
+    return go.Scatter(
+        x=logistic["Intensity"],
+        y=logistic[y],
+        mode="lines",
+        name=name,
+        marker_color=color,
+    )
+
+
+def generate_index(n_levels: int, x_range: list[float]) -> pd.Index:
+    """Generate evenly-spaced values along the modulated stimulus dimension."""
+    min_x = x_range[0]
+    max_x = x_range[1]
+    return pd.Index(np.linspace(min_x, max_x, n_levels), name="Intensity")
```

### Comparing `psychoanalyze-0.4.9/psychoanalyze/data/sessions.py` & `psychoanalyze-0.5.0/psychoanalyze/data/sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 
 # PsychoAnalyze is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
-# You should have received a copy of the GNU General Public License along with Foobar.
-# If not, see <https://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
 """Utilities for session-level data.
 
 **Sessions** represent a single day of experiments performed by a subject. It may
 contain several blocks.
 """
 from pathlib import Path
```

### Comparing `psychoanalyze-0.4.9/psychoanalyze/data/stimulus.py` & `psychoanalyze-0.5.0/psychoanalyze/data/stimulus.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,13 +5,13 @@
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 
 # PsychoAnalyze is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
-# You should have received a copy of the GNU General Public License along with Foobar.
-# If not, see <https://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
 """Constants for dimension labels."""
 ref_dims = ["Amp2", "Width2", "Freq2", "Dur2"]
 comp_dims = ["Amp1", "Width1", "Freq1", "Dur1"]
```

### Comparing `psychoanalyze-0.4.9/psychoanalyze/data/subjects.py` & `psychoanalyze-0.5.0/psychoanalyze/data/subjects.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 
 # PsychoAnalyze is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
-# You should have received a copy of the GNU General Public License along with Foobar.
-# If not, see <https://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
 """Data transformation functions for subject-level data."""
 import string
 from pathlib import Path
 
 import pandas as pd
```

### Comparing `psychoanalyze-0.4.9/psychoanalyze/data/trials.py` & `psychoanalyze-0.5.0/psychoanalyze/data/trials.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,57 +5,62 @@
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 
 # PsychoAnalyze is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
-# You should have received a copy of the GNU General Public License along with Foobar.
-# If not, see <https://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
 """Functions for data manipulations at the trial level."""
 import json
 import random
 from pathlib import Path
 from typing import TypedDict
 
 import numpy as np
 import pandas as pd
-from pandera import SeriesSchema
+from pandera import SeriesSchema, check_output
 from sklearn.linear_model import LogisticRegression
 
 from psychoanalyze.data import types
 
 schema = SeriesSchema(bool, name="Test Trials")
 
 data_path = Path("data/trials.csv")
 
 codes = {0: "Miss", 1: "Hit"}
 
 
 Trial = TypedDict("Trial", {"Result": bool, "Stimulus Magnitude": float})
 
 
-def generate_n(n_trials: int, options: list[float]) -> pd.Series:
+def generate_trial_index(n_trials: int, options: pd.Index) -> pd.Series:
     """Generate n trials (no outcomes)."""
     return pd.Series(
         [random.choice(options) for _ in range(n_trials)],
         name="Intensity",
     )
 
 
+@check_output(types.trials)
 def generate(
-    n: pd.Series,
-    outcomes: list[int],
-) -> pd.Series:
+    n_trials: int,
+    options: pd.Index,
+    params: dict[str, float],
+) -> pd.DataFrame:
     """Generate n trials with outcomes."""
-    return pd.Series(
-        [random.choice(outcomes) for _ in range(n)],
-        name="Result",
-        index=n,
+    x = generate_trial_index(n_trials, options)
+    p = {option: psi(option, params) for option in options}
+    return pd.DataFrame(
+        {
+            "Result": [int(random.random() <= p[x_val]) for x_val in x],
+            "Intensity": x,
+        },
     )
 
 
 def load(data_path: Path = Path("data")) -> pd.DataFrame:
     """Load trials data from csv."""
     return types.trials.validate(
         pd.read_csv(
@@ -116,34 +121,37 @@
 
 
 def labels(results: list[int]) -> list[str]:
     """Convert a list of outcome codes to their labels."""
     return [codes[result] for result in results]
 
 
-def psi(gamma: float, lambda_: float, k: float, intensity: float, x_0: float) -> float:
+def psi(intensity: float, params: dict[str, float]) -> float:
     """Calculate the value of the psychometric function for a given intensity."""
+    gamma = params["Guess Rate"]
+    lambda_ = params["Lapse Rate"]
+    k = params["Slope"]
+    x_0 = params["Threshold"]
     return gamma + (1 - gamma - lambda_) * (1 / (1 + np.exp(-k * (intensity - x_0))))
 
 
 def moc_sample(n_trials: int, model_params: dict[str, float]) -> pd.DataFrame:
     """Sample results from a method-of-constant-stimuli experiment."""
     x_0 = model_params["x_0"]
     k = model_params["k"]
-    gamma = model_params["gamma"]
-    lambda_ = model_params["lambda"]
     intensity_choices = np.linspace(x_0 - 4 / k, x_0 + 4 / k, 7)
     intensities = [float(random.choice(intensity_choices)) for _ in range(n_trials)]
     intensity_index = pd.Index(intensities, name="Intensity")
     results = [
-        int(random.random() <= psi(gamma, lambda_, k, intensity, x_0))
+        int(random.random() <= psi(intensity, model_params))
         for intensity in intensities
     ]
     return pd.DataFrame(
         {"Result": pd.Series(results, dtype=int)},
         index=intensity_index,
     )
 
 
-def fit(trials: pd.DataFrame) -> pd.DataFrame:
+def fit(trials: pd.DataFrame) -> dict[str, float]:
     """Fit trial data using logistic regression."""
-    return LogisticRegression().fit(trials[["Intensity"]], trials["Result"])
+    fits = LogisticRegression().fit(trials[["Intensity"]], trials["Result"])
+    return {"Threshold": -fits.intercept_[0], "Slope": fits.coef_[0][0]}
```

### Comparing `psychoanalyze-0.4.9/psychoanalyze/data/types.py` & `psychoanalyze-0.5.0/psychoanalyze/data/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,83 +5,71 @@
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 
 # PsychoAnalyze is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
-# You should have received a copy of the GNU General Public License along with Foobar.
-# If not, see <https://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
 """Pandera schemas for psychoanalyze dataframes.
 
 Contains data table schemas of the hierarchical entities described above.
 """
-from pandera import Column, DataFrameModel, DataFrameSchema, Index, MultiIndex, typing
+from pandera import (
+    Column,
+    DataFrameModel,
+    DataFrameSchema,
+    Index,
+    MultiIndex,
+    typing,
+)
 
 session_dims = ["Monkey", "Date"]
 block_stim_dims = ["Amp2", "Width2", "Freq2", "Dur2"]
 block_channel_dims = ["Active Channels", "Return Channels"]
 block_dims = block_stim_dims + block_channel_dims
 point_dims = ["Amp1", "Width1", "Freq1", "Dur1"]
 
 block_index_levels = session_dims + block_dims
 points_index_levels = block_index_levels + point_dims
 
 
 points = DataFrameSchema(
     {
         "n": Column(int),
-        "Intensity": Column(float),
         "Hits": Column(int),
+        "Hit Rate": Column(float),
+        "logit(Hit Rate)": Column(float),
     },
+    index=Index(float, name="Intensity", unique=True),
 )
 
-trials_schema = DataFrameSchema(
-    columns={"Intensity": Column(float), "Outcome": Column(str, required=False)},
-    index=Index(int, name="TrialID"),
-)
-
-
-points_schema = DataFrameSchema(
+trials = DataFrameSchema(
     columns={
         "Intensity": Column(float),
-        "n": Column(int),
-        "Hits": Column(int),
-        "Hit Rate": Column(float, required=False),
+        "Result": Column(int),
     },
 )
 
+
 blocks = DataFrameSchema(
     columns={"Threshold": Column(dtype=float), "width": Column(dtype=float)},
     index=MultiIndex(
         [
             Index(str, name="Monkey"),
             Index("datetime64", name="Date", coerce=True),
         ]
         + [Index(float, name=dim) for dim in block_stim_dims]
         + [Index(int, name=dim) for dim in block_channel_dims],
     ),
 )
 
 
-trials = DataFrameSchema(
-    {"Result": Column(int, coerce=True)},
-    index=MultiIndex(
-        [
-            Index(str, name="Monkey"),
-            Index("datetime64", name="Date", coerce=True),
-        ]
-        + [Index(float, name=dim) for dim in block_stim_dims]
-        + [Index(int, name=dim) for dim in block_channel_dims]
-        + [Index(float, name=dim) for dim in point_dims],
-    ),
-    coerce=True,
-)
-
 psi_animation = DataFrameSchema(
     {
         "Trial": Column(int),
         "Intensity": Column(float),
         "Hit Rate": Column(float),
     },
 )
```

### Comparing `psychoanalyze-0.4.9/psychoanalyze/plot.py` & `psychoanalyze-0.5.0/psychoanalyze/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 
 # PsychoAnalyze is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
-# You should have received a copy of the GNU General Public License along with Foobar.
-# If not, see <https://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
 """Global plot settings and generic plot utilities."""
 from plotly import graph_objects as go
 
 axis_settings = {
     "ticks": "outside",
     "showgrid": False,
```

### Comparing `psychoanalyze-0.4.9/psychoanalyze/sigmoids.py` & `psychoanalyze-0.5.0/psychoanalyze/sigmoids.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 
 # PsychoAnalyze is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
-# You should have received a copy of the GNU General Public License along with Foobar.
-# If not, see <https://www.gnu.org/licenses/>.
+# You should have received a copy of the GNU General Public License along with
+# PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
 """Sigmoid functions used in the psychometric function."""
 from typing import Any
 
 import numpy as np
```

### Comparing `psychoanalyze-0.4.9/pyproject.toml` & `psychoanalyze-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "psychoanalyze"
-version = "0.4.9"
+version = "0.5.0"
 description = "A Pythonic analysis package for psychophysics data"
 authors = ["Ty Schlichenmeyer <t.schlic@wustl.edu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.11.4"
 pandas = "^2.0.2"
 scipy = "^1.10.1"
 numpy = "^1.25.0"
 dash-bootstrap-components = "^1.4.1"
 statsmodels = "^0.14.0"
 dash-daq = "^0.5.0"
-dash = "^2.10.2"
+dash = "^2.11.1"
 dbt-duckdb = "^1.5.1"
 scikit-learn = "^1.2.2"
 bambi = "^0.11.0"
 cmdstanpy = "^1.1.0"
 pandas-stubs = "^2.0.2.230605"
 pandera = {extras = ["mypy"], version = "^0.15.1"}
 pytest = "^7.3.2"
@@ -26,29 +26,28 @@
 datatest = "^0.11.1"
 pytest-mock = "^3.11.1"
 gunicorn = "^20.1.0"
 mypy = "^1.4.1"
 click = "^8.1.3"
 typer = {extras = ["all"], version = "^0.9.0"}
 tuna = "^0.5.11"
-nbdev = "^2.3.12"
 ruff = "^0.0.276"
 black = "^23.3.0"
 mkdocs = "^1.4.3"
 mkdocs-material = "^9.1.18"
 mkdocstrings = {extras = ["python"], version = "^0.22.0"}
+ipykernel = "^6.24.0"
+ipywidgets = "^8.0.7"
+kaleido = "0.2.1"
+pyarrow = "^12.0.1"
 
 [tool.poetry.scripts]
 psychoanalyze = "psychoanalyze.__main__:main"
 
 
-[tool.poetry.group.dev.dependencies]
-ipython = "^8.14.0"
-ipykernel = "^6.23.2"
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = [
     "psychoanalyze/__init__.py:__version__",
@@ -59,17 +58,15 @@
 major_on_zero = true
 
 [tool.bandit]
 targets = ["psychoanalyze/"]
 skips = ["B311", "B104"]
 
 [tool.mypy]
-exclude = [
-    'target'
-]
+exclude = ['target']
 
 [[tool.mypy.overrides]]
 module = [
     'dash',
     'plotly.*',
     'dash_bootstrap_components',
     'plotly.express',
```

### Comparing `psychoanalyze-0.4.9/PKG-INFO` & `psychoanalyze-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 Metadata-Version: 2.1
 Name: psychoanalyze
-Version: 0.4.9
+Version: 0.5.0
 Summary: A Pythonic analysis package for psychophysics data
 License: GPL-3.0-or-later
 Author: Ty Schlichenmeyer
 Author-email: t.schlic@wustl.edu
 Requires-Python: ==3.11.4
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: bambi (>=0.11.0,<0.12.0)
 Requires-Dist: black (>=23.3.0,<24.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cmdstanpy (>=1.1.0,<2.0.0)
-Requires-Dist: dash (>=2.10.2,<3.0.0)
+Requires-Dist: dash (>=2.11.1,<3.0.0)
 Requires-Dist: dash-bootstrap-components (>=1.4.1,<2.0.0)
 Requires-Dist: dash-daq (>=0.5.0,<0.6.0)
 Requires-Dist: datatest (>=0.11.1,<0.12.0)
 Requires-Dist: dbt-duckdb (>=1.5.1,<2.0.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: hypothesis (>=6.79.0,<7.0.0)
+Requires-Dist: ipykernel (>=6.24.0,<7.0.0)
+Requires-Dist: ipywidgets (>=8.0.7,<9.0.0)
+Requires-Dist: kaleido (==0.2.1)
 Requires-Dist: mkdocs (>=1.4.3,<2.0.0)
 Requires-Dist: mkdocs-material (>=9.1.18,<10.0.0)
 Requires-Dist: mkdocstrings[python] (>=0.22.0,<0.23.0)
 Requires-Dist: mypy (>=1.4.1,<2.0.0)
-Requires-Dist: nbdev (>=2.3.12,<3.0.0)
 Requires-Dist: numpy (>=1.25.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pandas-stubs (>=2.0.2.230605,<3.0.0.0)
 Requires-Dist: pandera[mypy] (>=0.15.1,<0.16.0)
+Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
 Requires-Dist: pytest (>=7.3.2,<8.0.0)
 Requires-Dist: pytest-mock (>=3.11.1,<4.0.0)
 Requires-Dist: ruff (>=0.0.276,<0.0.277)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Requires-Dist: tuna (>=0.5.11,<0.6.0)
@@ -40,15 +43,14 @@
 
 # PsychoAnalyze
 
 Psychophysics analysis in Python.
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/psychoanalyze)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]()
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 [![Open in Remote - Containers](https://img.shields.io/static/v1?label=Remote%20-%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/psychoanalyze/psychoanalyze)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/psychoanalyze/psychoanalyze/main.svg)](https://results.pre-commit.ci/latest/github/psychoanalyze/psychoanalyze/main)
 
 
 
 ## Installation
```

