# Comparing `tmp/figaro-1.1.0.tar.gz` & `tmp/figaro-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "figaro-1.1.0.tar", last modified: Fri Jul 14 18:00:13 2023, max compression
+gzip compressed data, was "figaro-1.1.1.tar", last modified: Fri Jul 14 18:59:55 2023, max compression
```

## Comparing `figaro-1.1.0.tar` & `figaro-1.1.1.tar`

### file list

```diff
@@ -1,49 +1,47 @@
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-14 18:00:13.871003 figaro-1.1.0/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1072 2022-02-08 13:50:37.000000 figaro-1.1.0/LICENSE
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      143 2023-07-14 17:53:26.000000 figaro-1.1.0/MANIFEST.in
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-07-14 18:00:13.870517 figaro-1.1.0/PKG-INFO
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4255 2023-02-20 15:52:20.000000 figaro-1.1.0/README.md
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-14 18:00:13.854375 figaro-1.1.0/figaro/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)        0 2022-05-05 11:31:57.000000 figaro-1.1.0/figaro/__init__.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2475 2022-05-01 13:54:12.000000 figaro-1.1.0/figaro/coordinates.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)  1002062 2023-07-14 17:57:15.000000 figaro-1.1.0/figaro/cosmology.c
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     3649 2022-11-17 15:54:02.000000 figaro-1.1.0/figaro/cosmology.pxd
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5144 2023-07-14 17:50:31.000000 figaro-1.1.0/figaro/cosmology.pyx
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     7637 2022-05-15 14:27:47.000000 figaro-1.1.0/figaro/credible_regions.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)   297682 2023-03-13 16:06:47.000000 figaro-1.1.0/figaro/cumulative.c
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1911 2022-05-18 11:00:07.000000 figaro-1.1.0/figaro/cumulative.pyx
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1996 2023-03-08 12:59:32.000000 figaro-1.1.0/figaro/decorators.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     8535 2023-07-07 12:21:05.000000 figaro-1.1.0/figaro/diagnostic.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1249 2023-07-07 12:34:31.000000 figaro-1.1.0/figaro/exceptions.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5301 2023-07-07 12:27:53.000000 figaro-1.1.0/figaro/likelihood.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    26863 2023-07-13 15:53:30.000000 figaro-1.1.0/figaro/load.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5981 2023-07-12 07:21:45.000000 figaro-1.1.0/figaro/marginal.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    41110 2023-07-14 08:28:34.000000 figaro-1.1.0/figaro/mixture.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2610 2023-01-31 15:40:41.000000 figaro-1.1.0/figaro/montecarlo.py
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-14 18:00:13.869010 figaro-1.1.0/figaro/pipelines/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     6409 2022-05-15 14:27:47.000000 figaro-1.1.0/figaro/pipelines/create_glade.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    16259 2023-06-25 09:51:30.000000 figaro-1.1.0/figaro/pipelines/entropy.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4583 2022-11-17 16:07:28.000000 figaro-1.1.0/figaro/pipelines/gen_mock_data.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    12961 2023-06-30 08:48:22.000000 figaro-1.1.0/figaro/pipelines/hierarchical_inference.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    17678 2023-06-30 08:48:22.000000 figaro-1.1.0/figaro/pipelines/par_hierarchical_inference.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    10389 2023-06-25 09:51:30.000000 figaro-1.1.0/figaro/pipelines/par_probability_density.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    11156 2023-03-29 08:52:28.000000 figaro-1.1.0/figaro/pipelines/ppplot.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     9184 2023-07-13 15:25:45.000000 figaro-1.1.0/figaro/pipelines/probability_density.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    31946 2023-07-07 12:44:53.000000 figaro-1.1.0/figaro/plot.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      933 2023-06-27 13:05:57.000000 figaro-1.1.0/figaro/plot_settings.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    39776 2023-07-07 12:44:53.000000 figaro-1.1.0/figaro/threeDvolume.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2236 2023-06-25 09:51:30.000000 figaro-1.1.0/figaro/transform.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    15184 2023-07-14 08:00:31.000000 figaro-1.1.0/figaro/utils.py
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-14 18:00:13.858686 figaro-1.1.0/figaro.egg-info/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-07-14 18:00:13.000000 figaro-1.1.0/figaro.egg-info/PKG-INFO
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1000 2023-07-14 18:00:13.000000 figaro-1.1.0/figaro.egg-info/SOURCES.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)        1 2023-07-14 18:00:13.000000 figaro-1.1.0/figaro.egg-info/dependency_links.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      483 2023-07-14 18:00:13.000000 figaro-1.1.0/figaro.egg-info/entry_points.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)       94 2023-07-14 18:00:13.000000 figaro-1.1.0/figaro.egg-info/requires.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      279 2023-07-14 18:00:13.000000 figaro-1.1.0/figaro.egg-info/top_level.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      477 2023-02-20 15:52:20.000000 figaro-1.1.0/figaro_env.yml
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      565 2023-02-20 15:52:20.000000 figaro-1.1.0/install.sh
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)       85 2023-07-14 17:39:59.000000 figaro-1.1.0/pyproject.toml
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)       93 2023-03-13 15:25:38.000000 figaro-1.1.0/requirements.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)       38 2023-07-14 18:00:13.871195 figaro-1.1.0/setup.cfg
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4919 2023-07-14 17:56:03.000000 figaro-1.1.0/setup.py
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-14 18:59:55.692126 figaro-1.1.1/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1072 2022-02-08 13:50:37.000000 figaro-1.1.1/LICENSE
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      205 2023-07-14 18:25:52.000000 figaro-1.1.1/MANIFEST.in
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-07-14 18:59:55.691622 figaro-1.1.1/PKG-INFO
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4255 2023-02-20 15:52:20.000000 figaro-1.1.1/README.md
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-14 18:59:55.682100 figaro-1.1.1/figaro/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)        0 2022-05-05 11:31:57.000000 figaro-1.1.1/figaro/__init__.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2475 2022-05-01 13:54:12.000000 figaro-1.1.1/figaro/coordinates.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)  1000222 2023-07-14 18:59:55.000000 figaro-1.1.1/figaro/cosmology.c
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     3649 2023-07-14 18:58:34.000000 figaro-1.1.1/figaro/cosmology.pxd
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5030 2023-07-14 18:58:50.000000 figaro-1.1.1/figaro/cosmology.pyx
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     7637 2022-05-15 14:27:47.000000 figaro-1.1.1/figaro/credible_regions.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)   297682 2023-03-13 16:06:47.000000 figaro-1.1.1/figaro/cumulative.c
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1911 2022-05-18 11:00:07.000000 figaro-1.1.1/figaro/cumulative.pyx
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1996 2023-03-08 12:59:32.000000 figaro-1.1.1/figaro/decorators.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     8535 2023-07-07 12:21:05.000000 figaro-1.1.1/figaro/diagnostic.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1249 2023-07-07 12:34:31.000000 figaro-1.1.1/figaro/exceptions.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5301 2023-07-07 12:27:53.000000 figaro-1.1.1/figaro/likelihood.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    26785 2023-07-14 18:57:48.000000 figaro-1.1.1/figaro/load.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5981 2023-07-12 07:21:45.000000 figaro-1.1.1/figaro/marginal.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    41110 2023-07-14 08:28:34.000000 figaro-1.1.1/figaro/mixture.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2610 2023-01-31 15:40:41.000000 figaro-1.1.1/figaro/montecarlo.py
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-14 18:59:55.690972 figaro-1.1.1/figaro/pipelines/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     6409 2022-05-15 14:27:47.000000 figaro-1.1.1/figaro/pipelines/create_glade.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    16259 2023-06-25 09:51:30.000000 figaro-1.1.1/figaro/pipelines/entropy.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4583 2022-11-17 16:07:28.000000 figaro-1.1.1/figaro/pipelines/gen_mock_data.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    12961 2023-06-30 08:48:22.000000 figaro-1.1.1/figaro/pipelines/hierarchical_inference.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    17678 2023-06-30 08:48:22.000000 figaro-1.1.1/figaro/pipelines/par_hierarchical_inference.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    10389 2023-06-25 09:51:30.000000 figaro-1.1.1/figaro/pipelines/par_probability_density.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    11156 2023-03-29 08:52:28.000000 figaro-1.1.1/figaro/pipelines/ppplot.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     9184 2023-07-13 15:25:45.000000 figaro-1.1.1/figaro/pipelines/probability_density.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    31946 2023-07-07 12:44:53.000000 figaro-1.1.1/figaro/plot.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      933 2023-06-27 13:05:57.000000 figaro-1.1.1/figaro/plot_settings.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    39776 2023-07-07 12:44:53.000000 figaro-1.1.1/figaro/threeDvolume.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2236 2023-06-25 09:51:30.000000 figaro-1.1.1/figaro/transform.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    15184 2023-07-14 08:00:31.000000 figaro-1.1.1/figaro/utils.py
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-14 18:59:55.685924 figaro-1.1.1/figaro.egg-info/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-07-14 18:59:55.000000 figaro-1.1.1/figaro.egg-info/PKG-INFO
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      974 2023-07-14 18:59:55.000000 figaro-1.1.1/figaro.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)        1 2023-07-14 18:59:55.000000 figaro-1.1.1/figaro.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      483 2023-07-14 18:59:55.000000 figaro-1.1.1/figaro.egg-info/entry_points.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)       94 2023-07-14 18:59:55.000000 figaro-1.1.1/figaro.egg-info/requires.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      279 2023-07-14 18:59:55.000000 figaro-1.1.1/figaro.egg-info/top_level.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      110 2023-07-14 18:33:57.000000 figaro-1.1.1/pyproject.toml
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)       93 2023-03-13 15:25:38.000000 figaro-1.1.1/requirements.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)       38 2023-07-14 18:59:55.692290 figaro-1.1.1/setup.cfg
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4460 2023-07-14 18:56:51.000000 figaro-1.1.1/setup.py
```

### Comparing `figaro-1.1.0/LICENSE` & `figaro-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/PKG-INFO` & `figaro-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.1.0
+Version: 1.1.1
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Home-page: https://github.com/sterinaldi/figaro
 Author: Stefano Rinaldi, Walter Del Pozzo, Daniele Sanfratello
 Author-email: stefano.rinaldi@phd.unipi.it, walter.delpozzo@unipi.it, d.sanfratello@studenti.unipi.it
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `figaro-1.1.0/README.md` & `figaro-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/coordinates.py` & `figaro-1.1.1/figaro/coordinates.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/cosmology.c` & `figaro-1.1.1/figaro/cosmology.c`

 * *Files 1% similar despite different names*

```diff
@@ -2483,15 +2483,14 @@
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_struct[] = "struct";
 static const char __pyx_k_unpack[] = "unpack";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_fortran[] = "fortran";
 static const char __pyx_k_memview[] = "memview";
 static const char __pyx_k_Ellipsis[] = "Ellipsis";
-static const char __pyx_k_Planck18[] = "Planck18";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_itemsize[] = "itemsize";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
@@ -2558,15 +2557,14 @@
 static PyObject *__pyx_kp_s_Invalid_shape_in_axis_d_d;
 static PyObject *__pyx_n_s_MemoryError;
 static PyObject *__pyx_kp_s_MemoryView_of_r_at_0x_x;
 static PyObject *__pyx_kp_s_MemoryView_of_r_object;
 static PyObject *__pyx_n_b_O;
 static PyObject *__pyx_kp_s_Out_of_bounds_on_buffer_access_a;
 static PyObject *__pyx_n_s_PickleError;
-static PyObject *__pyx_n_s_Planck18;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
 static PyObject *__pyx_n_s_allocate_buffer;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_c;
@@ -2711,19 +2709,14 @@
 static PyObject *__pyx_pf___pyx_memoryviewslice_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_6figaro_9cosmology_CosmologicalParameters(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_float_0_;
-static PyObject *__pyx_float_0_315;
-static PyObject *__pyx_float_0_674;
-static PyObject *__pyx_float_0_685;
-static PyObject *__pyx_float_neg_1_;
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_112105877;
 static PyObject *__pyx_int_136983863;
 static PyObject *__pyx_int_184977713;
 static PyObject *__pyx_int_neg_1;
 static PyObject *__pyx_tuple_;
@@ -2749,16 +2742,15 @@
 static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__22;
 static PyObject *__pyx_tuple__23;
 static PyObject *__pyx_tuple__24;
 static PyObject *__pyx_tuple__25;
 static PyObject *__pyx_tuple__26;
 static PyObject *__pyx_tuple__27;
-static PyObject *__pyx_tuple__28;
-static PyObject *__pyx_codeobj__29;
+static PyObject *__pyx_codeobj__28;
 /* Late includes */
 
 /* "figaro/cosmology.pyx":7
  * cdef class CosmologicalParameters:
  * 
  *     def __cinit__(self, double h, double om, double ol, double w0, double w1):             # <<<<<<<<<<<<<<
  *         self.h = h
@@ -5279,24 +5271,21 @@
   __Pyx_RefNannySetupContext("DestroyCosmologicalParameters", 0);
 
   /* "figaro/cosmology.pyx":120
  * 
  *     def DestroyCosmologicalParameters(self):
  *         self._DestroyCosmologicalParameters()             # <<<<<<<<<<<<<<
  *         return
- * 
  */
   ((struct __pyx_vtabstruct_6figaro_9cosmology_CosmologicalParameters *)__pyx_v_self->__pyx_vtab)->_DestroyCosmologicalParameters(__pyx_v_self);
 
   /* "figaro/cosmology.pyx":121
  *     def DestroyCosmologicalParameters(self):
  *         self._DestroyCosmologicalParameters()
  *         return             # <<<<<<<<<<<<<<
- * 
- * # Planck 2018 [https://arxiv.org/abs/1807.06209]
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
 
   /* "figaro/cosmology.pyx":119
  *         return self._ComovingVolume(z)
@@ -20769,15 +20758,14 @@
   {&__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_k_Invalid_shape_in_axis_d_d, sizeof(__pyx_k_Invalid_shape_in_axis_d_d), 0, 0, 1, 0},
   {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
   {&__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_k_MemoryView_of_r_at_0x_x, sizeof(__pyx_k_MemoryView_of_r_at_0x_x), 0, 0, 1, 0},
   {&__pyx_kp_s_MemoryView_of_r_object, __pyx_k_MemoryView_of_r_object, sizeof(__pyx_k_MemoryView_of_r_object), 0, 0, 1, 0},
   {&__pyx_n_b_O, __pyx_k_O, sizeof(__pyx_k_O), 0, 0, 0, 1},
   {&__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_k_Out_of_bounds_on_buffer_access_a, sizeof(__pyx_k_Out_of_bounds_on_buffer_access_a), 0, 0, 1, 0},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
-  {&__pyx_n_s_Planck18, __pyx_k_Planck18, sizeof(__pyx_k_Planck18), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
@@ -21087,101 +21075,87 @@
   __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(3, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
   __pyx_tuple__21 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(3, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
 
-  /* "figaro/cosmology.pyx":124
- * 
- * # Planck 2018 [https://arxiv.org/abs/1807.06209]
- * Planck18 = CosmologicalParameters(0.674, 0.315, 0.685, -1., 0.)             # <<<<<<<<<<<<<<
- */
-  __pyx_tuple__22 = PyTuple_Pack(5, __pyx_float_0_674, __pyx_float_0_315, __pyx_float_0_685, __pyx_float_neg_1_, __pyx_float_0_); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 124, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(3, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(3, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(3, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(3, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(3, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(3, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(3, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(3, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(3, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(3, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__28 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(3, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(3, 1, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(3, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(3, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_float_0_ = PyFloat_FromDouble(0.); if (unlikely(!__pyx_float_0_)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_float_0_315 = PyFloat_FromDouble(0.315); if (unlikely(!__pyx_float_0_315)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_float_0_674 = PyFloat_FromDouble(0.674); if (unlikely(!__pyx_float_0_674)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_float_0_685 = PyFloat_FromDouble(0.685); if (unlikely(!__pyx_float_0_685)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_float_neg_1_ = PyFloat_FromDouble(-1.); if (unlikely(!__pyx_float_neg_1_)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
@@ -21599,28 +21573,20 @@
  * cimport cython
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "figaro/cosmology.pyx":124
- * 
- * # Planck 2018 [https://arxiv.org/abs/1807.06209]
- * Planck18 = CosmologicalParameters(0.674, 0.315, 0.685, -1., 0.)             # <<<<<<<<<<<<<<
- */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_6figaro_9cosmology_CosmologicalParameters), __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Planck18, __pyx_t_1) < 0) __PYX_ERR(0, 124, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "figaro/cosmology.pyx":1
- * import numpy as np             # <<<<<<<<<<<<<<
- * cimport numpy as np
- * cimport cython
+  /* "figaro/cosmology.pxd":76
+ *     cdef public double ol
+ *     cdef public double w0
+ *     cdef public double w1             # <<<<<<<<<<<<<<
+ *     cdef public double _HubbleParameter(self,double z) nogil
+ *     cdef public double _LuminosityDistance_double(self, double z) nogil
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "View.MemoryView":210
@@ -21639,71 +21605,71 @@
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 287, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 287, __pyx_L1_error)
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
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 288, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 288, __pyx_L1_error)
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
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 289, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 289, __pyx_L1_error)
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
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 292, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 292, __pyx_L1_error)
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
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 293, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":317
```

### Comparing `figaro-1.1.0/figaro/cosmology.pxd` & `figaro-1.1.1/figaro/cosmology.pxd`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/cosmology.pyx` & `figaro-1.1.1/figaro/cosmology.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -115,10 +115,7 @@
 
     def ComovingVolume(self, np.ndarray[double, ndim=1, mode="c"] z):
         return self._ComovingVolume(z)
 
     def DestroyCosmologicalParameters(self):
         self._DestroyCosmologicalParameters()
         return
-
-# Planck 2018 [https://arxiv.org/abs/1807.06209]
-Planck18 = CosmologicalParameters(0.674, 0.315, 0.685, -1., 0.)
```

### Comparing `figaro-1.1.0/figaro/credible_regions.py` & `figaro-1.1.1/figaro/credible_regions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/cumulative.c` & `figaro-1.1.1/figaro/cumulative.c`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/cumulative.pyx` & `figaro-1.1.1/figaro/cumulative.pyx`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/decorators.py` & `figaro-1.1.1/figaro/decorators.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/diagnostic.py` & `figaro-1.1.1/figaro/diagnostic.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/exceptions.py` & `figaro-1.1.1/figaro/exceptions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/likelihood.py` & `figaro-1.1.1/figaro/likelihood.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/load.py` & `figaro-1.1.1/figaro/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import numpy as np
 import h5py
 import warnings
 import json
 import dill
 from figaro.exceptions import FIGAROException
 from figaro.mixture import mixture
-try:
-    from figaro.cosmology import CosmologicalParameters
-    lal_flag = True
-except ModuleNotFoundError:
-    lal_flag = False
+from figaro.cosmology import CosmologicalParameters
 from pathlib import Path
 from scipy.optimize import newton
 from tqdm import tqdm
 
 supported_extensions = ['h5', 'hdf5', 'txt', 'dat', 'csv']
 supported_waveforms  = ['combined', 'imr', 'seob']
```

### Comparing `figaro-1.1.0/figaro/marginal.py` & `figaro-1.1.1/figaro/marginal.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/mixture.py` & `figaro-1.1.1/figaro/mixture.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/montecarlo.py` & `figaro-1.1.1/figaro/montecarlo.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/pipelines/create_glade.py` & `figaro-1.1.1/figaro/pipelines/create_glade.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/pipelines/entropy.py` & `figaro-1.1.1/figaro/pipelines/entropy.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/pipelines/gen_mock_data.py` & `figaro-1.1.1/figaro/pipelines/gen_mock_data.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/pipelines/hierarchical_inference.py` & `figaro-1.1.1/figaro/pipelines/hierarchical_inference.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/pipelines/par_hierarchical_inference.py` & `figaro-1.1.1/figaro/pipelines/par_hierarchical_inference.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/pipelines/par_probability_density.py` & `figaro-1.1.1/figaro/pipelines/par_probability_density.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/pipelines/ppplot.py` & `figaro-1.1.1/figaro/pipelines/ppplot.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/pipelines/probability_density.py` & `figaro-1.1.1/figaro/pipelines/probability_density.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/plot.py` & `figaro-1.1.1/figaro/plot.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/plot_settings.py` & `figaro-1.1.1/figaro/plot_settings.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/threeDvolume.py` & `figaro-1.1.1/figaro/threeDvolume.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/transform.py` & `figaro-1.1.1/figaro/transform.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro/utils.py` & `figaro-1.1.1/figaro/utils.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.0/figaro.egg-info/PKG-INFO` & `figaro-1.1.1/figaro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.1.0
+Version: 1.1.1
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Home-page: https://github.com/sterinaldi/figaro
 Author: Stefano Rinaldi, Walter Del Pozzo, Daniele Sanfratello
 Author-email: stefano.rinaldi@phd.unipi.it, walter.delpozzo@unipi.it, d.sanfratello@studenti.unipi.it
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `figaro-1.1.0/figaro.egg-info/SOURCES.txt` & `figaro-1.1.1/figaro.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 LICENSE
 MANIFEST.in
 README.md
-figaro_env.yml
-install.sh
 pyproject.toml
 requirements.txt
 setup.py
 figaro/__init__.py
 figaro/coordinates.py
 figaro/cosmology.c
 figaro/cosmology.pxd
```

### Comparing `figaro-1.1.0/setup.py` & `figaro-1.1.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,20 +4,14 @@
 from setuptools.command.build_ext import build_ext as _build_ext
 from codecs import open
 from os import path
 from distutils.extension import Extension
 import os
 import warnings
 
-lal_flag = True
-try:
-    import lal
-except ModuleNotFoundError:
-    lal_flag = False
-
 ray_flag = True
 try:
     import ray
 except ModuleNotFoundError:
     ray_flag = False
 
 try:
@@ -38,34 +32,34 @@
              Extension("figaro.cumulative",
                        sources=[os.path.join("figaro","cumulative.pyx")],
                        libraries=["m"], # Unix-like specific
                        extra_compile_args=["-O3","-ffast-math"],
                        include_dirs=['figaro', numpy.get_include()]
                        ),
             ]
-if lal_flag:
-    if "LAL_PREFIX" in os.environ:
-        # Older LAL installations requires this
-        lal_prefix     = os.environ.get("LAL_PREFIX")
-        lal_includes   = lal_prefix+"/include"
-        lal_libs       = lal_prefix+"/lib"
-        ext_modules.append(Extension("figaro.cosmology",
-                          sources=[os.path.join("figaro","cosmology.pyx")],
-                          libraries=["m", "lal"], # Unix-like specific
-                          library_dirs = [lal_libs],
-                          extra_compile_args=["-O3","-ffast-math"],
-                          include_dirs=['figaro', lal_includes, numpy.get_include()]
-                          ))
-    else:
-        ext_modules.append(Extension("figaro.cosmology",
-                           sources=[os.path.join("figaro","cosmology.pyx")],
-                           libraries=["m", "lal"], # Unix-like specific
-                           extra_compile_args=["-O3","-ffast-math"],
-                           include_dirs=['figaro', numpy.get_include()]
-                           ))
+
+if "LAL_PREFIX" in os.environ:
+    # Older LAL installations requires this
+    lal_prefix     = os.environ.get("LAL_PREFIX")
+    lal_includes   = lal_prefix+"/include"
+    lal_libs       = lal_prefix+"/lib"
+    ext_modules.append(Extension("figaro.cosmology",
+                      sources=[os.path.join("figaro","cosmology.pyx")],
+                      libraries=["m", "lal"], # Unix-like specific
+                      library_dirs = [lal_libs],
+                      extra_compile_args=["-O3","-ffast-math"],
+                      include_dirs=['figaro', lal_includes, numpy.get_include()]
+                      ))
+else:
+    ext_modules.append(Extension("figaro.cosmology",
+                       sources=[os.path.join("figaro","cosmology.pyx")],
+                       libraries=["m", "lal"], # Unix-like specific
+                       extra_compile_args=["-O3","-ffast-math"],
+                       include_dirs=['figaro', numpy.get_include()]
+                       ))
 
 ext_modules = cythonize(ext_modules, compiler_directives={'language_level' : "3"})
 
 scripts = ['figaro-density=figaro.pipelines.probability_density:main',
            'figaro-hierarchical=figaro.pipelines.hierarchical_inference:main',
            'figaro-glade=figaro.pipelines.create_glade:main',
            'figaro-pp_plot=figaro.pipelines.ppplot:main',
@@ -104,19 +98,17 @@
     include_dirs = ['figaro', numpy.get_include()],
     setup_requires=['numpy', 'cython'],
     package_data={"": ['*.c', '*.pyx', '*.pxd']},
     ext_modules=ext_modules,
     entry_points = {
         'console_scripts': scripts,
         },
-    version='1.1.0',
+    version='1.1.1',
     long_description=long_description,
     long_description_content_type='text/markdown',
     cmdclass = {
             "build_ext": build_ext
             }
     )
 
-if not lal_flag:
-    warnings.warn("\n\nWARNING: No LAL installation found, please install LAL - see https://wiki.ligo.org/Computing/LALSuiteInstall. Some functions - GW posterior samples loading and catalog loading - won't be available and errors might be raised.\n", stacklevel = 2)
 if not ray_flag:
     warnings.warn("\n\nWARNING: Ray is not installed: parallelized pipelines won't be available. If you want to use them, please install Ray (pip install ray) and reinstall FIGARO.\n", stacklevel = 2)
```

