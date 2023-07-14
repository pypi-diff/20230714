# Comparing `tmp/figaro-1.0.6.tar.gz` & `tmp/figaro-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "figaro-1.0.6.tar", last modified: Mon Mar 13 16:38:36 2023, max compression
+gzip compressed data, was "figaro-1.1.0.tar", last modified: Fri Jul 14 18:00:13 2023, max compression
```

## Comparing `figaro-1.0.6.tar` & `figaro-1.1.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-03-13 16:38:36.859373 figaro-1.0.6/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1072 2022-02-08 13:50:37.000000 figaro-1.0.6/LICENSE
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)       96 2023-03-13 16:37:56.000000 figaro-1.0.6/MANIFEST.in
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-03-13 16:38:36.858788 figaro-1.0.6/PKG-INFO
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4255 2023-02-20 15:52:20.000000 figaro-1.0.6/README.md
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-03-13 16:38:36.845956 figaro-1.0.6/figaro/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)        0 2022-05-05 11:31:57.000000 figaro-1.0.6/figaro/__init__.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2475 2022-05-01 13:54:12.000000 figaro-1.0.6/figaro/coordinates.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)  1000222 2023-03-13 16:06:47.000000 figaro-1.0.6/figaro/cosmology.c
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     3649 2022-11-17 15:54:02.000000 figaro-1.0.6/figaro/cosmology.pxd
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5030 2022-11-17 15:54:02.000000 figaro-1.0.6/figaro/cosmology.pyx
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     7637 2022-05-15 14:27:47.000000 figaro-1.0.6/figaro/credible_regions.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)   297682 2023-03-13 16:06:47.000000 figaro-1.0.6/figaro/cumulative.c
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1911 2022-05-18 11:00:07.000000 figaro-1.0.6/figaro/cumulative.pyx
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1996 2023-03-08 12:59:32.000000 figaro-1.0.6/figaro/decorators.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     8540 2023-01-27 08:07:34.000000 figaro-1.0.6/figaro/diagnostic.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1249 2022-05-18 11:00:07.000000 figaro-1.0.6/figaro/exceptions.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5298 2023-03-13 14:30:31.000000 figaro-1.0.6/figaro/likelihood.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    26409 2023-03-09 17:42:52.000000 figaro-1.0.6/figaro/load.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5022 2023-02-20 15:52:20.000000 figaro-1.0.6/figaro/marginal.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    35503 2023-03-13 14:49:21.000000 figaro-1.0.6/figaro/mixture.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2610 2023-01-31 15:40:41.000000 figaro-1.0.6/figaro/montecarlo.py
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-03-13 16:38:36.857588 figaro-1.0.6/figaro/pipelines/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     6409 2022-05-15 14:27:47.000000 figaro-1.0.6/figaro/pipelines/create_glade.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    16083 2022-12-10 23:30:50.000000 figaro-1.0.6/figaro/pipelines/entropy.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4583 2022-11-17 16:07:28.000000 figaro-1.0.6/figaro/pipelines/gen_mock_data.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    12804 2023-03-09 17:42:52.000000 figaro-1.0.6/figaro/pipelines/hierarchical_inference.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    17267 2023-03-09 17:42:52.000000 figaro-1.0.6/figaro/pipelines/par_hierarchical_inference.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    10092 2023-03-09 17:42:52.000000 figaro-1.0.6/figaro/pipelines/par_probability_density.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    11197 2023-03-09 17:42:52.000000 figaro-1.0.6/figaro/pipelines/ppplot.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     8985 2023-03-09 17:42:52.000000 figaro-1.0.6/figaro/pipelines/probability_density.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    31752 2023-03-09 17:42:52.000000 figaro-1.0.6/figaro/plot.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      607 2023-02-26 09:19:53.000000 figaro-1.0.6/figaro/plot_settings.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    39807 2023-01-26 15:26:12.000000 figaro-1.0.6/figaro/threeDvolume.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2035 2023-03-13 14:57:44.000000 figaro-1.0.6/figaro/transform.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    13917 2023-03-13 10:23:39.000000 figaro-1.0.6/figaro/utils.py
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-03-13 16:38:36.850452 figaro-1.0.6/figaro.egg-info/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-03-13 16:38:36.000000 figaro-1.0.6/figaro.egg-info/PKG-INFO
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      985 2023-03-13 16:38:36.000000 figaro-1.0.6/figaro.egg-info/SOURCES.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)        1 2023-03-13 16:38:36.000000 figaro-1.0.6/figaro.egg-info/dependency_links.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      483 2023-03-13 16:38:36.000000 figaro-1.0.6/figaro.egg-info/entry_points.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)       94 2023-03-13 16:38:36.000000 figaro-1.0.6/figaro.egg-info/requires.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      279 2023-03-13 16:38:36.000000 figaro-1.0.6/figaro.egg-info/top_level.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      477 2023-02-20 15:52:20.000000 figaro-1.0.6/figaro_env.yml
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      565 2023-02-20 15:52:20.000000 figaro-1.0.6/install.sh
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)       93 2023-03-13 15:25:38.000000 figaro-1.0.6/requirements.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)       38 2023-03-13 16:38:36.859534 figaro-1.0.6/setup.cfg
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4919 2023-03-13 16:36:28.000000 figaro-1.0.6/setup.py
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-14 18:00:13.871003 figaro-1.1.0/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1072 2022-02-08 13:50:37.000000 figaro-1.1.0/LICENSE
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      143 2023-07-14 17:53:26.000000 figaro-1.1.0/MANIFEST.in
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-07-14 18:00:13.870517 figaro-1.1.0/PKG-INFO
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4255 2023-02-20 15:52:20.000000 figaro-1.1.0/README.md
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-14 18:00:13.854375 figaro-1.1.0/figaro/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)        0 2022-05-05 11:31:57.000000 figaro-1.1.0/figaro/__init__.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2475 2022-05-01 13:54:12.000000 figaro-1.1.0/figaro/coordinates.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)  1002062 2023-07-14 17:57:15.000000 figaro-1.1.0/figaro/cosmology.c
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     3649 2022-11-17 15:54:02.000000 figaro-1.1.0/figaro/cosmology.pxd
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5144 2023-07-14 17:50:31.000000 figaro-1.1.0/figaro/cosmology.pyx
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     7637 2022-05-15 14:27:47.000000 figaro-1.1.0/figaro/credible_regions.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)   297682 2023-03-13 16:06:47.000000 figaro-1.1.0/figaro/cumulative.c
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1911 2022-05-18 11:00:07.000000 figaro-1.1.0/figaro/cumulative.pyx
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1996 2023-03-08 12:59:32.000000 figaro-1.1.0/figaro/decorators.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     8535 2023-07-07 12:21:05.000000 figaro-1.1.0/figaro/diagnostic.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1249 2023-07-07 12:34:31.000000 figaro-1.1.0/figaro/exceptions.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5301 2023-07-07 12:27:53.000000 figaro-1.1.0/figaro/likelihood.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    26863 2023-07-13 15:53:30.000000 figaro-1.1.0/figaro/load.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5981 2023-07-12 07:21:45.000000 figaro-1.1.0/figaro/marginal.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    41110 2023-07-14 08:28:34.000000 figaro-1.1.0/figaro/mixture.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2610 2023-01-31 15:40:41.000000 figaro-1.1.0/figaro/montecarlo.py
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-14 18:00:13.869010 figaro-1.1.0/figaro/pipelines/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     6409 2022-05-15 14:27:47.000000 figaro-1.1.0/figaro/pipelines/create_glade.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    16259 2023-06-25 09:51:30.000000 figaro-1.1.0/figaro/pipelines/entropy.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4583 2022-11-17 16:07:28.000000 figaro-1.1.0/figaro/pipelines/gen_mock_data.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    12961 2023-06-30 08:48:22.000000 figaro-1.1.0/figaro/pipelines/hierarchical_inference.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    17678 2023-06-30 08:48:22.000000 figaro-1.1.0/figaro/pipelines/par_hierarchical_inference.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    10389 2023-06-25 09:51:30.000000 figaro-1.1.0/figaro/pipelines/par_probability_density.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    11156 2023-03-29 08:52:28.000000 figaro-1.1.0/figaro/pipelines/ppplot.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     9184 2023-07-13 15:25:45.000000 figaro-1.1.0/figaro/pipelines/probability_density.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    31946 2023-07-07 12:44:53.000000 figaro-1.1.0/figaro/plot.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      933 2023-06-27 13:05:57.000000 figaro-1.1.0/figaro/plot_settings.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    39776 2023-07-07 12:44:53.000000 figaro-1.1.0/figaro/threeDvolume.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2236 2023-06-25 09:51:30.000000 figaro-1.1.0/figaro/transform.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    15184 2023-07-14 08:00:31.000000 figaro-1.1.0/figaro/utils.py
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-14 18:00:13.858686 figaro-1.1.0/figaro.egg-info/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-07-14 18:00:13.000000 figaro-1.1.0/figaro.egg-info/PKG-INFO
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1000 2023-07-14 18:00:13.000000 figaro-1.1.0/figaro.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)        1 2023-07-14 18:00:13.000000 figaro-1.1.0/figaro.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      483 2023-07-14 18:00:13.000000 figaro-1.1.0/figaro.egg-info/entry_points.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)       94 2023-07-14 18:00:13.000000 figaro-1.1.0/figaro.egg-info/requires.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      279 2023-07-14 18:00:13.000000 figaro-1.1.0/figaro.egg-info/top_level.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      477 2023-02-20 15:52:20.000000 figaro-1.1.0/figaro_env.yml
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      565 2023-02-20 15:52:20.000000 figaro-1.1.0/install.sh
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)       85 2023-07-14 17:39:59.000000 figaro-1.1.0/pyproject.toml
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)       93 2023-03-13 15:25:38.000000 figaro-1.1.0/requirements.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)       38 2023-07-14 18:00:13.871195 figaro-1.1.0/setup.cfg
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4919 2023-07-14 17:56:03.000000 figaro-1.1.0/setup.py
```

### Comparing `figaro-1.0.6/LICENSE` & `figaro-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `figaro-1.0.6/PKG-INFO` & `figaro-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.0.6
+Version: 1.1.0
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Home-page: https://github.com/sterinaldi/figaro
 Author: Stefano Rinaldi, Walter Del Pozzo, Daniele Sanfratello
 Author-email: stefano.rinaldi@phd.unipi.it, walter.delpozzo@unipi.it, d.sanfratello@studenti.unipi.it
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `figaro-1.0.6/README.md` & `figaro-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `figaro-1.0.6/figaro/coordinates.py` & `figaro-1.1.0/figaro/coordinates.py`

 * *Files identical despite different names*

### Comparing `figaro-1.0.6/figaro/cosmology.c` & `figaro-1.1.0/figaro/cosmology.c`

 * *Files 1% similar despite different names*

```diff
@@ -2483,14 +2483,15 @@
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_struct[] = "struct";
 static const char __pyx_k_unpack[] = "unpack";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_fortran[] = "fortran";
 static const char __pyx_k_memview[] = "memview";
 static const char __pyx_k_Ellipsis[] = "Ellipsis";
+static const char __pyx_k_Planck18[] = "Planck18";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_itemsize[] = "itemsize";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
@@ -2557,14 +2558,15 @@
 static PyObject *__pyx_kp_s_Invalid_shape_in_axis_d_d;
 static PyObject *__pyx_n_s_MemoryError;
 static PyObject *__pyx_kp_s_MemoryView_of_r_at_0x_x;
 static PyObject *__pyx_kp_s_MemoryView_of_r_object;
 static PyObject *__pyx_n_b_O;
 static PyObject *__pyx_kp_s_Out_of_bounds_on_buffer_access_a;
 static PyObject *__pyx_n_s_PickleError;
+static PyObject *__pyx_n_s_Planck18;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
 static PyObject *__pyx_n_s_allocate_buffer;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_c;
@@ -2709,14 +2711,19 @@
 static PyObject *__pyx_pf___pyx_memoryviewslice_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_6figaro_9cosmology_CosmologicalParameters(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_float_0_;
+static PyObject *__pyx_float_0_315;
+static PyObject *__pyx_float_0_674;
+static PyObject *__pyx_float_0_685;
+static PyObject *__pyx_float_neg_1_;
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_112105877;
 static PyObject *__pyx_int_136983863;
 static PyObject *__pyx_int_184977713;
 static PyObject *__pyx_int_neg_1;
 static PyObject *__pyx_tuple_;
@@ -2742,15 +2749,16 @@
 static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__22;
 static PyObject *__pyx_tuple__23;
 static PyObject *__pyx_tuple__24;
 static PyObject *__pyx_tuple__25;
 static PyObject *__pyx_tuple__26;
 static PyObject *__pyx_tuple__27;
-static PyObject *__pyx_codeobj__28;
+static PyObject *__pyx_tuple__28;
+static PyObject *__pyx_codeobj__29;
 /* Late includes */
 
 /* "figaro/cosmology.pyx":7
  * cdef class CosmologicalParameters:
  * 
  *     def __cinit__(self, double h, double om, double ol, double w0, double w1):             # <<<<<<<<<<<<<<
  *         self.h = h
@@ -5271,21 +5279,24 @@
   __Pyx_RefNannySetupContext("DestroyCosmologicalParameters", 0);
 
   /* "figaro/cosmology.pyx":120
  * 
  *     def DestroyCosmologicalParameters(self):
  *         self._DestroyCosmologicalParameters()             # <<<<<<<<<<<<<<
  *         return
+ * 
  */
   ((struct __pyx_vtabstruct_6figaro_9cosmology_CosmologicalParameters *)__pyx_v_self->__pyx_vtab)->_DestroyCosmologicalParameters(__pyx_v_self);
 
   /* "figaro/cosmology.pyx":121
  *     def DestroyCosmologicalParameters(self):
  *         self._DestroyCosmologicalParameters()
  *         return             # <<<<<<<<<<<<<<
+ * 
+ * # Planck 2018 [https://arxiv.org/abs/1807.06209]
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
 
   /* "figaro/cosmology.pyx":119
  *         return self._ComovingVolume(z)
@@ -20758,14 +20769,15 @@
   {&__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_k_Invalid_shape_in_axis_d_d, sizeof(__pyx_k_Invalid_shape_in_axis_d_d), 0, 0, 1, 0},
   {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
   {&__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_k_MemoryView_of_r_at_0x_x, sizeof(__pyx_k_MemoryView_of_r_at_0x_x), 0, 0, 1, 0},
   {&__pyx_kp_s_MemoryView_of_r_object, __pyx_k_MemoryView_of_r_object, sizeof(__pyx_k_MemoryView_of_r_object), 0, 0, 1, 0},
   {&__pyx_n_b_O, __pyx_k_O, sizeof(__pyx_k_O), 0, 0, 0, 1},
   {&__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_k_Out_of_bounds_on_buffer_access_a, sizeof(__pyx_k_Out_of_bounds_on_buffer_access_a), 0, 0, 1, 0},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
+  {&__pyx_n_s_Planck18, __pyx_k_Planck18, sizeof(__pyx_k_Planck18), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
@@ -21075,87 +21087,101 @@
   __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(3, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
   __pyx_tuple__21 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(3, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
 
+  /* "figaro/cosmology.pyx":124
+ * 
+ * # Planck 2018 [https://arxiv.org/abs/1807.06209]
+ * Planck18 = CosmologicalParameters(0.674, 0.315, 0.685, -1., 0.)             # <<<<<<<<<<<<<<
+ */
+  __pyx_tuple__22 = PyTuple_Pack(5, __pyx_float_0_674, __pyx_float_0_315, __pyx_float_0_685, __pyx_float_neg_1_, __pyx_float_0_); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
+
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(3, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(3, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(3, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(3, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(3, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(3, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(3, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(3, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(3, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(3, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__27 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(3, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
-  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(3, 1, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(3, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(3, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_float_0_ = PyFloat_FromDouble(0.); if (unlikely(!__pyx_float_0_)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_float_0_315 = PyFloat_FromDouble(0.315); if (unlikely(!__pyx_float_0_315)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_float_0_674 = PyFloat_FromDouble(0.674); if (unlikely(!__pyx_float_0_674)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_float_0_685 = PyFloat_FromDouble(0.685); if (unlikely(!__pyx_float_0_685)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_float_neg_1_ = PyFloat_FromDouble(-1.); if (unlikely(!__pyx_float_neg_1_)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
@@ -21573,20 +21599,28 @@
  * cimport cython
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "figaro/cosmology.pxd":76
- *     cdef public double ol
- *     cdef public double w0
- *     cdef public double w1             # <<<<<<<<<<<<<<
- *     cdef public double _HubbleParameter(self,double z) nogil
- *     cdef public double _LuminosityDistance_double(self, double z) nogil
+  /* "figaro/cosmology.pyx":124
+ * 
+ * # Planck 2018 [https://arxiv.org/abs/1807.06209]
+ * Planck18 = CosmologicalParameters(0.674, 0.315, 0.685, -1., 0.)             # <<<<<<<<<<<<<<
+ */
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_6figaro_9cosmology_CosmologicalParameters), __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Planck18, __pyx_t_1) < 0) __PYX_ERR(0, 124, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "figaro/cosmology.pyx":1
+ * import numpy as np             # <<<<<<<<<<<<<<
+ * cimport numpy as np
+ * cimport cython
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "View.MemoryView":210
@@ -21605,71 +21639,71 @@
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 287, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(generic);
   __Pyx_DECREF_SET(generic, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 288, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(strided);
   __Pyx_DECREF_SET(strided, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 289, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect);
   __Pyx_DECREF_SET(indirect, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 292, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(contiguous);
   __Pyx_DECREF_SET(contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 293, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":317
```

### Comparing `figaro-1.0.6/figaro/cosmology.pxd` & `figaro-1.1.0/figaro/cosmology.pxd`

 * *Files identical despite different names*

### Comparing `figaro-1.0.6/figaro/cosmology.pyx` & `figaro-1.1.0/figaro/cosmology.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -115,7 +115,10 @@
 
     def ComovingVolume(self, np.ndarray[double, ndim=1, mode="c"] z):
         return self._ComovingVolume(z)
 
     def DestroyCosmologicalParameters(self):
         self._DestroyCosmologicalParameters()
         return
+
+# Planck 2018 [https://arxiv.org/abs/1807.06209]
+Planck18 = CosmologicalParameters(0.674, 0.315, 0.685, -1., 0.)
```

### Comparing `figaro-1.0.6/figaro/credible_regions.py` & `figaro-1.1.0/figaro/credible_regions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.0.6/figaro/cumulative.c` & `figaro-1.1.0/figaro/cumulative.c`

 * *Files identical despite different names*

### Comparing `figaro-1.0.6/figaro/cumulative.pyx` & `figaro-1.1.0/figaro/cumulative.pyx`

 * *Files identical despite different names*

### Comparing `figaro-1.0.6/figaro/decorators.py` & `figaro-1.1.0/figaro/decorators.py`

 * *Files identical despite different names*

### Comparing `figaro-1.0.6/figaro/diagnostic.py` & `figaro-1.1.0/figaro/diagnostic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import numpy as np
 
-from numba import jit, prange
+from numba import njit, prange
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 from matplotlib import rcParams
 from distutils.spawn import find_executable
 
 from figaro.cumulative import fast_cumulative
 from figaro.exceptions import FIGAROException
 from figaro import plot_settings
 
 log2e = np.log2(np.e)
 
-@jit
+@njit
 def angular_coefficient(x, y):
     """
     Angular coefficient obtained from linear regression.
     
     Arguments:
         :np.ndarray x: independent variables
         :np.ndarray y: dependent variables
@@ -78,15 +78,15 @@
     if show:
         plt.show()
     if save:
         fig.savefig(Path(out_folder, name+'_angular_coefficient.pdf'), bbox_inches = 'tight')
     plt.close()
     return S
 
-@jit
+@njit
 def compute_autocorrelation(draws, mean, dx):
     """
     Computes autocorrelation of subsequent draws as <∫(draw[i]-mean)*(draw[i+t]-mean)*dx/∫(draw[i]-mean)**2*dx>
     
     Arguments:
         :np.ndarray draws: evaluated mixtures (2d array)
         :np.ndarray mean:  bin-wise mean of evaluated mixtures (1d array)
@@ -135,15 +135,15 @@
             warnings.warn("The provided lower bound is invalid for at least one draw. {0} will be used instead.".format(x_min))
         else:
             x_min = bounds[0]
         if not bounds[1] <= x_max:
             warnings.warn("The provided upper bound is invalid for at least one draw. {0} will be used instead.".format(x_max))
         else:
             x_max = bounds[1]
-    x  = np.linspace(x_min, x_max, n_points+2)[1:-1]
+    x  = np.linspace(x_min, x_max, n_points)
     dx = x[1] - x[0]
     
     functions = np.array([mix.pdf(x) for mix in draws])
     mean      = np.mean(functions, axis = 0)
     
     taumax, ac = compute_autocorrelation(functions, mean, dx)
```

### Comparing `figaro-1.0.6/figaro/exceptions.py` & `figaro-1.1.0/figaro/exceptions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.0.6/figaro/likelihood.py` & `figaro-1.1.0/figaro/likelihood.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from numba import jit, njit, prange
+from numba import njit, prange
 
 LOG2PI = np.log(2*np.pi)
 
 #-----------#
 # Functions #
 #-----------#
 
@@ -11,15 +11,15 @@
 def inv_jit(M):
   return np.linalg.inv(M)
 
 @njit
 def logdet_jit(M):
     return np.log(np.linalg.det(M))
 
-@jit
+@njit
 def logsumexp_jit(a, b):
     a_max = np.max(a)
     tmp = b * np.exp(a - a_max)
     return np.log(np.sum(tmp)) + a_max
 
 @njit
 def scalar_product(v, M, n):
@@ -36,30 +36,30 @@
     """
     res = 0.
     for i in prange(n):
         for j in prange(n):
             res = res + M[i,j]*v[i]*v[j]
     return res
 
-@jit
+@njit
 def log_norm_1d(x, m, s):
     """
     1D Normal logpdf
     
     Arguments:
         :double x: value
         :double m: mean
         :double s: var
     
     Returns:
         Normal(m,s).logpdf(x)
     """
     return -(x-m)**2/(2*s) - 0.5*np.log(2*np.pi*s)
 
-@jit
+@njit
 def log_norm(x, mu, cov):
     """
     Multivariate Normal logpdf
     
     Arguments:
         :np.ndarray x:   value
         :np.ndarray mu:  mean vector
@@ -69,15 +69,15 @@
         :double: MultivariateNormal(m,s).logpdf(x)
     """
     inv_cov  = inv_jit(cov)
     exponent = -0.5*scalar_product(x-mu, inv_cov, len(mu))
     lognorm  = 0.5*len(mu)*LOG2PI+0.5*logdet_jit(cov)
     return -lognorm+exponent
 
-@jit
+@njit
 def log_norm_int(x, mu, cov_1, inv_cov_1, cov_2):
     """
     Multivariate Normal logpdf (tailored to this problem!)
     See https://arxiv.org/pdf/1811.04751v1.pdf
     
     Arguments:
         :np.ndarray x:         value
@@ -95,15 +95,15 @@
     lognorm    = 0.5*len(mu)*LOG2PI+0.5*(logdet_jit(cov_1) + logdet_jit(cov_2) + logdet_jit(inv_cov_1+inv_cov_2))
     return -lognorm+exponent
 
 #------------#
 # 1D methods #
 #------------#
 
-@jit
+@njit
 def eval_mix_1d(mu, sigma, means, covs):
     """
     Computes N(mu_k| mu, (sigma_k^2+sigma^2) for all the components of a mixture (for predictive likelihood, 1D).
     
     Arguments:
         :np.ndarray mu:    temptative mean of the parent mixture component
         :np.ndarray sigma: temptative variance of the parent mixture component
@@ -111,15 +111,15 @@
         :np.ndarray vars:  variances of the event mixture components
     
     Returns:
         :np.ndarray: probability for each event mixture components
     """
     return np.array([log_norm_1d(means[i,0], mu, sigma+covs[i,0,0]) for i in prange(len(means))])
 
-@jit
+@njit
 def evaluate_mixture_MC_draws_1d(mu, sigma, means, vars, w):
     """
     Computes N(mu_k| mu, (sigma_k^2+sigma^2) for a set of MC draws for mu and sigma.
     
     Arguments:
         :np.ndarray mu:    MC draws for the mean of the parent mixture component
         :np.ndarray sigma: MC draws for the variance of the parent mixture component
@@ -135,15 +135,15 @@
         logP[i] = logsumexp_jit(eval_mix_1d(mu[i], sigma[i], means, vars), b = w)
     return logP
 
 #------------#
 # ND methods #
 #------------#
 
-@jit
+@njit
 def eval_mix(mu, sigma, means, covs):
     """
     Computes N(mu_k| mu, (sigma_k^2+sigma^2) for all the components of a mixture (for predictive likelihood, ND).
     
     Arguments:
         :np.ndarray mu:    temptative mean of the parent mixture component
         :np.ndarray sigma: temptative covariance matrix of the parent mixture component
@@ -152,15 +152,15 @@
     
     Returns:
         :np.ndarray: probability for each event mixture components
     """
     inv_sigma = inv_jit(sigma)
     return np.array([log_norm_int(means[i], mu, sigma, inv_sigma, covs[i]) for i in prange(len(means))])
 
-@jit
+@njit
 def evaluate_mixture_MC_draws(mu, sigma, means, covs, w):
     """
     Computes N(mu_k| mu, (sigma_k^2+sigma^2) for a set of MC draws for mu and sigma.
     
     Arguments:
         :np.ndarray mu:    MC draws for the mean vector of the parent mixture component
         :np.ndarray sigma: MC draws for the covariance matrix of the parent mixture component
```

### Comparing `figaro-1.0.6/figaro/load.py` & `figaro-1.1.0/figaro/load.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,30 +18,42 @@
 supported_waveforms  = ['combined', 'imr', 'seob']
 
 GW_par = {'m1'                 : 'mass_1_source',
           'm2'                 : 'mass_2_source',
           'm1_detect'          : 'mass_1',
           'm2_detect'          : 'mass_2',
           'mc'                 : 'chirp_mass_source',
+          'mc_detect'          : 'chirp_mass',
           'mt'                 : 'total_mass_source',
           'z'                  : 'redshift',
           'q'                  : 'mass_ratio',
+          'eta'                : 'symmetric_mass_ratio',
           'chi_eff'            : 'chi_eff',
           'ra'                 : 'ra',
           'dec'                : 'dec',
           'luminosity_distance': 'luminosity_distance',
           'cos_theta_jn'       : 'cos_theta_jn',
           'cos_tilt_1'         : 'cos_tilt_1',
           'cos_tilt_2'         : 'cos_tilt_2',
+          's1x'                : 'spin_1x',
+          's2x'                : 'spin_2x',
+          's1y'                : 'spin_1y',
+          's2y'                : 'spin_2y',
           's1z'                : 'spin_1z',
           's2z'                : 'spin_2z',
           's1'                 : 'spin_1',
           's2'                 : 'spin_2',
+          'psi'                : 'psi',
+          'cos_iota'           : 'cos_iota',
+          'phase'              : 'phase',
+          'tc'                 : 'geocent_time',
           'snr'                : 'network_matched_filter_snr',
           'far'                : 'far',
+          'log_prior'          : 'log_prior',
+          'log_likelihood'     : 'log_likelihood',
           }
 
 def _find_redshift(omega, dl):
     """
     Find redshift given a luminosity distance and a cosmology using Newton's method
     
     Arguments:
@@ -94,19 +106,19 @@
         par = ['ra', 'dec', 'luminosity_distance']
     if not ext in supported_extensions:
         raise TypeError("File {0}.{1} is not supported".format(name, ext))
     if ext == 'txt' or ext == 'dat':
         if par is not None:
             warnings.warn("Par names (or volume keyword) are ignored for .txt/.dat/.csv files")
         if n_samples > -1:
-            samples = np.atleast_1d(np.genfromtxt(event))
+            samples = np.atleast_1d(np.loadtxt(event))
             s = int(min([n_samples, len(samples)]))
             out = samples[rdstate.choice(np.arange(len(samples)), size = s, replace = False)]
         else:
-            out = np.genfromtxt(event)
+            out = np.loadtxt(event)
     else:
         # Check that a list of parameters is passed
         if par is None:
             raise TypeError("Please provide a list of parameter names you want to load (e.g. ['m1']).")
         # Check that all the parametes are loadable
         if not np.all([p in GW_par.keys() for p in par]):
             wrong_pars = [p for p in par if not p in GW_par.keys()]
@@ -165,23 +177,23 @@
         if not ext in supported_extensions:
             raise TypeError("File {0}.{1} is not supported".format(name, ext))
         
         if ext == 'txt' or ext == 'dat':
             if par is not None:
                 warnings.warn("Par names (or volume keyword) are ignored for .txt/.dat files")
             if n_samples > -1:
-                samples = np.atleast_1d(np.genfromtxt(event))
+                samples = np.atleast_1d(np.loadtxt(event))
                 s = int(min([n_samples, len(samples)]))
                 samples_subset = samples[rdstate.choice(np.arange(len(samples)), size = s, replace = False)]
                 if len(np.shape(samples_subset)) == 1:
                     samples_subset = np.atleast_2d(samples_subset).T
                 events.append(samples_subset)
                     
             else:
-                samples = np.atleast_1d(np.genfromtxt(event))
+                samples = np.atleast_1d(np.loadtxt(event))
                 if len(np.shape(samples)) == 1:
                     samples = np.atleast_2d(samples).T
                 events.append(samples)
                 
         else:
             # Check that a list of parameters is passed
             if par is None:
@@ -250,14 +262,15 @@
     elif snr_threshold is not None:
         if not 'snr' in par:
             par = np.append(par, 'snr')
     
     with h5py.File(Path(event), 'r') as f:
         samples     = []
         loaded_pars = []
+        flag_filter = False
         try:
             try:
                 # LVK R&P mock data challenge
                 try:
                     data = f['MDC']['posterior_samples']
                 # Playground
                 except:
@@ -330,35 +343,31 @@
                                 except:
                                     try:
                                         data = f['C01:SEOBNRv4T_surrogate_LS']['posterior_samples']
                                     except:
                                         data = f['SEOBNRv4T_surrogate_LS']['posterior_samples']
                 
             for name, lab in zip(GW_par.keys(), GW_par.values()):
-                flag_filter = False
                 if name in par:
                     if name == 'snr':
                         try:
-                            if MDC_flag:
-                                snr = np.array(data['snr'])
-                                samples.append(data['snr'])
-                            elif waveform != 'combined':
+                            if MDC_flag or waveform != 'combined':
                                 snr = np.array(data[lab])
                                 samples.append(data[lab])
                             if snr_threshold is not None:
                                 flag_filter = True
                         except:
                             warnings.warn("SNR filter is not available with this dataset.")
-                    if name == 'far' and far_threshold is not None:
+                    elif name == 'far' and far_threshold is not None:
                         try:
                             flag_filter = True
                             far = np.array(data[lab])
                         except:
                             warnings.warn("FAR filter is not available with this dataset.")
-                    if name == 's1':
+                    elif name == 's1':
                         try:
                             samples.append(data[lab])
                         except:
                             samples.append(np.sqrt(data['spin_1x']**2+data['spin_1y']**2+data['spin_1z']**2))
                     elif name == 's2':
                         try:
                             samples.append(data[lab])
@@ -432,14 +441,15 @@
             # Derived quantities
             ss['z']       = np.array([_find_redshift(omega, l) for l in ss['luminosity_distance']])
             ss['m1']      = ss['m1_detect']/(1+ss['z'])
             ss['m2']      = ss['m2_detect']/(1+ss['z'])
             ss['mc']      = (ss['m1']*ss['m2'])**(3./5.)/(ss['m1']+ss['m2'])**(1./5.)
             ss['mt']      = ss['m1']+ss['m2']
             ss['q']       = ss['m2']/ss['m1']
+            ss['eta']     = ss['m1']*ss['m2']/(ss['m1']+ss['m2'])**2
             ss['s1z']     = ss['s1']*ss['cos_tilt_1']
             ss['s2z']     = ss['s2']*ss['cos_tilt_2']
             ss['chi_eff'] = (ss['s1z'] + ss['q']*ss['s2z'])/(1+ss['q'])
 
             for name in GW_par.keys():
                 if name in par:
                     if not (name == 'snr' or name == 'far'):
@@ -454,15 +464,14 @@
                 samples_loaded = np.array(samples)
                 samples = []
                 for pi in par:
                     if not (pi == 'snr' or pi == 'far'):
                         samples.append(samples_loaded[np.where(loaded_pars == pi)[0]].flatten())
                 samples = np.array(samples)
                 samples = samples.T
-
             if n_samples > -1:
                 s = int(min([n_samples, len(samples)]))
                 return samples[rdstate.choice(np.arange(len(samples)), size = s, replace = False)]
             else:
                 return samples
 
 def save_density(draws, folder = '.', name = 'density', ext = 'pkl'):
```

### Comparing `figaro-1.0.6/figaro/marginal.py` & `figaro-1.1.0/figaro/marginal.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 from numba import njit
+from scipy.special import logsumexp
 from figaro.exceptions import FIGAROException
 from figaro.likelihood import log_norm, inv_jit
 from figaro.decorators import probit
 
 @njit
 def _cond_mean_cov(vals, mu1, mu2, s11, s22, s12):
     """
@@ -65,72 +66,86 @@
         return draws
     if np.iterable(draws):
         return np.array([_marginalise(d, axis) for d in draws])
     else:
         return _marginalise(draws, axis)
 
 @probit
-def _condition(mix, vals, dims, norm = True):
+def _condition(mix, vals, dims, norm = True, filter = True, tol = 1e-4):
     """
     Probability density conditioned on specific values of a subset of parameters.
     See:
      * https://stats.stackexchange.com/questions/348941/general-conditional-distributions-for-multivariate-gaussian-mixtures
      * https://stats.stackexchange.com/questions/30588/deriving-the-conditional-distributions-of-a-multivariate-normal-distribution
     
     Arguments:
         :figaro.mixture.mixture mix: mixture
         :iterable vals:              value(s) to condition on
         :int or list of int dims:    dimension(s) associated with given vals (starting from 0)
         :bool norm:                  normalize the distribution
+        :bool filter:                  filter the components with weight < tol
+        :double tol:                   tolerance on the sum of the weights
     
     Returns:
         :figaro.mixture.mixture: the conditioned mixture(s)
     """
     # Circular import
     from figaro.mixture import mixture
     ax   = np.atleast_1d(dims)
     vals = vals[ax]
     dim  = mix.dim - len(ax)
     idx  = np.array([i in ax for i in range(mix.dim)])
     if dim < 1:
         raise FIGAROException("Cannot condition on all dimensions")
-    bounds    = np.delete(mix.bounds, ax, axis = 0)
-    means     = np.zeros(shape = (mix.n_cl, dim))
-    covs      = np.zeros(shape = (mix.n_cl, dim, dim))
-    weights   = np.zeros(shape = mix.n_cl)
+    bounds      = np.delete(mix.bounds, ax, axis = 0)
+    means       = np.zeros(shape = (mix.n_cl, dim))
+    covs        = np.zeros(shape = (mix.n_cl, dim, dim))
+    log_weights = np.zeros(shape = mix.n_cl)
     for i, (mu, cov) in enumerate(zip(mix.means, mix.covs)):
         # Subvectors and submatrices
         mu1 = mu[~idx]
         mu2 = mu[idx]
         s11 = cov[~idx,:][:,~idx]
         s12 = cov[idx,:][:,~idx]
         s22 = cov[idx,:][:,idx]
         # Parameters
-        means[i], covs[i] = _cond_mean_cov(vals, mu1, mu2, s11, s22, s12)
-        weights[i] = np.exp(log_norm(vals, mu2, s22))
+        means[i], covs[i] = _cond_mean_cov(vals, mu1, mu2, s11, s22, s12.T)
+        log_weights[i]    = log_norm(vals, mu2, s22)
     # Weights
-    weights = mix.w*weights
+    log_weights = mix.log_w + log_weights
     if norm:
-        weights /= _marginalise(mix, axis = np.arange(mix.dim)[~idx]).pdf(vals)
-    return mixture(means, covs, weights, bounds, dim, mix.n_cl, mix.n_pts, probit = mix.probit)
+        log_weights -= _marginalise(mix, axis = np.arange(mix.dim)[~idx])._logpdf_probit(vals)
+    # Filter out components with negligible weights
+    idx_filt = [True for _ in range(len(log_weights))]
+    norm_const = 0.
+    if filter:
+        ww = np.exp(log_weights)
+        idx = np.argsort(ww)
+        m = np.where(np.cumsum(ww[idx]) > tol*np.sum(ww))[0].min()
+        idx_filt = [i in idx[m:] for i in range(len(ww))]
+        if norm:
+            log_weights -= logsumexp(log_weights[idx_filt])
+    return mixture(means[idx_filt], covs[idx_filt], np.exp(log_weights[idx_filt]), bounds, dim, len(log_weights[idx_filt]), mix.n_pts, probit = mix.probit, log_w = log_weights[idx_filt])
 
-def condition(draws, vals, dims, norm = True):
+def condition(draws, vals, dims, norm = True, filter = True, tol = 1e-4):
     """
     Probability density conditioned on specific values of a subset of parameters.
     
     Arguments:
         :figaro.mixture.mixture draws: mixture(s)
         :iterable vals:                value(s) to condition on
         :int or list of int dims:      dimension(s) associated with given vals (starting from 0)
         :bool norm:                    normalize the distribution
+        :bool filter:                  filter the components with weight < tol
+        :double tol:                   tolerance on the sum of the weights
     
     Returns:
         :figaro.mixture.mixture: the conditioned mixture(s)
     """
     if np.iterable(draws):
         v       = np.mean(draws[0].bounds, axis = -1)
         v[dims] = vals
-        return np.array([_condition(d, v, dims, norm) for d in draws])
+        return np.array([_condition(d, v, dims, norm, filter, tol) for d in draws])
     else:
         v       = np.mean(draws.bounds, axis = -1)
         v[dims] = vals
-        return _condition(draws, v, dims, norm)
+        return _condition(draws, v, dims, norm, filter, tol)
```

### Comparing `figaro-1.0.6/figaro/mixture.py` & `figaro-1.1.0/figaro/mixture.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import dill
 
 from collections import Counter
 from pathlib import Path
 
 from scipy.special import gammaln, logsumexp
 from scipy.stats import multivariate_normal as mn
-from scipy.stats import invwishart, norm, invgamma
+from scipy.stats import invwishart, norm, invgamma, dirichlet
 
 from figaro.decorators import *
 from figaro.transform import *
-from figaro.likelihood import evaluate_mixture_MC_draws, evaluate_mixture_MC_draws_1d, logsumexp_jit, log_norm
+from figaro.likelihood import evaluate_mixture_MC_draws, evaluate_mixture_MC_draws_1d, logsumexp_jit, log_norm, inv_jit
 from figaro.exceptions import except_hook, FIGAROException
 from figaro.utils import get_priors
 from figaro.marginal import _condition, _marginalise
 
-from numba import jit, njit, prange
+from numba import njit, prange
 from numba.extending import get_cython_function_address
 import ctypes
 
 #-----------#
 # Utilities #
 #-----------#
 
@@ -43,15 +43,15 @@
 # Functions #
 #-----------#
 
 @njit
 def _numba_gammaln(x):
     return gammaln_float64(x)
 
-@jit
+@njit
 def _student_t(df, t, mu, sigma, dim):
     """
     Multivariate student-t pdf.
     As in http://gregorygundersen.com/blog/2020/01/20/multivariate-t/
     
     Arguments:
         :float df:         degrees of freedom
@@ -75,15 +75,15 @@
     B = _numba_gammaln(0.5 * df)
     C = dim/2. * np.log(df * np.pi)
     D = 0.5 * logdet
     E = -x * np.log1p((1./df) * maha)
 
     return (A - B - C - D + E)[0]
 
-@jit
+@njit
 def update_alpha(alpha, n, K, burnin = 1000):
     """
     Update concentration parameter using a Metropolis-Hastings sampling scheme.
     
     Arguments:
         :double alpha: Initial value for concentration parameter
         :int n:        Number of samples
@@ -100,15 +100,15 @@
         if a_new > 0.:
             logP_old = _numba_gammaln(a_old) - _numba_gammaln(a_old + n) + K * np.log(a_old) - 1./a_old
             logP_new = _numba_gammaln(a_new) - _numba_gammaln(a_new + n) + K * np.log(a_new) - 1./a_new
             if logP_new - logP_old > np.log(np.random.random()):
                 a_old = a_new
     return a_old
 
-@jit
+@njit
 def compute_t_pars(k, mu, nu, L, mean, S, N, dim):
     """
     Compute parameters for student-t distribution.
     
     Arguments:
         :double k:        Normal std parameter (for NIW)
         :np.ndarray mu:   Normal mean parameter (for NIW)
@@ -127,15 +127,15 @@
     # Update hyperparameters
     k_n, mu_n, nu_n, L_n = compute_hyperpars(k, mu, nu, L, mean, S, N)
     # Update t-parameters
     t_df    = nu_n - dim + 1
     t_shape = L_n*(k_n+1)/(k_n*t_df)
     return t_df, t_shape, mu_n
 
-@jit
+@njit
 def compute_hyperpars(k, mu, nu, L, mean, S, N):
     """
     Update hyperparameters for Normal Inverse Gamma/Wishart (NIG/NIW).
     See https://www.cs.ubc.ca/~murphyk/Papers/bayesGauss.pdf
     
     Arguments:
         :double k:        Normal std parameter (for NIG/NIW)
@@ -154,15 +154,15 @@
     """
     k_n  = k + N
     mu_n = (mu*k + N*mean)/k_n
     nu_n = nu + N
     L_n  = L + S + k*N*((mean - mu).T@(mean - mu))/k_n
     return k_n, mu_n, nu_n, L_n
 
-@jit
+@njit
 def compute_component_suffstats(x, mean, S, N, p_mu, p_k, p_nu, p_L):
     """
     Update mean, covariance, number of samples and maximum a posteriori for mean and covariance.
     
     Arguments:
         :np.ndarray x:    sample to add
         :np.ndarray mean: mean of samples already in the cluster
@@ -172,15 +172,15 @@
         :double p_k:      NIG Normal std parameter
         :int p_nu:        NIG Gamma df parameter
         :np.ndarray p_L:  NIG Gamma scale matrix
     
     Returns:
         :np.ndarray: updated mean
         :np.ndarray: updated covariance
-        :int N:      updated number of samples
+        :int:        updated number of samples
         :np.ndarray: mean (maximum a posteriori)
         :np.ndarray: covariance (maximum a posteriori)
     """
     new_mean  = (mean*N+x)/(N+1)
     new_S     = (S + N*mean.T@mean + x.T@x) - new_mean.T@new_mean*(N+1)
     new_N     = N+1
     new_mu    = ((p_mu*p_k + new_N*new_mean)/(p_k + new_N))[0]
@@ -251,23 +251,24 @@
         self.means  = [x.means]
         self.covs   = [x.covs]
         self.log_w  = [x.log_w]
         self.logL_D = logL_D
         
         log_norm_D = logsumexp_jit(logL_D, b = b_ones)
         
-        self.mu    = np.average(mu_MC, weights = np.exp(logL_D - log_norm_D), axis = 0)
-        self.sigma = np.average(sigma_MC, weights = np.exp(logL_D - log_norm_D), axis = 0)
+        idx        = np.random.choice(len(mu_MC), p = np.exp(logL_D - log_norm_D))
+        self.mu    = np.copy(mu_MC[idx])
+        self.sigma = np.copy(sigma_MC[idx])
         if dim == 1:
             self.mu = np.atleast_2d(self.mu).T
             self.sigma = np.atleast_2d(self.sigma).T
             
 class _density:
     """
-    Class to initialise a common set of methods for mixture models. Not to be used
+    Class to initialise a common set of methods for mixture models. Not to be used.
     """
     def __init__(self):
         pass
         
     def __call__(self, x):
         return self.pdf(x)
 
@@ -275,25 +276,29 @@
         if self.n_cl == 0:
             raise FIGAROException("You are trying to evaluate an empty mixture.\n If you are using the density_from_samples() method, you may want to evaluate the output of that method.")
         if len(np.shape(x)) < 2:
             if self.dim == 1:
                 x = np.atleast_2d(x).T
             else:
                 x = np.atleast_2d(x)
-        return self._pdf(x)
+        with np.errstate(invalid = 'ignore'):
+            p = np.nan_to_num(self._pdf(x), nan = 0.)
+        return p
 
     def logpdf(self, x):
         if self.n_cl == 0:
             raise FIGAROException("You are trying to evaluate an empty mixture.\n If you are using the density_from_samples() method, you may want to evaluate the output of that method.")
         if len(np.shape(x)) < 2:
             if self.dim == 1:
                 x = np.atleast_2d(x).T
             else:
                 x = np.atleast_2d(x)
-        return self._logpdf(x)
+        with np.errstate(invalid = 'ignore'):
+            logp = np.nan_to_num(self._logpdf(x), nan = -np.inf)
+        return logp
 
     @probit
     def _pdf(self, x):
         """
         Evaluate mixture at point(s) x
         
         Arguments:
@@ -424,15 +429,65 @@
         
         Arguments:
             :np.ndarray x: point(s) to evaluate the mixture at (in probit space)
         
         Returns:
             :np.ndarray: mixture.pdf(x)
         """
-        return np.sum(np.array([w*mn(mean, cov).pdf(x) for mean, cov, w in zip(self.means, self.covs, self.w)]), axis = 0)
+        return np.sum(np.array([w*mn(mean, cov, allow_singular = True).pdf(x) for mean, cov, w in zip(self.means, self.covs, self.w)]), axis = 0)
+    
+    @probit
+    def _pdf_array(self, x):
+        """
+        Evaluate every mixture component at point(s) x.
+        
+        Arguments:
+            :np.ndarray x: point(s) to evaluate the components at
+        
+        Returns:
+            :np.ndarray: component.pdf(x) for each mixture component
+        """
+        return _pdf_array_probit(x) * np.exp(-probit_logJ(x, self.bounds, self.probit))
+
+    def _pdf_array_probit(self, x):
+        """
+        Evaluate every mixture component at point(s) x.
+        
+        Arguments:
+            :np.ndarray x: point(s) to evaluate the components at (in probit space)
+        
+        Returns:
+            :np.ndarray: component.pdf(x) for each mixture component
+        """
+        return np.array([w*mn(mean, cov, allow_singular = True).pdf(x) for mean, cov, w in zip(self.means, self.covs, self.w)])
+
+    @probit
+    def _fast_pdf_array(self, x):
+        """
+        Evaluate every mixture component at point(s) x.
+        
+        Arguments:
+            :np.ndarray x: point(s) to evaluate the components at
+        
+        Returns:
+            :np.ndarray: component.pdf(x) for each mixture component
+        """
+        return _fast_pdf_array_probit(x) * np.exp(-probit_logJ(x, self.bounds, self.probit))
+
+    def _fast_pdf_array_probit(self, x):
+        """
+        Evaluate every mixture component at point(s) x.
+        
+        Arguments:
+            :np.ndarray x: point(s) to evaluate the components at (in probit space)
+        
+        Returns:
+            :np.ndarray: component.pdf(x) for each mixture component
+        """
+        return np.array([w*np.exp(log_norm(x[0], mean, cov)) for mean, cov, w in zip(self.means, self.covs, self.w)])
 
     @probit
     def _logpdf_no_jacobian(self, x):
         """
         Evaluate log mixture at point(s) x without jacobian
         
         Arguments:
@@ -449,15 +504,15 @@
         
         Arguments:
             :np.ndarray x: point(s) to evaluate the mixture at (in probit space)
         
         Returns:
             :np.ndarray: mixture.logpdf(x)
         """
-        return logsumexp(np.array([w + mn(mean, cov).logpdf(x) for mean, cov, w in zip(self.means, self.covs, self.log_w)]), axis = 0)
+        return logsumexp(np.array([w + mn(mean, cov, allow_singular = True).logpdf(x) for mean, cov, w in zip(self.means, self.covs, self.log_w)]), axis = 0)
 
     def cdf(self, x):
         if self.dim > 1:
             raise FIGAROException("cdf is provided only for 1-dimensional distributions")
         if len(np.shape(x)) < 2:
             x = np.atleast_2d(x).T
         return self._cdf(x)
@@ -492,49 +547,121 @@
         
         Returns:
             :np.ndarray: mixture.logcdf(x)
         """
         return logsumexp(np.array([w + norm(mean[0], cov[0,0]).logcdf(x) for mean, cov, w in zip(self.means, np.sqrt(self.covs), self.log_w)]), axis = 0)
 
     @from_probit
-    def rvs(self, n_samps):
+    def rvs(self, size = 1):
         """
         Draw samples from mixture
         
         Arguments:
-            :int n_samps: number of samples to draw
+            :int size: number of samples to draw
         
         Returns:
             :np.ndarray: samples
         """
         if self.n_cl == 0:
             raise FIGAROException("You are trying to draw samples from an empty mixture.\n If you are using the density_from_samples() method, you may want to draw samples from the output of that method.")
-        return self._rvs_probit(n_samps)
+        return self._rvs_probit(size)
         
-    def _rvs_probit(self, n_samps):
+    def _rvs_probit(self, size = 1):
         """
         Draw samples from mixture in probit space
         
         Arguments:
-            :int n_samps: number of samples to draw
+            :int size: number of samples to draw
         
         Returns:
             :np.ndarray: samples in probit space
         """
-        idx = np.random.choice(np.arange(self.n_cl), p = self.w, size = n_samps)
+        idx = np.random.choice(np.arange(self.n_cl), p = self.w, size = size)
         ctr = Counter(idx)
         if self.dim > 1:
             samples = np.empty(shape = (1,self.dim))
             for i, n in zip(ctr.keys(), ctr.values()):
-                samples = np.concatenate((samples, np.atleast_2d(mn(self.means[i], self.covs[i]).rvs(size = n))))
+                samples = np.concatenate((samples, np.atleast_2d(mn(self.means[i], self.covs[i], allow_singular = True).rvs(size = n))))
         else:
             samples = np.array([np.zeros(1)])
             for i, n in zip(ctr.keys(), ctr.values()):
-                samples = np.concatenate((samples, np.atleast_2d(mn(self.means[i], self.covs[i]).rvs(size = n)).T))
+                samples = np.concatenate((samples, np.atleast_2d(mn(self.means[i], self.covs[i], allow_singular = True).rvs(size = n)).T))
         return np.array(samples[1:])
+    
+    def gradient(self, x):
+        """
+        Gradient of the mixture.
+        
+        Arguments:
+            :np.ndarray x: point to evaluate the gradient at
+        
+        Returns:
+            :np.ndarray: gradient
+        """
+        if self.n_cl == 0:
+            raise FIGAROException("You are trying to evaluate an empty mixture.\n If you are using the density_from_samples() method, you may want to evaluate the output of that method.")
+        if len(np.shape(x)) < 2:
+            if self.dim == 1:
+                x = np.atleast_2d(x).T
+            else:
+                x = np.atleast_2d(x)
+        with np.errstate(invalid = 'ignore'):
+            g = np.nan_to_num([self._gradient(xi) for xi in x], nan = 0.)
+        return g
+    
+    def log_gradient(self, x):
+        """
+        Logarithmic gradient of the mixture.
+        
+        Arguments:
+            :np.ndarray x: point to evaluate the gradient at
+        
+        Returns:
+            :np.ndarray: logarithmic gradient
+        """
+        if self.n_cl == 0:
+            raise FIGAROException("You are trying to evaluate an empty mixture.\n If you are using the density_from_samples() method, you may want to evaluate the output of that method.")
+        if len(np.shape(x)) < 2:
+            if self.dim == 1:
+                x = np.atleast_2d(x).T
+            else:
+                x = np.atleast_2d(x)
+        with np.errstate(invalid = 'ignore'):
+            g = np.nan_to_num([self._log_gradient(xi) for xi in x], nan = 0.)
+        return g
+    
+    def _gradient(self, x):
+        """
+        Gradient of the mixture.
+        
+        Arguments:
+            :np.ndarray x: point to evaluate the gradient at
+        
+        Returns:
+            :np.ndarray: gradient
+        """
+        return self._fast_pdf(x)*self._log_gradient(x)
+    
+    @probit
+    def _log_gradient(self, x):
+        """
+        Logarithmic gradient of the mixture.
+        
+        Arguments:
+            :np.ndarray x: point to evaluate the gradient at
+        
+        Returns:
+            :np.ndarray: logarithmic gradient
+        """
+        p = self._pdf_array_probit(x)
+        B = np.array([-np.dot(inv_jit(sigma),(x - mu)) for mu, sigma in zip(self.means, self.covs)])
+        try:
+            return np.average(B, weights = p, axis = 0) + log_gradient_inv_jacobian(x, self.bounds, self.probit)
+        except ZeroDivisionError:
+            return np.zeros(x.shape[-1])
 
 class mixture(_density):
     """
     Class to store a single draw from DPGMM/(H)DPGMM.
     Methods inherited from _density class.
     
     Arguments:
@@ -545,53 +672,57 @@
         :int dim:           number of dimensions
         :int n_cl:          number of clusters in the mixture
         :bool probit:       whether to use the probit transformation or not
     
     Returns:
         :mixture: instance of mixture class
     """
-    def __init__(self, means, covs, w, bounds, dim, n_cl, n_pts, probit = True):
+    def __init__(self, means, covs, w, bounds, dim, n_cl, n_pts, probit = True, log_w = None):
         self.means  = means
         self.covs   = covs
-        self.w      = w
-        self.log_w  = np.log(w)
+        if log_w is None:
+            self.w      = w
+            self.log_w  = np.log(w)
+        else:
+            self.log_w  = log_w
+            self.w      = np.exp(log_w)
         self.bounds = bounds
         self.dim    = dim
         self.n_cl   = n_cl
         self.n_pts  = n_pts
         self.probit = probit
     
     def marginalise(self, axis = -1):
         """
         Marginalise out one or more dimensions from the mixture.
         
         Arguments:
-            :int or list of int axis:      axis to marginalise on
+            :int or list of int axis: axis to marginalise on. Default: last
         
         Returns:
-            :figaro.mixture.mixture: the marginalised mixture
+            :figaro.mixture.mixture: marginalised mixture
         """
         return _marginalise(self, axis)
     
     def condition(self, vals, dims, norm = True):
         """
         Mixture conditioned on specific values of a subset of parameters.
         
         Arguments:
-            :iterable vals:                value(s) to condition on
-            :int or list of int dims:      dimension(s) associated with given vals (starting from 0)
-            :bool norm:                    normalize the distribution
+            :iterable vals:           value(s) to condition on
+            :int or list of int dims: dimension(s) associated with given vals (starting from 0)
+            :bool norm:               whether to normalize the distribution or not
         
         Returns:
-            :figaro.mixture.mixture: the conditioned mixture
+            :figaro.mixture.mixture: conditioned mixture
         """
         v       = np.mean(self.bounds, axis = -1)
         v[dims] = vals
         return _condition(self, v, dims, norm)
-
+    
 #-------------------#
 # Inference classes #
 #-------------------#
 
 class DPGMM(_density):
     """
     Class to infer a distribution given a set of samples.
@@ -672,15 +803,15 @@
         Arguments:
             :np.ndarray x: sample
             :component ss: component to update
         
         Returns:
             :double: log Likelihood
         """
-        if ss == "new":
+        if ss is None:
             ss = component(np.zeros(self.dim), prior = self.prior)
             ss.N = 0.
         t_df, t_shape, mu_n = compute_t_pars(self.prior.k, self.prior.mu, self.prior.nu, self.prior.L, ss.mean, ss.S, ss.N, self.dim)
         return _student_t(df = t_df, t = x, mu = mu_n, sigma = t_shape, dim = self.dim)
 
     def _cluster_assignment_distribution(self, x):
         """
@@ -688,46 +819,42 @@
         
         Arguments:
             :np.ndarray x: sample
         
         Returns:
             :dict: p_i for each component
         """
-        scores = {}
-        for i in list(np.arange(self.n_cl)) + ["new"]:
-            if i == "new":
-                ss = "new"
-            else:
-                ss = self.mixture[i]
-            scores[i] = self._log_predictive_likelihood(x, ss)
-            if ss == "new":
-                scores[i] += np.log(self.alpha)
+        scores = np.zeros(self.n_cl+1)
+        for i in range(self.n_cl+1):
+            if i == 0:
+                ss        = None
+                scores[i] = np.log(self.alpha)
             else:
-                scores[i] += np.log(ss.N)
-        norm   = logsumexp(np.array([score for score in scores.values()]), b = np.ones(self.n_cl+1))
-        scores = {cid: (np.exp(score - norm) if score < np.inf else 0) for cid, score in scores.items()} # score < inf checks also for NaNs
-        return scores
+                ss        = self.mixture[i-1]
+                scores[i] = np.log(ss.N)
+            scores[i] += self._log_predictive_likelihood(x, ss)
+        norm = logsumexp_jit(scores, b = np.ones(self.n_cl+1))
+        return np.exp(scores - norm)
 
     def _assign_to_cluster(self, x):
         """
         Assign the new sample x to an existing cluster or to a new cluster according to the marginal distribution of cluster assignment.
         
         Arguments:
             :np.ndarray x: sample
         """
-        scores = self._cluster_assignment_distribution(x).items()
-        labels, scores = zip(*scores)
-        cid = np.random.choice(labels, p=scores)
-        if cid == "new":
+        scores = self._cluster_assignment_distribution(x)
+        cid = np.random.choice(self.n_cl+1, p=scores)
+        if cid == 0:
             self.mixture.append(component(x, prior = self.prior))
             self.N_list.append(1.)
             self.n_cl += 1
         else:
-            self.mixture[int(cid)] = self._add_datapoint_to_component(x, self.mixture[int(cid)])
-            self.N_list[int(cid)] += 1
+            self.mixture[int(cid)-1] = self._add_datapoint_to_component(x, self.mixture[int(cid)-1])
+            self.N_list[int(cid)-1] += 1
         # Update weights
         self.w = np.array(self.N_list)
         self.w = self.w/self.w.sum()
         self.log_w = np.log(self.w)
         return
     
     def density_from_samples(self, samples):
@@ -765,62 +892,69 @@
         Instances a mixture class representing the inferred distribution
         
         Returns:
             :mixture: the inferred distribution
         """
         if self.n_cl == 0:
             raise FIGAROException("You are trying to build an empty mixture - perhaps you called the initialise() method. If you are using the density_from_samples() method, the inferred mixture is returned by that method as an instance of mixture class.")
-        return mixture(np.array([comp.mu for comp in self.mixture]), np.array([comp.sigma for comp in self.mixture]), np.array(self.w), self.bounds, self.dim, self.n_cl, self.n_pts, probit = self.probit)
+        means     = np.zeros((self.n_cl, self.dim))
+        variances = np.zeros((self.n_cl, self.dim, self.dim))
+        for i, ss in enumerate(self.mixture):
+            k_n, mu_n, nu_n, L_n = compute_hyperpars(self.prior.k, self.prior.mu, self.prior.nu, self.prior.L, ss.mean, ss.S, ss.N)
+            variances[i] = invwishart(df = nu_n, scale = L_n).rvs()
+            means[i]     = mn(mean = mu_n[0], cov = variances[i]/k_n, allow_singular = True).rvs()
+        w = dirichlet(self.w*self.n_pts+self.alpha/self.n_cl).rvs()[0]
+        return mixture(means, variances, w, self.bounds, self.dim, self.n_cl, self.n_pts, probit = self.probit)
 
     # Methods to overwrite _density methods
-    def _rvs_probit(self, n_samps):
+    def _rvs_probit(self, size = 1):
         """
         Draw samples from mixture in probit space
         
         Arguments:
-            :int n_samps: number of samples to draw
+            :int size: number of samples to draw
         
         Returns:
             :np.ndarray: samples in probit space
         """
-        idx = np.random.choice(np.arange(self.n_cl), p = self.w, size = n_samps)
+        idx = np.random.choice(np.arange(self.n_cl), p = self.w, size = size)
         ctr = Counter(idx)
         if self.dim > 1:
             samples = np.empty(shape = (1,self.dim))
             for i, n in zip(ctr.keys(), ctr.values()):
-                samples = np.concatenate((samples, np.atleast_2d(mn(self.mixture[i].mu, self.mixture[i].sigma).rvs(size = n))))
+                samples = np.concatenate((samples, np.atleast_2d(mn(self.mixture[i].mu, self.mixture[i].sigma, allow_singular = True).rvs(size = n))))
         else:
             samples = np.array([np.zeros(1)])
             for i, n in zip(ctr.keys(), ctr.values()):
-                samples = np.concatenate((samples, np.atleast_2d(mn(self.mixture[i].mu, self.mixture[i].sigma).rvs(size = n)).T))
+                samples = np.concatenate((samples, np.atleast_2d(mn(self.mixture[i].mu, self.mixture[i].sigma, allow_singular = True).rvs(size = n)).T))
         return samples[1:]
 
     def _pdf_probit(self, x):
         """
         Evaluate mixture at point(s) x in probit space
         
         Arguments:
             :np.ndarray x: point(s) to evaluate the mixture at (in probit space)
         
         Returns:
             :np.ndarray: mixture.pdf(x)
         """
-        return np.sum(np.array([w*mn(comp.mu, comp.sigma).pdf(x) for comp, w in zip(self.mixture, self.w)]), axis = 0)
+        return np.sum(np.array([w*mn(comp.mu, comp.sigma, allow_singular = True).pdf(x) for comp, w in zip(self.mixture, self.w)]), axis = 0)
 
     def _logpdf_probit(self, x):
         """
         Evaluate log mixture at point(s) x in probit space
         
         Arguments:
             :np.ndarray x: point(s) to evaluate the mixture at (in probit space)
         
         Returns:
             :np.ndarray: mixture.logpdf(x)
         """
-        return logsumexp(np.array([w + mn(comp.mu, comp.sigma).logpdf(x) for comp, w in zip(self.mixture, self.log_w)]), axis = 0)
+        return logsumexp(np.array([w + mn(comp.mu, comp.sigma, allow_singular = True).logpdf(x) for comp, w in zip(self.mixture, self.log_w)]), axis = 0)
 
     def _fast_pdf_probit(self, x):
         """
         Evaluate mixture at point x in probit space
         
         Arguments:
             :np.ndarray x: point to evaluate the mixture at (in probit space)
@@ -857,26 +991,29 @@
     
     Returns:
         :HDPGMM: instance of HDPGMM class
     """
     def __init__(self, bounds,
                        alpha0     = 1.,
                        prior_pars = None,
-                       MC_draws   = 2e3,
+                       MC_draws   = None,
                        probit     = True,
                        ):
         bounds   = np.atleast_2d(bounds)
         self.dim = len(bounds)
         super().__init__(bounds = bounds, alpha0 = alpha0, probit = probit)
         if prior_pars is not None:
             self.exp_sigma, self.a = prior_pars
         else:
             self.exp_sigma, self.a = get_priors(bounds = self.bounds, probit = self.probit, hierarchical = True)
         self.invgamma = invgamma(self.a)
-        self.MC_draws = int(MC_draws)
+        if MC_draws is None:
+            self.MC_draws = int((self.dim+1)*1e3)
+        else:
+            self.MC_draws = int(MC_draws)
         # For logsumexp_jit
         self.b_ones = np.ones(self.MC_draws)
         # MC samples
         self._draw_MC_samples()
         
     def initialise(self):
         """
@@ -893,15 +1030,17 @@
         self.mu_MC    = np.random.uniform(low = self.bounds[:,0], high = self.bounds[:,1], size = (self.MC_draws, self.dim))
         if self.probit:
             self.mu_MC = transform_to_probit(self.mu_MC, self.bounds)
         if self.dim == 1:
             self.sigma_MC = self.sigma_MC.flatten()
             self.mu_MC = self.mu_MC.flatten()
         else:
-            self.sigma_MC = np.array([invwishart(df = self.dim+2, scale = np.identity(self.dim)*cov).rvs() for cov in self.sigma_MC])
+            rhos = invwishart(df = self.dim+2, scale = np.identity(self.dim)).rvs(size = self.MC_draws)
+            rhos = np.array([r/np.outer(np.sqrt(np.diag(r)), np.sqrt(np.diag(r))) for r in rhos])
+            self.sigma_MC = np.array([r*np.outer(s,s) for r, s in zip(rhos, np.sqrt(self.sigma_MC))])
             
     def add_new_point(self, ev):
         """
         Update the probability density reconstruction adding a new sample
         
         Arguments:
             :iterable x: set of single-event draws from a DPGMM inference
@@ -917,59 +1056,55 @@
         
         Arguments:
             :np.ndarray x: sample
         
         Returns:
             :dict: p_i for each component
         """
-        scores = {}
-        logL_N = {}
+        scores = np.zeros(self.n_cl+1)
+        logL_N = np.zeros((self.n_cl+1, self.MC_draws))
         
         if self.dim == 1:
             logL_x = evaluate_mixture_MC_draws_1d(self.mu_MC, self.sigma_MC, x.means, x.covs, x.w)
         else:
             logL_x = evaluate_mixture_MC_draws(self.mu_MC, self.sigma_MC, x.means, x.covs, x.w)
-        for i in list(np.arange(self.n_cl)) + ["new"]:
-            if i == "new":
-                ss = "new"
+        for i in range(self.n_cl+1):
+            if i == 0:
+                ss = None
                 logL_D = np.zeros(self.MC_draws)
+                scores[i] = np.log(self.alpha)
             else:
-                ss = self.mixture[i]
-                logL_D = ss.logL_D
-            scores[i] = logsumexp_jit(logL_D + logL_x, b = self.b_ones) - logsumexp_jit(logL_D, b = self.b_ones)
-            logL_N[i] = logL_D + logL_x
-            if ss == "new":
-                scores[i] += np.log(self.alpha)
-            else:
-                scores[i] += np.log(ss.N)
-        norm   = logsumexp(np.array([score for score in scores.values()]), b = np.ones(self.n_cl+1))
-        scores = {cid: (np.exp(score - norm) if score < np.inf else 0)  for cid, score in scores.items()} # score < inf checks also for NaNs
+                ss        = self.mixture[i-1]
+                logL_D    = ss.logL_D
+                scores[i] = np.log(ss.N)
+            scores[i] += logsumexp_jit(logL_D + logL_x, b = self.b_ones) - logsumexp_jit(logL_D, b = self.b_ones)
+            logL_N[i]  = logL_D + logL_x
+        norm   = logsumexp_jit(scores, b = np.ones(self.n_cl+1))
+        scores = np.exp(scores-norm)
         return scores, logL_N
 
     def _assign_to_cluster(self, x):
         """
         Assign the new sample x to an existing cluster or to a new cluster according to the marginal distribution of cluster assignment.
         
         Arguments:
             :np.ndarray x: sample
         """
         scores, logL_N = self._cluster_assignment_distribution(x)
-        scores = scores.items()
-        labels, scores = zip(*scores)
         try:
-            cid = np.random.choice(labels, p=scores)
+            cid = np.random.choice(self.n_cl+1, p=scores)
         except ValueError:
-            cid = "new"
-        if cid == "new":
+            cid = 0
+        if cid == 0:
             self.mixture.append(component_h(x, self.dim, self.prior, logL_N[cid], self.mu_MC, self.sigma_MC, self.b_ones))
             self.N_list.append(1.)
             self.n_cl += 1
         else:
-            self.mixture[int(cid)] = self._add_datapoint_to_component(x, self.mixture[int(cid)], logL_N[int(cid)])
-            self.N_list[int(cid)] += 1
+            self.mixture[int(cid)-1] = self._add_datapoint_to_component(x, self.mixture[int(cid)-1], logL_N[int(cid)])
+            self.N_list[int(cid)-1] += 1
         # Update weights
         self.w = np.array(self.N_list)
         self.w = self.w/self.w.sum()
         self.log_w = np.log(self.w)
         return
 
     def _add_datapoint_to_component(self, x, ss, logL_D):
@@ -987,24 +1122,36 @@
         ss.events.append(x)
         ss.means.append(x.means)
         ss.covs.append(x.covs)
         ss.log_w.append(x.log_w)
         ss.logL_D = logL_D
 
         log_norm_D = logsumexp_jit(logL_D, self.b_ones)
-
-        ss.mu    = np.average(self.mu_MC, weights = np.exp(logL_D - log_norm_D), axis = 0)
-        ss.sigma = np.average(self.sigma_MC, weights = np.exp(logL_D - log_norm_D), axis = 0)
+        
+        idx      = np.random.choice(self.MC_draws, p = np.exp(logL_D - log_norm_D))
+        ss.mu    = np.copy(self.mu_MC[idx])
+        ss.sigma = np.copy(self.sigma_MC[idx])
         if self.dim == 1:
             ss.mu = np.atleast_2d(ss.mu).T
             ss.sigma = np.atleast_2d(ss.sigma).T
         
         ss.N += 1
         return ss
 
+    def build_mixture(self):
+        """
+        Instances a mixture class representing the inferred distribution
+        
+        Returns:
+            :mixture: the inferred distribution
+        """
+        if self.n_cl == 0:
+            raise FIGAROException("You are trying to build an empty mixture - perhaps you called the initialise() method. If you are using the density_from_samples() method, the inferred mixture is returned by that method as an instance of mixture class.")
+        return mixture(np.array([comp.mu for comp in self.mixture]), np.array([comp.sigma for comp in self.mixture]), np.array(self.w), self.bounds, self.dim, self.n_cl, self.n_pts, probit = self.probit)
+
     def density_from_samples(self, events):
         """
         Reconstruct the probability density from a set of samples.
         
         Arguments:
             :iterable samples: set of single-event draws from DPGMM
```

### Comparing `figaro-1.0.6/figaro/montecarlo.py` & `figaro-1.1.0/figaro/montecarlo.py`

 * *Files identical despite different names*

### Comparing `figaro-1.0.6/figaro/pipelines/create_glade.py` & `figaro-1.1.0/figaro/pipelines/create_glade.py`

 * *Files identical despite different names*

### Comparing `figaro-1.0.6/figaro/pipelines/entropy.py` & `figaro-1.1.0/figaro/pipelines/entropy.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     # Settings
     parser.add_option("--draws", type = "int", dest = "n_draws", help = "Number of draws", default = 100)
     parser.add_option("--se_draws", type = "int", dest = "n_se_draws", help = "Number of draws for single-event distribution. Default: same as hierarchical distribution", default = None)
     parser.add_option("--n_samples_dsp", type = "int", dest = "n_samples_dsp", help = "Number of samples to analyse (downsampling). Default: all", default = -1)
     parser.add_option("--exclude_points", dest = "exclude_points", action = 'store_true', help = "Exclude points outside bounds from analysis", default = False)
     parser.add_option("--cosmology", type = "string", dest = "cosmology", help = "Cosmological parameters (h, om, ol). Default values from Planck (2021)", default = '0.674,0.315,0.685')
     parser.add_option("--sigma_prior", dest = "sigma_prior", type = "string", help = "Expected standard deviation (prior) - single value or n-dim values. If None, it is estimated from samples", default = None)
+    parser.add_option("--fraction", dest = "scale", type = "float", help = "Fraction of samples standard deviation for sigma prior. Overrided by sigma_prior.", default = None)
     parser.add_option("-e", "--events", dest = "run_events", action = 'store_false', help = "Skip single-event analysis", default = True)
     parser.add_option("--snr_threshold", dest = "snr_threshold", type = "float", help = "SNR threshold for simulated GW datasets", default = None)
     parser.add_option("--far_threshold", dest = "far_threshold", type = "float", help = "FAR threshold for simulated GW datasets", default = None)
     parser.add_option("--zero_crossings", dest = "zero_crossings", type = "int", help = "Number of zero-crossings of the entropy derivative to call the number of samples sufficient. Default as in Appendix B of Rinaldi & Del Pozzo (2021)", default = 5)
     parser.add_option("--window", dest = "window", type = "int", help = "Number of points to use to approximate the entropy derivative", default = 200)
     parser.add_option("--entropy_interval", dest = "entropy_interval", type = "int", help = "Number of samples between two entropy evaluations", default = 100)
     parser.add_option("--entropy_draws", dest = "entropy_draws", type = "string", help = "Number of monte carlo samples for entropy evaluation", default = '1e3')
```

### Comparing `figaro-1.0.6/figaro/pipelines/gen_mock_data.py` & `figaro-1.1.0/figaro/pipelines/gen_mock_data.py`

 * *Files identical despite different names*

### Comparing `figaro-1.0.6/figaro/pipelines/hierarchical_inference.py` & `figaro-1.1.0/figaro/pipelines/hierarchical_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,16 @@
     parser.add_option("--se_draws", type = "int", dest = "n_se_draws", help = "Number of draws for single-event distribution. Default: same as hierarchical distribution", default = None)
     parser.add_option("--n_samples_dsp", type = "int", dest = "n_samples_dsp", help = "Number of samples to analyse (downsampling). Default: all", default = -1)
     parser.add_option("--exclude_points", dest = "exclude_points", action = 'store_true', help = "Exclude points outside bounds from analysis", default = False)
     parser.add_option("--cosmology", type = "string", dest = "cosmology", help = "Cosmological parameters (h, om, ol). Default values from Planck (2021)", default = '0.674,0.315,0.685')
     parser.add_option("-e", "--events", dest = "run_events", action = 'store_false', help = "Skip single-event analysis", default = True)
     parser.add_option("--se_sigma_prior", dest = "se_sigma_prior", type = "string", help = "Expected standard deviation (prior) for single-event inference - single value or n-dim values. If None, it is estimated from samples", default = None)
     parser.add_option("--sigma_prior", dest = "sigma_prior", type = "string", help = "Expected standard deviation (prior) for hierarchical inference - single value or n-dim values. If None, it is estimated from samples", default = None)
-    parser.add_option("--mc_draws", dest = "mc_draws", type = "int", help = "Number of draws for assignment MC integral", default = 2000)
+    parser.add_option("--fraction", dest = "scale", type = "float", help = "Fraction of samples standard deviation for sigma prior. Overrided by sigma_prior.", default = None)
+    parser.add_option("--mc_draws", dest = "mc_draws", type = "int", help = "Number of draws for assignment MC integral", default = None)
     parser.add_option("--snr_threshold", dest = "snr_threshold", type = "float", help = "SNR threshold for simulated GW datasets", default = None)
     parser.add_option("--far_threshold", dest = "far_threshold", type = "float", help = "FAR threshold for simulated GW datasets", default = None)
     parser.add_option("--no_probit", dest = "probit", action = 'store_false', help = "Disable probit transformation", default = True)
     parser.add_option("--config", dest = "config", type = "string", help = "Config file. Warning: command line options are ignored if provided", default = None)
     
     (options, args) = parser.parse_args()
 
@@ -131,15 +132,14 @@
         dim = np.shape(events[0][0])[-1]
     except IndexError:
         dim = 1
     if options.exclude_points:
         print("Ignoring points outside bounds.")
         for i, ev in enumerate(events):
             events[i] = ev[np.where((np.prod(options.bounds[:,0] < ev, axis = 1) & np.prod(ev < options.bounds[:,1], axis = 1)))]
-        all_samples = np.atleast_2d(np.concatenate(events))
     else:
         # Check if all samples are within bounds
         all_samples = np.atleast_2d(np.concatenate(events))
         if options.probit:
             if not np.alltrue([(all_samples[:,i] > options.bounds[i,0]).all() and (all_samples[:,i] < options.bounds[i,1]).all() for i in range(dim)]):
                 raise ValueError("One or more samples are outside the given bounds.")
 
@@ -159,15 +159,15 @@
         if options.run_events:
             mix = DPGMM(options.bounds, probit = options.probit)
             posteriors = []
             # Run each single-event analysis
             for i in tqdm(range(len(events)), desc = 'Events'):
                 ev   = events[i]
                 name = names[i]
-                prior_pars = get_priors(mix.bounds, samples = ev, probit = options.probit, std = options.se_sigma_prior, hierarchical = False)
+                prior_pars = get_priors(mix.bounds, samples = ev, probit = options.probit, std = options.se_sigma_prior, scale = options.scale, hierarchical = False)
                 mix.initialise(prior_pars = prior_pars)
                 # Draw samples
                 draws = [mix.density_from_samples(ev) for _ in range(options.n_se_draws)]
                 posteriors.append(draws)
                 # Make plots
                 if options.save_single_event:
                     plt_bounds = np.atleast_2d([ev.min(axis = 0), ev.max(axis = 0)]).T
@@ -180,15 +180,15 @@
             # Save all single-event draws together
             posteriors = np.array(posteriors)
             save_density(posteriors, folder = output_draws, name = 'posteriors_single_event', ext = options.ext)
         else:
             # Load pre-computed posteriors
             posteriors = load_density(Path(output_draws, 'posteriors_single_event.'+options.ext))
         # Run hierarchical analysis
-        prior_pars = get_priors(options.bounds, samples = all_samples, std = options.sigma_prior, probit = options.probit, hierarchical = True)
+        prior_pars = get_priors(options.bounds, samples = events, std = options.sigma_prior, scale = options.scale, probit = options.probit, hierarchical = True)
         mix        = HDPGMM(options.bounds, prior_pars = prior_pars, MC_draws = options.mc_draws, probit = options.probit)
         draws      = np.array([mix.density_from_samples(posteriors) for _ in tqdm(range(options.n_draws), desc = 'Hierarchical')])
         # Save draws
         save_density(draws, folder = output_draws, name = 'draws_'+options.h_name, ext = options.ext)
     else:
         draws = load_density(Path(output_draws, 'draws_'+options.h_name+'.'+options.ext))
     # Plot
```

### Comparing `figaro-1.0.6/figaro/pipelines/par_hierarchical_inference.py` & `figaro-1.1.0/figaro/pipelines/par_hierarchical_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,51 +20,55 @@
 class worker:
     def __init__(self, bounds,
                        out_folder_plots,
                        out_folder_draws,
                        ext         = 'pkl',
                        se_sigma    = None,
                        hier_sigma  = None,
-                       all_samples = None,
+                       scale       = None,
+                       events      = None,
                        label       = None,
                        unit        = None,
                        save_se     = True,
-                       MC_draws    = 2000,
+                       MC_draws    = None,
                        probit      = True,
                        ):
         self.dim                  = bounds.shape[0]
         self.bounds               = bounds
         self.mixture              = DPGMM(self.bounds, probit = probit)
         self.hierarchical_mixture = HDPGMM(self.bounds,
                                            MC_draws   = MC_draws,
                                            probit     = probit,
                                            prior_pars = get_priors(self.bounds,
-                                                                   samples      = all_samples,
+                                                                   samples      = events,
                                                                    std          = hier_sigma,
+                                                                   scale        = scale,
                                                                    probit       = probit,
                                                                    hierarchical = True,
                                                                    )
                                             )
         self.out_folder_plots = out_folder_plots
         self.out_folder_draws = out_folder_draws
+        self.se_sigma         = se_sigma
+        self.scale            = scale
         self.save_se          = save_se
         self.label            = label
         self.unit             = unit
         self.posteriors       = None
         self.probit           = probit
         self.ext              = ext
 
     def run_event(self, pars):
         # Unpack data
         samples, name, n_draws = pars
         # Copying (issues with shuffling)
         ev = np.copy(samples)
         ev.setflags(write = True)
         # Actual inference
-        prior_pars = get_priors(self.bounds, samples = ev, probit = self.probit, std = self.se_sigma, hierarchical = False)
+        prior_pars = get_priors(self.bounds, samples = ev, probit = self.probit, std = self.se_sigma, scale = self.scale, hierarchical = False)
         self.mixture.initialise(prior_pars = prior_pars)
         draws      = [self.mixture.density_from_samples(ev) for _ in range(n_draws)]
         # Plots
         plt_bounds = np.atleast_2d([ev.min(axis = 0), ev.max(axis = 0)]).T
         if self.save_se:
             if self.dim == 1:
                 plot_median_cr(draws,
@@ -123,16 +127,17 @@
     parser.add_option("--se_draws", type = "int", dest = "n_se_draws", help = "Number of draws for single-event distribution. Default: same as hierarchical distribution", default = None)
     parser.add_option("--n_samples_dsp", type = "int", dest = "n_samples_dsp", help = "Number of samples to analyse (downsampling). Default: all", default = -1)
     parser.add_option("--exclude_points", dest = "exclude_points", action = 'store_true', help = "Exclude points outside bounds from analysis", default = False)
     parser.add_option("--cosmology", type = "string", dest = "cosmology", help = "Cosmological parameters (h, om, ol). Default values from Planck (2021)", default = '0.674,0.315,0.685')
     parser.add_option("-e", "--events", dest = "run_events", action = 'store_false', help = "Skip single-event analysis", default = True)
     parser.add_option("--se_sigma_prior", dest = "se_sigma_prior", type = "string", help = "Expected standard deviation (prior) for single-event inference - single value or n-dim values. If None, it is estimated from samples", default = None)
     parser.add_option("--sigma_prior", dest = "sigma_prior", type = "string", help = "Expected standard deviation (prior) for hierarchical inference - single value or n-dim values. If None, it is estimated from samples", default = None)
+    parser.add_option("--fraction", dest = "scale", type = "float", help = "Fraction of samples standard deviation for sigma prior. Overrided by sigma_prior.", default = None)
     parser.add_option("--n_parallel", dest = "n_parallel", type = "int", help = "Number of parallel threads", default = 4)
-    parser.add_option("--mc_draws", dest = "mc_draws", type = "int", help = "Number of draws for assignment MC integral", default = 2000)
+    parser.add_option("--mc_draws", dest = "mc_draws", type = "int", help = "Number of draws for assignment MC integral", default = None)
     parser.add_option("--snr_threshold", dest = "snr_threshold", type = "float", help = "SNR threshold for simulated GW datasets", default = None)
     parser.add_option("--far_threshold", dest = "far_threshold", type = "float", help = "FAR threshold for simulated GW datasets", default = None)
     parser.add_option("--no_probit", dest = "probit", action = 'store_false', help = "Disable probit transformation", default = True)
     parser.add_option("--config", dest = "config", type = "string", help = "Config file. Warning: command line options are ignored if provided", default = None)
 
     (options, args) = parser.parse_args()
 
@@ -218,15 +223,14 @@
         dim = np.shape(events[0][0])[-1]
     except IndexError:
         dim = 1
     if options.exclude_points:
         print("Ignoring points outside bounds.")
         for i, ev in enumerate(events):
             events[i] = ev[np.where((np.prod(options.bounds[:,0] < ev, axis = 1) & np.prod(ev < options.bounds[:,1], axis = 1)))]
-        all_samples = np.atleast_2d(np.concatenate(events))
     else:
         # Check if all samples are within bounds
         all_samples = np.atleast_2d(np.concatenate(events))
         if options.probit:
             if not np.alltrue([(all_samples[:,i] > options.bounds[i,0]).all() and (all_samples[:,i] < options.bounds[i,1]).all() for i in range(dim)]):
                 raise ValueError("One or more samples are outside the given bounds.")
 
@@ -249,15 +253,16 @@
         ray.init(num_cpus = options.n_parallel)
         pool = ActorPool([worker.remote(bounds           = options.bounds,
                                         out_folder_plots = output_plots,
                                         out_folder_draws = output_draws,
                                         ext              = options.ext,
                                         se_sigma         = options.se_sigma_prior,
                                         hier_sigma       = options.sigma_prior,
-                                        all_samples      = all_samples,
+                                        scale            = options.scale,
+                                        events           = events,
                                         label            = symbols,
                                         unit             = units,
                                         save_se          = options.save_single_event,
                                         MC_draws         = options.mc_draws,
                                         probit           = options.probit,
                                         )
                           for _ in range(options.n_parallel)])
```

### Comparing `figaro-1.0.6/figaro/pipelines/par_probability_density.py` & `figaro-1.1.0/figaro/pipelines/par_probability_density.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 
 @ray.remote
 class worker:
     def __init__(self, bounds,
                        sigma = None,
                        samples = None,
                        probit = True,
+                       scale = None,
                        ):
         self.dim     = bounds.shape[-1]
-        self.mixture = DPGMM(bounds, prior_pars = get_priors(bounds, samples = samples, std = sigma, probit = probit, hierarchical = False), probit = probit)
+        self.mixture = DPGMM(bounds, prior_pars = get_priors(bounds, samples = samples, std = sigma, scale = scale, probit = probit, hierarchical = False), probit = probit)
         self.samples = np.copy(samples)
         self.samples.setflags(write = True)
 
     def draw_sample(self):
         return self.mixture.density_from_samples(self.samples)
 
 def main():
@@ -48,14 +49,15 @@
     parser.add_option("--unit", type = "string", dest = "unit", help = "LaTeX-style quantity unit, for plotting purposes", default = None)
     # Settings
     parser.add_option("--draws", type = "int", dest = "n_draws", help = "Number of draws", default = 100)
     parser.add_option("--n_samples_dsp", type = "int", dest = "n_samples_dsp", help = "Number of samples to analyse (downsampling). Default: all", default = -1)
     parser.add_option("--exclude_points", dest = "exclude_points", action = 'store_true', help = "Exclude points outside bounds from analysis", default = False)
     parser.add_option("--cosmology", type = "string", dest = "cosmology", help = "Cosmological parameters (h, om, ol). Default values from Planck (2021)", default = '0.674,0.315,0.685')
     parser.add_option("--sigma_prior", dest = "sigma_prior", type = "string", help = "Expected standard deviation (prior) - single value or n-dim values. If None, it is estimated from samples", default = None)
+    parser.add_option("--fraction", dest = "scale", type = "float", help = "Fraction of samples standard deviation for sigma prior. Overrided by sigma_prior.", default = None)
     parser.add_option("--n_parallel", dest = "n_parallel", type = "int", help = "Number of parallel threads", default = 4)
     parser.add_option("--snr_threshold", dest = "snr_threshold", type = "float", help = "SNR threshold for simulated GW datasets", default = None)
     parser.add_option("--far_threshold", dest = "far_threshold", type = "float", help = "FAR threshold for simulated GW datasets", default = None)
     parser.add_option("--no_probit", dest = "probit", action = 'store_false', help = "Disable probit transformation", default = True)
     parser.add_option("--config", dest = "config", type = "string", help = "Config file. Warning: command line options are ignored if provided", default = None)
     
     (options, args) = parser.parse_args()
@@ -149,14 +151,15 @@
 
         # Reconstruction
         if not options.postprocess:
             # Actual analysis
             desc = name + ' ({0}/{1})'.format(i+1, len(files))
             pool = ActorPool([worker.remote(bounds  = options.bounds,
                                             sigma   = options.sigma_prior,
+                                            scale   = options.scale,
                                             samples = samples,
                                             probit  = options.probit,
                                             )
                               for _ in range(options.n_parallel)])
             draws = []
             for s in tqdm(pool.map_unordered(lambda a, v: a.draw_sample.remote(), [_ for _ in range(options.n_draws)]), total = options.n_draws, desc = desc):
                 draws.append(s)
```

### Comparing `figaro-1.0.6/figaro/pipelines/ppplot.py` & `figaro-1.1.0/figaro/pipelines/ppplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,19 @@
     events, names = load_data(options.samples_folder, n_samples = options.n_samples_dsp)
     try:
         dim = np.shape(events[0][0])[-1]
     except IndexError:
         dim = 1
     if dim > 3:
         raise Exception("PP-plots can be computed up to 3 dimensions")
+    # Load true values
+    if options.true_vals is not None:
+        options.true_vals = Path(options.true_vals).resolve()
+        with open(options.true_vals, 'r') as f:
+            true_vals = json.load(f)
     # Check all events have an entry in true_vals dict
     if not np.array([name in true_vals.keys() for name in names]).all():
         raise Exception("Please provide a dictionary storing all the true values. Dict keys must match event names. The following events appear not to have a true value:\n{0}".format(np.array(names)[np.where([name not in true_vals.keys() for name in names])]))
 
     if options.exclude_points:
         print("Ignoring points outside bounds.")
         for i, ev in enumerate(events):
@@ -115,30 +120,24 @@
             symbols = options.symbol
         if options.unit is not None:
             units = options.unit.split(',')
         else:
             units = options.unit
     # Read grid points
     if options.grid_points is not None:
-        pts = options.grid_points.split('.')
+        pts = options.grid_points.split(',')
         if len(pts) == dim:
             options.grid_points = np.array([int(d) for d in pts])
         elif len(pts) == 1:
             options.grid_points = np.ones(dim, dtype = int)*int(pts[0])
         else:
             print("Wrong number of grid point provided. Falling back to default number")
-            options.grid_points = np.ones(dim, dtype = int)*int((1000/dim**2)**dim)
+            options.grid_points = np.ones(dim, dtype = int)*200
     else:
-        options.grid_points = np.ones(dim, dtype = int)*int((1000/dim**2)**dim)
-
-    # Load true values
-    if options.true_vals is not None:
-        options.true_vals = Path(options.true_vals).resolve()
-        with open(options.true_vals, 'r') as f:
-            true_vals = json.load(f)
+        options.grid_points = np.ones(dim, dtype = int)*200
 
     # Reconstruction
     if not options.postprocess:
         mix        = DPGMM(options.bounds, probit = options.probit)
         grid, diff = recursive_grid(options.bounds, options.grid_points)
         logdiff    = np.sum(np.log(diff))
         posteriors = []
```

### Comparing `figaro-1.0.6/figaro/pipelines/probability_density.py` & `figaro-1.1.0/figaro/pipelines/probability_density.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     parser.add_option("--unit", type = "string", dest = "unit", help = "LaTeX-style quantity unit, for plotting purposes", default = None)
     # Settings
     parser.add_option("--draws", type = "int", dest = "n_draws", help = "Number of draws", default = 100)
     parser.add_option("--n_samples_dsp", type = "int", dest = "n_samples_dsp", help = "Number of samples to analyse (downsampling). Default: all", default = -1)
     parser.add_option("--exclude_points", dest = "exclude_points", action = 'store_true', help = "Exclude points outside bounds from analysis", default = False)
     parser.add_option("--cosmology", type = "string", dest = "cosmology", help = "Cosmological parameters (h, om, ol). Default values from Planck (2021)", default = '0.674,0.315,0.685')
     parser.add_option("--sigma_prior", dest = "sigma_prior", type = "string", help = "Expected standard deviation (prior) - single value or n-dim values. If None, it is estimated from samples", default = None)
+    parser.add_option("--fraction", dest = "scale", type = "float", help = "Fraction of samples standard deviation for sigma prior. Overrided by sigma_prior.", default = None)
     parser.add_option("--snr_threshold", dest = "snr_threshold", type = "float", help = "SNR threshold for simulated GW datasets", default = None)
     parser.add_option("--far_threshold", dest = "far_threshold", type = "float", help = "FAR threshold for simulated GW datasets", default = None)
     parser.add_option("--no_probit", dest = "probit", action = 'store_false', help = "Disable probit transformation", default = True)
     parser.add_option("--config", dest = "config", type = "string", help = "Config file. Warning: command line options are ignored if provided", default = None)
     
     (options, args) = parser.parse_args()
 
@@ -122,15 +123,15 @@
             if options.probit:
                 if not np.alltrue([(samples[:,i] > options.bounds[i,0]).all() and (samples[:,i] < options.bounds[i,1]).all() for i in range(dim)]):
                     raise ValueError("One or more samples are outside the given bounds.")
 
         # Reconstruction
         if not options.postprocess:
             # Actual analysis
-            prior_pars = get_priors(options.bounds, samples = samples, std = options.sigma_prior, probit = options.probit, hierarchical = False)
+            prior_pars = get_priors(options.bounds, samples = samples, std = options.sigma_prior, scale = options.scale, probit = options.probit, hierarchical = False)
             mix        = DPGMM(options.bounds, prior_pars = prior_pars, probit = options.probit)
             desc       = name + ' ({0}/{1})'.format(i+1, len(files))
             draws      = np.array([mix.density_from_samples(samples) for _ in tqdm(range(options.n_draws), desc = desc)])
             # Save reconstruction
             save_density(draws, folder = output_draws, name = 'draws_'+name, ext = options.ext)
         else:
             draws = load_density(Path(output_draws, 'draws_'+name+'.'+options.ext))
```

### Comparing `figaro-1.0.6/figaro/plot.py` & `figaro-1.1.0/figaro/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,37 +141,38 @@
             x_min = bounds[0]
         if not bounds[1] <= x_max and probit:
             warnings.warn("The provided upper bound is invalid for at least one draw. {0} will be used instead.".format(x_max))
         else:
             x_max = bounds[1]
 
     fig, ax = plt.subplots()
+
     # If samples are available, use them as bounds
     if samples is not None:
         ax.hist(samples, bins = int(np.sqrt(len(samples))), histtype = 'step', density = True, label = '$\mathrm{Samples}$', log = True)
-        x_min_l, x_max_l = ax.get_xlim()
-        x_min = np.max((x_min, x_min_l))
-        x_max = np.min((x_max, x_max_l))
-        
-    x    = np.linspace(x_min, x_max, n_pts+2)[1:-1]
+        if bounds is None:
+            x_min_l, x_max_l = ax.get_xlim()
+            x_min = np.max((x_min, x_min_l))
+            x_max = np.min((x_max, x_max_l))
+    xlim = (x_min, x_max)
+    x    = np.linspace(x_min, x_max, n_pts)
     dx   = x[1]-x[0]
     
     probs = np.array([d.pdf(x) for d in draws])
     
     percentiles = [50, 5, 16, 84, 95]
     p = {}
     for perc in percentiles:
         p[perc] = np.percentile(probs, perc, axis = 0)
     norm = p[50].sum()*dx
     for perc in percentiles:
         p[perc] = p[perc]/norm
 
     # Samples (if available)
     if samples is not None:
-        xlim = ax.get_xlim()
         ylim = ax.get_ylim()
     else:
         ax.set_yscale('log')
     
     # CR
     ax.fill_between(x, p[95], p[5], color = 'mediumturquoise', alpha = 0.25)
     ax.fill_between(x, p[84], p[16], color = 'darkturquoise', alpha = 0.25)
@@ -291,15 +292,15 @@
         if show:
             ax.set_yscale('linear')
             ax.autoscale(True)
             plt.show()
         plt.close()
     
 
-def plot_multidim(draws, samples = None, bounds = None, out_folder = '.', name = 'density', labels = None, units = None, hierarchical = False, show = False, save = True, subfolder = False, n_pts = 200, true_value = None, figsize = 7, levels = [0.5, 0.68, 0.9], scatter_points = False, median_label = None):
+def plot_multidim(draws, samples = None, bounds = None, out_folder = '.', name = 'density', labels = None, units = None, hierarchical = False, show = False, save = True, subfolder = False, n_pts = 200, true_value = None, levels = [0.5, 0.68, 0.9], scatter_points = False, median_label = None):
     """
     Plot the recovered multidimensional distribution along with samples from the true distribution (if available) as corner plot.
     
     Arguments:
         :iterable draws:         container for mixture instances
         :int dim:                number of dimensions
         :np.ndarray samples:     samples from the true distribution (if available)
@@ -310,36 +311,38 @@
         :list-of-str units:      LaTeX-style quantity unit, for plotting purposes
         :bool hierarchical:      hierarchical inference, for plotting purposes
         :bool save:              whether to save the plot or not
         :bool show:              whether to show the plot during the run or not
         :bool subfolder:         whether to save in a dedicated subfolder
         :int n_pts:              number of grid points (same for each dimension)
         :iterable true_value:    true value to plot
-        :double figsize:         figure size (matplotlib)
         :iterable levels:        credible levels to plot
         :bool scatter_points:    scatter samples on 2d plots
         :str median_label:       label to assign to the reconstruction
     """
     
     dim = draws[0].dim
     if median_label is None:
         if hierarchical:
             median_label = '\mathrm{(H)DPGMM}'
         else:
             median_label = '\mathrm{DPGMM}'
     if labels is None:
-        labels = ['$x_{0}$'.format(i+1) for i in range(dim)]
+        labels = ['$x_{'+'{0}'.format(i+1)+'}$' for i in range(dim)]
     else:
         labels = ['${0}$'.format(l) for l in labels]
     
     if units is not None:
         labels = [l[:-1]+'\ [{0}]$'.format(u) if not u == '' else l for l, u in zip(labels, units)]
     
     levels = np.atleast_1d(levels)
-
+    
+    ext_bounds = False
+    if bounds is not None:
+        ext_bounds = True
     all_bounds = np.atleast_2d([d.bounds for d in draws])
     x_min = np.min(all_bounds, axis = -1).max(axis = 0)
     x_max = np.max(all_bounds, axis = -1).min(axis = 0)
     
     probit = np.array([d.probit for d in draws]).any()
     
     if bounds is not None:
@@ -354,46 +357,46 @@
                 warnings.warn("The provided upper bound is invalid for at least one draw. Default values will be used instead.")
             x_max[np.where(bounds[:,1] <= x_max)] = bounds[:,1][np.where(bounds[:,1] <= x_max)]
         else:
             warnings.warn("The provided bounds have an invalid shape {0}. Shape must be (1,2) or (dim, 2).\nDefault bounds will be used instead.".format(bounds.shape))
     bounds = np.array([x_min, x_max]).T
     
     K = dim
-    factor = 2.0          # size of one side of one panel
+    factor = 3.0          # size of one side of one panel
     lbdim = 0.5 * factor  # size of left/bottom margin
     trdim = 0.2 * factor  # size of top/right margin
-    whspace = 0.1         # w/hspace size
+    whspace = 0.2         # w/hspace size
     plotdim = factor * dim + factor * (K - 1.0) * whspace
     dim_plt = lbdim + plotdim + trdim
     
-    fig, axs = plt.subplots(K, K, figsize=(figsize, figsize))
+    fig, axs = plt.subplots(K, K, figsize=(dim_plt, dim_plt))
     # Format the figure.
     lb = lbdim / dim_plt
     tr = (lbdim + plotdim) / dim_plt
     fig.subplots_adjust(left=lb, bottom=lb, right=tr, top=tr, wspace=whspace, hspace=whspace)
     # Samples (if available)
     if samples is not None:
-        bins = [int(np.sqrt(len(samples[:, c]))) for c in range(dim)]
-        corner(samples, color = '#1f77b4', fig = fig, hist_kwargs = {'density': True, 'label':'$\mathrm{Samples}$', 'linewidth':0.7} , plot_density = False, contour_kwargs = {'linewidths':0.3, 'linestyles':'dashed'}, levels = [0.5,0.68,0.9], no_fill_contours = True, bins = bins)
+        bins = np.array([int(np.sqrt(len(samples[:, c]))) for c in range(dim)])
+        corner(samples, color = '#1f77b4', fig = fig, hist_kwargs = {'density': True, 'label':'$\mathrm{Samples}$', 'linewidth':0.7} , plot_density = False, contour_kwargs = {'linewidths':0.3, 'linestyles':'dashed'}, levels = [0.5,0.68,0.9], no_fill_contours = True, hist_bin_factor = bins/20, quiet = True)
         
     # 1D plots (diagonal)
     for column in range(K):
         ax = axs[column, column]
         # Marginalise over all uninterested columns
         dims = list(np.arange(dim))
         dims.remove(column)
         marg_draws = marginalise(draws, dims)
         # Credible regions
         lim = bounds[column]
-        if samples is not None:
+        if samples is not None and not ext_bounds:
             lim_l = ax.get_xlim()
             lim[0] = np.max((lim[0], lim_l[0]))
             lim[1] = np.min((lim[1], lim_l[1]))
             
-        x   = np.linspace(lim[0], lim[1], n_pts+2)[1:-1]
+        x   = np.linspace(lim[0], lim[1], n_pts)
         dx  = x[1]-x[0]
         
         probs = np.array([d.pdf(x) for d in marg_draws])
         
         percentiles = [50, 5, 16, 84, 95]
         p = {}
         for perc in percentiles:
@@ -437,24 +440,24 @@
             dims = list(np.arange(dim))
             dims.remove(column)
             dims.remove(row)
             marg_draws = marginalise(draws, dims)
             
             # Credible regions
             lim = bounds[[row, column]]
-            if samples is not None:
+            if samples is not None and not ext_bounds:
                 lim_l = np.array([ax.get_ylim(), ax.get_xlim()])
                 for i in range(2):
                     lim[i,0] = np.max((lim[i,0], lim_l[i,0]))
                     lim[i,1] = np.min((lim[i,1], lim_l[i,1]))
                 
             grid, dgrid = recursive_grid(lim[::-1], np.ones(2, dtype = int)*int(n_pts))
             
-            x = np.linspace(lim[0,0], lim[0,1], n_pts+2)[1:-1]
-            y = np.linspace(lim[1,0], lim[1,1], n_pts+2)[1:-1]
+            x = np.linspace(lim[0,0], lim[0,1], n_pts)
+            y = np.linspace(lim[1,0], lim[1,1], n_pts)
             
             dd = np.array([d.pdf(grid) for d in marg_draws])
             median = np.percentile(dd, 50, axis = 0)
             median = median/(median.sum()*np.prod(dgrid))
             median = median.reshape(n_pts, n_pts)
             
             X,Y = np.meshgrid(x,y)
@@ -483,18 +486,21 @@
             yticks = np.linspace(lim[0,0], lim[0,1], 5)
             ax.set_yticks(yticks)
             ax.set_xlim(*lim[1])
             ax.set_ylim(*lim[0])
             if column == 0:
                 ax.set_ylabel(labels[row])
                 [l.set_rotation(45) for l in ax.get_yticklabels()]
+            else:
+                ax.set_yticklabels([])
             if row == K - 1:
                 [l.set_rotation(45) for l in ax.get_xticklabels()]
                 ax.set_xlabel(labels[column])
-
+            else:
+                ax.set_xticklabels([])
     fig.axes[K-1].legend(*fig.axes[0].get_legend_handles_labels(), loc = 'center')
     fig.align_labels()
     
     if show:
         plt.show()
     if save:
         if not subfolder:
@@ -658,15 +664,15 @@
         :str name:               name to be given to outputs
         :bool save:              whether to save the plot or not
         :bool show:              whether to show the plot during the run or not
     """
     all_bounds = np.atleast_2d([d.bounds[0] for d in draws])
     x_min = np.max(all_bounds[:,0])
     x_max = np.min(all_bounds[:,1])
-    x = np.linspace(x_min, x_max, n_points+2)[1:-1]
+    x = np.linspace(x_min, x_max, n_points)
     
     functions     = np.array([mix(x) for mix in draws])
     median        = np.percentile(functions, 50, axis = 0)
     cdf_draws     = np.array([fast_cumulative(d) for d in functions])
     cdf_median    = fast_cumulative(median)
     cdf_injection = fast_cumulative(injection(x))
```

### Comparing `figaro-1.0.6/figaro/threeDvolume.py` & `figaro-1.1.0/figaro/threeDvolume.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from astropy.io import fits
 from astropy.wcs import WCS
 import pyvo as vo
 import socket
 
 from scipy.special import logsumexp
 from scipy.stats import multivariate_normal as mn
-from numba import jit, prange
+from numba import njit, prange
 import dill
 
 from figaro.mixture import DPGMM
 from figaro.transform import *
 from figaro.coordinates import celestial_to_cartesian, cartesian_to_celestial, inv_Jacobian
 from figaro.credible_regions import ConfidenceArea, ConfidenceVolume, FindNearest_Volume, FindLevelForHeight
 from figaro.diagnostic import compute_entropy_single_draw, angular_coefficient
@@ -37,15 +37,15 @@
     warnings.warn("LAL is not installed. If provided, galaxy catalog will not be loaded")
     lal_flag = False
 
 from pathlib import Path
 from distutils.spawn import find_executable
 from tqdm import tqdm
 
-@jit
+@njit
 def log_add(x, y):
     """
     Compute log(np.exp(x) + np.exp(y))
     
     Arguments:
         :double x: first addend (log)
         :double y: second addend (log)
@@ -54,15 +54,15 @@
         :double: log(np.exp(x) + np.exp(y))
     """
     if x >= y:
         return x+np.log1p(np.exp(y-x))
     else:
         return y+np.log1p(np.exp(x-y))
 
-@jit
+@njit
 def log_add_array(x,y):
     """
     Compute log(np.exp(x) + np.exp(y)) element-wise
     
     Arguments:
         :np.ndarray x: first addend (log)
         :np.ndarray y: second addend (log)
@@ -157,17 +157,17 @@
             
         if latex:
             if find_executable('latex'):
                 rcParams["text.usetex"] = True
         self.latex = latex
         
         # Grid
-        self.ra   = np.linspace(0,2*np.pi, n_gridpoints[0], endpoint = False)
-        self.dec  = np.linspace(-np.pi/2, np.pi/2., n_gridpoints[1]+2)[1:-1]
-        self.dist = np.linspace(0, max_dist, n_gridpoints[2]+2)[1:-1]
+        self.ra   = np.linspace(0,2*np.pi, n_gridpoints[0])
+        self.dec  = np.linspace(-np.pi/2, np.pi/2., n_gridpoints[1])
+        self.dist = np.linspace(0, max_dist, n_gridpoints[2])
         self.dD   = np.diff(self.dist)[0]
         self.dra  = np.diff(self.ra)[0]
         self.ddec = np.diff(self.dec)[0]
         # For loops
         grid = []
         measure_3d = []
         distance_measure_3d = []
```

### Comparing `figaro-1.0.6/figaro/transform.py` & `figaro-1.1.0/figaro/transform.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,16 +49,24 @@
     cdf = 0.5*(1.0+erf(x/(np.sqrt(2.0)*sigma)))
     o = bounds[:,0]+dbounds*cdf
     return o
 
 def probit_log_jacobian(x, bounds):
     dbounds = bounds[:,1]-bounds[:,0]
     sigma   = dbounds*0.34
-    return -0.5*(x/sigma)**2-0.5*(log2PI + np.log(sigma))+np.log(dbounds)
+    res     = -0.5*(x/sigma)**2-0.5*(log2PI)+np.log(dbounds)-np.log(sigma)
+    return res
 
 def probit_logJ(x, bounds, flag = True):
     if not flag:
         return np.zeros(len(x))
     dbounds = bounds[:,1]-bounds[:,0]
     sigma   = dbounds*0.34
-    res     = np.sum(-0.5*(x/sigma)**2-0.5*(log2PI + np.log(sigma))+np.log(dbounds), axis = -1)
+    res     = np.sum(-0.5*(x/sigma)**2-0.5*log2PI+np.log(dbounds)-np.log(sigma), axis = -1)
     return res
+
+def log_gradient_inv_jacobian(x, bounds, flag = True):
+    if not flag:
+        return np.zeros(len(x))
+    dbounds = bounds[:,1]-bounds[:,0]
+    sigma   = dbounds*0.34
+    return x/sigma
```

### Comparing `figaro-1.0.6/figaro/utils.py` & `figaro-1.1.0/figaro/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pathlib import Path
 from tqdm import tqdm
 from typing import cast
 from collections import Counter
 from scipy.stats import multivariate_normal as mn
 
-from figaro.transform import transform_to_probit
+from figaro.transform import transform_to_probit, transform_from_probit
 from figaro.exceptions import FIGAROException
 
 #-–––––––––-#
 # Utilities #
 #-----------#
 
 def recursive_grid(bounds, n_pts, get_1d = False):
@@ -29,25 +29,25 @@
         :np.ndarray: grid
         :np.ndarray: differential for each grid
         :np.ndarray: list of 1d-arrays (one per dimension)
     """
     bounds = np.atleast_2d(bounds)
     n_pts  = np.atleast_1d(n_pts)
     if len(bounds) == 1:
-        d  = np.linspace(bounds[0,0], bounds[0,1], n_pts[0]+2)[1:-1]
+        d  = np.linspace(bounds[0,0], bounds[0,1], n_pts[0])
         dD = d[1]-d[0]
         if get_1d:
             return np.atleast_2d(d).T, [dD], [d]
         return np.atleast_2d(d).T, [dD]
     else:
         if get_1d:
             grid_nm1, diff, l_1d = recursive_grid(np.array(bounds)[1:], n_pts[1:], get_1d)
         else:
             grid_nm1, diff = recursive_grid(np.array(bounds)[1:], n_pts[1:], get_1d)
-        d = np.linspace(bounds[0,0], bounds[0,1], n_pts[0]+2)[1:-1]
+        d = np.linspace(bounds[0,0], bounds[0,1], n_pts[0])
         diff.insert(0, d[1]-d[0])
         grid     = []
         for di in d:
             for gi in grid_nm1:
                 grid.append([di,*gi])
         if get_1d:
             l_1d.insert(0, d)
@@ -76,15 +76,15 @@
     while len(samples) < n_draws:
         pts   = np.random.uniform(bounds[0], bounds[1], size = n_draws)
         probs = f(pts)*selfunc(pts)
         h     = np.random.uniform(0, top, size = n_draws)
         samples.extend(pts[np.where(h < probs)])
     return np.array(samples).flatten()[:n_draws]
 
-def get_priors(bounds, samples = None, mean = None, std = None, cov = None, df = None, k = None, a = None, scale = 5., probit = True, hierarchical = False):
+def get_priors(bounds, samples = None, mean = None, std = None, cov = None, df = None, k = None, a = None, scale = None, probit = True, hierarchical = False):
     """
     This method takes the prior parameters for the Normal-Inverse-Wishart distribution in the natural space and returns them as parameters in the probit space, ordered as required by FIGARO. In the following, D will denote the dimensionality of the inferred distribution.
 
     Four parameters are returned:
     * df, is the number of degrees of freedom for the Inverse Wishart distribution,. It must be greater than D+1. If this parameter is None or does not satisfy the condition df > D+1, the default value D+2 is used;
     * k is the scale parameter for the multivariate Normal distribution. Suggested values are  k <~ 1e-1. If None, the default value 1e-2 is used.
     * mu is the mean of the multivariate Normal distribution. It can be either estimated from the available samples or passed directly as a 1D array with length D (the keyword argument mean overrides the samples). If None, the default value 0 (corresponding to the parameter space center) is used.
@@ -93,15 +93,15 @@
         * passed as 1D array with shape (D,) or double: vector of standard deviations (if double, it assumes that the same std has to be used for all dimensions) - keyword std;
         * estimated from samples - keyword samples.
        
     The order in which they are returned is (k,L,df,mu).
     
     Arguments:
         :np.ndarray bounds:              boundaries for probit transformation
-        :np.ndarray samples:             2D array with samples
+        :np.ndarray samples:             2D [DPGMM] or 3D [(H)DPGMM] array with samples
         :double or np.ndarray mean:      mean [DPGMM]
         :double or np.ndarray std:       expected standard deviation (if double, the same std is used for all dimensions, if np.ndarray must match the number of dimensions) [DPGMM and (H)DPGMM]
         :np.ndarray cov:                 covariance matrix [DPGMM]
         :int df:                         degrees of freedom for Inverse Wishart distribution [DPGMM]
         :double k:                       scale parameter for Normal distribution [DPGMM]
         :double a:                       shape parameter for the Inverse Gamma distribution [(H)DPGMM]
         :double scale:                   fraction of samples std [DPGMM]
@@ -109,42 +109,48 @@
         :bool hierarchical:              returns the prior pars for (H)DPGMM rather than for DPGMM
         
     Returns:
         :tuple: prior parameters ordered as in (H)/DPGMM
     """
     bounds = np.atleast_2d(bounds)
     dim = len(bounds)
+    if scale is None:
+        scale = 5.
     if samples is not None:
-        if len(np.shape(samples)) < 2:
+        if not np.iterable(samples[0]):
             samples = np.atleast_2d(samples).T
         if probit:
-            probit_samples = transform_to_probit(samples, bounds)
+            if hierarchical:
+                probit_samples = [transform_to_probit(s, bounds) for s in samples]
+            else:
+                probit_samples = transform_to_probit(samples, bounds)
     if hierarchical:
         if std is not None:
             out_sigma = np.atleast_2d(std)*np.ones((1, dim))
             if probit:
                 out_sigma = transform_to_probit(np.mean(bounds, axis = -1)+out_sigma, bounds)
         elif samples is not None:
             if probit:
-                out_sigma = np.sqrt(np.diag(np.atleast_2d(np.cov(probit_samples.T))))
+                all_samples     = np.concatenate(probit_samples, axis = 0)
+                events_avg_cov  = np.diag(np.atleast_2d(np.mean([np.cov(ev.T) for ev in probit_samples], axis = 0)))
             else:
-                out_sigma = np.sqrt(np.diag(np.atleast_2d(np.cov(samples.T))))
-            out_sigma = out_sigma/scale
+                all_samples     = np.concatenate(samples, axis = 0)
+                events_avg_cov  = np.diag(np.atleast_2d(np.mean([np.cov(ev.T) for ev in samples], axis = 0)))
+            all_samples_cov = np.diag(np.atleast_2d(np.cov(all_samples.T)))
+            out_sigma       = (np.sqrt(all_samples_cov - events_avg_cov)/scale).flatten()
         else:
-            out_sigma = np.diff(bounds, axis = -1)/10.
+            out_sigma = np.diff(bounds, axis = -1)/scale
             if probit:
                 out_sigma = transform_to_probit(np.mean(bounds, axis = -1)+out_sigma, bounds)
         out_sigma = out_sigma.flatten()
         if a is not None:
             out_a = a
         else:
             out_a = 2.
-            
         return (out_sigma, out_a)
-    
     else:
         # DF
         if df is not None and df > dim+2:
             df_out = df
         else:
             df_out = dim+2
             
@@ -156,70 +162,78 @@
                 raise ValueError("Mean is outside of the given bounds")
             if probit:
                 mu_out = transform_to_probit(mean, bounds)
             else:
                 mu_out = mean
         elif samples is not None:
             if probit:
-                mu_out = np.atleast_1d(np.mean(probit_samples, axis = 0))
+                mu_out = np.atleast_1d(np.median(probit_samples, axis = 0))
             else:
-                mu_out = np.atleast_1d(np.mean(samples, axis = 0))
+                mu_out = np.atleast_1d(np.median(samples, axis = 0))
         else:
             if probit:
                 mu_out = np.zeros(dim)
             else:
                 mu_out = np.atleast_1d(np.mean(bounds, axis = 1))
         # L
         if cov is not None:
             L_out = cov
             if probit:
                 draw_flag = True
         elif std is not None:
-            L_out = np.identity(dim)*std**2
             if probit:
-                draw_flag = True
+                L_out = np.identity(dim)*np.minimum(np.abs(mu_out - transform_to_probit((transform_from_probit(mu_out, bounds) + std), bounds)), np.abs(mu_out - transform_to_probit((transform_from_probit(mu_out, bounds) - std), bounds)))**2
+            else:
+                L_out = np.identity(dim)*std**2
         elif samples is not None:
             if probit:
-                L_out = np.atleast_2d(np.cov(probit_samples.T))
+                cov_samples = np.atleast_2d(np.cov(probit_samples.T))
             else:
-                L_out = np.atleast_2d(np.cov(samples.T))
-            L_out = np.identity(dim)*np.diag(L_out/scale**2)
+                cov_samples = np.atleast_2d(np.cov(samples.T))
+            L_out = np.identity(dim)*np.diag(cov_samples/scale**2)
         else:
             if probit:
-                L_out = np.identity(dim)*0.2**2
+                sigma = transform_to_probit(np.atleast_2d(np.mean(bounds, axis = -1)+np.diff(bounds, axis = -1).flatten()/scale), bounds)[0]
+                L_out = np.identity(dim)*sigma**2
             else:
-                L_out = np.identity(dim)*(np.diff(bounds, axis = 1)/10)**2
+                L_out = np.identity(dim)*(np.diff(bounds, axis = -1).flatten()/scale)**2
         if draw_flag:
-            ss = mn(np.mean(bounds, axis = -1), L_out).rvs(3000)
+            ss = mn(np.mean(bounds, axis = -1), L_out, allow_singular = True).rvs(3000)
             if dim == 1:
                 ss = np.atleast_2d(ss).T
             # Keeping only samples within bounds
             ss = ss[np.where((np.prod(bounds[:,0] < ss, axis = 1) & np.prod(ss < bounds[:,1], axis = 1)))]
-            probit_samples = transform_to_probit(ss, bounds)
-            L_out = np.atleast_2d(np.cov(probit_samples.T))
+            probit_ss = transform_to_probit(ss, bounds)
+            L_out = np.identity(dim)*np.diag(np.atleast_2d(np.cov(probit_ss.T)))
         # k
         if k is not None:
             k_out = k
         else:
-            s, log_k_out = np.linalg.slogdet(L_out)
-            k_out = np.exp(log_k_out/dim)
+            if samples is not None:
+                if probit:
+                    cov_samples = np.atleast_2d(np.cov(probit_samples.T))
+                else:
+                    cov_samples = np.atleast_2d(np.cov(samples.T))
+                k_out = np.min(np.diag(L_out)/np.diag(cov_samples))
+            else:
+                k_out = 1./(scale)
         return (k_out, L_out, df_out, mu_out)
 
-def rvs_median(draws, n_draws):
+def rvs_median(draws, size = 1):
     """
     Generates samples from median distribution of a set of draws.
     
     Arguments:
         :iterable draws: container for mixture instances
-        :int n_draws:    number of samples
+        :int size:    number of samples
     
     Returns:
         :np.ndarray: samples
     """
-    idx = np.random.choice(np.arange(len(draws)), size = int(n_draws))
+    idx = np.random.choice(np.arange(len(draws)), size = int(size))
     ctr = Counter(idx)
     samples = np.empty(shape = (1, draws[0].dim))
     for i, n in zip(ctr.keys(), ctr.values()):
         samples = np.concatenate((samples, draws[i].rvs(n)))
     return samples[1:]
     
 def make_single_gaussian_mixture(mu, cov, bounds, out_folder = '.', save = False, n_samps = 3000, probit = True):
@@ -258,15 +272,15 @@
     
     if len(cov.shape) == 1:
         cov = np.atleast_2d(cov).T
     
     mixtures = []
     for i, (m, c) in enumerate(zip(mu, cov)):
         if probit:
-            ss = np.atleast_2d(mn(m, c).rvs(n_samps))
+            ss = np.atleast_2d(mn(m, c, allow_singular = True).rvs(n_samps))
             # 1D issue
             if c.shape == (1,) or c.shape == (1,1):
                 ss = ss.T
             # Keeping only samples within bounds
             ss = ss[np.where((np.prod(bounds[:,0] < ss, axis = 1) & np.prod(ss < bounds[:,1], axis = 1)))]
             if save:
                 np.savetxt(Path(events_folder, 'event_{0}.txt'.format(i+1)), ss)
@@ -274,15 +288,15 @@
             p_ss = transform_to_probit(ss, bounds)
             mm = np.mean(p_ss, axis = 0)
             cc = np.atleast_2d(np.cov(p_ss.T))
         else:
             mm = m
             cc = c
             if save:
-                ss = np.atleast_2d(mn(m, c).rvs(n_samps))
+                ss = np.atleast_2d(mn(m, c, allow_singular = True).rvs(n_samps))
                 if c.shape == (1,1):
                     ss = ss.T
                 np.savetxt(Path(events_folder, 'event_{0}.txt'.format(i+1)), ss)
         mix = mixture(np.atleast_2d([mm]), np.atleast_3d([cc]), np.ones(1), bounds, len(bounds), 1, None, probit = probit)
         mixtures.append([mix])
     
     mixtures = np.array(mixtures)
```

### Comparing `figaro-1.0.6/figaro.egg-info/PKG-INFO` & `figaro-1.1.0/figaro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.0.6
+Version: 1.1.0
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Home-page: https://github.com/sterinaldi/figaro
 Author: Stefano Rinaldi, Walter Del Pozzo, Daniele Sanfratello
 Author-email: stefano.rinaldi@phd.unipi.it, walter.delpozzo@unipi.it, d.sanfratello@studenti.unipi.it
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `figaro-1.0.6/figaro.egg-info/SOURCES.txt` & `figaro-1.1.0/figaro.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 figaro_env.yml
 install.sh
+pyproject.toml
 requirements.txt
 setup.py
 figaro/__init__.py
 figaro/coordinates.py
 figaro/cosmology.c
 figaro/cosmology.pxd
 figaro/cosmology.pyx
```

### Comparing `figaro-1.0.6/install.sh` & `figaro-1.1.0/install.sh`

 * *Files identical despite different names*

### Comparing `figaro-1.0.6/setup.py` & `figaro-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     include_dirs = ['figaro', numpy.get_include()],
     setup_requires=['numpy', 'cython'],
     package_data={"": ['*.c', '*.pyx', '*.pxd']},
     ext_modules=ext_modules,
     entry_points = {
         'console_scripts': scripts,
         },
-    version='1.0.6',
+    version='1.1.0',
     long_description=long_description,
     long_description_content_type='text/markdown',
     cmdclass = {
             "build_ext": build_ext
             }
     )
```

