# Comparing `tmp/acryo-0.4.2.tar.gz` & `tmp/acryo-0.4.3.tar.gz`

## Comparing `acryo-0.4.2.tar` & `acryo-0.4.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/__init__.py
--rw-r--r--   0        0        0     6201 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/_dask.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/_reader.py
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/_rotation.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/_typed_scipy.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/_types.py
--rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/_utils.py
--rw-r--r--   0        0        0    21652 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/simulator.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/alignment/__init__.py
--rw-r--r--   0        0        0    32560 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/alignment/_base.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/alignment/_bound.py
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/alignment/_concrete.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/backend/__init__.py
--rw-r--r--   0        0        0    17080 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/backend/_api.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/backend/_bandpass.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/backend/_missing_wedge.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/backend/_pcc.py
--rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/backend/_zncc.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/classification/__init__.py
--rw-r--r--   0        0        0    18578 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/classification/_dask_pca.py
--rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/classification/pca.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/loader/__init__.py
--rw-r--r--   0        0        0    38952 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/loader/_base.py
--rw-r--r--   0        0        0     8085 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/loader/_batch.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/loader/_cache.py
--rw-r--r--   0        0        0    19585 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/loader/_group.py
--rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/loader/_loader.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/loader/_misc.py
--rw-r--r--   0        0        0    10507 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/loader/_mock.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/molecules/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/molecules/_cut.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/molecules/_group.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/molecules/_rotation.py
--rw-r--r--   0        0        0    35292 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/molecules/core.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/pick/__init__.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/pick/_base.py
--rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/pick/_concrete.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/pipe/__init__.py
--rw-r--r--   0        0        0    13063 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/pipe/_classes.py
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/pipe/_curry.py
--rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/pipe/_imread.py
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/pipe/_masking.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/pipe/_transform.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/testing/__init__.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/testing/_templates.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 acryo-0.4.2/acryo/testing/core.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 acryo-0.4.2/.gitignore
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 acryo-0.4.2/LICENSE
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 acryo-0.4.2/README.md
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 acryo-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 acryo-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/__init__.py
+-rw-r--r--   0        0        0     6201 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/_dask.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/_reader.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/_rotation.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/_typed_scipy.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/_types.py
+-rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/_utils.py
+-rw-r--r--   0        0        0    21652 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/simulator.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/alignment/__init__.py
+-rw-r--r--   0        0        0    32639 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/alignment/_base.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/alignment/_bound.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/alignment/_concrete.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/backend/__init__.py
+-rw-r--r--   0        0        0    17080 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/backend/_api.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/backend/_bandpass.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/backend/_missing_wedge.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/backend/_pcc.py
+-rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/backend/_zncc.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/classification/__init__.py
+-rw-r--r--   0        0        0    18578 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/classification/_dask_pca.py
+-rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/classification/pca.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/loader/__init__.py
+-rw-r--r--   0        0        0    38898 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/loader/_base.py
+-rw-r--r--   0        0        0     8085 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/loader/_batch.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/loader/_cache.py
+-rw-r--r--   0        0        0    19585 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/loader/_group.py
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/loader/_loader.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/loader/_misc.py
+-rw-r--r--   0        0        0    10507 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/loader/_mock.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/molecules/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/molecules/_cut.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/molecules/_group.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/molecules/_rotation.py
+-rw-r--r--   0        0        0    35564 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/molecules/core.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/pick/__init__.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/pick/_base.py
+-rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/pick/_concrete.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/pipe/__init__.py
+-rw-r--r--   0        0        0    13063 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/pipe/_classes.py
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/pipe/_curry.py
+-rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/pipe/_imread.py
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/pipe/_masking.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/pipe/_transform.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/testing/__init__.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/testing/_templates.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 acryo-0.4.3/acryo/testing/core.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 acryo-0.4.3/.gitignore
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 acryo-0.4.3/LICENSE
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 acryo-0.4.3/README.md
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 acryo-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 acryo-0.4.3/PKG-INFO
```

### Comparing `acryo-0.4.2/acryo/_dask.py` & `acryo-0.4.3/acryo/_dask.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/_reader.py` & `acryo-0.4.3/acryo/_reader.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/_rotation.py` & `acryo-0.4.3/acryo/_rotation.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/_typed_scipy.py` & `acryo-0.4.3/acryo/_typed_scipy.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/_utils.py` & `acryo-0.4.3/acryo/_utils.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/simulator.py` & `acryo-0.4.3/acryo/simulator.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/alignment/_base.py` & `acryo-0.4.3/acryo/alignment/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -673,15 +673,15 @@
             temp, matrix=matrix, cval=_cval, order=order, prefilter=prefilter
         )
         return self.pre_transform(temp_transformed, backend)
 
     def _get_template_and_mask_input(
         self,
         backend: Backend | None = None,
-    ) -> tuple[_Template, NDArray[np.float32]]:
+    ) -> tuple[_Template, AnyArray[np.float32]]:
         """
         Returns proper template image for alignment.
 
         Template dimensionality will be dispatched according to the input
         parameters. Returned template should be used in line of the
         :func:`get_alignment_function`.
 
@@ -694,14 +694,16 @@
             - has rotation, single template image ... 4D
             - no rotation, many template images ... 4D
             - has rotation, many template images ... 4D and when iterated over
               the first axis yielded images will be (rot0, temp0),
               (rot0, temp1), ...
         """
         xp = backend or Backend()
+        if out := self._template_mask_cache.get(xp):
+            return out
         if self._n_rotations > 1:
             rotators = [Rotation.from_quat(r).inv() for r in self.quaternions]
             matrices = compose_matrices(
                 np.array(self._template.shape[-3:]) / 2 - 0.5, rotators
             )
             cval = float(np.percentile(self._template, 1))
             if self._n_templates > 1:
```

### Comparing `acryo-0.4.2/acryo/alignment/_bound.py` & `acryo-0.4.3/acryo/alignment/_bound.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/alignment/_concrete.py` & `acryo-0.4.3/acryo/alignment/_concrete.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/backend/_api.py` & `acryo-0.4.3/acryo/backend/_api.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/backend/_bandpass.py` & `acryo-0.4.3/acryo/backend/_bandpass.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/backend/_missing_wedge.py` & `acryo-0.4.3/acryo/backend/_missing_wedge.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/backend/_pcc.py` & `acryo-0.4.3/acryo/backend/_pcc.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/backend/_zncc.py` & `acryo-0.4.3/acryo/backend/_zncc.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/classification/_dask_pca.py` & `acryo-0.4.3/acryo/classification/_dask_pca.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/classification/pca.py` & `acryo-0.4.3/acryo/classification/pca.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/loader/_base.py` & `acryo-0.4.3/acryo/loader/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -975,15 +975,15 @@
 
     @overload
     def groupby(
         self, by: Sequence[IntoExpr] | tuple[IntoExpr, ...]
     ) -> LoaderGroup[tuple[str, ...], Self]:
         ...
 
-    def groupby(self, by: IntoExpr | Sequence[IntoExpr] | tuple[IntoExpr, ...]):
+    def groupby(self, by):
         """
         Group loader by given feature column(s).
 
         >>> for key, loader in loader.groupby("score"):
         ...     print(key, loader)
         """
         if isinstance(by, (str, pl.Expr)):
```

### Comparing `acryo-0.4.2/acryo/loader/_batch.py` & `acryo-0.4.3/acryo/loader/_batch.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/loader/_cache.py` & `acryo-0.4.3/acryo/loader/_cache.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/loader/_group.py` & `acryo-0.4.3/acryo/loader/_group.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/loader/_loader.py` & `acryo-0.4.3/acryo/loader/_loader.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/loader/_misc.py` & `acryo-0.4.3/acryo/loader/_misc.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/loader/_mock.py` & `acryo-0.4.3/acryo/loader/_mock.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/molecules/_cut.py` & `acryo-0.4.3/acryo/molecules/_cut.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/molecules/_group.py` & `acryo-0.4.3/acryo/molecules/_group.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/molecules/_rotation.py` & `acryo-0.4.3/acryo/molecules/_rotation.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/molecules/core.py` & `acryo-0.4.3/acryo/molecules/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,17 +259,20 @@
                     f"{len(df)} features were given."
                 )
             self._features = df
         return None
 
     def to_dataframe(self) -> pl.DataFrame:
         """Convert coordinates, rotation and features into a single data frame."""
-        import polars as pl
-
-        rotvec = self.rotvec()
+        if dup := set(self.features.columns).intersection(_CSV_COLUMNS):
+            raise ValueError(
+                "Duplication between feature columns and postion, rotation columns. "
+                f"Features should not contain {dup!r}. Please rename them."
+            )
+        rotvec = self.rotvec().astype(np.float32)
         data = np.concatenate([self.pos, rotvec], axis=1)
         df = pl.DataFrame(data, schema=_CSV_COLUMNS)
         if self._features is not None:
             df = df.with_columns(list(self._features))
         return df
 
     def to_csv(self, save_path: PathLike, float_precision: int | None = 4) -> None:
```

### Comparing `acryo-0.4.2/acryo/pick/_base.py` & `acryo-0.4.3/acryo/pick/_base.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/pick/_concrete.py` & `acryo-0.4.3/acryo/pick/_concrete.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/pipe/__init__.py` & `acryo-0.4.3/acryo/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/pipe/_classes.py` & `acryo-0.4.3/acryo/pipe/_classes.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/pipe/_curry.py` & `acryo-0.4.3/acryo/pipe/_curry.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/pipe/_imread.py` & `acryo-0.4.3/acryo/pipe/_imread.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/pipe/_masking.py` & `acryo-0.4.3/acryo/pipe/_masking.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/pipe/_transform.py` & `acryo-0.4.3/acryo/pipe/_transform.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/testing/_templates.py` & `acryo-0.4.3/acryo/testing/_templates.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/acryo/testing/core.py` & `acryo-0.4.3/acryo/testing/core.py`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/.gitignore` & `acryo-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/LICENSE` & `acryo-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/README.md` & `acryo-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/pyproject.toml` & `acryo-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acryo-0.4.2/PKG-INFO` & `acryo-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acryo
-Version: 0.4.2
+Version: 0.4.3
 Summary: An extensible cryo-EM/ET toolkit for Python.
 Author-email: Hanjin Liu <liuhanjin-sc@g.ecc.u-tokyo.ac.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Hanjin Liu
         All rights reserved.
```

