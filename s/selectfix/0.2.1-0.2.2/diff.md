# Comparing `tmp/selectfix-0.2.1.tar.gz` & `tmp/selectfix-0.2.2.tar.gz`

## Comparing `selectfix-0.2.1.tar` & `selectfix-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 selectfix-0.2.1/Cargo.toml
--rw-r--r--   0     1001      123     1209 2023-04-14 04:29:21.000000 selectfix-0.2.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     1046 2023-04-14 04:29:21.000000 selectfix-0.2.1/.github/workflows/_workflow.yml
--rw-r--r--   0     1001      123      685 2023-04-14 04:29:21.000000 selectfix-0.2.1/.gitignore
--rw-r--r--   0     1001      123      125 2023-04-14 04:29:21.000000 selectfix-0.2.1/README.md
--rw-r--r--   0     1001      123      313 2023-04-14 04:29:21.000000 selectfix-0.2.1/pyproject.toml
--rwxr-xr-x   0     1001      123     1058 2023-04-14 04:31:36.000000 selectfix-0.2.1/run-maturin-action.sh
--rw-r--r--   0     1001      123     6268 2023-04-14 04:29:21.000000 selectfix-0.2.1/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-04-14 04:29:21.000000 selectfix-0.2.1/tests/__init__.py
--rw-r--r--   0     1001      123     2461 2023-04-14 04:29:21.000000 selectfix-0.2.1/tests/test_selectfix.py
--rw-r--r--   0     1001      123     8559 2023-04-14 04:29:21.000000 selectfix-0.2.1/Cargo.lock
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 selectfix-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 selectfix-0.2.2/Cargo.toml
+-rw-r--r--   0     1001      123     1272 2023-07-14 06:46:14.000000 selectfix-0.2.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     1046 2023-07-14 06:46:14.000000 selectfix-0.2.2/.github/workflows/_workflow.yml
+-rw-r--r--   0     1001      123      685 2023-07-14 06:46:14.000000 selectfix-0.2.2/.gitignore
+-rw-r--r--   0     1001      123      125 2023-07-14 06:46:14.000000 selectfix-0.2.2/README.md
+-rw-r--r--   0     1001      123      313 2023-07-14 06:46:14.000000 selectfix-0.2.2/pyproject.toml
+-rw-r--r--   0     1001      123     8854 2023-07-14 06:46:14.000000 selectfix-0.2.2/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-07-14 06:46:14.000000 selectfix-0.2.2/tests/__init__.py
+-rw-r--r--   0     1001      123     2893 2023-07-14 06:46:14.000000 selectfix-0.2.2/tests/test_selectfix.py
+-rw-r--r--   0     1001      123     8559 2023-07-14 06:46:14.000000 selectfix-0.2.2/Cargo.lock
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 selectfix-0.2.2/PKG-INFO
```

### Comparing `selectfix-0.2.1/.github/workflows/CI.yml` & `selectfix-0.2.2/.github/workflows/CI.yml`

 * *Files 14% similar despite different names*

```diff
@@ -24,19 +24,22 @@
     uses: ./.github/workflows/_workflow.yml
     with:
       runs-on: windows-latest
       maturin-target: x64
       maturin-build-args: --release -o dist --find-interpreter
 
   macos:
+    strategy:
+      matrix:
+        target: [x86_64, aarch64]
     uses: ./.github/workflows/_workflow.yml
     with:
       runs-on: macos-latest
-      maturin-target: x86_64
-      maturin-build-args: --release -o dist --universal2 --find-interpreter
+      maturin-target: ${{ matrix.target }}
+      maturin-build-args: --release -o dist --find-interpreter
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
     needs: [ macos, windows, linux ]
     steps:
```

### Comparing `selectfix-0.2.1/.github/workflows/_workflow.yml` & `selectfix-0.2.2/.github/workflows/_workflow.yml`

 * *Files identical despite different names*

### Comparing `selectfix-0.2.1/.gitignore` & `selectfix-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `selectfix-0.2.1/src/lib.rs` & `selectfix-0.2.2/src/lib.rs`

 * *Files 20% similar despite different names*

```diff
@@ -3,25 +3,32 @@
 use pyo3::types::PyBytes;
 
 use anyhow::Result;
 use bincode::{deserialize, serialize};
 use ordered_float::OrderedFloat;
 use serde::{Deserialize, Serialize};
 use std::cmp;
+use std::collections::HashMap;
 
+/// A selector for the fixed value.
+/// This class selects the variables which are closest to the fixed value.
 #[derive(Serialize, Deserialize)]
 #[pyclass(module = "selectfix")]
 struct Selector {
     #[pyo3(get)]
     n_select: usize,
     #[pyo3(get)]
     candidates: Vec<String>,
     #[pyo3(get)]
     exclude_free: Vec<Vec<String>>,
+    #[pyo3(get)]
     fixed_val: f64,
+    #[pyo3(get)]
+    ranges: HashMap<String, (f64, f64)>,
+    #[pyo3(get)]
     eps: f64,
 }
 
 impl Selector {
     fn is_excluded(&self, names: Vec<&String>) -> bool {
         self.exclude_free
             .iter()
@@ -48,85 +55,138 @@
                 return (tmp_searched, res);
             }
         }
         (close_idxs, false)
     }
     fn compute_indices(
         &self,
-        xdic: IndexMap<String, f64>,
+        xdic: &IndexMap<String, f64>,
     ) -> Result<(Vec<usize>, Vec<OrderedFloat<f64>>)> {
-        let xdic = if self.candidates.is_empty() {
-            xdic
+        let xdic_new = if self.candidates.is_empty() {
+            xdic.clone()
         } else {
+            // Extract the candidates from xdic.
             self.candidates
                 .iter()
                 .map(|can| (can.clone(), xdic[can]))
                 .collect::<IndexMap<_, _>>()
         };
-        let violations = xdic
+        let violations = xdic_new
             .iter()
             .map(|(_, &x)| {
                 cmp::min(
                     OrderedFloat(-(x - self.fixed_val).abs() + self.eps),
                     OrderedFloat(0.0),
                 )
             })
             .collect::<Vec<_>>();
         let mut indices = (0..violations.len()).collect::<Vec<_>>();
         indices.sort_by(|&i, &j| violations[i].cmp(&violations[j]));
         if self.exclude_free.len() > 0 {
             let (searched, res) =
-                self.search_free(indices.clone(), &xdic.keys().cloned().collect(), vec![]);
+                self.search_free(indices.clone(), &xdic_new.keys().cloned().collect(), vec![]);
             if !res {
                 return Err(anyhow::anyhow!(
                     "Not found the selections with the given exclude_free.",
                 ));
             }
             indices = searched;
         }
         indices.reverse();
         Ok((indices, violations))
     }
 }
 
 #[pymethods]
 impl Selector {
+    /// Create a new selector.
+    ///
+    /// # Arguments
+    /// * `n_select` - The number of variables to be selected to fix.
+    /// * `candidates` - Candidates for selection.
+    /// * `exclude_free` - Combinations you want to exclude among non-fixed variables.
+    /// * `fixed_val` - Target value of variable to be fixed.
+    /// * `ranges` - Range to be set on unfixed variables.
+    /// * `eps` - Tolerance for fixed variables and fixed_val.
     #[new]
     fn new(
         n_select: usize,
         candidates: Vec<String>,
         exclude_free: Vec<Vec<String>>,
         fixed_val: f64,
+        ranges: HashMap<String, (f64, f64)>,
         eps: f64,
     ) -> Self {
         Selector {
             n_select: n_select,
             candidates: candidates,
             exclude_free: exclude_free,
             fixed_val: fixed_val,
+            ranges: ranges,
             eps: eps,
         }
     }
     fn __call__(&self, xdic: IndexMap<String, f64>) -> PyResult<f64> {
         let (indices, violations) = self
-            .compute_indices(xdic)
+            .compute_indices(&xdic)
             .map_err(|e| pyo3::exceptions::PyValueError::new_err(e.to_string()))?;
+        // Compute the additional penalty.
+        // This is the penalty for the variables which are not selected.
+        // The penalty is the minimum of the distance from the fixed value to the lower and upper bounds.
+        let additional: f64 = if self.candidates.is_empty() || self.ranges.is_empty() {
+            0.0
+        } else {
+            (self.n_select..indices.len())
+                .map(|i| {
+                    let key = &self.candidates[indices[i]];
+                    if let (Some(range), Some(x)) = (self.ranges.get(key), xdic.get(key)) {
+                        if range.0 <= *x && *x <= range.1 {
+                            0.0
+                        } else {
+                            cmp::min(
+                                OrderedFloat((range.0 - x).abs()),
+                                OrderedFloat((range.1 - x).abs()),
+                            )
+                            .0
+                        }
+                    } else {
+                        0.0
+                    }
+                })
+                .sum()
+        };
         Ok((0..self.n_select)
             .map(|i| f64::from(violations[indices[i]]))
-            .sum())
+            .sum::<f64>()
+            - additional)
     }
     fn jacobian(&self, xdic: IndexMap<String, f64>) -> PyResult<Vec<f64>> {
         let ndim = xdic.len();
         let (indices, _) = self
-            .compute_indices(xdic)
+            .compute_indices(&xdic)
             .map_err(|e| pyo3::exceptions::PyValueError::new_err(e.to_string()))?;
         let mut jac = vec![0.0; ndim];
         for i in 0..self.n_select {
             jac[indices[i]] = 1.0;
         }
+        if self.candidates.is_empty() || self.ranges.is_empty() {
+            return Ok(jac);
+        }
+        for i in self.n_select..indices.len() {
+            let key = &self.candidates[indices[i]];
+            if let (Some(range), Some(x)) = (self.ranges.get(key), xdic.get(key)) {
+                if range.0 <= *x && *x <= range.1 {
+                    jac[indices[i]] = 0.0;
+                } else {
+                    jac[indices[i]] = if range.0 < *x { -1.0 } else { 1.0 };
+                }
+            } else {
+                jac[indices[i]] = 0.0;
+            }
+        }
         Ok(jac)
     }
     fn hessian(&self, xdic: IndexMap<String, f64>) -> PyResult<Vec<Vec<f64>>> {
         Ok(vec![vec![0.0; xdic.len()]; xdic.len()])
     }
     fn __setstate__(&mut self, _py: Python, state: &PyBytes) -> PyResult<()> {
         *self = deserialize(state.as_bytes()).unwrap();
@@ -164,14 +224,15 @@
                 "a".to_string(),
                 "b".to_string(),
                 "c".to_string(),
                 "d".to_string(),
             ],
             vec![vec!["a".to_string(), "b".to_string()]],
             0.0,
+            HashMap::new(),
             0.0,
         );
         assert_eq!(
             selector.is_excluded(vec![&"a".to_string(), &"b".to_string()]),
             true
         );
         assert_eq!(selector.is_excluded(vec![&"a".to_string()]), false);
@@ -190,14 +251,15 @@
                 "a".to_string(),
                 "b".to_string(),
                 "c".to_string(),
                 "d".to_string(),
             ],
             vec![vec!["a".to_string(), "b".to_string()]],
             0.0,
+            HashMap::new(),
             0.0,
         );
         let (searched, res) = selector.search_free(
             vec![0, 1, 2, 3],
             &vec![
                 "a".to_string(),
                 "b".to_string(),
```

### Comparing `selectfix-0.2.1/tests/test_selectfix.py` & `selectfix-0.2.2/tests/test_selectfix.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,60 @@
 import unittest
 
 import numpy as np
 
 import selectfix
 
 class TestSelectfix(unittest.TestCase):
-    def test_selectfix(self):
-        sel = selectfix.Selector(2, [], [], 0.0, 0.0)
+    def test_selectfix_basic(self):
+        sel = selectfix.Selector(2, [], [], 0.0, {}, 0.0)
         val = sel({"x1": 10, "x2": 10, "x3": 0, "x4": 0})
         assert val == 0
         val = sel({"x1": 10, "x2": 10, "x3": 10, "x4": 0})
         assert val == -10
         val = sel({"x1": 10, "x2": 10, "x3": 10, "x4": 10})
         assert val == -20
 
-        sel = selectfix.Selector(1, ["x1", "x2", "x3"], [], 0.0, 0.0)
+    def test_selectfix_jacobian(self):
+        sel = selectfix.Selector(1, ["x1", "x2", "x3"], [], 0.0, {}, 0.0)
         val = sel({"x1": 10, "x2": 10, "x3": 0, "x4": 0})
         assert val == 0
         val = sel({"x1": 10, "x2": 10, "x3": 10, "x4": 0})
         assert val == -10
         val = sel({"x1": 10, "x2": 10, "x3": 10, "x4": 10})
         assert val == -10
         np.testing.assert_array_equal(sel.jacobian({"x1": 10, "x2": 10, "x3": 10, "x4": 0}), np.array([0, 0, 1, 0]))
         np.testing.assert_array_equal(sel.jacobian({"x1": 10, "x2": 10, "x3": 0, "x4": 0}), np.array([0, 0, 1, 0]))
         np.testing.assert_array_equal(sel.hessian({"x1": 10, "x2": 10, "x3": 0, "x4": 0}), np.zeros((4, 4)))
 
-        sel = selectfix.Selector(1, ["x1", "x2", "x3"], [["x1", "x2"]], 0.0, 0.0)
+    def test_selectfix_using_exclude_free(self):
+        sel = selectfix.Selector(1, ["x1", "x2", "x3"], [["x1", "x2"]], 0.0, {}, 0.0)
         val = sel({"x1": 10, "x2": 10, "x3": 0, "x4": 0})
         assert val == -10
         np.testing.assert_array_equal(sel.jacobian({"x1": 10, "x2": 10, "x3": 0, "x4": 0}), np.array([0, 1, 0, 0]))
         np.testing.assert_array_equal(sel.hessian({"x1": 10, "x2": 10, "x3": 0, "x4": 0}), np.zeros((4, 4)))
 
-        sel = selectfix.Selector(1, ["x1", "x2", "x3"], [["x1", "x2"], ["x2", "x3"]], 0.0, 0.0)
+        sel = selectfix.Selector(1, ["x1", "x2", "x3"], [["x1", "x2"], ["x2", "x3"]], 0.0, {}, 0.0)
         val = sel({"x1": 10, "x2": 11, "x3": 12, "x4": 0})
         assert val == -11
         np.testing.assert_array_equal(sel.jacobian({"x1": 10, "x2": 10, "x3": 0, "x4": 0}), np.array([0, 1, 0, 0]))
         np.testing.assert_array_equal(sel.hessian({"x1": 10, "x2": 10, "x3": 0, "x4": 0}), np.zeros((4, 4)))
 
         sel = selectfix.Selector(
-            2, ["x1", "x2", "x3", "x4", "x5"], [["x1", "x2"], ["x1", "x3"], ["x1", "x4"]], 0.0, 0.0
+            2, ["x1", "x2", "x3", "x4", "x5"], [["x1", "x2"], ["x1", "x3"], ["x1", "x4"]], 0.0, {}, 0.0
         )
         val = sel({"x1": 14, "x2": 13, "x3": 12, "x4": 11, "x5": 10})
         assert val == -24
         np.testing.assert_array_equal(
             sel.jacobian({"x1": 14, "x2": 13, "x3": 12, "x4": 11, "x5": 10}), np.array([1, 0, 0, 0, 1])
         )
         np.testing.assert_array_equal(sel.hessian({"x1": 14, "x2": 13, "x3": 12, "x4": 11, "x5": 10}), np.zeros((5, 5)))
 
+    def test_selectfix_using_range_penalty(self):
+        sel = selectfix.Selector(1, ["x1", "x2", "x3"], [], 0.0, {"x1": (20, 30)}, 0.0)
+        val = sel({"x1": 10, "x2": 10, "x3": 0})
+        assert val == -10
+        np.testing.assert_array_equal(sel.jacobian({"x1": 10, "x2": 10, "x3": 0}), np.array([1, 0, 1]))
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `selectfix-0.2.1/Cargo.lock` & `selectfix-0.2.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "selectfix"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "anyhow",
  "bincode",
  "indexmap",
  "ordered-float",
  "pyo3",
  "serde",
```

