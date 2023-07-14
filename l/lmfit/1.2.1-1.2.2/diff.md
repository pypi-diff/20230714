# Comparing `tmp/lmfit-1.2.1.tar.gz` & `tmp/lmfit-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmfit-1.2.1.tar", last modified: Tue May  2 17:52:43 2023, max compression
+gzip compressed data, was "lmfit-1.2.2.tar", last modified: Fri Jul 14 02:56:03 2023, max compression
```

## Comparing `lmfit-1.2.1.tar` & `lmfit-1.2.2.tar`

### file list

```diff
@@ -1,203 +1,206 @@
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.183141 lmfit-1.2.1/
--rw-r--r--   0 Newville   (501) staff       (20)      308 2023-04-18 14:52:43.000000 lmfit-1.2.1/.codecov.yml
--rw-r--r--   0 Newville   (501) staff       (20)      393 2023-04-18 14:52:43.000000 lmfit-1.2.1/.gitattributes
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.150931 lmfit-1.2.1/.github/
--rw-r--r--   0 Newville   (501) staff       (20)     5158 2023-04-18 14:52:43.000000 lmfit-1.2.1/.github/CONTRIBUTING.md
--rw-r--r--   0 Newville   (501) staff       (20)     2465 2023-04-18 14:52:43.000000 lmfit-1.2.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 Newville   (501) staff       (20)     2211 2023-04-18 14:52:43.000000 lmfit-1.2.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 Newville   (501) staff       (20)      502 2023-04-18 14:52:43.000000 lmfit-1.2.1/.github/dependabot.yml
--rw-r--r--   0 Newville   (501) staff       (20)      323 2023-04-18 14:52:43.000000 lmfit-1.2.1/.gitignore
--rw-r--r--   0 Newville   (501) staff       (20)     1676 2023-05-02 16:08:38.000000 lmfit-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 Newville   (501) staff       (20)     3015 2023-04-18 14:52:43.000000 lmfit-1.2.1/AUTHORS.txt
--rw-r--r--   0 Newville   (501) staff       (20)     3670 2023-04-18 14:52:43.000000 lmfit-1.2.1/LICENSE
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.158832 lmfit-1.2.1/NIST_STRD/
--rw-r--r--   0 Newville   (501) staff       (20)     6869 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Bennett5.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1713 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/BoxBOD.dat
--rw-r--r--   0 Newville   (501) staff       (20)     7558 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Chwirut1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     3060 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Chwirut2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1990 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/DanWood.dat
--rw-r--r--   0 Newville   (501) staff       (20)     6761 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/ENSO.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2773 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Eckerle4.dat
--rw-r--r--   0 Newville   (501) staff       (20)     8098 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Gauss1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     8100 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Gauss2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     8102 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Gauss3.dat
--rw-r--r--   0 Newville   (501) staff       (20)     9276 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Hahn1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     5858 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Kirby2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2945 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Lanczos1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2601 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Lanczos2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2574 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Lanczos3.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2305 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/MGH09.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2335 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/MGH10.dat
--rw-r--r--   0 Newville   (501) staff       (20)     3078 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/MGH17.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1853 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Misra1a.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1845 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Misra1b.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1839 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Misra1c.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1843 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Misra1d.dat
--rw-r--r--   0 Newville   (501) staff       (20)     6401 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Models
--rw-r--r--   0 Newville   (501) staff       (20)     7001 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Nelson.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1873 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Rat42.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2072 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Rat43.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2486 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Roszman1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     3026 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Thurber.dat
--rw-r--r--   0 Newville   (501) staff       (20)     7730 2023-05-02 17:52:43.183287 lmfit-1.2.1/PKG-INFO
--rw-r--r--   0 Newville   (501) staff       (20)     6229 2023-04-22 17:52:19.000000 lmfit-1.2.1/README.rst
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.159329 lmfit-1.2.1/asv_benchmarking/
--rw-r--r--   0 Newville   (501) staff       (20)       43 2023-04-18 14:52:43.000000 lmfit-1.2.1/asv_benchmarking/README.md
--rw-r--r--   0 Newville   (501) staff       (20)     2793 2023-04-18 14:52:43.000000 lmfit-1.2.1/asv_benchmarking/asv.conf.json
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.159580 lmfit-1.2.1/asv_benchmarking/benchmarks/
--rw-r--r--   0 Newville   (501) staff       (20)        0 2023-04-18 14:52:43.000000 lmfit-1.2.1/asv_benchmarking/benchmarks/__init__.py
--rw-r--r--   0 Newville   (501) staff       (20)     4394 2023-04-18 14:52:43.000000 lmfit-1.2.1/asv_benchmarking/benchmarks/benchmarks.py
--rw-r--r--   0 Newville   (501) staff       (20)      350 2023-04-18 14:52:43.000000 lmfit-1.2.1/asv_benchmarking/run_benchmark_code.py
--rw-r--r--   0 Newville   (501) staff       (20)    12176 2023-05-02 16:08:38.000000 lmfit-1.2.1/azure-pipelines.yml
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.162399 lmfit-1.2.1/doc/
--rw-r--r--   0 Newville   (501) staff       (20)     4386 2023-05-02 17:31:02.000000 lmfit-1.2.1/doc/Makefile
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.162548 lmfit-1.2.1/doc/_static/
--rw-r--r--   0 Newville   (501) staff       (20)        0 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/_static/empty
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.162675 lmfit-1.2.1/doc/_templates/
--rw-r--r--   0 Newville   (501) staff       (20)      756 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/_templates/indexsidebar.html
--rw-r--r--   0 Newville   (501) staff       (20)     3499 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/bounds.rst
--rw-r--r--   0 Newville   (501) staff       (20)    30647 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/builtin_models.rst
--rw-r--r--   0 Newville   (501) staff       (20)     6527 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/conf.py
--rw-r--r--   0 Newville   (501) staff       (20)    15659 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/confidence.rst
--rw-r--r--   0 Newville   (501) staff       (20)     8110 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/constraints.rst
--rw-r--r--   0 Newville   (501) staff       (20)      223 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/contents.rst
--rwxr-xr-x   0 Newville   (501) staff       (20)     1943 2023-05-02 17:29:24.000000 lmfit-1.2.1/doc/doc_examples_to_gallery.py
--rw-r--r--   0 Newville   (501) staff       (20)    12177 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/faq.rst
--rw-r--r--   0 Newville   (501) staff       (20)    34852 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/fitting.rst
--rw-r--r--   0 Newville   (501) staff       (20)     2915 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/index.rst
--rw-r--r--   0 Newville   (501) staff       (20)     5102 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/installation.rst
--rw-r--r--   0 Newville   (501) staff       (20)     9268 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/intro.rst
--rw-r--r--   0 Newville   (501) staff       (20)      941 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/make.bat
--rw-r--r--   0 Newville   (501) staff       (20)    43609 2023-05-02 17:45:23.000000 lmfit-1.2.1/doc/model.rst
--rw-r--r--   0 Newville   (501) staff       (20)     4611 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/parameters.rst
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.162956 lmfit-1.2.1/doc/sphinx/
--rw-r--r--   0 Newville   (501) staff       (20)      460 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/ext_imgmath.py
--rw-r--r--   0 Newville   (501) staff       (20)      407 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/ext_mathjax.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.145809 lmfit-1.2.1/doc/sphinx/theme/
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.163376 lmfit-1.2.1/doc/sphinx/theme/sphinx13/
--rw-r--r--   0 Newville   (501) staff       (20)     7546 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/basic_layout.html
--rw-r--r--   0 Newville   (501) staff       (20)     3080 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/layout.html
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.164427 lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/
--rw-r--r--   0 Newville   (501) staff       (20)      429 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/bodybg.png
--rw-r--r--   0 Newville   (501) staff       (20)      180 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/footerbg.png
--rw-r--r--   0 Newville   (501) staff       (20)      189 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/headerbg.png
--rw-r--r--   0 Newville   (501) staff       (20)      149 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/listitem.png
--rw-r--r--   0 Newville   (501) staff       (20)     9907 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/lmfitheader.png
--rw-r--r--   0 Newville   (501) staff       (20)      183 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/relbg.png
--rw-r--r--   0 Newville   (501) staff       (20)     7978 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/sphinx13.css
--rw-r--r--   0 Newville   (501) staff       (20)       72 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/theme.conf
--rw-r--r--   0 Newville   (501) staff       (20)     1500 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/support.rst
--rw-r--r--   0 Newville   (501) staff       (20)    26325 2023-05-02 16:14:37.000000 lmfit-1.2.1/doc/whatsnew.rst
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.172295 lmfit-1.2.1/examples/
--rw-r--r--   0 Newville   (501) staff       (20)     8195 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/NIST_Gauss2.dat
--rw-r--r--   0 Newville   (501) staff       (20)      419 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/README.txt
--rw-r--r--   0 Newville   (501) staff       (20)     1419 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_builtinmodels_nistgauss.py
--rw-r--r--   0 Newville   (501) staff       (20)     1010 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_builtinmodels_nistgauss2.py
--rw-r--r--   0 Newville   (501) staff       (20)     1364 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_builtinmodels_peakmodels.py
--rw-r--r--   0 Newville   (501) staff       (20)     1961 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_builtinmodels_splinemodel.py
--rw-r--r--   0 Newville   (501) staff       (20)      784 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_builtinmodels_stepmodel.py
--rw-r--r--   0 Newville   (501) staff       (20)     1964 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_confidence_advanced.py
--rw-r--r--   0 Newville   (501) staff       (20)      481 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_confidence_basic.py
--rw-r--r--   0 Newville   (501) staff       (20)     3850 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_confidence_chi2_maps.py
--rw-r--r--   0 Newville   (501) staff       (20)     3359 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_fitting_emcee.py
--rw-r--r--   0 Newville   (501) staff       (20)      969 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_fitting_withreport.py
--rw-r--r--   0 Newville   (501) staff       (20)     1953 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_composite.py
--rw-r--r--   0 Newville   (501) staff       (20)      651 2023-04-30 01:28:00.000000 lmfit-1.2.1/examples/doc_model_gaussian.py
--rw-r--r--   0 Newville   (501) staff       (20)      774 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_loadmodel.py
--rw-r--r--   0 Newville   (501) staff       (20)      531 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_loadmodelresult.py
--rw-r--r--   0 Newville   (501) staff       (20)      537 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_loadmodelresult2.py
--rw-r--r--   0 Newville   (501) staff       (20)      337 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_savemodel.py
--rw-r--r--   0 Newville   (501) staff       (20)      423 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_savemodelresult.py
--rw-r--r--   0 Newville   (501) staff       (20)      996 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_savemodelresult2.py
--rw-r--r--   0 Newville   (501) staff       (20)      862 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_two_components.py
--rw-r--r--   0 Newville   (501) staff       (20)      834 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_uncertainty.py
--rw-r--r--   0 Newville   (501) staff       (20)     3148 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_uncertainty2.py
--rw-r--r--   0 Newville   (501) staff       (20)     1051 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_with_iter_callback.py
--rw-r--r--   0 Newville   (501) staff       (20)      775 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_with_nan_policy.py
--rw-r--r--   0 Newville   (501) staff       (20)     1499 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_parameters_basic.py
--rw-r--r--   0 Newville   (501) staff       (20)     1252 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_parameters_valuesdict.py
--rw-r--r--   0 Newville   (501) staff       (20)     7666 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_Model_interface.py
--rw-r--r--   0 Newville   (501) staff       (20)    17926 2023-05-02 16:08:13.000000 lmfit-1.2.1/examples/example_brute.py
--rw-r--r--   0 Newville   (501) staff       (20)     4731 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_complex_resonator_model.py
--rw-r--r--   0 Newville   (501) staff       (20)     4378 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_confidence_interval.py
--rw-r--r--   0 Newville   (501) staff       (20)     3331 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_detect_outliers.py
--rw-r--r--   0 Newville   (501) staff       (20)     1795 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_diffev.py
--rw-r--r--   0 Newville   (501) staff       (20)     4098 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_emcee_Model_interface.py
--rw-r--r--   0 Newville   (501) staff       (20)     1273 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_expression_model.py
--rw-r--r--   0 Newville   (501) staff       (20)     2716 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_fit_multi_datasets.py
--rw-r--r--   0 Newville   (501) staff       (20)     1417 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_fit_with_algebraic_constraint.py
--rw-r--r--   0 Newville   (501) staff       (20)     2161 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_fit_with_bounds.py
--rw-r--r--   0 Newville   (501) staff       (20)     2666 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_fit_with_derivfunc.py
--rw-r--r--   0 Newville   (501) staff       (20)     2190 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_fit_with_inequality.py
--rw-r--r--   0 Newville   (501) staff       (20)     2378 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_reduce_fcn.py
--rw-r--r--   0 Newville   (501) staff       (20)     2915 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_sympy.py
--rw-r--r--   0 Newville   (501) staff       (20)     6112 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_two_dimensional_peak.py
--rw-r--r--   0 Newville   (501) staff       (20)      851 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_use_pandas.py
--rw-r--r--   0 Newville   (501) staff       (20)     7776 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/lmfit_emcee_model_selection.py
--rw-r--r--   0 Newville   (501) staff       (20)     2373 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/model1d_gauss.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1987 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/peak.csv
--rw-r--r--   0 Newville   (501) staff       (20)     2464 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/sinedata.dat
--rw-r--r--   0 Newville   (501) staff       (20)     9496 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/test_peak.dat
--rw-r--r--   0 Newville   (501) staff       (20)    11611 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/test_splinepeak.dat
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.175604 lmfit-1.2.1/lmfit/
--rw-r--r--   0 Newville   (501) staff       (20)     1956 2023-04-18 14:52:43.000000 lmfit-1.2.1/lmfit/__init__.py
--rw-r--r--   0 Newville   (501) staff       (20)    10016 2023-04-18 14:52:43.000000 lmfit-1.2.1/lmfit/_ampgo.py
--rw-r--r--   0 Newville   (501) staff       (20)    21034 2023-04-26 01:48:37.000000 lmfit-1.2.1/lmfit/conf_emcee.py
--rw-r--r--   0 Newville   (501) staff       (20)    15312 2023-04-18 14:52:43.000000 lmfit-1.2.1/lmfit/confidence.py
--rw-r--r--   0 Newville   (501) staff       (20)     4808 2023-04-18 14:52:43.000000 lmfit-1.2.1/lmfit/jsonutils.py
--rw-r--r--   0 Newville   (501) staff       (20)    16911 2023-04-18 14:52:43.000000 lmfit-1.2.1/lmfit/lineshapes.py
--rw-r--r--   0 Newville   (501) staff       (20)   105487 2023-05-02 16:07:56.000000 lmfit-1.2.1/lmfit/minimizer.py
--rw-r--r--   0 Newville   (501) staff       (20)    84462 2023-05-02 16:08:38.000000 lmfit-1.2.1/lmfit/model.py
--rw-r--r--   0 Newville   (501) staff       (20)    65998 2023-04-18 14:52:43.000000 lmfit-1.2.1/lmfit/models.py
--rw-r--r--   0 Newville   (501) staff       (20)    36709 2023-04-18 14:52:43.000000 lmfit-1.2.1/lmfit/parameter.py
--rw-r--r--   0 Newville   (501) staff       (20)    15394 2023-04-18 14:52:43.000000 lmfit-1.2.1/lmfit/printfuncs.py
--rw-r--r--   0 Newville   (501) staff       (20)      160 2023-05-02 17:52:43.000000 lmfit-1.2.1/lmfit/version.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.176207 lmfit-1.2.1/lmfit.egg-info/
--rw-r--r--   0 Newville   (501) staff       (20)     7730 2023-05-02 17:52:43.000000 lmfit-1.2.1/lmfit.egg-info/PKG-INFO
--rw-r--r--   0 Newville   (501) staff       (20)     4953 2023-05-02 17:52:43.000000 lmfit-1.2.1/lmfit.egg-info/SOURCES.txt
--rw-r--r--   0 Newville   (501) staff       (20)        1 2023-05-02 17:52:43.000000 lmfit-1.2.1/lmfit.egg-info/dependency_links.txt
--rw-r--r--   0 Newville   (501) staff       (20)      669 2023-05-02 17:52:43.000000 lmfit-1.2.1/lmfit.egg-info/requires.txt
--rw-r--r--   0 Newville   (501) staff       (20)        6 2023-05-02 17:52:43.000000 lmfit-1.2.1/lmfit.egg-info/top_level.txt
--rwxr-xr-x   0 Newville   (501) staff       (20)     1010 2023-04-18 14:52:43.000000 lmfit-1.2.1/publish_docs.sh
--rw-r--r--   0 Newville   (501) staff       (20)      202 2023-04-18 14:52:43.000000 lmfit-1.2.1/pyproject.toml
--rw-r--r--   0 Newville   (501) staff       (20)     2447 2023-05-02 17:52:43.183892 lmfit-1.2.1/setup.cfg
--rw-r--r--   0 Newville   (501) staff       (20)       92 2023-04-18 14:52:43.000000 lmfit-1.2.1/setup.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.183000 lmfit-1.2.1/tests/
--rw-r--r--   0 Newville   (501) staff       (20)     6109 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/NISTModels.py
--rw-r--r--   0 Newville   (501) staff       (20)        0 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/__init__.py
--rw-r--r--   0 Newville   (501) staff       (20)      893 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/conftest.py
--rw-r--r--   0 Newville   (501) staff       (20)     5656 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/gauss_modelresult_lmfit100.sav
--rw-r--r--   0 Newville   (501) staff       (20)     1374 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_1variable.py
--rw-r--r--   0 Newville   (501) staff       (20)     7097 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_NIST_Strd.py
--rw-r--r--   0 Newville   (501) staff       (20)     3951 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_algebraic_constraint.py
--rw-r--r--   0 Newville   (501) staff       (20)     5063 2023-05-02 16:08:38.000000 lmfit-1.2.1/tests/test_ampgo.py
--rw-r--r--   0 Newville   (501) staff       (20)     1238 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_basicfit.py
--rw-r--r--   0 Newville   (501) staff       (20)     3911 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_basinhopping.py
--rw-r--r--   0 Newville   (501) staff       (20)     1900 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_bounded_jacobian.py
--rw-r--r--   0 Newville   (501) staff       (20)     1413 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_bounds.py
--rw-r--r--   0 Newville   (501) staff       (20)    11428 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_brute.py
--rw-r--r--   0 Newville   (501) staff       (20)    11953 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_builtin_models.py
--rw-r--r--   0 Newville   (501) staff       (20)     9251 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_confidence.py
--rw-r--r--   0 Newville   (501) staff       (20)     9987 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_covariance_matrix.py
--rw-r--r--   0 Newville   (501) staff       (20)     1235 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_custom_independentvar.py
--rw-r--r--   0 Newville   (501) staff       (20)      612 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_default_kws.py
--rw-r--r--   0 Newville   (501) staff       (20)     2595 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_dual_annealing.py
--rw-r--r--   0 Newville   (501) staff       (20)     4364 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_itercb.py
--rw-r--r--   0 Newville   (501) staff       (20)     3066 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_jsonutils.py
--rw-r--r--   0 Newville   (501) staff       (20)     6266 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_least_squares.py
--rw-r--r--   0 Newville   (501) staff       (20)     4804 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_lineshapes.py
--rw-r--r--   0 Newville   (501) staff       (20)      781 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_manypeaks_speed.py
--rw-r--r--   0 Newville   (501) staff       (20)     3689 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_max_nfev.py
--rw-r--r--   0 Newville   (501) staff       (20)      545 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_minimizer.py
--rw-r--r--   0 Newville   (501) staff       (20)    52838 2023-05-02 16:08:38.000000 lmfit-1.2.1/tests/test_model.py
--rw-r--r--   0 Newville   (501) staff       (20)    10484 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_model_saveload.py
--rw-r--r--   0 Newville   (501) staff       (20)     4354 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_model_uncertainties.py
--rw-r--r--   0 Newville   (501) staff       (20)     4965 2023-04-30 00:05:44.000000 lmfit-1.2.1/tests/test_models.py
--rw-r--r--   0 Newville   (501) staff       (20)     2181 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_multidatasets.py
--rw-r--r--   0 Newville   (501) staff       (20)    24031 2023-05-02 16:26:12.000000 lmfit-1.2.1/tests/test_nose.py
--rw-r--r--   0 Newville   (501) staff       (20)     1168 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_pandas.py
--rw-r--r--   0 Newville   (501) staff       (20)    19779 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_parameter.py
--rw-r--r--   0 Newville   (501) staff       (20)    21287 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_parameters.py
--rw-r--r--   0 Newville   (501) staff       (20)    14990 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_printfuncs.py
--rw-r--r--   0 Newville   (501) staff       (20)     4784 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_shgo.py
--rw-r--r--   0 Newville   (501) staff       (20)     1503 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_stepmodel.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.903850 lmfit-1.2.2/
+-rw-r--r--   0 Newville   (501) staff       (20)      308 2023-07-14 02:55:52.000000 lmfit-1.2.2/.codecov.yml
+-rw-r--r--   0 Newville   (501) staff       (20)      393 2023-07-14 02:55:52.000000 lmfit-1.2.2/.gitattributes
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.876691 lmfit-1.2.2/.github/
+-rw-r--r--   0 Newville   (501) staff       (20)     5158 2023-07-14 02:55:52.000000 lmfit-1.2.2/.github/CONTRIBUTING.md
+-rw-r--r--   0 Newville   (501) staff       (20)     2901 2023-07-14 02:55:52.000000 lmfit-1.2.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 Newville   (501) staff       (20)     2211 2023-07-14 02:55:52.000000 lmfit-1.2.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 Newville   (501) staff       (20)      502 2023-07-14 02:55:52.000000 lmfit-1.2.2/.github/dependabot.yml
+-rw-r--r--   0 Newville   (501) staff       (20)      323 2023-07-14 02:55:52.000000 lmfit-1.2.2/.gitignore
+-rw-r--r--   0 Newville   (501) staff       (20)     1676 2023-07-14 02:55:52.000000 lmfit-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 Newville   (501) staff       (20)     3015 2023-07-14 02:55:52.000000 lmfit-1.2.2/AUTHORS.txt
+-rw-r--r--   0 Newville   (501) staff       (20)     3670 2023-07-14 02:55:52.000000 lmfit-1.2.2/LICENSE
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.880166 lmfit-1.2.2/NIST_STRD/
+-rw-r--r--   0 Newville   (501) staff       (20)     6869 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Bennett5.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1713 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/BoxBOD.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     7558 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Chwirut1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     3060 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Chwirut2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1990 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/DanWood.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     6761 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/ENSO.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2773 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Eckerle4.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     8098 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Gauss1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     8100 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Gauss2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     8102 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Gauss3.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     9276 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Hahn1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     5858 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Kirby2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2945 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Lanczos1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2601 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Lanczos2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2574 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Lanczos3.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2305 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/MGH09.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2335 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/MGH10.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     3078 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/MGH17.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1853 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Misra1a.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1845 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Misra1b.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1839 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Misra1c.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1843 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Misra1d.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     6401 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Models
+-rw-r--r--   0 Newville   (501) staff       (20)     7001 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Nelson.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1873 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Rat42.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2072 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Rat43.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2486 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Roszman1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     3026 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Thurber.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     7730 2023-07-14 02:56:03.904109 lmfit-1.2.2/PKG-INFO
+-rw-r--r--   0 Newville   (501) staff       (20)     6229 2023-07-14 02:55:52.000000 lmfit-1.2.2/README.rst
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.880533 lmfit-1.2.2/asv_benchmarking/
+-rw-r--r--   0 Newville   (501) staff       (20)       43 2023-07-14 02:55:52.000000 lmfit-1.2.2/asv_benchmarking/README.md
+-rw-r--r--   0 Newville   (501) staff       (20)     2793 2023-07-14 02:55:52.000000 lmfit-1.2.2/asv_benchmarking/asv.conf.json
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.880759 lmfit-1.2.2/asv_benchmarking/benchmarks/
+-rw-r--r--   0 Newville   (501) staff       (20)        0 2023-07-14 02:55:52.000000 lmfit-1.2.2/asv_benchmarking/benchmarks/__init__.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4394 2023-07-14 02:55:52.000000 lmfit-1.2.2/asv_benchmarking/benchmarks/benchmarks.py
+-rw-r--r--   0 Newville   (501) staff       (20)      350 2023-07-14 02:55:52.000000 lmfit-1.2.2/asv_benchmarking/run_benchmark_code.py
+-rw-r--r--   0 Newville   (501) staff       (20)    12176 2023-07-14 02:55:52.000000 lmfit-1.2.2/azure-pipelines.yml
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.883343 lmfit-1.2.2/doc/
+-rw-r--r--   0 Newville   (501) staff       (20)     4460 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/Makefile
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.883479 lmfit-1.2.2/doc/_static/
+-rw-r--r--   0 Newville   (501) staff       (20)        0 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/_static/empty
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.883586 lmfit-1.2.2/doc/_templates/
+-rw-r--r--   0 Newville   (501) staff       (20)      756 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/_templates/indexsidebar.html
+-rw-r--r--   0 Newville   (501) staff       (20)     3499 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/bounds.rst
+-rw-r--r--   0 Newville   (501) staff       (20)    30647 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/builtin_models.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     6527 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/conf.py
+-rw-r--r--   0 Newville   (501) staff       (20)    15659 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/confidence.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     8110 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/constraints.rst
+-rw-r--r--   0 Newville   (501) staff       (20)      223 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/contents.rst
+-rwxr-xr-x   0 Newville   (501) staff       (20)     1943 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/doc_examples_to_gallery.py
+-rw-r--r--   0 Newville   (501) staff       (20)    12177 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/faq.rst
+-rwxr-xr-x   0 Newville   (501) staff       (20)      657 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/filter_spurious_link_from_html.py
+-rw-r--r--   0 Newville   (501) staff       (20)    38148 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/fitting.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     2915 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/index.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     5102 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/installation.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     9268 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/intro.rst
+-rw-r--r--   0 Newville   (501) staff       (20)      941 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/make.bat
+-rw-r--r--   0 Newville   (501) staff       (20)    47467 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/model.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     4670 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/parameters.rst
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.883826 lmfit-1.2.2/doc/sphinx/
+-rw-r--r--   0 Newville   (501) staff       (20)      460 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/ext_imgmath.py
+-rw-r--r--   0 Newville   (501) staff       (20)      407 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/ext_mathjax.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.874288 lmfit-1.2.2/doc/sphinx/theme/
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.884194 lmfit-1.2.2/doc/sphinx/theme/sphinx13/
+-rw-r--r--   0 Newville   (501) staff       (20)     7546 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/basic_layout.html
+-rw-r--r--   0 Newville   (501) staff       (20)     3080 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/layout.html
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.889679 lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/
+-rw-r--r--   0 Newville   (501) staff       (20)      429 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/bodybg.png
+-rw-r--r--   0 Newville   (501) staff       (20)      180 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/footerbg.png
+-rw-r--r--   0 Newville   (501) staff       (20)      189 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/headerbg.png
+-rw-r--r--   0 Newville   (501) staff       (20)      149 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/listitem.png
+-rw-r--r--   0 Newville   (501) staff       (20)     9907 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/lmfitheader.png
+-rw-r--r--   0 Newville   (501) staff       (20)      183 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/relbg.png
+-rw-r--r--   0 Newville   (501) staff       (20)     7978 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/sphinx13.css
+-rw-r--r--   0 Newville   (501) staff       (20)       72 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/theme.conf
+-rw-r--r--   0 Newville   (501) staff       (20)     1500 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/support.rst
+-rw-r--r--   0 Newville   (501) staff       (20)    28488 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/whatsnew.rst
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.896318 lmfit-1.2.2/examples/
+-rw-r--r--   0 Newville   (501) staff       (20)     8195 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/NIST_Gauss2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)      419 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/README.txt
+-rw-r--r--   0 Newville   (501) staff       (20)     1419 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_builtinmodels_nistgauss.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1010 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_builtinmodels_nistgauss2.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1364 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_builtinmodels_peakmodels.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1961 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_builtinmodels_splinemodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)      784 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_builtinmodels_stepmodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1964 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_confidence_advanced.py
+-rw-r--r--   0 Newville   (501) staff       (20)      481 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_confidence_basic.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3850 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_confidence_chi2_maps.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3359 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_fitting_emcee.py
+-rw-r--r--   0 Newville   (501) staff       (20)      969 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_fitting_withreport.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1953 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_composite.py
+-rw-r--r--   0 Newville   (501) staff       (20)      651 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_gaussian.py
+-rw-r--r--   0 Newville   (501) staff       (20)      774 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_loadmodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)      531 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_loadmodelresult.py
+-rw-r--r--   0 Newville   (501) staff       (20)      537 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_loadmodelresult2.py
+-rw-r--r--   0 Newville   (501) staff       (20)      337 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_savemodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)      423 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_savemodelresult.py
+-rw-r--r--   0 Newville   (501) staff       (20)      996 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_savemodelresult2.py
+-rw-r--r--   0 Newville   (501) staff       (20)      862 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_two_components.py
+-rw-r--r--   0 Newville   (501) staff       (20)      834 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_uncertainty.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3148 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_uncertainty2.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1051 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_with_iter_callback.py
+-rw-r--r--   0 Newville   (501) staff       (20)      775 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_with_nan_policy.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1499 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_parameters_basic.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1252 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_parameters_valuesdict.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2417 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_uvars_params.py
+-rw-r--r--   0 Newville   (501) staff       (20)     7666 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_Model_interface.py
+-rw-r--r--   0 Newville   (501) staff       (20)    17926 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_brute.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4731 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_complex_resonator_model.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4378 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_confidence_interval.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3331 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_detect_outliers.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1795 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_diffev.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4098 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_emcee_Model_interface.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1273 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_expression_model.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2716 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_fit_multi_datasets.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1417 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_fit_with_algebraic_constraint.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2161 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_fit_with_bounds.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2666 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_fit_with_derivfunc.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2190 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_fit_with_inequality.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2378 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_reduce_fcn.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2915 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_sympy.py
+-rw-r--r--   0 Newville   (501) staff       (20)     6112 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_two_dimensional_peak.py
+-rw-r--r--   0 Newville   (501) staff       (20)      851 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_use_pandas.py
+-rw-r--r--   0 Newville   (501) staff       (20)     7776 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/lmfit_emcee_model_selection.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2373 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/model1d_gauss.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1987 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/peak.csv
+-rw-r--r--   0 Newville   (501) staff       (20)     2464 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/sinedata.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     9496 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/test_peak.dat
+-rw-r--r--   0 Newville   (501) staff       (20)    11611 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/test_splinepeak.dat
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.898138 lmfit-1.2.2/lmfit/
+-rw-r--r--   0 Newville   (501) staff       (20)     1956 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/__init__.py
+-rw-r--r--   0 Newville   (501) staff       (20)    10016 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/_ampgo.py
+-rw-r--r--   0 Newville   (501) staff       (20)    21034 2023-04-26 01:48:37.000000 lmfit-1.2.2/lmfit/conf_emcee.py
+-rw-r--r--   0 Newville   (501) staff       (20)    15312 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/confidence.py
+-rw-r--r--   0 Newville   (501) staff       (20)     5060 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/jsonutils.py
+-rw-r--r--   0 Newville   (501) staff       (20)    16913 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/lineshapes.py
+-rw-r--r--   0 Newville   (501) staff       (20)   106040 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/minimizer.py
+-rw-r--r--   0 Newville   (501) staff       (20)    85772 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/model.py
+-rw-r--r--   0 Newville   (501) staff       (20)    68610 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/models.py
+-rw-r--r--   0 Newville   (501) staff       (20)    40026 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/parameter.py
+-rw-r--r--   0 Newville   (501) staff       (20)    16055 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/printfuncs.py
+-rw-r--r--   0 Newville   (501) staff       (20)      160 2023-07-14 02:56:03.000000 lmfit-1.2.2/lmfit/version.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.898758 lmfit-1.2.2/lmfit.egg-info/
+-rw-r--r--   0 Newville   (501) staff       (20)     7730 2023-07-14 02:56:03.000000 lmfit-1.2.2/lmfit.egg-info/PKG-INFO
+-rw-r--r--   0 Newville   (501) staff       (20)     5047 2023-07-14 02:56:03.000000 lmfit-1.2.2/lmfit.egg-info/SOURCES.txt
+-rw-r--r--   0 Newville   (501) staff       (20)        1 2023-07-14 02:56:03.000000 lmfit-1.2.2/lmfit.egg-info/dependency_links.txt
+-rw-r--r--   0 Newville   (501) staff       (20)      669 2023-07-14 02:56:03.000000 lmfit-1.2.2/lmfit.egg-info/requires.txt
+-rw-r--r--   0 Newville   (501) staff       (20)        6 2023-07-14 02:56:03.000000 lmfit-1.2.2/lmfit.egg-info/top_level.txt
+-rwxr-xr-x   0 Newville   (501) staff       (20)     1010 2023-07-14 02:55:52.000000 lmfit-1.2.2/publish_docs.sh
+-rw-r--r--   0 Newville   (501) staff       (20)      202 2023-07-14 02:55:52.000000 lmfit-1.2.2/pyproject.toml
+-rw-r--r--   0 Newville   (501) staff       (20)     2447 2023-07-14 02:56:03.904931 lmfit-1.2.2/setup.cfg
+-rw-r--r--   0 Newville   (501) staff       (20)       92 2023-07-14 02:55:52.000000 lmfit-1.2.2/setup.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.903712 lmfit-1.2.2/tests/
+-rw-r--r--   0 Newville   (501) staff       (20)     6109 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/NISTModels.py
+-rw-r--r--   0 Newville   (501) staff       (20)        0 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/__init__.py
+-rw-r--r--   0 Newville   (501) staff       (20)      893 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/conftest.py
+-rw-r--r--   0 Newville   (501) staff       (20)     5656 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/gauss_modelresult_lmfit100.sav
+-rw-r--r--   0 Newville   (501) staff       (20)     1374 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_1variable.py
+-rw-r--r--   0 Newville   (501) staff       (20)     7097 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_NIST_Strd.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4008 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_algebraic_constraint.py
+-rw-r--r--   0 Newville   (501) staff       (20)     5063 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_ampgo.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1238 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_basicfit.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3911 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_basinhopping.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1900 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_bounded_jacobian.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1413 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_bounds.py
+-rw-r--r--   0 Newville   (501) staff       (20)    11428 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_brute.py
+-rw-r--r--   0 Newville   (501) staff       (20)    11953 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_builtin_models.py
+-rw-r--r--   0 Newville   (501) staff       (20)     9251 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_confidence.py
+-rw-r--r--   0 Newville   (501) staff       (20)     9987 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_covariance_matrix.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1235 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_custom_independentvar.py
+-rw-r--r--   0 Newville   (501) staff       (20)      612 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_default_kws.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2595 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_dual_annealing.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4292 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_itercb.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3066 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_jsonutils.py
+-rw-r--r--   0 Newville   (501) staff       (20)     6266 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_least_squares.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4780 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_lineshapes.py
+-rw-r--r--   0 Newville   (501) staff       (20)      781 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_manypeaks_speed.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3689 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_max_nfev.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2686 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_minimizer.py
+-rw-r--r--   0 Newville   (501) staff       (20)    56579 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_model.py
+-rw-r--r--   0 Newville   (501) staff       (20)    10484 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_model_saveload.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4354 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_model_uncertainties.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4965 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_models.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2181 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_multidatasets.py
+-rw-r--r--   0 Newville   (501) staff       (20)    24063 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_nose.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1168 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_pandas.py
+-rw-r--r--   0 Newville   (501) staff       (20)    19779 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_parameter.py
+-rw-r--r--   0 Newville   (501) staff       (20)    21303 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_parameters.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3169 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_params_uvars.py
+-rw-r--r--   0 Newville   (501) staff       (20)    14955 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_printfuncs.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4237 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_shgo.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1503 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_stepmodel.py
```

### Comparing `lmfit-1.2.1/.github/CONTRIBUTING.md` & `lmfit-1.2.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/.github/ISSUE_TEMPLATE.md` & `lmfit-1.2.2/.github/ISSUE_TEMPLATE.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,60 @@
 ### DO NOT IGNORE ###
 
 READ THESE INSTRUCTIONS FULLY. IF YOU DO NOT, YOUR ISSUE WILL BE CLOSED.
 
-If you have not submitted a GitHub Issue to lmfit before, read
-[this](https://github.com/lmfit/lmfit-py/blob/master/.github/CONTRIBUTING.md) first.
+If you have not submitted a GitHub Issue to lmfit before, read [this](https://github.com/lmfit/lmfit-py/blob/master/.github/CONTRIBUTING.md) first.
 
-***DO NOT USE GitHub Issues for questions, it is only for bugs!***
+***DO NOT USE GitHub Issues for questions, it is only for bugs in the lmfit code!***
 
-If you **think** something is an Issue, it probably is not an Issue.
-Getting a "bad fit" definitely does NOT qualify as an Issue! Issues here
-are concerned with errors or problems in the lmfit code.
-
-Use the [mailing list](https://groups.google.com/group/lmfit-py) or
-[GitHub discussions page](https://github.com/lmfit/lmfit-py/discussions) for
-questions about lmfit or things you think might be problems. We don't feel
-obligated to spend our free time helping people who do not respect our
-chosen work processes, so if you ignore this advice and post a question as
-a GitHub Issue anyway, it is quite likely that your Issue will be closed
-and not answered. If you have any doubt, start with a discussion either on
-the mailing list or discussions page.
-
-To submit an Issue, you MUST provide ALL of the following information. If
-you delete any of these sections, your Issue may be closed. If you think one
-of the sections does not apply to your Issue, state that explicitly.
+Issues here are concerned with errors or problems in the lmfit code.  We use it as our bug
+tracker.  There are other places to get support and help with using lmfit.
+
+If you **think** something is an Issue, it probably is not an Issue. If the behavior you
+want to report involves a fit that runs to completion without raising an exception but
+that gives a result that you think is incorrect, that is almost certainly not an Issue.
+
+Use the [mailing list](https://groups.google.com/group/lmfit-py) or [GitHub discussions
+page](https://github.com/lmfit/lmfit-py/discussions) for questions about lmfit or things
+you think might be problems.  We don't feel obligated to spend our free time helping
+people who do not respect our chosen work processes, so if you ignore this advice and post
+a question as a GitHub Issue anyway, it is quite likely that your Issue will be closed and
+not answered. If you have any doubt at all, do NOT submit an Issue.
+
+To submit an Issue, you MUST provide ALL of the following information.  If you delete any
+of these sections, your Issue may be closed. If you think one of the sections does not
+apply to your Issue, state that explicitly. We will probably disagree with you and insist
+that you provide that information. If we have to ask for it twice, we will expect it to be
+correct and prompt.
 
 #### First Time Issue Code
 <!-- If this is your first Issue, you will write down the Secret Code for First Time Issues from the CONTRIBUTING.md file linked to above -->
 
 #### Description
 <!-- Provide a short description of the issue, describe the expected outcome, and give the actual result -->
 
 ###### A Minimal, Complete, and Verifiable example
 <!-- see, for example, https://stackoverflow.com/help/mcve on how to do this -->
 
+
+###### Fit report:
+<!-- paste the *full* fit report here  -->
+
+
 ###### Error message:
 <!-- If any, paste the *full* error message inside a code block (starting from line Traceback) -->
 
 ```
 Traceback (most recent call last):
   File "<stdin>", line 1, in <module>
   ...
 ```
 
 ###### Version information
 <!-- Generate version information with this command in the Python shell and copy the output here:
 import sys, lmfit, numpy, scipy, asteval, uncertainties
 print(f"Python: {sys.version}\n\nlmfit: {lmfit.__version__}, scipy: {scipy.__version__}, numpy: {numpy.__version__},"
-	  f"asteval: {asteval.__version__}, uncertainties: {uncertainties.__version__}")
+      f"asteval: {asteval.__version__}, uncertainties: {uncertainties.__version__}")
 -->
 
 ###### Link(s)
 <!-- If you started a discussion on the lmfit mailing list, discussion page, or Stack Overflow, please provide the relevant link(s) -->
```

### Comparing `lmfit-1.2.1/.github/PULL_REQUEST_TEMPLATE.md` & `lmfit-1.2.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/.pre-commit-config.yaml` & `lmfit-1.2.2/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 exclude: 'doc/conf.py'
 
 repos:
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.2
+    rev: v3.7.0
     hooks:
     -   id: pyupgrade
         args: [--py37-plus]
 
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
@@ -47,20 +47,20 @@
     hooks:
     -   id: rst-backticks
     -   id: rst-directive-colons
     -   id: rst-inline-touching-normal
     -   id: python-check-blanket-noqa
 
 -   repo: https://github.com/codespell-project/codespell
-    rev: v2.2.4
+    rev: v2.2.5
     hooks:
     -   id: codespell
         files: '.py|.rst'
         exclude: 'doc/doc_examples_to_gallery.py'
         # escaped characters currently do not work correctly
         # so \nnumber is considered a spelling error....
         args: ["-L nnumber", "-L mone"]
 
 -   repo: https://github.com/asottile/yesqa
-    rev: v1.4.0
+    rev: v1.5.0
     hooks:
     -   id: yesqa
```

### Comparing `lmfit-1.2.1/AUTHORS.txt` & `lmfit-1.2.2/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/LICENSE` & `lmfit-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Bennett5.dat` & `lmfit-1.2.2/NIST_STRD/Bennett5.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/BoxBOD.dat` & `lmfit-1.2.2/NIST_STRD/BoxBOD.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Chwirut1.dat` & `lmfit-1.2.2/NIST_STRD/Chwirut1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Chwirut2.dat` & `lmfit-1.2.2/NIST_STRD/Chwirut2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/DanWood.dat` & `lmfit-1.2.2/NIST_STRD/DanWood.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/ENSO.dat` & `lmfit-1.2.2/NIST_STRD/ENSO.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Eckerle4.dat` & `lmfit-1.2.2/NIST_STRD/Eckerle4.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Gauss1.dat` & `lmfit-1.2.2/NIST_STRD/Gauss1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Gauss2.dat` & `lmfit-1.2.2/NIST_STRD/Gauss2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Gauss3.dat` & `lmfit-1.2.2/NIST_STRD/Gauss3.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Hahn1.dat` & `lmfit-1.2.2/NIST_STRD/Hahn1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Kirby2.dat` & `lmfit-1.2.2/NIST_STRD/Kirby2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Lanczos1.dat` & `lmfit-1.2.2/NIST_STRD/Lanczos1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Lanczos2.dat` & `lmfit-1.2.2/NIST_STRD/Lanczos2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Lanczos3.dat` & `lmfit-1.2.2/NIST_STRD/Lanczos3.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/MGH09.dat` & `lmfit-1.2.2/NIST_STRD/MGH09.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/MGH10.dat` & `lmfit-1.2.2/NIST_STRD/MGH10.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/MGH17.dat` & `lmfit-1.2.2/NIST_STRD/MGH17.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Misra1a.dat` & `lmfit-1.2.2/NIST_STRD/Misra1a.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Misra1b.dat` & `lmfit-1.2.2/NIST_STRD/Misra1b.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Misra1c.dat` & `lmfit-1.2.2/NIST_STRD/Misra1c.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Misra1d.dat` & `lmfit-1.2.2/NIST_STRD/Misra1d.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Models` & `lmfit-1.2.2/NIST_STRD/Models`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Nelson.dat` & `lmfit-1.2.2/NIST_STRD/Nelson.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Rat42.dat` & `lmfit-1.2.2/NIST_STRD/Rat42.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Rat43.dat` & `lmfit-1.2.2/NIST_STRD/Rat43.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Roszman1.dat` & `lmfit-1.2.2/NIST_STRD/Roszman1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/NIST_STRD/Thurber.dat` & `lmfit-1.2.2/NIST_STRD/Thurber.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/PKG-INFO` & `lmfit-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmfit
-Version: 1.2.1
+Version: 1.2.2
 Summary: Least-Squares Minimization with Bounds and Constraints
 Home-page: https://lmfit.github.io//lmfit-py/
 Author: LMFit Development Team
 Author-email: matt.newville@gmail.com
 License: BSD 3-Clause
 Project-URL: Source, https://github.com/lmfit/lmfit-py
 Project-URL: Changelog, https://lmfit.github.io/lmfit-py/whatsnew.html
```

### Comparing `lmfit-1.2.1/README.rst` & `lmfit-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/asv_benchmarking/asv.conf.json` & `lmfit-1.2.2/asv_benchmarking/asv.conf.json`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/asv_benchmarking/benchmarks/benchmarks.py` & `lmfit-1.2.2/asv_benchmarking/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/azure-pipelines.yml` & `lmfit-1.2.2/azure-pipelines.yml`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,15 @@
             ##curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
             ##python3.12 get-pip.py --user
             python3.12 -m ensurepip --upgrade
             pip3.12 install -U build pip setuptools wheel pybind11 cython || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
           displayName: 'Install build, pip, setuptools, wheel, pybind11, and cython'
         - script: |
             export PATH=/home/vsts/.local/bin:$PATH
-            export numpy_version=1.24.3
+            export numpy_version=1.25.0
             wget https://github.com/numpy/numpy/releases/download/v${numpy_version}/numpy-${numpy_version}.tar.gz
             tar xzvf numpy-${numpy_version}.tar.gz
             cd numpy-${numpy_version}
             python3.12 setup.py install --user || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
           displayName: 'Install latest available version of NumPy'
         - script: |
             export PATH=/home/vsts/.local/bin:$PATH
```

### Comparing `lmfit-1.2.1/doc/Makefile` & `lmfit-1.2.2/doc/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -22,25 +22,27 @@
 	$(SPHINXBUILD) -b html $(SPHINX_OUTPUT) $(SPHINX_OPTS) . $(BUILDDIR)/html
 	@echo
 	@echo "html build finished: $(BUILDDIR)/html."
 
 debug:  gallery
 	cp sphinx/ext_mathjax.py extensions.py
 	$(SPHINXBUILD) -b html $(SPHINX_OUTPUT) $(SPHINX_DEBUGOPTS) . $(BUILDDIR)/html
+	./filter_spurious_link_from_html.py
 	@echo
 	@echo "html build finished: $(BUILDDIR)/html."
 
 gallery: examples/index.rst
 
 examples/index.rst:
 	./doc_examples_to_gallery.py
 
 htmlzip: html
 	cp sphinx/ext_mathjax.py extensions.py
 	$(SPHINXBUILD) -b html $(SPHINX_OUTPUT) $(SPHINX_OPTS) . $(BUILDDIR)/lmfit_doc
+	./filter_spurious_link_from_html.py
 	cd $(BUILDDIR) && zip -pur html/lmfit_doc.zip lmfit_doc
 
 epub: gallery
 	cp sphinx/ext_imgmath.py extensions.py
 	$(SPHINXBUILD) -b epub  $(SPHINX_OUTPUT) $(SPHINX_OPTS) . $(BUILDDIR)/epub
 	mkdir -p $(BUILDDIR)/html
 	cp -pr $(BUILDDIR)/epub/*.epub $(BUILDDIR)/html/.
```

### Comparing `lmfit-1.2.1/doc/_templates/indexsidebar.html` & `lmfit-1.2.2/doc/_templates/indexsidebar.html`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/doc/bounds.rst` & `lmfit-1.2.2/doc/bounds.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/doc/builtin_models.rst` & `lmfit-1.2.2/doc/builtin_models.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/doc/conf.py` & `lmfit-1.2.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/doc/confidence.rst` & `lmfit-1.2.2/doc/confidence.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/doc/constraints.rst` & `lmfit-1.2.2/doc/constraints.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/doc/doc_examples_to_gallery.py` & `lmfit-1.2.2/doc/doc_examples_to_gallery.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/doc/faq.rst` & `lmfit-1.2.2/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/doc/fitting.rst` & `lmfit-1.2.2/doc/fitting.rst`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 =====================================
 
 As shown in the previous chapter, a simple fit can be performed with the
 :func:`minimize` function. For more sophisticated modeling, the
 :class:`Minimizer` class can be used to gain a bit more control, especially
 when using complicated constraints or comparing results from related fits.
 
-
 The :func:`minimize` function
 =============================
 
 The :func:`minimize` function is a wrapper around :class:`Minimizer` for
 running an optimization problem. It takes an objective function (the
 function that calculates the array to be minimized), a :class:`Parameters`
 object, and several optional arguments. See :ref:`fit-func-label` for
@@ -117,14 +116,78 @@
 
     if abs(period) < 1.e-10:
         period = sign(period)*1.e-10
 
 is also a reasonable approach. Similarly, one could place bounds on the
 ``decay`` parameter to take values only between ``-pi/2`` and ``pi/2``.
 
+..  _fit-data-label:
+
+Types of Data to Use for Fitting
+===================================
+
+Minimization methods assume that data is numerical.  For all the fitting
+methods supported by lmfit, data and fitting parameters are also assumed to
+be continuous variables.  As the routines make heavy use of numpy and scipy,
+the most natural data to use in fitting is then numpy nd-arrays.  In fact, many
+of the underlying fitting algorithms - including the default :meth:`leastsq`
+method - **require** the values in the residual array used for the
+minimization to be a 1-dimensional numpy array with data type (`dtype`) of
+"float64": a 64-bit representation of a floating point number (sometimes called
+a "double precision float").
+
+Python is generally forgiving about data types, and in the scientific Python
+community there is a concept of an object being "array like" which essentially
+means that the can usually be coerced or interpreted as a numpy array, often
+with that object having an ``__array__()`` method specially designed for that
+conversion.  Important examples of objects that can be considered "array like"
+include Lists and Tuples that contain only numbers, pandas Series, and HDF5
+Datasets. Many objects from data-processing libraries like dask, xarray, zarr,
+and more are also "array like".
+
+Lmfit tries to be accommodating in the data that can be used in the fitting
+process. When using :class:`Minimizer`, the data you pass in as extra arrays for the
+calculation of the residual array will not be altered, and can be used in your
+objective function in whatever form you send.  Usually, "array like" data will
+work, but some care may be needed.  In the example above, if ``x`` was not a
+numpy array but a list of numbers, this would give an error message like::
+
+   TypeError: unsupported operand type(s) for /: 'list' and 'float'
+
+or::
+
+  TypeError: can't multiply sequence by non-int of type 'float'
+
+because a list of numbers is only sometimes "array like".
+
+Sending in a "more array-like" object like a pandas Series will avoid many
+(though maybe not all!) such exceptions, but the resulting calculation returned
+from the function would then also be a pandas Series.  Lmfit :meth:`minimize` will
+always coerce the return value from the objective function into a 1-D numpy
+array with ``dtype`` of "float64".  This will usually "just work", but there
+may be exceptions.
+
+When in doubt, or if running it trouble, converting data to float64 numpy
+arrays before being used in a fit is recommended.  If using complex data or
+functions, a ``dtype`` of "complex128" will also always work, and will be
+converted to "float64" with ``ndaarray.view("float64")``.  Numpy arrays of other
+``dtype`` (say, "int16" or "float32") should be used with caution.  In
+particular, "float32" data should be avoided: Multiplying a "float32" array and
+a Python float will result in a "float32" array for example.  As fitting
+variables may have small changes made to them, the results may be at or below
+"float32" precision, which will cause the fit to give up.  For integer data,
+results are more sometimes promoted to "float64", but many numpy ufuncs (say,
+``numpy.exp()``) will promote only to "float32", so care is still needed.
+
+
+See also :ref:`model_data_coercion_section` for discussion of data passed in for
+curve-fitting.
+
+
+
 ..  _fit-methods-label:
 
 Choosing Different Fitting Methods
 ==================================
 
 By default, the `Levenberg-Marquardt
 <https://en.wikipedia.org/wiki/Levenberg-Marquardt_algorithm>`_ algorithm is
@@ -187,15 +250,15 @@
  | Basinhopping             |  ``basinhopping``                                                |
  +--------------------------+------------------------------------------------------------------+
  | Adaptive Memory          |  ``ampgo``                                                       |
  | Programming for Global   |                                                                  |
  | Optimization             |                                                                  |
  +--------------------------+------------------------------------------------------------------+
  | Simplicial Homology      |  ``shgo``                                                        |
- | Global Ooptimization     |                                                                  |
+ | Global Optimization      |                                                                  |
  +--------------------------+------------------------------------------------------------------+
  | Dual Annealing           |  ``dual_annealing``                                              |
  +--------------------------+------------------------------------------------------------------+
  | Maximum likelihood via   |  ``emcee``                                                       |
  | Monte-Carlo Markov Chain |                                                                  |
  +--------------------------+------------------------------------------------------------------+
 
@@ -220,16 +283,14 @@
   well.
 
 ..  _fit-results-label:
 
 :class:`MinimizerResult` -- the optimization result
 ===================================================
 
-.. versionadded:: 0.9.0
-
 An optimization with :func:`minimize` or :meth:`Minimizer.minimize`
 will return a :class:`MinimizerResult` object. This is an otherwise
 plain container object (that is, with no methods of its own) that
 simply holds the results of the minimization. These results will
 include several pieces of informational data such as status and error
 messages, fit statistics, and the updated parameters themselves.
 
@@ -245,15 +306,14 @@
 with ``results`` being a ``MinimizerResult`` object. Note that the method
 :meth:`~lmfit.parameter.Parameters.pretty_print` accepts several arguments
 for customizing the output (e.g., column width, numeric format, etcetera).
 
 .. autoclass:: MinimizerResult
 
 
-
 Goodness-of-Fit Statistics
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. _goodfit-table:
 
  Table of Fit Results: These values, including the standard Goodness-of-Fit statistics,
  are all attributes of the :class:`MinimizerResult` object returned by
@@ -540,15 +600,15 @@
 not be used for fitting, but it is a useful method to to more thoroughly
 explore the parameter space around the solution after a fit has been done and
 thereby get an improved understanding of the probability distribution for the
 parameters. It may be able to refine your estimate of the most likely values
 for a set of parameters, but it will not iteratively find a good solution to
 the minimization problem. To use this method effectively, you should first
 use another minimization method and then use this method to explore the
-parameter space around thosee best-fit values.
+parameter space around those best-fit values.
 
 To illustrate this, we'll use an example problem of fitting data to function
 of a double exponential decay, including a modest amount of Gaussian noise to
 the data. Note that this example is the same problem used in
 :ref:`label-confidence-advanced` for evaluating confidence intervals in the
 parameters, which is a similar goal to the one here.
```

### Comparing `lmfit-1.2.1/doc/index.rst` & `lmfit-1.2.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/doc/installation.rst` & `lmfit-1.2.2/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/doc/intro.rst` & `lmfit-1.2.2/doc/intro.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/doc/make.bat` & `lmfit-1.2.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/doc/model.rst` & `lmfit-1.2.2/doc/model.rst`

 * *Files 4% similar despite different names*

```diff
@@ -236,14 +236,20 @@
 
 .. automethod:: Model.set_param_hint
 
    See :ref:`model_param_hints_section`.
 
 .. automethod:: Model.print_param_hints
 
+   See :ref:`model_param_hints_section`.
+
+..  automethod:: Model.post_fit
+
+   See :ref:`modelresult_uvars_postfit_section`.
+
 
 :class:`Model` class Attributes
 -------------------------------
 
 .. attribute:: func
 
    The model function used to calculate the model.
@@ -605,63 +611,68 @@
 
 The model as defined by your model function will use the independent
 variable(s) you specify to best match the data you provide.  The model is meant
 to be an abstract representation for data, but when you do a fit with
 :meth:`Model.fit`, you really need to pass in values for the data to be modeled
 and the independent data used to calculate that data.
 
-The mathematical solvers used by ``lmfit`` all work exclusively with
-1-dimensional numpy arrays of datatype (dtype) ``float64``.  The value of the
-calculation ``(model-data)*weights`` using the calculation of your model
-function, and the data and weights you pass in *will be coerced* to an
-1-dimensional ndarray with dtype ``float64`` when it is passed to the solver.
-
-If the data you pass to :meth:`Model.fit` is not an ndarray of dtype
-``float64`` but is instead a tuples of numbers, a list of numbers, or a
-``pandas.Series``, it will be coerced into an ndarray.  If your data is a list,
-tuple, or Series of complex numbers, it *will be coerced* to an ndarray with
-dtype ``complex128``.
-
-If your data is a numpy array of dtype ``float32``, it *will not be coerced* to
-``float64``, as we assume this was an intentional choice.  That may make all of
-the calculations done in your model function be in single-precision which may
-make fits less sensitive, but the values will be converted to ``float64``
-before being sent to the solver, so the fit should work.
 
-The independent data for models using ``Model`` are meant to be truly
-independent, and not **not** required to be strictly numerical or objects that
-are easily converted to arrays of numbers.  That is, independent data for a
-model could be a dictionary, an instance of a user-defined class, or other type
-of structured data.  You can use independent data any way you want in your
-model function.
+As discussed in :ref:`fit-data-label`, the mathematical solvers used by
+``lmfit`` all work exclusively with 1-dimensional numpy arrays of datatype
+(dtype) "float64".  The value of the calculation ``(model-data)*weights`` using
+the calculation of your model function, and the data and weights you pass in
+**will always be coerced** to an 1-dimensional ndarray with dtype "float64"
+when it is passed to the solver.  If it cannot be coerced, an error will occur
+and the fit will be aborted.
+
+That coercion will usually work for "array like" data that is not already a
+float64 ndarray.  But, depending on the model function, the calculations within
+the model function may not always work well for some "array like" data types
+- especially independent data that are in list of numbers and ndarrays of type
+"float32" or "int16" or less precision.
 
+
+To be clear, independent data for models using ``Model`` are meant to be truly
+independent, and not **not** required to be strictly numerical or objects that
+are easily converted to arrays of numbers.  The could, for example, be a
+dictionary, an instance of a user-defined class, or other type of structured
+data.  You can use independent data any way you want in your model function.
 But, as with almost all the examples given here, independent data is often also
-a 1-dimensonal array of values, say ``x``, and a simple view of the fit would be
-to plot the data as ``y`` as a function of ``x``.  Again, this is not required, but
-it is very common.  Because of this very common usage, if your independent data
-is a tuple or list of numbers or ``pandas.Series``, it *will be coerced* to be
-an ndarray of dtype ``float64``.  But as with the primary data, if your
-independent data is an ndarray of some different dtype (``float32``,
-``uint16``, etc), it *will not be coerced* to ``float64``, as we assume this
-was intentional.
-
-.. note::
-
-  Data and independent data that are tuples or lists of numbers, or
-  ``panda.Series`` will be coerced to an ndarray of dtype ``float64`` before
-  passing to the model function.  Data with other dtypes (or independent data
-  of other object types such as dicts) will not be coerced to ``float64``.
+a 1-dimensional array of values, say ``x``, and a simple view of the fit would
+be to plot the data as ``y`` as a function of ``x``.  Again, this is not
+required, but it is very common, especially for novice users.
+
+By default, all data and independent data passed to :meth:`Model.fit` that is
+"array like" - a list or tuple of numbers, a ``pandas.Series``, and
+``h5py.Dataset``, or any object that has an ``__array__()`` method -- will be
+converted to a "float64" ndarray before the fit begins.  If the array-like data
+is complex, it will be converted to a "complex128" ndarray, which will always
+work too.  This conversion before the fit begins ensures that the model
+function sees only "float64 ndarrays", and nearly guarantees that data type
+conversion will not cause problems for the fit.  But it also means that if you
+have passed a ``pandas.Series`` as data or independent data, not all of the
+methods or attributes of that ``Series`` will be available by default within
+the model function.
+
+.. versionadded:: 1.2.2
+
+This coercion can be turned of with the ``coerce_farray`` option to
+:meth:`Model.fit`.  When set to ``False``, neither the data nor the independent
+data will be coerced from their original data type, and the user will be
+responsible to arrange for the calculation and return value from the model
+function to be allow a proper and accurate conversion to a "float64" ndarray.
 
+See also :ref:`fit-data-label` for general advise and recommendations on
+types of data to use when fitting data.
 
 .. _model_saveload_sec:
 
 Saving and Loading Models
 -------------------------
 
-.. versionadded:: 0.9.8
 
 It is sometimes desirable to save a :class:`Model` for later use outside of
 the code used to define the model. Lmfit provides a :func:`save_model`
 function that will save a :class:`Model` to a file. There is also a
 companion :func:`load_model` function that can read this file and
 reconstruct a :class:`Model` from it.
 
@@ -761,49 +772,81 @@
 .. automethod:: ModelResult.plot
 
 .. automethod:: ModelResult.plot_fit
 
 .. automethod:: ModelResult.plot_residuals
 
 
+.. method:: ModelResult.iter_cb
+
+   Optional callable function, to be called at each fit iteration. This
+   must take take arguments of ``(params, iter, resid, *args, **kws)``, where
+   ``params`` will have the current parameter values, ``iter`` the
+   iteration, ``resid`` the current residual array, and ``*args`` and
+   ``**kws`` as passed to the objective function. See :ref:`fit-itercb-label`.
+
+.. method:: ModelResult.jacfcn
+
+   Optional callable function, to be called to calculate Jacobian array.
+
+
 :class:`ModelResult` attributes
 -------------------------------
 
-.. attribute:: aic
-
-   Floating point best-fit Akaike Information Criterion statistic
-   (see :ref:`fit-results-label`).
+A :class:`ModelResult` will take all of the attributes of
+:class:`MinimizerResult`, and several more. Here, we arrange them into
+categories.
 
-.. attribute:: best_fit
 
-   numpy.ndarray result of model function, evaluated at provided
-   independent variables and with best-fit parameters.
+Parameters and Variables
+~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. attribute:: best_values
 
    Dictionary with parameter names as keys, and best-fit values as values.
 
-.. attribute:: bic
+.. attribute:: init_params
 
-   Floating point best-fit Bayesian Information Criterion statistic
-   (see :ref:`fit-results-label`).
+   Initial parameters, as passed to :meth:`Model.fit`.
 
-.. attribute:: chisqr
+.. attribute:: init_values
 
-   Floating point best-fit chi-square statistic (see :ref:`fit-results-label`).
+   Dictionary with parameter names as keys, and initial values as values.
 
-.. attribute:: ci_out
+.. attribute:: init_vals
+
+   list of values for the variable parameters.
+
+.. attribute::  params
+
+   Parameters used in fit; will contain the best-fit values.
+
+.. attribute:: uvars
+
+   Dictionary of ``uncertainties`` ufloats from Parameters.
+
+.. attribute::   var_names
+
+   List of variable Parameter names used in optimization in the
+   same order as the values in :attr:`init_vals` and :attr:`covar`.
+
+Fit Arrays and Model
+~~~~~~~~~~~~~~~~~~~~~~~
+
+.. attribute:: best_fit
+
+   numpy.ndarray result of model function, evaluated at provided
+   independent variables and with best-fit parameters.
 
-   Confidence interval data (see :ref:`confidence_chapter`) or ``None`` if
-   the confidence intervals have not been calculated.
 
 .. attribute:: covar
 
    numpy.ndarray (square) covariance matrix returned from fit.
 
+
 .. attribute:: data
 
    numpy.ndarray of data to compare to model.
 
 .. attribute:: dely
 
    numpy.ndarray of estimated uncertainties in the ``y`` values of the model
@@ -811,46 +854,54 @@
 
 .. attribute:: dely_comps
 
    a dictionary of estimated uncertainties in the ``y`` values of the model
    components, from :meth:`ModelResult.eval_uncertainty` (see
    :ref:`eval_uncertainty_sec`).
 
-.. attribute:: errorbars
+.. attribute:: init_fit
 
-   Boolean for whether error bars were estimated by fit.
+   numpy.ndarray result of model function, evaluated at provided
+   independent variables and with initial parameters.
 
-.. attribute::  ier
+.. attribute::  residual
 
-   Integer returned code from :scipydoc:`optimize.leastsq`.
+   numpy.ndarray for residual.
 
-.. attribute:: init_fit
+.. attribute:: weights
 
-   numpy.ndarray result of model function, evaluated at provided
-   independent variables and with initial parameters.
+   numpy.ndarray (or ``None``) of weighting values to be used in fit. If not
+   ``None``, it will be used as a multiplicative factor of the residual
+   array, so that ``weights*(data - fit)`` is minimized in the
+   least-squares sense.
 
-.. attribute:: init_params
+.. attribute:: components
 
-   Initial parameters.
+   List of components of the :class:`Model`.
 
-.. attribute:: init_values
 
-   Dictionary with parameter names as keys, and initial values as values.
 
-.. attribute:: iter_cb
+Fit Status
+~~~~~~~~~~~~~~~~~~~
 
-   Optional callable function, to be called at each fit iteration. This
-   must take take arguments of ``(params, iter, resid, *args, **kws)``, where
-   ``params`` will have the current parameter values, ``iter`` the
-   iteration, ``resid`` the current residual array, and ``*args`` and
-   ``**kws`` as passed to the objective function. See :ref:`fit-itercb-label`.
+.. attribute:: aborted
 
-.. attribute:: jacfcn
+   Whether the fit was aborted.
 
-   Optional callable function, to be called to calculate Jacobian array.
+.. attribute:: errorbars
+
+   Boolean for whether error bars were estimated by fit.
+
+.. attribute:: flatchain
+
+   A ``pandas.DataFrame`` view of the sampling chain if the ``emcee`` method is uses.
+
+.. attribute::  ier
+
+   Integer returned code from :scipydoc:`optimize.leastsq`.
 
 .. attribute::  lmdif_message
 
    String message returned from :scipydoc:`optimize.leastsq`.
 
 .. attribute::  message
 
@@ -865,14 +916,51 @@
    Dict of keyword arguments actually send to underlying solver with
    :func:`~lmfit.minimizer.minimize`.
 
 .. attribute::  model
 
    Instance of :class:`Model` used for model.
 
+.. attribute::  scale_covar
+
+   Boolean flag for whether to automatically scale covariance matrix.
+
+
+.. attribute:: userargs
+
+   positional arguments passed to :meth:`Model.fit`, a tuple of (``y``, ``weights``)
+
+.. attribute:: userkws
+
+   keyword arguments passed to :meth:`Model.fit`, a dict, which will have independent data arrays such as ``x``.
+
+
+
+Fit Statistics
+~~~~~~~~~~~~~~~~~~~
+
+.. attribute:: aic
+
+   Floating point best-fit Akaike Information Criterion statistic
+   (see :ref:`fit-results-label`).
+
+.. attribute:: bic
+
+   Floating point best-fit Bayesian Information Criterion statistic
+   (see :ref:`fit-results-label`).
+
+.. attribute:: chisqr
+
+   Floating point best-fit chi-square statistic (see :ref:`fit-results-label`).
+
+.. attribute:: ci_out
+
+   Confidence interval data (see :ref:`confidence_chapter`) or ``None`` if
+   the confidence intervals have not been calculated.
+
 .. attribute::  ndata
 
    Integer number of data points.
 
 .. attribute::  nfev
 
    Integer number of function evaluations used for fit.
@@ -881,61 +969,37 @@
 
    Integer number of free parameters in fit.
 
 .. attribute::  nvarys
 
    Integer number of independent, freely varying variables in fit.
 
-.. attribute::  params
-
-   Parameters used in fit; will contain the best-fit values.
 
 .. attribute::  redchi
 
    Floating point reduced chi-square statistic (see :ref:`fit-results-label`).
 
-.. attribute::  residual
-
-   numpy.ndarray for residual.
-
 .. attribute:: rsquared
 
-   Floating point :math:`R^2` statisic, defined for data :math:`y` and best-fit model :math:`f` as
+   Floating point :math:`R^2` statistic, defined for data :math:`y` and best-fit model :math:`f` as
 
 .. math::
    :nowrap:
 
    \begin{eqnarray*}
      R^2 &=&  1 - \frac{\sum_i (y_i - f_i)^2}{\sum_i (y_i - \bar{y})^2}
     \end{eqnarray*}
 
-.. attribute::  scale_covar
-
-   Boolean flag for whether to automatically scale covariance matrix.
-
 .. attribute:: success
 
-   Boolean value of whether fit succeeded.
-
-.. attribute:: userargs
-
-   positional arguments passed to :meth:`Model.fit`, a tuple of (``y``, ``weights``)
+   Boolean value of whether fit succeeded. This is an optimistic
+   view of success, meaning that the method finished without error.
 
-.. attribute:: userkws
-
-   keyword arguments passed to :meth:`Model.fit`, a dict, which will have independent data arrays such as ``x``.
 
 
-.. attribute:: weights
-
-   numpy.ndarray (or ``None``) of weighting values to be used in fit. If not
-   ``None``, it will be used as a multiplicative factor of the residual
-   array, so that ``weights*(data - fit)`` is minimized in the
-   least-squares sense.
-
 .. _eval_uncertainty_sec:
 
 Calculating uncertainties in the model function
 -----------------------------------------------
 
 We return to the first example above and ask not only for the
 uncertainties in the fitted parameters but for the range of values that
@@ -984,21 +1048,67 @@
 
 An example script shows how the uncertainties in components of a composite
 model can be calculated and used:
 
 .. jupyter-execute:: ../examples/doc_model_uncertainty2.py
 
 
+
+.. _modelresult_uvars_postfit_section:
+
+Using uncertainties in the fitted parameters for post-fit calculations
+--------------------------------------------------------------------------
+
+.. versionadded:: 1.2.2
+
+.. _uncertainties package:   https://pythonhosted.org/uncertainties/
+
+As with the previous section, after a fit is complete, you may want to do some
+further calculations with the resulting Parameter values.  Since these
+Parameters will have not only best-fit values but also usually have
+uncertainties, it is desirable for subsequent calculations to be able to
+propagate those uncertainties to any resulting calculated value.  In addition,
+it is common for Parameters to have finite - and sometimes large -
+correlations which should be taken into account in such calculations.
+
+The :attr:`ModelResult.uvars` will be a dictionary with keys for all variable
+Parameters and values that are ``uvalues`` from the `uncertainties package`_.
+When used in mathematical calculations with basic Python operators or numpy
+functions, these ``uvalues`` will automatically propagate their uncertainties
+to the resulting calculation, and taking into account the full covariance
+matrix describing the correlation between values.
+
+This readily allows "derived Parameters" to be evaluated just after the fit.
+In fact, it might be useful to have a Model always do such a calculation just
+after the fit.  The :meth:`Model.post_fit` method allows exactly that: you can
+overwrite this otherwise empty method for any Model.  It takes one argument:
+the :class:`ModelResult` instance just after the actual fit has run (and before
+:meth:`Model.fit` returns) and can be used to add Parameters or do other
+post-fit processing.
+
+The following example script shows two different methods for calculating a centroid
+value for two peaks, either by doing the calculation directly after the fit
+with the ``result.uvars`` or by capturing this in a :meth:`Model.post_fit`
+method that would be run for all instances of that model.  It also demonstrates
+that taking correlations between Parameters into account when performing
+calculations can have a noticeable influence on the resulting uncertainties.
+
+
+.. jupyter-execute:: ../examples/doc_uvars_params.py
+
+
+Note that the :meth:`Model.post_fit` does not need to be limited to this
+use case of adding derived Parameters.
+
+
 .. _modelresult_saveload_sec:
 
 Saving and Loading ModelResults
 -------------------------------
 
-.. versionadded:: 0.9.8
-
 As with saving models (see section :ref:`model_saveload_sec`), it is
 sometimes desirable to save a :class:`ModelResult`, either for later use or
 to organize and compare different fit results. Lmfit provides a
 :func:`save_modelresult` function that will save a :class:`ModelResult` to
 a file. There is also a companion :func:`load_modelresult` function that
 can read this file and reconstruct a :class:`ModelResult` from it.
```

### Comparing `lmfit-1.2.1/doc/parameters.rst` & `lmfit-1.2.2/doc/parameters.rst`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 
     .. automethod:: add_many
 
     .. automethod:: pretty_print
 
     .. automethod:: valuesdict
 
+    .. automethod:: create_uvars
+
     .. automethod:: dumps
 
     .. automethod:: dump
 
     .. automethod:: eval
 
     .. automethod:: loads
@@ -90,14 +92,16 @@
    recovered with the :meth:`load` and :meth:`loads`. See
    :ref:`model_saveload_sec` for further discussion.
 
 
 The :func:`create_params` function
 ==================================
 
+.. versionadded:: 1.2.0
+
 The :func:`create_params` function is probably the easiest method for making
 :class:`Parameters` objects, as it allows defining Parameter names by keyword
 with values either being the numerical initial value for the Parameter or being
 a dictionary with keyword/value pairs for ``value`` as well as other Parameter
 attribute such as ``min``, ``max``, ``expr``, and so forth.
 
 .. autofunction:: create_params
```

### Comparing `lmfit-1.2.1/doc/sphinx/theme/sphinx13/basic_layout.html` & `lmfit-1.2.2/doc/sphinx/theme/sphinx13/basic_layout.html`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/doc/sphinx/theme/sphinx13/layout.html` & `lmfit-1.2.2/doc/sphinx/theme/sphinx13/layout.html`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/lmfitheader.png` & `lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/lmfitheader.png`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/sphinx13.css` & `lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/sphinx13.css`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/doc/support.rst` & `lmfit-1.2.2/doc/support.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/doc/whatsnew.rst` & `lmfit-1.2.2/doc/whatsnew.rst`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,62 @@
 .. _lmfit GitHub repository: https://github.com/lmfit/lmfit-py
 
 This section discusses changes between versions, especially changes
 significant to the use and behavior of the library. This is not meant
 to be a comprehensive list of changes. For such a complete record,
 consult the `lmfit GitHub repository`_.
 
+.. _whatsnew_122_label:
+
+Version 1.2.2 Release Notes (July 14, 2023)
+=================================================
+
+New features:
+
+- add ``ModelResult.uvars`` output to a ``ModelResult`` after a successful fit
+  that contains ``ufloats`` from the ``uncertainties`` package which can be
+  used for downstream calculations that propagate the uncertainties (and
+  correlations) of the variable Parameters. (PR #888)
+
+- Outputs of residual functions, including ``Model._residual``, are more
+  explicitly coerced to 1d-arrays of datatype Float64.  This decreases the
+  expectation for the user-supplied code to return ndarrays, and increases the
+  tolerance for more "array-like" objects or ndarrays that are not Float64 or
+  1-dimensional. (PR #899)
+
+- ``Model.fit`` now takes a ``coerce_farray`` option, defaulting to ``True`` to
+  control whether to input data and independent variables that are "array-like"
+  are coerced to ndarrays of datatype Float64 or Complex128.  If set to
+  ``False`` then independent data that "array-like" (``pandas.Series``, int32
+  arrays, etc) will be sent to the model function unaltered. The user may then
+  use other features of these objects, but may also need to explicitly coerce
+  the datatype of the result the change described above about coercing the
+  result causes problems. (Discussion #873; PR #899)
+
+Bug fixes/enhancements:
+
+- fixed bug in ``Model.make_params()`` for non-composite models that use a
+  prefix (Discussion #892; Issue #893; PR #895)
+
+- fixed bug with aborted fits for several methods having incorrect or invalid
+  fit statistics. (Discussion #894; Issue #896; PR #897)
+
+- ``Model.eval_uncertainty`` now correctly calculates complex (real/imaginary pairs)
+  uncertainties for Models that generate complex results. (Issue #900; PR #901)
+
+- ``Model.eval`` now returns and array-like value. This adds to the coercion
+  features above and fixes a bug for composite models that return lists (Issue #875; PR #901)
+
+- the HTML representation for a ``ModelResult`` or ``MinimizerResult`` are
+  improved, and create fewer entries in the Table of Contents for Jupyter lab.
+  (Issue #884; PR #883; PR #902)
+
+
+
+
 .. _whatsnew_121_label:
 
 Version 1.2.1 Release Notes (May 02, 2023)
 =================================================
 
 Bug fixes/enhancements:
 
@@ -36,15 +84,15 @@
 - add ``ModelResult.summary()`` to return many resulting fit statistics and attributes into a JSON-able dict.
 - add ``correl_table()`` function to ``lmfit.printfuncs`` and ``correl_mode`` option to ``fit_report()`` and
   ``ModelResult.fit_report()`` to optionally display a RST-formatted table of a correlation matrix.
 
 Bug fixes/enhancements:
 
 - fix bug when setting ``param.vary=True`` for a constrained parameter (Issue #859; PR #860)
-- fix bug in reported uncertainties for constrained parameters by better propating uncertainties (Issue #855; PR #856)
+- fix bug in reported uncertainties for constrained parameters by better propagating uncertainties (Issue #855; PR #856)
 - Coercing of user input data and independent data for ``Model`` to float64 ndarrays is somewhat less aggressive and
   will not increase the precision of numpy ndarrays (see :ref:`model_data_coercion_section` for details). The resulting
   calculation from a model or objective function is more aggressively coerced to float64.  (Issue #850; PR #853)
 - the default value of ``epsfcn`` is increased to 1.e-10 to allow for handling of data with precision less than float64
   (Issue #850; PR #853)
 - fix ``conf_interval2d`` to use "increase chi-square by sigma**2*reduced chi-square" to give the ``sigma``-level
   probabilities (Issue #848; PR #852)
```

### Comparing `lmfit-1.2.1/examples/NIST_Gauss2.dat` & `lmfit-1.2.2/examples/NIST_Gauss2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_builtinmodels_nistgauss.py` & `lmfit-1.2.2/examples/doc_builtinmodels_nistgauss.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_builtinmodels_nistgauss2.py` & `lmfit-1.2.2/examples/doc_builtinmodels_nistgauss2.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_builtinmodels_peakmodels.py` & `lmfit-1.2.2/examples/doc_builtinmodels_peakmodels.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_builtinmodels_splinemodel.py` & `lmfit-1.2.2/examples/doc_builtinmodels_splinemodel.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_builtinmodels_stepmodel.py` & `lmfit-1.2.2/examples/doc_builtinmodels_stepmodel.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_confidence_advanced.py` & `lmfit-1.2.2/examples/doc_confidence_advanced.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_confidence_chi2_maps.py` & `lmfit-1.2.2/examples/doc_confidence_chi2_maps.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_fitting_emcee.py` & `lmfit-1.2.2/examples/doc_fitting_emcee.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_fitting_withreport.py` & `lmfit-1.2.2/examples/doc_fitting_withreport.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_model_composite.py` & `lmfit-1.2.2/examples/doc_model_composite.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_model_gaussian.py` & `lmfit-1.2.2/examples/doc_model_gaussian.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_model_loadmodel.py` & `lmfit-1.2.2/examples/doc_model_loadmodel.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_model_loadmodelresult.py` & `lmfit-1.2.2/examples/doc_model_loadmodelresult.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_model_loadmodelresult2.py` & `lmfit-1.2.2/examples/doc_model_loadmodelresult2.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_model_savemodelresult2.py` & `lmfit-1.2.2/examples/doc_model_savemodelresult2.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_model_two_components.py` & `lmfit-1.2.2/examples/doc_model_two_components.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_model_uncertainty.py` & `lmfit-1.2.2/examples/doc_model_uncertainty.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_model_uncertainty2.py` & `lmfit-1.2.2/examples/doc_model_uncertainty2.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_model_with_iter_callback.py` & `lmfit-1.2.2/examples/doc_model_with_iter_callback.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_model_with_nan_policy.py` & `lmfit-1.2.2/examples/doc_model_with_nan_policy.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_parameters_basic.py` & `lmfit-1.2.2/examples/doc_parameters_basic.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/doc_parameters_valuesdict.py` & `lmfit-1.2.2/examples/doc_parameters_valuesdict.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/example_Model_interface.py` & `lmfit-1.2.2/examples/example_Model_interface.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/example_brute.py` & `lmfit-1.2.2/examples/example_brute.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/example_complex_resonator_model.py` & `lmfit-1.2.2/examples/example_complex_resonator_model.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/example_confidence_interval.py` & `lmfit-1.2.2/examples/example_confidence_interval.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/example_detect_outliers.py` & `lmfit-1.2.2/examples/example_detect_outliers.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/example_diffev.py` & `lmfit-1.2.2/examples/example_diffev.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/example_emcee_Model_interface.py` & `lmfit-1.2.2/examples/example_emcee_Model_interface.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/example_expression_model.py` & `lmfit-1.2.2/examples/example_expression_model.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/example_fit_multi_datasets.py` & `lmfit-1.2.2/examples/example_fit_multi_datasets.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/example_fit_with_algebraic_constraint.py` & `lmfit-1.2.2/examples/example_fit_with_algebraic_constraint.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/example_fit_with_bounds.py` & `lmfit-1.2.2/examples/example_fit_with_bounds.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/example_fit_with_derivfunc.py` & `lmfit-1.2.2/examples/example_fit_with_derivfunc.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/example_fit_with_inequality.py` & `lmfit-1.2.2/examples/example_fit_with_inequality.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/example_reduce_fcn.py` & `lmfit-1.2.2/examples/example_reduce_fcn.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/example_sympy.py` & `lmfit-1.2.2/examples/example_sympy.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/example_two_dimensional_peak.py` & `lmfit-1.2.2/examples/example_two_dimensional_peak.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/example_use_pandas.py` & `lmfit-1.2.2/examples/example_use_pandas.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/lmfit_emcee_model_selection.py` & `lmfit-1.2.2/examples/lmfit_emcee_model_selection.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/model1d_gauss.dat` & `lmfit-1.2.2/examples/model1d_gauss.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/peak.csv` & `lmfit-1.2.2/examples/peak.csv`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/sinedata.dat` & `lmfit-1.2.2/examples/sinedata.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/test_peak.dat` & `lmfit-1.2.2/examples/test_peak.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/examples/test_splinepeak.dat` & `lmfit-1.2.2/examples/test_splinepeak.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/lmfit/__init__.py` & `lmfit-1.2.2/lmfit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     capabilities of `scipy.optimize.curve_fit`, allowing you to turn a
     function that models your data into a Python class that helps you
     parametrize and fit data with that model.
 
   * Many built-in models for common lineshapes are included and ready
     to use.
 
-Copyright (c) 2022 Lmfit Developers ; BSD-3 license ; see LICENSE
+Copyright (c) 2023 Lmfit Developers ; BSD-3 license ; see LICENSE
 
 """
 from asteval import Interpreter
 
 from .confidence import conf_interval, conf_interval2d
 from .minimizer import Minimizer, MinimizerException, minimize
 from .parameter import Parameter, Parameters, create_params
```

### Comparing `lmfit-1.2.1/lmfit/_ampgo.py` & `lmfit-1.2.2/lmfit/_ampgo.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/lmfit/conf_emcee.py` & `lmfit-1.2.2/lmfit/conf_emcee.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/lmfit/confidence.py` & `lmfit-1.2.2/lmfit/confidence.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/lmfit/jsonutils.py` & `lmfit-1.2.2/lmfit/jsonutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """JSON utilities."""
 
 from base64 import b64decode, b64encode
 import sys
 import warnings
 
 import numpy as np
+import uncertainties
 
 try:
     import dill
     HAS_DILL = True
 except ImportError:
     HAS_DILL = False
 
@@ -53,14 +54,16 @@
     - complex numbers
 
     """
     if isinstance(obj, DataFrame):
         return dict(__class__='PDataFrame', value=obj.to_json())
     if isinstance(obj, Series):
         return dict(__class__='PSeries', value=obj.to_json())
+    if isinstance(obj, uncertainties.core.AffineScalarFunc):
+        return dict(__class__='UFloat', val=obj.nominal_value, err=obj.std_dev)
     if isinstance(obj, np.ndarray):
         if 'complex' in obj.dtype.name:
             val = [(obj.real).tolist(), (obj.imag).tolist()]
         elif obj.dtype.name == 'object':
             val = [encode4js(item) for item in obj]
         else:
             val = obj.flatten().tolist()
@@ -100,15 +103,14 @@
     """Return decoded Python object from encoded object."""
     if not isinstance(obj, dict):
         return obj
     out = obj
     classname = obj.pop('__class__', None)
     if classname is None:
         return obj
-
     if classname == 'Complex':
         out = obj['value'][0] + 1j*obj['value'][1]
     elif classname in ('List', 'Tuple'):
         out = []
         for item in obj['value']:
             out.append(decode4js(item))
         if classname == 'Tuple':
@@ -124,14 +126,16 @@
         else:
             out = np.fromiter(obj['value'], dtype=obj['__dtype__'])
         out.shape = obj['__shape__']
     elif classname == 'PDataFrame' and read_json is not None:
         out = read_json(obj['value'])
     elif classname == 'PSeries' and read_json is not None:
         out = read_json(obj['value'], typ='series')
+    elif classname == 'UFloat':
+        out = uncertainties.ufloat(obj['val'], obj['err'])
     elif classname == 'Callable':
         out = obj['__name__']
         try:
             out = import_from(obj['importer'], out)
             unpacked = True
         except (ImportError, AttributeError):
             unpacked = False
```

### Comparing `lmfit-1.2.1/lmfit/lineshapes.py` & `lmfit-1.2.2/lmfit/lineshapes.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,23 +102,23 @@
     return amp*(ss*(x < center)/(ss+xc2) + rr*(x >= center)/(rr+xc2))
 
 
 def voigt(x, amplitude=1.0, center=0.0, sigma=1.0, gamma=None):
     """Return a 1-dimensional Voigt function.
 
     voigt(x, amplitude, center, sigma, gamma) =
-        amplitude*wofz(z).real / (sigma*s2pi)
+        amplitude*real(wofz(z)) / (sigma*s2pi)
 
     For more information, see: https://en.wikipedia.org/wiki/Voigt_profile
 
     """
     if gamma is None:
         gamma = sigma
     z = (x-center + 1j*gamma) / max(tiny, (sigma*s2))
-    return amplitude*wofz(z).real / max(tiny, (sigma*s2pi))
+    return amplitude*real(wofz(z)) / max(tiny, (sigma*s2pi))
 
 
 def pvoigt(x, amplitude=1.0, center=0.0, sigma=1.0, fraction=0.5):
     """Return a 1-dimensional pseudo-Voigt function.
 
     pvoigt(x, amplitude, center, sigma, fraction) =
         amplitude*(1-fraction)*gaussian(x, center, sigma_g) +
```

### Comparing `lmfit-1.2.1/lmfit/minimizer.py` & `lmfit-1.2.2/lmfit/minimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 from scipy.optimize import leastsq as scipy_leastsq
 from scipy.optimize import minimize as scipy_minimize
 from scipy.optimize import shgo as scipy_shgo
 from scipy.sparse import issparse
 from scipy.sparse.linalg import LinearOperator
 from scipy.stats import cauchy as cauchy_dist
 from scipy.stats import norm as norm_dist
-import uncertainties
 
 from ._ampgo import ampgo
 from .parameter import Parameter, Parameters
 from .printfuncs import fitreport_html_table
 
 # check for EMCEE
 try:
@@ -84,61 +83,14 @@
     """Return the name of calling function."""
     try:
         return inspect.stack()[1].function
     except AttributeError:
         return inspect.stack()[1][3]
 
 
-def asteval_with_uncertainties(*vals, **kwargs):
-    """Calculate object value, given values for variables.
-
-    This is used by the uncertainties package to calculate the
-    uncertainty in an object even with a complicated expression.
-
-    """
-    _obj = kwargs.get('_obj', None)
-    _pars = kwargs.get('_pars', None)
-    _names = kwargs.get('_names', None)
-    _asteval = _pars._asteval
-    if (_obj is None or _pars is None or _names is None or
-            _asteval is None or _obj._expr_ast is None):
-        return 0
-    for val, name in zip(vals, _names):
-        _asteval.symtable[name] = val
-
-    # re-evaluate all constraint parameters to
-    # force the propagation of uncertainties
-    [p._getval() for p in _pars.values()]
-    return _asteval.eval(_obj._expr_ast)
-
-
-wrap_ueval = uncertainties.wrap(asteval_with_uncertainties)
-
-
-def eval_stderr(obj, uvars, _names, _pars):
-    """Evaluate uncertainty and set ``.stderr`` for a parameter `obj`.
-
-    Given the uncertain values `uvars` (list of `uncertainties.ufloats`),
-    a list of parameter names that matches `uvars`, and a dictionary of
-    parameter objects, keyed by name.
-
-    This uses the uncertainties package wrapped function to evaluate the
-    uncertainty for an arbitrary expression (in ``obj._expr_ast``) of
-    parameters.
-
-    """
-    if not isinstance(obj, Parameter) or getattr(obj, '_expr_ast', None) is None:
-        return
-    uval = wrap_ueval(*uvars, _obj=obj, _names=_names, _pars=_pars)
-    try:
-        obj.stderr = uval.std_dev
-    except Exception:
-        obj.stderr = 0
-
-
 class MinimizerException(Exception):
     """General Purpose Exception."""
 
     def __init__(self, msg):
         Exception.__init__(self)
         self.msg = msg
 
@@ -248,68 +200,73 @@
     fit statistics, and the updated (i.e., best-fit) parameters themselves
     in the :attr:`params` attribute.
 
     The list of (possible) `MinimizerResult` attributes is given below:
 
     Attributes
     ----------
+    residual : numpy.ndarray
+        Residual array :math:`{\rm Resid_i}`. Return value of the objective
+        function when using the best-fit values of the parameters.
     params : Parameters
-        The best-fit parameters resulting from the fit.
-    status : int
-        Termination status of the optimizer. Its value depends on the
-        underlying solver. Refer to `message` for details.
+        The best-fit Parameters resulting from the fit.
+    uvars : dict
+        Dictionary of uncertainties ufloats from Parameters
     var_names : list
-        Ordered list of variable parameter names used in optimization, and
-        useful for understanding the values in :attr:`init_vals` and
-        :attr:`covar`.
-    covar : numpy.ndarray
+        list of variable Parameter names used in optimization in the
+        same order as the values in :attr:`init_vals` and :attr:`covar`.
+    covar : numpy.ndarray or None
         Covariance matrix from minimization, with rows and columns
-        corresponding to :attr:`var_names`.
+        corresponding to :attr:`var_names`.  If uncertainties cannot
+        be determined, this value will be ``None``.
     init_vals : list
         List of initial values for variable parameters using
         :attr:`var_names`.
     init_values : dict
         Dictionary of initial values for variable parameters.
-    nfev : int
-        Number of function evaluations.
+    aborted : bool
+        Whether the fit was aborted.
+    status : int
+        Termination status of the optimizer. Its value depends on the
+        underlying solver. Refer to `message` for details.
     success : bool
-        True if the fit succeeded, otherwise False.
+        True if the fit succeeded, otherwise False. This is an optimistic
+        view of success, meaning that the method finished without error.
     errorbars : bool
-        True if uncertainties were estimated, otherwise False.
+        whether uncertainties were estimated for variable Parameters.
     message : str
         Message about fit success.
-    call_kws : dict
-        Keyword arguments sent to underlying solver.
     ier : int
         Integer error value from :scipydoc:`optimize.leastsq` (`'leastsq'`
         method only).
     lmdif_message : str
         Message from :scipydoc:`optimize.leastsq` (`'leastsq'` method only).
+    call_kws : dict
+        Keyword arguments sent to underlying solver.
+    flatchain : pandas.DataFrame
+        A flatchain view of the sampling chain from the `emcee` method.
+    nfev : int
+        Number of function evaluations.
     nvarys : int
         Number of variables in fit: :math:`N_{\rm varys}`.
     ndata : int
         Number of data points: :math:`N`.
     nfree : int
         Degrees of freedom in fit: :math:`N - N_{\rm varys}`.
-    residual : numpy.ndarray
-        Residual array :math:`{\rm Resid_i}`. Return value of the objective
-        function when using the best-fit values of the parameters.
     chisqr : float
         Chi-square: :math:`\chi^2 = \sum_i^N [{\rm Resid}_i]^2`.
     redchi : float
         Reduced chi-square:
         :math:`\chi^2_{\nu}= {\chi^2} / {(N - N_{\rm varys})}`.
     aic : float
         Akaike Information Criterion statistic:
         :math:`N \ln(\chi^2/N) + 2 N_{\rm varys}`.
     bic : float
         Bayesian Information Criterion statistic:
         :math:`N \ln(\chi^2/N) + \ln(N) N_{\rm varys}`.
-    flatchain : pandas.DataFrame
-        A flatchain view of the sampling chain from the `emcee` method.
 
     Methods
     -------
     show_candidates
         :meth:`pretty_print` representation of candidates from the `brute`
         fitting method.
 
@@ -378,16 +335,17 @@
         self.chisqr = max(self.chisqr, 1.e-250*self.ndata)
         _neg2_log_likel = self.ndata * np.log(self.chisqr / self.ndata)
         self.aic = _neg2_log_likel + 2 * self.nvarys
         self.bic = _neg2_log_likel + np.log(self.ndata) * self.nvarys
 
     def _repr_html_(self, show_correl=True, min_correl=0.1):
         """Return a HTML representation of parameters data."""
-        return fitreport_html_table(self, show_correl=show_correl,
-                                    min_correl=min_correl)
+        report = fitreport_html_table(self, show_correl=show_correl,
+                                      min_correl=min_correl)
+        return f"<h2>Fit Result</h2> {report}"
 
 
 class Minimizer:
     """A general minimizer for curve fitting and optimization."""
 
     _err_nonparam = ("params must be a minimizer.Parameters() instance or"
                      " list of Parameters()")
@@ -597,16 +555,15 @@
         if self._abort:
             self.result.residual = out
             self.result.aborted = True
             self.result.message = "Fit aborted by user callback. Could not estimate error-bars."
             self.result.success = False
             raise AbortFitException("fit aborted by user.")
         else:
-            return _nan_policy(np.asfarray(out).ravel(),
-                               nan_policy=self.nan_policy)
+            return coerce_float64(out, nan_policy=self.nan_policy)
 
     def __jacobian(self, fvars):
         """Return analytical jacobian to be used with Levenberg-Marquardt.
 
         modified 02-01-2012 by Glenn Jones, Aberystwyth University
         modified 06-29-2015 by M Newville to apply gradient scaling for
         bounded variables (thanks to JJ Helmus, N Mayorov)
@@ -620,15 +577,15 @@
             grad_scale[ivar] = pars[name].scale_gradient(val)
 
         pars.update_constraints()
 
         # compute the jacobian for "internal" unbounded variables,
         # then rescale for bounded "external" variables.
         jac = self.jacfcn(pars, *self.userargs, **self.userkws)
-        jac = _nan_policy(jac, nan_policy=self.nan_policy)
+        jac = coerce_float64(jac, nan_policy=self.nan_policy, ravel=False)
 
         if self.col_deriv:
             jac = (jac.transpose()*grad_scale).transpose()
         else:
             jac *= grad_scale
         return jac
 
@@ -842,50 +799,30 @@
     def _calculate_uncertainties_correlations(self):
         """Calculate parameter uncertainties and correlations."""
         self.result.errorbars = True
 
         if self.scale_covar:
             self.result.covar *= self.result.redchi
 
-        vbest = np.atleast_1d([self.result.params[name].value for name in
-                               self.result.var_names])
-
-        has_expr = False
         for par in self.result.params.values():
             par.stderr, par.correl = 0, None
-            has_expr = has_expr or par.expr is not None
-
         for ivar, name in enumerate(self.result.var_names):
             par = self.result.params[name]
             par.stderr = np.sqrt(self.result.covar[ivar, ivar])
             par.correl = {}
             try:
                 self.result.errorbars = self.result.errorbars and (par.stderr > 0.0)
                 for jvar, varn2 in enumerate(self.result.var_names):
                     if jvar != ivar:
                         par.correl[varn2] = (self.result.covar[ivar, jvar] /
                                              (par.stderr * np.sqrt(self.result.covar[jvar, jvar])))
             except ZeroDivisionError:
                 self.result.errorbars = False
-
-        if has_expr:
-            try:
-                uvars = uncertainties.correlated_values(vbest, self.result.covar)
-            except (LinAlgError, ValueError):
-                uvars = None
-
-            # for uncertainties on constrained parameters, use the calculated
-            # "correlated_values", evaluate the uncertainties on the constrained
-            # parameters and reset the Parameters to best-fit value
-            if uvars is not None:
-                for par in self.result.params.values():
-                    eval_stderr(par, uvars, self.result.var_names, self.result.params)
-                # restore nominal values
-                for v, name in zip(uvars, self.result.var_names):
-                    self.result.params[name].value = v.nominal_value
+        if self.result.errorbars:
+            self.result.uvars = self.result.params.create_uvars(covar=self.result.covar)
 
     def scalar_minimize(self, method='Nelder-Mead', params=None, max_nfev=None,
                         **kws):
         """Scalar minimization using :scipydoc:`optimize.minimize`.
 
         Perform fit with any of the scalar minimization algorithms
         supported by :scipydoc:`optimize.minimize`. Default argument
@@ -960,17 +897,23 @@
         """
         result = self.prepare_fit(params=params)
         result.method = method
         variables = result._init_vals_internal
         params = result.params
 
         self.set_max_nfev(max_nfev, 2000*(result.nvarys+1))
+
         fmin_kws = dict(method=method, options={'maxiter': 2*self.max_nfev})
         if method == 'L-BFGS-B':
             fmin_kws['options']['maxfun'] = 2*self.max_nfev
+        elif method == 'COBYLA':
+            # for this method, we explicitly let the solver reach
+            # the users max nfev, and do not abort in _residual.
+            fmin_kws['options']['maxiter'] = self.max_nfev
+            self.max_nfev = 5*self.max_nfev
 
         # fmin_kws = dict(method=method, options={'maxfun': 2*self.max_nfev})
         fmin_kws.update(self.kws)
 
         if 'maxiter' in kws:
             warnings.warn(maxeval_warning.format('maxiter', thisfuncname()),
                           RuntimeWarning)
@@ -1055,14 +998,15 @@
             self._abort = False
             result.residual = self.__residual(result.x)
             result.nfev += 1
 
         result._calculate_statistics()
 
         # calculate the cov_x and estimate uncertainties/correlations
+        self.result.uvars = None
         if (not result.aborted and self.calc_covar and HAS_NUMDIFFTOOLS and
                 len(result.residual) > len(result.var_names)):
             _covar_ndt = self._calculate_covariance_matrix(result.x)
             if _covar_ndt is not None:
                 result.covar = self._int2ext_cov_x(_covar_ndt, result.x)
                 self._calculate_uncertainties_correlations()
 
@@ -1131,17 +1075,16 @@
                                  *userargs, **userkwargs)
             self._abort = self._abort or abort
         if self._abort:
             self.result.residual = out
             self._lastpos = theta
             raise AbortFitException("fit aborted by user.")
         else:
-            out = _nan_policy(np.asarray(out).ravel(),
-                              nan_policy=self.nan_policy)
-        lnprob = np.asarray(out).ravel()
+            out = coerce_float64(out, nan_policy=self.nan_policy)
+        lnprob = coerce_float64(out, nan_policy=self.nan_policy)
         if len(lnprob) == 0:
             lnprob = np.array([-1.e100])
         if lnprob.size > 1:
             # objective function returns a vector of residuals
             if '__lnsigma' in params and not is_weighted:
                 # marginalise over a constant data uncertainty
                 __lnsigma = params['__lnsigma'].value
@@ -1502,16 +1445,16 @@
             result.acor = self.sampler.get_autocorr_time()
         except AutocorrError as e:
             print(str(e))
         result.acceptance_fraction = self.sampler.acceptance_fraction
 
         # Calculate the residual with the "best fit" parameters
         out = self.userfcn(params, *self.userargs, **self.userkws)
-        result.residual = _nan_policy(out, nan_policy=self.nan_policy,
-                                      handle_inf=False)
+        result.residual = coerce_float64(out, nan_policy=self.nan_policy,
+                                         handle_inf=False)
 
         # If uncertainty was automatically estimated, weight the residual properly
         if not is_weighted and result.residual.size > 1 and '__lnsigma' in params:
             result.residual /= np.exp(params['__lnsigma'].value)
 
         # Calculate statistics for the two standard cases:
         if isinstance(result.residual, np.ndarray) or (float_behavior == 'chi2'):
@@ -1596,22 +1539,27 @@
 
         try:
             ret = least_squares(self.__residual, start_vals,
                                 bounds=(lower_bounds, upper_bounds),
                                 **least_squares_kws)
             result.residual = ret.fun
         except AbortFitException:
-            pass
+            ret = None
+            result.aborted = True
 
         # Note: scipy.optimize.least_squares is actually returning the
         # "last evaluation", which is not necessarily the "best result"; so we
         # do that here for consistency
         if not result.aborted:
             result.nfev -= 1
             result.residual = self.__residual(ret.x, False)
+        elif result.nfev > self.max_nfev-5:
+            result.nfev -= 2
+            _best = result.last_internal_values
+            result.residual = self.__residual(_best, False)
         result._calculate_statistics()
 
         if not result.aborted:
             for attr in ret:
                 outattr = attr
                 if attr == 'nfev':
                     outattr = 'least_squares_nfev'
@@ -1804,14 +1752,18 @@
         except AbortFitException:
             pass
 
         if not result.aborted:
             result.message = ret.message
             result.residual = self.__residual(ret.x)
             result.nfev -= 1
+        elif result.nfev > self.max_nfev-5:
+            result.nfev -= 2
+            _best = result.last_internal_values
+            result.residual = self.__residual(_best, False)
 
         result._calculate_statistics()
 
         # calculate the cov_x and estimate uncertainties/correlations
         if (not result.aborted and self.calc_covar and HAS_NUMDIFFTOOLS and
                 len(result.residual) > len(result.var_names)):
             _covar_ndt = self._calculate_covariance_matrix(ret.x)
@@ -1983,15 +1935,18 @@
                     pars[par].value = data[0][i]
                 result.candidates.append(Candidate(params=pars, score=data[1]))
 
             result.params = result.candidates[0].params
             result.residual = self.__residual(result.brute_x0,
                                               apply_bounds_transformation=False)
             result.nfev = len(result.brute_Jout.ravel())
-
+        elif result.nfev > self.max_nfev-5:
+            result.nfev -= 2
+            _best = result.last_internal_values
+            result.residual = self.__residual(_best, False)
         result._calculate_statistics()
 
         return result
 
     def ampgo(self, params=None, max_nfev=None, **kws):
         """Find the global minimum of a multivariate function using AMPGO.
 
@@ -2106,14 +2061,18 @@
             result.ampgo_tunnel = ret[4]
 
             for i, par in enumerate(result.var_names):
                 result.params[par].value = result.ampgo_x0[i]
 
             result.residual = self.__residual(result.ampgo_x0)
             result.nfev -= 1
+        elif result.nfev > self.max_nfev-5:
+            result.nfev -= 2
+            _best = result.last_internal_values
+            result.residual = self.__residual(_best, False)
 
         result._calculate_statistics()
 
         # calculate the cov_x and estimate uncertainties/correlations
         if (not result.aborted and self.calc_covar and HAS_NUMDIFFTOOLS and
                 len(result.residual) > len(result.var_names)):
             _covar_ndt = self._calculate_covariance_matrix(result.ampgo_x0)
@@ -2184,15 +2143,18 @@
                 if attr in ['success', 'message']:
                     setattr(result, attr, value)
                 else:
                     setattr(result, f'shgo_{attr}', value)
 
             result.residual = self.__residual(result.shgo_x, False)
             result.nfev -= 1
-
+        elif result.nfev > self.max_nfev-5:
+            result.nfev -= 2
+            _best = result.last_internal_values
+            result.residual = self.__residual(_best, False)
         result._calculate_statistics()
 
         # calculate the cov_x and estimate uncertainties/correlations
         if (not result.aborted and self.calc_covar and HAS_NUMDIFFTOOLS and
                 len(result.residual) > len(result.var_names)):
             result.covar = self._calculate_covariance_matrix(result.shgo_x)
             if result.covar is not None:
@@ -2265,14 +2227,18 @@
                 if attr in ['success', 'message']:
                     setattr(result, attr, value)
                 else:
                     setattr(result, f'da_{attr}', value)
 
             result.residual = self.__residual(result.da_x, False)
             result.nfev -= 1
+        elif result.nfev > self.max_nfev-5:
+            result.nfev -= 2
+            _best = result.last_internal_values
+            result.residual = self.__residual(_best, False)
 
         result._calculate_statistics()
 
         # calculate the cov_x and estimate uncertainties/correlations
         if (not result.aborted and self.calc_covar and HAS_NUMDIFFTOOLS and
                 len(result.residual) > len(result.var_names)):
             result.covar = self._calculate_covariance_matrix(result.da_x)
@@ -2394,43 +2360,59 @@
         return np.random.RandomState(seed)
     if isinstance(seed, np.random.RandomState):
         return seed
     raise ValueError(f'{seed:r} cannot be used to seed a numpy.random.RandomState'
                      ' instance')
 
 
-def _nan_policy(arr, nan_policy='raise', handle_inf=True):
-    """Specify behaviour when array contains ``numpy.nan`` or ``numpy.inf``.
+def coerce_float64(arr, nan_policy='raise', handle_inf=True,
+                   ravel=True, ravel_order='C'):
+    """coerce array-like objects to be a float64 ndarrays, usually forcing to 1D arrays.
+
+    also handles behaviour when array contains ``numpy.nan`` or ``numpy.inf``.
 
     Parameters
     ----------
     arr : array_like
         Input array to consider.
     nan_policy : {'raise', 'propagate', 'omit'}, optional
-        One of:
+        policy for handling NaN values. One of:
 
         `'raise'` - raise a `ValueError` if `arr` contains NaN (default)
         `'propagate'` - propagate NaN
         `'omit'` - filter NaN from input array
-
     handle_inf : bool, optional
-        Whether to apply the `nan_policy` to +/- infinity (default is
-        True).
+        Whether to apply the `nan_policy` to +/-Inf (default is True).
+    ravel : bool, optional
+        Whether to force to be 1D array (default is True).
+    ravel_order : str, optional
+        array ordering to assume when unravelling array (default is 'C')
 
     Returns
     -------
-    array_like
-        Result of `arr` after applying the `nan_policy`.
+    array
+        ndarray of type np.float64, possibly after applying the `nan_policy`,
+        and usually raveling to 1-D array
 
     Notes
     -----
-    This function is copied, then modified, from
-    scipy/stats/stats.py/_contains_nan
+    Parts of this function are based on scipy/stats/stats.py/_contains_nan
 
+    support for 'array-like` objects is from numpy `asfarray`, which includes
+    lists of numbers, pandas.Series, h5py.Datasets, and many other array-like
+    Python objects
     """
+    if np.iscomplexobj(arr):
+        arr = np.asfarray(arr, dtype=np.complex128).view(np.float64)
+    else:
+        arr = np.asfarray(arr, dtype=np.float64)
+
+    if ravel:
+        arr = arr.ravel(order=ravel_order)
+
     if nan_policy not in ('propagate', 'omit', 'raise'):
         raise ValueError("nan_policy must be 'propagate', 'omit', or 'raise'.")
 
     if handle_inf:
         handler_func = lambda x: ~np.isfinite(x)
     else:
         handler_func = isnull
@@ -2460,14 +2442,23 @@
                    'your objective/model function - fitting algorithms cannot '
                    'handle this! Please read https://lmfit.github.io/lmfit-py/faq.html#i-get-errors-from-nan-in-my-fit-what-can-i-do '
                    'for more information.')
             raise ValueError(msg)
     return arr
 
 
+# coerce_float64 replaces _nan_policy.  That was never part of the public API,
+# but we'll have it raise a DeprecationWarning for a while.
+# This change happened in June, 2023, v 1.2.1, so this function can removed
+# sometime in 2024, or after v 1.3.
+def _nan_policy(arr, nan_policy='raise', handle_inf=True, **kws):
+    warnings.warn('`_nan_policy` has been replaced with coerce_float64`', DeprecationWarning)
+    return coerce_float64(arr, nan_policy=nan_policy, handle_inf=handle_inf, **kws)
+
+
 def minimize(fcn, params, method='leastsq', args=None, kws=None, iter_cb=None,
              scale_covar=True, nan_policy='raise', reduce_fcn=None,
              calc_covar=True, max_nfev=None, **fit_kws):
     """Perform the minimization of the objective function.
 
     The minimize function takes an objective function to be minimized,
     a dictionary (:class:`~lmfit.parameter.Parameters` ; Parameters) containing
```

### Comparing `lmfit-1.2.1/lmfit/model.py` & `lmfit-1.2.2/lmfit/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,28 @@
                     err[err == np.inf] = np.pi
     else:
         err = dz
 
     return err
 
 
+def coerce_arraylike(x):
+    """
+    coerce lists, tuples, and pandas Series, hdf5 Groups, etc to an
+    ndarray float64 or complex128, but leave other data structures
+    and objects unchanged
+    """
+    if isinstance(x, (list, tuple, Series)) or hasattr(x, '__array__'):
+        if np.isrealobj(x):
+            return np.asfarray(x)
+        if np.iscomplexobj(x):
+            return np.asfarray(x, dtype=np.complex128)
+    return x
+
+
 class Model:
     """Create a model from a user-supplied model function."""
 
     _forbidden_args = ('data', 'weights', 'params')
     _invalid_ivar = "Invalid independent variable name ('%s') for function %s"
     _invalid_par = "Invalid parameter name ('%s') for function %s"
     _invalid_hint = "unknown parameter hint '%s' for param '%s'"
@@ -696,15 +710,15 @@
                 for item in self._hint_names:
                     if item in hint:
                         setattr(par, item, hint[item])
             # apply values passed in through kw args
             if basename in kwargs:
                 setpar(par, kwargs[basename])
             if name in kwargs:
-                setpar(par, kwargs[basename])
+                setpar(par, kwargs[name])
             params.add(par)
             if verbose:
                 print(f' - Adding parameter "{name}"')
 
         # next build parameters defined in param_hints
         # note that composites may define their own additional
         # convenience parameters here
@@ -807,15 +821,15 @@
                     # weights are complex
                     weights = weights.ravel().view(float)
                 else:
                     # real weights but complex data
                     weights = (weights + 1j * weights).ravel().view(float)
         if weights is not None:
             diff *= weights
-        return np.asarray(diff).ravel()  # for compatibility with pandas.Series
+        return diff
 
     def _strip_prefix(self, name):
         npref = len(self._prefix)
         if npref > 0 and name.startswith(self._prefix):
             name = name[npref:]
         return name
 
@@ -863,14 +877,20 @@
                 out[name] = val
 
         # 4. finally, reset any values that have overwritten parameter values
         for name, val in saved_values.items():
             params[name].value = val
         return out
 
+    def post_fit(self, fitresult):
+        """function that is called just after fit, can be overloaded by
+        subclasses to add non-fitting 'calculated parameters'
+        """
+        pass
+
     def _make_all_args(self, params=None, **kwargs):
         """Generate **all** function args for all functions."""
         args = {}
         for key, val in self.make_funcargs(params, kwargs).items():
             args[f"{self._prefix}{key}"] = val
         return args
 
@@ -903,15 +923,15 @@
         keyword arguments.
 
         4. The return types are generally `numpy.ndarray`, but may depends on
         the model function and input independent variables. That is, return
         values may be Python `float`, `int`, or  `complex` values.
 
         """
-        return self.func(**self.make_funcargs(params, kwargs))
+        return coerce_arraylike(self.func(**self.make_funcargs(params, kwargs)))
 
     @property
     def components(self):
         """Return components for composite model."""
         return [self]
 
     def eval_components(self, params=None, **kwargs):
@@ -934,15 +954,16 @@
         key = self._prefix
         if len(key) < 1:
             key = self._name
         return {key: self.eval(params=params, **kwargs)}
 
     def fit(self, data, params=None, weights=None, method='leastsq',
             iter_cb=None, scale_covar=True, verbose=False, fit_kws=None,
-            nan_policy=None, calc_covar=True, max_nfev=None, **kwargs):
+            nan_policy=None, calc_covar=True, max_nfev=None,
+            coerce_farray=True, **kwargs):
         """Fit the model to the data using the supplied Parameters.
 
         Parameters
         ----------
         data : array_like
             Array of data to be fit.
         params : Parameters, optional
@@ -968,14 +989,19 @@
         calc_covar : bool, optional
             Whether to calculate the covariance matrix (default is True)
             for solvers other than `'leastsq'` and `'least_squares'`.
             Requires the ``numdifftools`` package to be installed.
         max_nfev : int or None, optional
             Maximum number of function evaluations (default is None). The
             default value depends on the fitting method.
+        coerce_farray : bool, optional
+            Whether to coerce data and independent data to be ndarrays
+            with dtype of float64 (or complex128).  If set to False, data
+            and independent data are not coerced at all, but the output of
+            the model function will be. (default is True)
         **kwargs : optional
             Arguments to pass to the model function, possibly overriding
             parameters.
 
         Returns
         -------
         ModelResult
@@ -1056,33 +1082,20 @@
 
         # If independent_vars and data are alignable (pandas), align them,
         # and apply the mask from above if there is one.
         for var in self.independent_vars:
             if not np.isscalar(kwargs[var]):
                 kwargs[var] = _align(kwargs[var], mask, data)
 
-        def coerce_arraylike(x):
-            """
-            coerce lists, tuples, and pandas Series to float64 or complex128,
-            but leave other ndarrays of different dtypes and objects unchanged
-            """
-            if isinstance(x, (list, tuple, Series)):
-                if np.isrealobj(x):
-                    return np.asfarray(x)
-                elif np.iscomplexobj(x):
-                    return np.asarray(x, dtype='complex128')
-            return x
-
-        # coerce data and independent variable(s) that are 'array-like' (list,
-        # tuples, pandas Series) to float64/complex128. Note: this will not
-        # alter the dtype of data or independent variables that are already
-        # ndarrays but with dtype other than float64/complex128.
-        data = coerce_arraylike(data)
-        for var in self.independent_vars:
-            kwargs[var] = coerce_arraylike(kwargs[var])
+        if coerce_farray:
+            # coerce data and independent variable(s) that are 'array-like' (list,
+            # tuples, pandas Series) to float64/complex128.
+            data = coerce_arraylike(data)
+            for var in self.independent_vars:
+                kwargs[var] = coerce_arraylike(kwargs[var])
 
         if fit_kws is None:
             fit_kws = {}
 
         output = ModelResult(self, params, method=method, iter_cb=iter_cb,
                              scale_covar=scale_covar, fcn_kws=kwargs,
                              nan_policy=self.nan_policy, calc_covar=calc_covar,
@@ -1199,14 +1212,21 @@
 
     def eval_components(self, **kwargs):
         """Return dictionary of name, results for each component."""
         out = dict(self.left.eval_components(**kwargs))
         out.update(self.right.eval_components(**kwargs))
         return out
 
+    def post_fit(self, fitresult):
+        """function that is called just after fit, can be overloaded by
+        subclasses to add non-fitting 'calculated parameters'
+        """
+        self.left.post_fit(fitresult)
+        self.right.post_fit(fitresult)
+
     @property
     def param_names(self):
         """Return parameter names for composite model."""
         return self.left.param_names + self.right.param_names
 
     @property
     def components(self):
@@ -1441,24 +1461,27 @@
             self.nan_policy = nan_policy
 
         self.ci_out = None
         self.userargs = (self.data, self.weights)
         self.userkws.update(kwargs)
         self.init_fit = self.model.eval(params=self.params, **self.userkws)
         _ret = self.minimize(method=self.method)
+        self.model.post_fit(_ret)
+        _ret.params.create_uvars(covar=_ret.covar)
 
         for attr in dir(_ret):
             if not attr.startswith('_'):
                 try:
                     setattr(self, attr, getattr(_ret, attr))
                 except AttributeError:
                     pass
 
         if self.data is not None and len(self.data) > 1:
-            sstot = ((self.data - self.data.mean())**2).sum()
+            dat = coerce_arraylike(self.data)
+            sstot = ((dat - dat.mean())**2).sum()
             if isinstance(self.residual, np.ndarray) and len(self.residual) > 1:
                 self.rsquared = 1.0 - (self.residual**2).sum()/max(tiny, sstot)
 
         self.init_values = self.model._make_all_args(self.init_params)
         self.best_values = self.model._make_all_args(_ret.params)
         self.best_fit = self.model.eval(params=_ret.params, **self.userkws)
 
@@ -1558,26 +1581,28 @@
         userkws = self.userkws.copy()
         userkws.update(kwargs)
         if params is None:
             params = self.params
 
         nvarys = self.nvarys
         # ensure fjac and df2 are correct size if independent var updated by kwargs
-        ndata = self.model.eval(params, **userkws).size
+        feval = self.model.eval(params, **userkws)
+        ndata = len(feval.view('float64'))        # allows feval to be complex
         covar = self.covar
         if any(p.stderr is None for p in params.values()):
             return np.zeros(ndata)
 
-        fjac = {'0': np.zeros((nvarys, ndata))}  # '0' signify 'Full', an invalid prefix
-        df2 = {'0': np.zeros(ndata)}
+        # '0' would be an invalid prefix, here signifying 'Full'
+        fjac = {'0': np.zeros((nvarys, ndata), dtype='float64')}
+        df2 = {'0': np.zeros(ndata, dtype='float64')}
 
         for comp in self.components:
             label = comp.prefix if len(comp.prefix) > 1 else comp._name
-            fjac[label] = np.zeros((nvarys, ndata))
-            df2[label] = np.zeros(ndata)
+            fjac[label] = np.zeros((nvarys, ndata), dtype='float64')
+            df2[label] = np.zeros(ndata, dtype='float64')
 
         # find derivative by hand!
         pars = params.copy()
         for i in range(nvarys):
             pname = self.var_names[i]
             val0 = pars[pname].value
             dval = pars[pname].stderr/3.0
@@ -1587,27 +1612,34 @@
 
             pars[pname].value = val0 - dval
             res2 = {'0': self.model.eval(pars, **userkws)}
             res2.update(self.model.eval_components(params=pars, **userkws))
 
             pars[pname].value = val0
             for key in fjac:
-                fjac[key][i] = (res1[key] - res2[key]) / (2*dval)
+                fjac[key][i] = (res1[key].view('float64')
+                                - res2[key].view('float64')) / (2*dval)
 
         for i in range(nvarys):
             for j in range(nvarys):
                 for key in fjac:
                     df2[key] += fjac[key][i] * fjac[key][j] * covar[i, j]
 
         if sigma < 1.0:
             prob = sigma
         else:
             prob = erf(sigma/np.sqrt(2))
 
         scale = t.ppf((prob+1)/2.0, self.ndata-nvarys)
+
+        # for complex data, convert back to real/imag pairs
+        if feval.dtype in ('complex64', 'complex128'):
+            for key in fjac:
+                df2[key] = df2[key][0::2] + 1j * df2[key][1::2]
+
         self.dely = scale * np.sqrt(df2.pop('0'))
 
         self.dely_comps = {}
         for key in df2:
             self.dely_comps[key] = scale * np.sqrt(df2[key])
         return self.dely
 
@@ -1689,15 +1721,15 @@
         return f'[[Model]]\n    {modname}\n{report}'
 
     def _repr_html_(self, show_correl=True, min_correl=0.1):
         """Return a HTML representation of parameters data."""
         report = fitreport_html_table(self, show_correl=show_correl,
                                       min_correl=min_correl)
         modname = self.model._reprstring(long=True)
-        return f"<h2> Model</h2> {modname} {report}"
+        return f"<h2>Fit Result</h2> <p>Model: {modname}</p> {report}"
 
     def summary(self):
         """Return a dictionary with statistics and attributes of a ModelResult.
 
         Returns
         -------
         dict
@@ -1881,14 +1913,18 @@
             par = self.init_params.get(parname, None)
             if par is not None:
                 par.correl = par.stderr = None
                 par.value = par.init_value = self.init_values[parname]
         self.init_fit = self.model.eval(self.init_params, **self.userkws)
         self.result = MinimizerResult()
         self.result.params = self.params
+
+        if self.errorbars and self.covar is not None:
+            self.uvars = self.result.params.create_uvars(covar=self.covar)
+
         self.init_vals = list(self.init_values.items())
         return self
 
     def load(self, fp, funcdefs=None, **kws):
         """Load JSON representation of ModelResult from a file-like object.
 
         Parameters
```

### Comparing `lmfit-1.2.1/lmfit/models.py` & `lmfit-1.2.2/lmfit/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,16 +200,16 @@
         def constant(x, re=0., im=0.):
             return (re + 1j*im) * np.ones(np.shape(x))
         super().__init__(constant, **kwargs)
 
     def guess(self, data, x=None, **kwargs):
         """Estimate initial model parameter values from data."""
         pars = self.make_params()
-        pars[f'{self.prefix}re'].set(value=data.real.mean())
-        pars[f'{self.prefix}im'].set(value=data.imag.mean())
+        pars[f'{self.prefix}re'].set(value=np.real(data).mean())
+        pars[f'{self.prefix}im'].set(value=np.imag(data).mean())
         return update_param_vals(pars, self.prefix, **kwargs)
 
     __init__.__doc__ = COMMON_INIT_DOC
     guess.__doc__ = COMMON_GUESS_DOC
 
 
 class LinearModel(Model):
@@ -518,14 +518,21 @@
         self._set_paramhints_prefix()
 
     def _set_paramhints_prefix(self):
         self.set_param_hint('sigma', min=0)
         self.set_param_hint('fwhm', expr=fwhm_expr(self))
         self.set_param_hint('height', expr=height_expr(self))
 
+#     def post_fit(self, result):
+#         addpar = result.params.add
+#         prefix = self.prefix
+#
+#         addpar(name=f'{prefix}fwhm', expr=fwhm_expr(self))
+#         addpar(name=f'{prefix}height', expr=height_expr(self))
+
     def guess(self, data, x, negative=False, **kwargs):
         """Estimate initial model parameter values from data."""
         pars = guess_from_peak(self, data, x, negative)
         return update_param_vals(pars, self.prefix, **kwargs)
 
     __init__.__doc__ = COMMON_INIT_DOC
     guess.__doc__ = COMMON_GUESS_DOC
@@ -571,14 +578,28 @@
         self.set_param_hint('fwhmx', expr=expr.replace('sigma', 'sigmax'))
         self.set_param_hint('fwhmy', expr=expr.replace('sigma', 'sigmay'))
         fmt = ("{factor:.7f}*{prefix:s}amplitude/(max({tiny}, {prefix:s}sigmax)"
                + "*max({tiny}, {prefix:s}sigmay))")
         expr = fmt.format(tiny=tiny, factor=self.height_factor, prefix=self.prefix)
         self.set_param_hint('height', expr=expr)
 
+#     def post_fit(self, result):
+#         addpar = result.params.add
+#         prefix = self.prefix
+#         result.params.add(name=f'{prefix}fwhm', expr=fwhm_expr(self))
+#         result.params.add(name=f'{prefix}height', expr=height_expr(self))
+#
+#         expr = fwhm_expr(self)
+#         addpar('{prefix}fwhmx', expr=expr.replace('sigma', 'sigmax'))
+#         addpar('{prefix}fwhmy', expr=expr.replace('sigma', 'sigmay'))
+#         fmt = ("{factor:.7f}*{prefix:s}amplitude/(max({tiny}, {prefix:s}sigmax)"
+#                + "*max({tiny}, {prefix:s}sigmay))")
+#         expr = fmt.format(tiny=tiny, factor=self.height_factor, prefix=prefix)
+#         addpar(f'{prefix}height', expr=expr)
+
     def guess(self, data, x, y, negative=False, **kwargs):
         """Estimate initial model parameter values from data."""
         pars = guess_from_peak2d(self, data, x, y, negative)
         return update_param_vals(pars, self.prefix, **kwargs)
 
     __init__.__doc__ = COMMON_INIT_DOC.replace("['x']", "['x', 'y']")
     guess.__doc__ = COMMON_GUESS_DOC
@@ -616,14 +637,20 @@
         self._set_paramhints_prefix()
 
     def _set_paramhints_prefix(self):
         self.set_param_hint('sigma', min=0)
         self.set_param_hint('fwhm', expr=fwhm_expr(self))
         self.set_param_hint('height', expr=height_expr(self))
 
+#     def post_fit(self, result):
+#         addpar = result.params.add
+#         prefix = self.prefix
+#         addpar(name=f'{prefix}fwhm', expr=fwhm_expr(self))
+#         addpar(name=f'{prefix}height', expr=height_expr(self))
+
     def guess(self, data, x, negative=False, **kwargs):
         """Estimate initial model parameter values from data."""
         pars = guess_from_peak(self, data, x, negative, ampscale=1.25)
         return update_param_vals(pars, self.prefix, **kwargs)
 
     __init__.__doc__ = COMMON_INIT_DOC
     guess.__doc__ = COMMON_GUESS_DOC
@@ -672,14 +699,22 @@
         fwhm_expr = '{pre:s}sigma+{pre:s}sigma_r'
         height_expr = '2*{pre:s}amplitude/{0:.7f}/max({1:.7f}, ({pre:s}sigma+{pre:s}sigma_r))'
         self.set_param_hint('sigma', min=0)
         self.set_param_hint('sigma_r', min=0)
         self.set_param_hint('fwhm', expr=fwhm_expr.format(pre=self.prefix))
         self.set_param_hint('height', expr=height_expr.format(np.pi, tiny, pre=self.prefix))
 
+#     def post_fit(self, result):
+#         fwhm_expr = '{pre:s}sigma+{pre:s}sigma_r'
+#         height_expr = '2*{pre:s}amplitude/{0:.7f}/max({1:.7f}, ({pre:s}sigma+{pre:s}sigma_r))'
+#         addpar = result.params.add
+#         prefix = self.prefix
+#         addpar(name=f'{prefix}fwhm', expr=fwhm_expr.format(pre=prefix))
+#         addpar(name=f'{prefix}height', expr=height_expr.format(np.pi, tiny, pre=prefix))
+
     def guess(self, data, x, negative=False, **kwargs):
         """Estimate initial model parameter values from data."""
         pars = guess_from_peak(self, data, x, negative, ampscale=1.25)
         sigma = pars[f'{self.prefix}sigma']
         pars[f'{self.prefix}sigma_r'].set(value=sigma.value, min=sigma.min, max=sigma.max)
         return update_param_vals(pars, self.prefix, **kwargs)
 
@@ -728,23 +763,32 @@
                        'independent_vars': independent_vars})
         super().__init__(voigt, **kwargs)
         self._set_paramhints_prefix()
 
     def _set_paramhints_prefix(self):
         self.set_param_hint('sigma', min=0)
         self.set_param_hint('gamma', expr=f'{self.prefix}sigma')
-
         fexpr = ("1.0692*{pre:s}gamma+" +
                  "sqrt(0.8664*{pre:s}gamma**2+5.545083*{pre:s}sigma**2)")
         hexpr = ("({pre:s}amplitude/(max({0}, {pre:s}sigma*sqrt(2*pi))))*"
-                 "wofz((1j*{pre:s}gamma)/(max({0}, {pre:s}sigma*sqrt(2)))).real")
-
+                 "real(wofz((1j*{pre:s}gamma)/(max({0}, {pre:s}sigma*sqrt(2)))))")
         self.set_param_hint('fwhm', expr=fexpr.format(pre=self.prefix))
         self.set_param_hint('height', expr=hexpr.format(tiny, pre=self.prefix))
 
+#     def post_fit(self, result):
+#         fexpr = ("1.0692*{pre:s}gamma+" +
+#                  "sqrt(0.8664*{pre:s}gamma**2+5.545083*{pre:s}sigma**2)")
+#         hexpr = ("({pre:s}amplitude/(max({0}, {pre:s}sigma*sqrt(2*pi))))*"
+#                  "wofz((1j*{pre:s}gamma)/(max({0}, {pre:s}sigma*sqrt(2)))).real")
+#
+#         addpar = result.params.add
+#         prefix = self.prefix
+#         addpar(name=f'{prefix}fwhm', expr=fexpr.format(pre=prefix))
+#         addpar(name=f'{prefix}height', expr=hexpr.format(tiny, pre=prefix))
+
     def guess(self, data, x, negative=False, **kwargs):
         """Estimate initial model parameter values from data."""
         pars = guess_from_peak(self, data, x, negative,
                                ampscale=1.5, sigscale=0.65)
         return update_param_vals(pars, self.prefix, **kwargs)
 
     __init__.__doc__ = COMMON_INIT_DOC
@@ -791,16 +835,28 @@
         self.set_param_hint('sigma', min=0)
         self.set_param_hint('fraction', value=0.5, min=0.0, max=1.0)
         self.set_param_hint('fwhm', expr=fwhm_expr(self))
         fmt = ("(((1-{prefix:s}fraction)*{prefix:s}amplitude)/"
                "max({0}, ({prefix:s}sigma*sqrt(pi/log(2))))+"
                "({prefix:s}fraction*{prefix:s}amplitude)/"
                "max({0}, (pi*{prefix:s}sigma)))")
+
         self.set_param_hint('height', expr=fmt.format(tiny, prefix=self.prefix))
 
+#     def post_fit(self, result):
+#         addpar = result.params.add
+#         prefix = self.prefix
+#         hexpr = ("(((1-{prefix:s}fraction)*{prefix:s}amplitude)/"
+#                  "max({0}, ({prefix:s}sigma*sqrt(pi/log(2))))+"
+#                  "({prefix:s}fraction*{prefix:s}amplitude)/"
+#                  "max({0}, (pi*{prefix:s}sigma)))")
+#
+#         addpar(name=f'{prefix}fwhm', expr=fwhm_expr(self))
+#         addpar(name=f'{prefix}height', expr=hexpr.format(tiny, prefix=prefix))
+
     def guess(self, data, x, negative=False, **kwargs):
         """Estimate initial model parameter values from data."""
         pars = guess_from_peak(self, data, x, negative, ampscale=1.25)
         pars[f'{self.prefix}fraction'].set(value=0.5, min=0.0, max=1.0)
         return update_param_vals(pars, self.prefix, **kwargs)
 
     __init__.__doc__ = COMMON_INIT_DOC
```

### Comparing `lmfit-1.2.1/lmfit/parameter.py` & `lmfit-1.2.2/lmfit/parameter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,68 @@
 """Parameter class."""
 
 from copy import deepcopy
 import json
 
 from asteval import Interpreter, get_ast_names, valid_symbol_name
 from numpy import arcsin, array, cos, inf, isclose, sin, sqrt
+from scipy.linalg import LinAlgError
 import scipy.special
+from uncertainties import correlated_values, ufloat
+from uncertainties import wrap as uwrap
 
 from .jsonutils import decode4js, encode4js
 from .lineshapes import tiny
 from .printfuncs import params_html_table
 
-SCIPY_FUNCTIONS = {'gamfcn': scipy.special.gamma, 'loggammafcn': scipy.special.loggamma, 'betalnfnc': scipy.special.betaln}
+SCIPY_FUNCTIONS = {'gamfcn': scipy.special.gamma,
+                   'loggammafcn': scipy.special.loggamma,
+                   'betalnfnc': scipy.special.betaln}
 for fnc_name in ('erf', 'erfc', 'wofz'):
     SCIPY_FUNCTIONS[fnc_name] = getattr(scipy.special, fnc_name)
 
 
 def check_ast_errors(expr_eval):
     """Check for errors derived from asteval."""
     if len(expr_eval.error) > 0:
         expr_eval.raise_exception(None)
 
 
+def asteval_with_uncertainties(*vals, obj=None, pars=None, names=None, **kwargs):
+    """Calculate object value, given values for variables.
+
+    This is used by the uncertainties package to calculate the
+    uncertainty in an object even with a complicated expression.
+    """
+    _asteval = getattr(pars, '_asteval', None)
+    if obj is None or pars is None or names is None or _asteval is None:
+        return 0
+    for val, name in zip(vals, names):
+        _asteval.symtable[name] = val
+
+    # re-evaluate constraint parameters topropagate uncertainties
+    [p._getval() for p in pars.values()]
+    return _asteval.eval(obj._expr_ast)
+
+
 class Parameters(dict):
     """A dictionary of Parameter objects.
 
     It should contain all Parameter objects that are required to specify
     a fit model. All minimization and Model fitting routines in lmfit will
     use exactly one Parameters object, typically given as the first
     argument to the objective function.
 
     All keys of a Parameters() instance must be strings and valid Python
     symbol names, so that the name must match ``[a-z_][a-z0-9_]*`` and
     cannot be a Python reserved word.
 
     All values of a Parameters() instance must be Parameter objects.
 
-    A Parameters() instance includes an `asteval` Interpreter used for
+    A Parameters(xs) instance includes an `asteval` Interpreter used for
     evaluation of constrained Parameters.
 
     Parameters() support copying and pickling, and have methods to convert
     to and from serializations using json strings.
 
     """
 
@@ -274,22 +296,19 @@
                      columns=['value', 'min', 'max', 'stderr', 'vary', 'expr',
                               'brute_step']):
         """Pretty-print of parameters data.
 
         Parameters
         ----------
         oneline : bool, optional
-            If True prints a one-line parameters representation (default
-            is False).
+            If True prints a one-line parameters representation [False]
         colwidth : int, optional
-            Column width for all columns specified in `columns` (default
-            is 8).
+            Column width for all columns specified in `columns` [8]
         precision : int, optional
-            Number of digits to be printed after floating point (default
-            is 4).
+            Number of digits to be printed after floating point [4]
         fmt : {'g', 'e', 'f'}, optional
             Single-character numeric formatter. Valid values are: `'g'`
             floating point and exponential (default), `'e'` exponential,
             or `'f'` floating point.
         columns : :obj:`list` of :obj:`str`, optional
             List of :class:`Parameter` attribute names to print (default
             is to show all attributes).
@@ -460,14 +479,75 @@
         dict
             A dictionary of :attr:`name`::attr:`value` pairs for each
             Parameter.
 
         """
         return {p.name: p.value for p in self.values()}
 
+    def create_uvars(self, covar=None):
+        """Return a dict of uncertainties ufloats from the current Parameter
+        values and stderr, and an optionally-supplied covariance matrix.
+        Uncertainties in Parameters with constraint expressions will be
+        calculated, propagating uncertaintes (and including correlations)
+
+        Parameters
+        ----------
+        covar : optional
+              Nvar x Nvar covariance matrix from fit
+
+        Returns
+        -------
+        dict with keys of Parameter names and values of uncertainties.ufloats.
+
+        Notes
+        -----
+        1.  if covar is provide, it must correspond to the existing *variable*
+            Parameters.  If covar is given, the returned uncertainties ufloats
+            will take the correlations into account when combining values.
+        2.  See the uncertainties package documentation
+            (https://pythonhosted.org/uncertainties) for more details.
+        """
+        uvars = {}
+        has_expr = False
+        vnames, vbest, vindex = [], [], -1
+        for par in self.values():
+            has_expr = has_expr or par.expr is not None
+            if par.vary:
+                vindex += 1
+                vnames.append(par.name)
+                vbest.append(par.value)
+                if getattr(par, 'sdterr', None) is None and covar is not None:
+                    par.stderr = sqrt(covar[vindex, vindex])
+            uvars[par.name] = ufloat(par.value, getattr(par, 'sdterr', 0.0))
+
+        corr_uvars = None
+        if covar is not None:
+            try:
+                corr_uvars = correlated_values(vbest, covar)
+                for name, cuv in zip(vnames, corr_uvars):
+                    uvars[name] = cuv
+            except (LinAlgError, ValueError):
+                pass
+
+        if has_expr and corr_uvars is not None:
+            # for uncertainties on constrained parameters, use the calculated
+            # correlated values, evaluate the uncertainties on the constrained
+            # parameters and reset the Parameters to best-fit value
+            wrap_ueval = uwrap(asteval_with_uncertainties)
+            for par in self.values():
+                if getattr(par, '_expr_ast', None) is not None:
+                    try:
+                        uval = wrap_ueval(*corr_uvars, obj=par,
+                                          pars=self, names=vnames)
+                        par.stderr = uval.std_dev
+                        uvars[par.name] = uval
+                    except Exception:
+                        par.stderr = 0
+        return uvars
+
     def dumps(self, **kws):
         """Represent Parameters as a JSON string.
 
         Parameters
         ----------
         **kws : optional
             Keyword arguments that are passed to `json.dumps`.
```

### Comparing `lmfit-1.2.1/lmfit/printfuncs.py` & `lmfit-1.2.2/lmfit/printfuncs.py`

 * *Files 3% similar despite different names*

```diff
@@ -220,14 +220,34 @@
             maxlen = max(len(k) for k in list(correls.keys()))
         for name, val in sort_correl:
             lspace = max(0, maxlen - len(name))
             add(f"    C({name}){(' '*30)[:lspace]} = {val:+.4f}")
     return '\n'.join(buff)
 
 
+def lcol(s, cat='td'):
+    "html left column"
+    return f"<{cat} style='text-align:left'>{s}</{cat}>"
+
+
+def rcol(s, cat='td'):
+    "html right column"
+    return f"<{cat} style='text-align:right'>{s}</{cat}>"
+
+
+def trow(columns, cat='td'):
+    "html row"
+    nlast = len(columns)-1
+    rows = []
+    for i, col in enumerate(columns):
+        cform = rcol if i == nlast else lcol
+        rows.append(cform(col, cat=cat))
+    return rows
+
+
 def fitreport_html_table(result, show_correl=True, min_correl=0.1):
     """Generate a report of the fitting result as an HTML table.
 
     Parameters
     ----------
     result : MinimizerResult or ModelResult
         Object containing the optimized parameters and several
@@ -242,31 +262,34 @@
     str
         Multi-line HTML code of fit report.
 
     """
     html = []
     add = html.append
 
-    def stat_row(label, val, val2=''):
-        add(f'<tr><td>{label}</td><td>{val}</td><td>{val2}</td></tr>')
+    def stat_row(label, val, val2=None, cat='td'):
+        if val2 is None:
+            rows = trow([label, val], cat=cat)
+        else:
+            rows = trow([label, val, val2], cat=cat)
+        add(f"<tr>{''.join(rows)}</tr>")
 
-    add('<h2>Fit Statistics</h2>')
-    add('<table>')
+    add('<table class="jp-toc-ignore">')
+    add('<caption class="jp-toc-ignore">Fit Statistics</caption>')
     stat_row('fitting method', result.method)
     stat_row('# function evals', result.nfev)
     stat_row('# data points', result.ndata)
     stat_row('# variables', result.nvarys)
     stat_row('chi-square', gformat(result.chisqr))
     stat_row('reduced chi-square', gformat(result.redchi))
     stat_row('Akaike info crit.', gformat(result.aic))
     stat_row('Bayesian info crit.', gformat(result.bic))
     if hasattr(result, 'rsquared'):
         stat_row('R-squared', gformat(result.rsquared))
     add('</table>')
-    add('<h2>Variables</h2>')
     add(params_html_table(result.params))
     if show_correl:
         correls = []
         parnames = list(result.params.keys())
         for i, name in enumerate(result.params):
             par = result.params[name]
             if not par.vary:
@@ -275,17 +298,18 @@
                 for name2 in parnames[i+1:]:
                     if (name != name2 and name2 in par.correl and
                             abs(par.correl[name2]) > min_correl):
                         correls.append((name, name2, par.correl[name2]))
         if len(correls) > 0:
             sort_correls = sorted(correls, key=lambda val: abs(val[2]))
             sort_correls.reverse()
-            extra = f'(unreported correlations are < {min_correl:.3f})'
-            add(f'<h2>Correlations {extra}</h2>')
-            add('<table>')
+            extra = f'(unreported values are < {min_correl:.3f})'
+            add('<table class="jp-toc-ignore">')
+            add(f'<caption>Correlations {extra}</caption>')
+            stat_row('Parameter1', 'Parameter 2', 'Correlation', cat='th')
             for name1, name2, val in sort_correls:
                 stat_row(name1, name2, f"{val:+.4f}")
             add('</table>')
     return ''.join(html)
 
 
 def correl_table(params):
@@ -341,29 +365,26 @@
     has_err = any(p.stderr is not None for p in params.values())
     has_expr = any(p.expr is not None for p in params.values())
     has_brute = any(p.brute_step is not None for p in params.values())
 
     html = []
     add = html.append
 
-    def cell(x, cat='td'):
-        return add(f'<{cat}> {x} </{cat}>')
-
-    add('<table><tr>')
+    add('<table class="jp-toc-ignore"><caption>Parameters</caption>')
     headers = ['name', 'value']
     if has_err:
         headers.extend(['standard error', 'relative error'])
     headers.extend(['initial value', 'min', 'max', 'vary'])
     if has_expr:
         headers.append('expression')
     if has_brute:
         headers.append('brute step')
-    for h in headers:
-        cell(h, cat='th')
-    add('</tr>')
+
+    hrow = trow(headers, cat='th')
+    add(f"<tr>{''.join(hrow)}</tr>")
 
     for par in params.values():
         rows = [par.name, gformat(par.value)]
         if has_err:
             serr = ''
             spercent = ''
             if par.stderr is not None:
@@ -382,18 +403,16 @@
             rows.append(expr)
         if has_brute:
             brute_step = 'None'
             if par.brute_step is not None:
                 brute_step = gformat(par.brute_step)
             rows.append(brute_step)
 
-        add('<tr>')
-        for r in rows:
-            cell(r)
-        add('</tr>')
+        hrow = trow(rows, cat='td')
+        add(f"<tr>{''.join(hrow)}</tr>")
     add('</table>')
     return ''.join(html)
 
 
 def report_fit(params, **kws):
     """Print a report of the fitting results."""
     print(fit_report(params, **kws))
```

### Comparing `lmfit-1.2.1/lmfit.egg-info/PKG-INFO` & `lmfit-1.2.2/lmfit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmfit
-Version: 1.2.1
+Version: 1.2.2
 Summary: Least-Squares Minimization with Bounds and Constraints
 Home-page: https://lmfit.github.io//lmfit-py/
 Author: LMFit Development Team
 Author-email: matt.newville@gmail.com
 License: BSD 3-Clause
 Project-URL: Source, https://github.com/lmfit/lmfit-py
 Project-URL: Changelog, https://lmfit.github.io/lmfit-py/whatsnew.html
```

### Comparing `lmfit-1.2.1/lmfit.egg-info/SOURCES.txt` & `lmfit-1.2.2/lmfit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 doc/builtin_models.rst
 doc/conf.py
 doc/confidence.rst
 doc/constraints.rst
 doc/contents.rst
 doc/doc_examples_to_gallery.py
 doc/faq.rst
+doc/filter_spurious_link_from_html.py
 doc/fitting.rst
 doc/index.rst
 doc/installation.rst
 doc/intro.rst
 doc/make.bat
 doc/model.rst
 doc/parameters.rst
@@ -102,14 +103,15 @@
 examples/doc_model_two_components.py
 examples/doc_model_uncertainty.py
 examples/doc_model_uncertainty2.py
 examples/doc_model_with_iter_callback.py
 examples/doc_model_with_nan_policy.py
 examples/doc_parameters_basic.py
 examples/doc_parameters_valuesdict.py
+examples/doc_uvars_params.py
 examples/example_Model_interface.py
 examples/example_brute.py
 examples/example_complex_resonator_model.py
 examples/example_confidence_interval.py
 examples/example_detect_outliers.py
 examples/example_diffev.py
 examples/example_emcee_Model_interface.py
@@ -177,10 +179,11 @@
 tests/test_model_uncertainties.py
 tests/test_models.py
 tests/test_multidatasets.py
 tests/test_nose.py
 tests/test_pandas.py
 tests/test_parameter.py
 tests/test_parameters.py
+tests/test_params_uvars.py
 tests/test_printfuncs.py
 tests/test_shgo.py
 tests/test_stepmodel.py
```

### Comparing `lmfit-1.2.1/lmfit.egg-info/requires.txt` & `lmfit-1.2.2/lmfit.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/publish_docs.sh` & `lmfit-1.2.2/publish_docs.sh`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/setup.cfg` & `lmfit-1.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/NISTModels.py` & `lmfit-1.2.2/tests/NISTModels.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/conftest.py` & `lmfit-1.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/gauss_modelresult_lmfit100.sav` & `lmfit-1.2.2/tests/gauss_modelresult_lmfit100.sav`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_1variable.py` & `lmfit-1.2.2/tests/test_1variable.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_NIST_Strd.py` & `lmfit-1.2.2/tests/test_NIST_Strd.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_algebraic_constraint.py` & `lmfit-1.2.2/tests/test_algebraic_constraint.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,18 +74,20 @@
     assert pfit['cen_l'].value == 1.5 + pfit['cen_g'].value
     assert pfit['amp_l'].value == pfit['amp_tot'].value - pfit['amp_g'].value
     assert pfit['wid_l'].value == 2.5 * pfit['wid_g'].value
 
 
 def test_constraints_function_call():
     """Test a constraint with simple function call in Model class."""
-    x = [1723, 1773, 1823, 1523, 1773, 1033.03078, 1042.98077, 1047.90937,
-         1053.95899, 1057.94906, 1063.13788, 1075.74218, 1086.03102]
-    y = [0.79934, -0.31876, -0.46852, 0.05, -0.21, 11.1708, 10.31844, 9.73069,
-         9.21319, 9.12457, 9.05243, 8.66407, 8.29664]
+
+    x = np.array([1723, 1773, 1823, 1523, 1773, 1033.03078, 1042.98077,
+                  1047.90937, 1053.95899, 1057.94906, 1063.13788, 1075.74218,
+                  1086.03102])
+    y = np.array([0.79934, -0.31876, -0.46852, 0.05, -0.21, 11.1708, 10.31844,
+                  9.73069, 9.21319, 9.12457, 9.05243, 8.66407, 8.29664])
 
     def VFT(T, ninf=-3, A=5e3, T0=800):
         return ninf + A/(T-T0)
 
     vftModel = Model(VFT)
     vftModel.set_param_hint('D', vary=False, expr=r'A*log(10)/T0')
     result = vftModel.fit(y, T=x)
```

### Comparing `lmfit-1.2.1/tests/test_ampgo.py` & `lmfit-1.2.2/tests/test_ampgo.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_basicfit.py` & `lmfit-1.2.2/tests/test_basicfit.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_basinhopping.py` & `lmfit-1.2.2/tests/test_basinhopping.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_bounded_jacobian.py` & `lmfit-1.2.2/tests/test_bounded_jacobian.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_bounds.py` & `lmfit-1.2.2/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_brute.py` & `lmfit-1.2.2/tests/test_brute.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_builtin_models.py` & `lmfit-1.2.2/tests/test_builtin_models.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_confidence.py` & `lmfit-1.2.2/tests/test_confidence.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_covariance_matrix.py` & `lmfit-1.2.2/tests/test_covariance_matrix.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_custom_independentvar.py` & `lmfit-1.2.2/tests/test_custom_independentvar.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_default_kws.py` & `lmfit-1.2.2/tests/test_default_kws.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_dual_annealing.py` & `lmfit-1.2.2/tests/test_dual_annealing.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_itercb.py` & `lmfit-1.2.2/tests/test_itercb.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,26 +62,23 @@
     assert not out.success
 
 
 @pytest.mark.parametrize("calc_covar", calc_covar_options)
 @pytest.mark.parametrize("method", fitmethods)
 def test_itercb_minimizer_class(method, calc_covar):
     """Test the iteration callback for all solvers."""
-    if method in ('nelder', 'differential_evolution'):
-        pytest.xfail("scalar_minimizers behave differently, but shouldn't!!")
-
     mini = Minimizer(residual, pars, fcn_args=(x, y), iter_cb=per_iteration,
                      calc_covar=calc_covar)
     out = mini.minimize(method=method)
-
     assert out.nfev == 17
     assert out.aborted
     assert not out.errorbars
     assert not out.success
-    assert mini._abort
+    if method not in ('nelder', 'differential_evolution'):
+        assert mini._abort
 
 
 fitmethods = ['leastsq', 'least_squares']
 
 
 @pytest.mark.parametrize("method", fitmethods)
 def test_itercb_reset_abort(method):
```

### Comparing `lmfit-1.2.1/tests/test_jsonutils.py` & `lmfit-1.2.2/tests/test_jsonutils.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_least_squares.py` & `lmfit-1.2.2/tests/test_least_squares.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_lineshapes.py` & `lmfit-1.2.2/tests/test_lineshapes.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 
 import lmfit
 from lmfit.lineshapes import not_zero, tiny
 
 
 @pytest.mark.parametrize(
     "value, expected_result",
-    [(1, 1.0), (-1, -1.0), (0, tiny), (-0, -tiny), (np.array([1]), 1.0)],
-)
+    [(1, 1.0), (-1, -1.0), (0, tiny), (-0, -tiny)])
 def test_not_zero(value, expected_result):
     """Test that not_zero gives the expected results"""
     assert_almost_equal(not_zero(value), expected_result)
 
 
 @pytest.mark.parametrize("lineshape", lmfit.lineshapes.functions)
 def test_no_ZeroDivisionError_and_finite_output(lineshape):
```

### Comparing `lmfit-1.2.1/tests/test_manypeaks_speed.py` & `lmfit-1.2.2/tests/test_manypeaks_speed.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_max_nfev.py` & `lmfit-1.2.2/tests/test_max_nfev.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_model.py` & `lmfit-1.2.2/tests/test_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Tests for the Model, CompositeModel, and ModelResult classes."""
 
 import functools
 import unittest
 import warnings
 
 import numpy as np
-from numpy.testing import assert_allclose
+from numpy.testing import assert_allclose, assert_almost_equal
 import pytest
 from scipy import __version__ as scipy_version
 
 import lmfit
-from lmfit import Model, models
+from lmfit import Model, Parameters, models
 from lmfit.lineshapes import gaussian, lorentzian
 from lmfit.model import get_reducer, propagate_err
-from lmfit.models import PseudoVoigtModel
+from lmfit.models import GaussianModel, PseudoVoigtModel
 
 
 @pytest.fixture()
 def gmodel():
     """Return a Gaussian model."""
     return Model(gaussian)
 
@@ -335,14 +335,44 @@
     assert mod._func_haskeywords is False
     assert mod.independent_vars == ['a']
 
     assert isinstance(mod.def_vals, dict)
     assert_allclose(mod.def_vals['c'], 10)
 
 
+def test_make_params_withprefixs():
+    # tests Github Issue #893
+    gmod1 = GaussianModel(prefix='p1_')
+    gmod2 = GaussianModel(prefix='p2_')
+
+    model = gmod1 + gmod2
+
+    pars_1a = gmod1.make_params(p1_amplitude=10, p1_center=600, p1_sigma=3)
+    pars_1b = gmod1.make_params(amplitude=10, center=600, sigma=3)
+
+    pars_2a = gmod2.make_params(p2_amplitude=30, p2_center=730, p2_sigma=4)
+    pars_2b = gmod2.make_params(amplitude=30, center=730, sigma=4)
+
+    pars_a = Parameters()
+    pars_a.update(pars_1a)
+    pars_a.update(pars_2a)
+
+    pars_b = Parameters()
+    pars_b.update(pars_1b)
+    pars_b.update(pars_2b)
+
+    pars_c = model.make_params()
+
+    for pname in ('p1_amplitude', 'p1_center', 'p1_sigma',
+                  'p2_amplitude', 'p2_center', 'p2_sigma'):
+        assert pname in pars_a
+        assert pname in pars_b
+        assert pname in pars_c
+
+
 def test__parse_params_forbidden_variable_names():
     """Tests for _parse_params function using invalid variable names."""
 
     def func_invalid_var(data, a):
         pass
 
     def func_invalid_par(a, weights):
@@ -353,53 +383,86 @@
         Model(func_invalid_var)
 
     msg = r"Invalid parameter name \('weights'\) for function func_invalid_par"
     with pytest.raises(ValueError, match=msg):
         Model(func_invalid_par)
 
 
-input_dtypes = [(np.int32, np.int32), (np.float32, np.float32),
-                (np.complex64, np.complex64), ('list', np.float64),
-                ('tuple', np.float64), ('pandas-real', np.float64),
-                ('pandas-complex', np.complex128)]
+@pytest.mark.parametrize('input_dtype', (np.int16, np.int32, np.float32,
+                                         np.complex64, np.complex128, 'list',
+                                         'tuple', 'pandas-real',
+                                         'pandas-complex'))
+def test_coercion_of_input_data(peakdata, input_dtype):
+    """Test for coercion of 'data' and 'independent_vars'.
 
+    'data' and `independent_vars` should be coerced to 'float64' or 'complex128'
 
-@pytest.mark.parametrize('input_dtype, expected_dtype', input_dtypes)
-def test_coercion_of_input_data(peakdata, input_dtype, expected_dtype):
-    """Test for coercion of 'data' and 'independent_vars'.
+    unless told not be coerced by setting ``coerce_farray=False``.
 
-    - 'data' should become 'float64' or 'complex128'
-    - dtype for 'indepdendent_vars' is only changed when the input is a list,
-        tuple, numpy.ndarray, or pandas.Series
+    # - dtype for 'indepdendent_vars' is only changed when the input is a list,
+    #    tuple, numpy.ndarray, or pandas.Series
 
     """
     x, y = peakdata
-    model = lmfit.Model(gaussian)
-    pars = model.make_params()
 
-    if (not lmfit.minimizer.HAS_PANDAS and input_dtype in ['pandas-real',
-                                                           'pandas-complex']):
-        return
-
-    elif input_dtype == 'pandas-real':
-        result = model.fit(lmfit.model.Series(y, dtype=np.float32), pars,
-                           x=lmfit.model.Series(x, dtype=np.float32))
-    elif input_dtype == 'pandas-complex':
-        result = model.fit(lmfit.model.Series(y, dtype=np.complex64), pars,
-                           x=lmfit.model.Series(x, dtype=np.complex64))
-    elif input_dtype == 'list':
-        result = model.fit(y.tolist(), pars, x=x.tolist())
-    elif input_dtype == 'tuple':
-        result = model.fit(tuple(y), pars, x=tuple(x))
-    else:
-        result = model.fit(np.asarray(y, dtype=input_dtype), pars,
-                           x=np.asarray(x, dtype=input_dtype))
+    def gaussian_lists(x, amplitude=1.0, center=0.0, sigma=1.0):
+        xarr = np.array(x, dtype=np.float64)
+        return ((amplitude/(max(1.e-15, np.sqrt(2*np.pi)*sigma)))
+                * np.exp(-(xarr-center)**2 / max(1.e-15, (2*sigma**2))))
+
+    for coerce_farray in True, False:
+        if (input_dtype in ('pandas-real', 'pandas-complex')
+           and not lmfit.minimizer.HAS_PANDAS):
+            return
+
+        if not coerce_farray and input_dtype in ('list', 'tuple'):
+            model = lmfit.Model(gaussian_lists)
+        else:
+            model = lmfit.Model(gaussian)
+
+        pars = model.make_params(amplitude=5, center=10, sigma=2)
+
+        if input_dtype == 'pandas-real':
+            result = model.fit(lmfit.model.Series(y, dtype=np.float32), pars,
+                               x=lmfit.model.Series(x, dtype=np.float32),
+                               coerce_farray=coerce_farray)
+
+            expected_dtype = np.float64 if coerce_farray else np.float32
+
+        elif input_dtype == 'pandas-complex':
+            result = model.fit(lmfit.model.Series(y, dtype=np.complex64), pars,
+                               x=lmfit.model.Series(x, dtype=np.complex64),
+                               coerce_farray=coerce_farray)
+            expected_dtype = np.complex128 if coerce_farray else np.complex64
+
+        elif input_dtype == 'list':
+            result = model.fit(y.tolist(), pars, x=x.tolist(),
+                               coerce_farray=coerce_farray)
+            expected_dtype = np.float64 if coerce_farray else list
+
+        elif input_dtype == 'tuple':
+            result = model.fit(tuple(y), pars, x=tuple(x),
+                               coerce_farray=coerce_farray)
+            expected_dtype = np.float64 if coerce_farray else tuple
 
-    assert result.__dict__['userkws']['x'].dtype == expected_dtype
-    assert result.__dict__['userargs'][0].dtype == expected_dtype
+        else:
+            result = model.fit(np.asarray(y, dtype=input_dtype), pars,
+                               x=np.asarray(x, dtype=input_dtype),
+                               coerce_farray=coerce_farray)
+            expected_dtype = np.float64
+            if input_dtype in (np.complex64, np.complex128):
+                expected_dtype = np.complex128
+            expected_dtype = expected_dtype if coerce_farray else input_dtype
+
+        if not coerce_farray and input_dtype in ('list', 'tuple'):
+            assert isinstance(result.userkws['x'], (list, tuple))
+            assert isinstance(result.userargs[0], (list, tuple))
+        else:
+            assert result.userkws['x'].dtype == expected_dtype
+            assert result.userargs[0].dtype == expected_dtype
 
 
 def test_figure_default_title(peakdata):
     """Test default figure title."""
     pytest.importorskip('matplotlib')
 
     x, y = peakdata
@@ -1073,15 +1136,15 @@
 
         m2 = models.GaussianModel(prefix='m2_')
         params.update(m2.make_params())
 
         _m = m1 + m2  # noqa: F841
 
         param_values = {name: p.value for name, p in params.items()}
-        self.assertTrue(param_values['m1_intercept'] < -0.0)
+        assert_almost_equal(param_values['m1_intercept'], 0.)
         self.assertEqual(param_values['m2_amplitude'], 1)
 
     def test_weird_param_hints(self):
         # tests Github Issue 312, a very weird way to access param_hints
         def func(x, amp):
             return amp*x
 
@@ -1429,7 +1492,46 @@
         pars = mod.make_params(amplitude='a string', frequency=2, shift=7)
 
     with pytest.raises(TypeError):
         pars = mod.make_params(amplitude={'v': 3}, frequency=2, shift=7)
 
     with pytest.raises(TypeError):
         pars = mod.make_params(amplitude={}, frequency=2, shift=7)
+
+
+def test_complex_model_eval_uncertainty():
+    """Github #900"""
+    def cmplx(f, omega, areal, aimag, off, sigma):
+        return (areal*np.cos(f*omega + off) + 1j*aimag*np.sin(f*omega + off))*np.exp(-f/sigma)
+
+    f = np.linspace(0, 10, 501)
+    dat = cmplx(f, 4, 10, 5, 0.2, 4.5) + (0.1 + 0.2j)*np.random.normal(scale=0.25, size=len(f))
+    mod = Model(cmplx)
+    params = mod.make_params(omega=5, areal=5, aimag=5,
+                             off={'value': 0.5, 'min': -2, 'max': 2},
+                             sigma={'value': 3, 'min': 1.e-5, 'max': 1000})
+
+    result = mod.fit(dat, params=params, f=f)
+    dfit = result.eval_uncertainty()
+    assert len(dfit) == len(f)
+    assert dfit.dtype == 'complex128'
+
+
+def test_compositemodel_returning_list():
+    """Github #875"""
+    def lin1(x, k):
+        return [k*x1 for x1 in x]
+
+    def lin2(x, k):
+        return [k*x1 for x1 in x]
+
+    y = np.linspace(0, 100, 100)
+    x = np.linspace(0, 100, 100)
+
+    Model1 = Model(lin1, independent_vars=["x"], prefix="m1_")
+    Model2 = Model(lin2, independent_vars=["x"], prefix="m2_")
+    ModelSum = Model1 + Model2
+    pars = Parameters()
+    pars.add('m1_k', value=0.5)
+    pars.add('m2_k', value=0.5)
+    result = ModelSum.fit(y, pars, x=x)
+    assert len(result.best_fit) == len(x)
```

### Comparing `lmfit-1.2.1/tests/test_model_saveload.py` & `lmfit-1.2.2/tests/test_model_saveload.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_model_uncertainties.py` & `lmfit-1.2.2/tests/test_model_uncertainties.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_models.py` & `lmfit-1.2.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_multidatasets.py` & `lmfit-1.2.2/tests/test_multidatasets.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_nose.py` & `lmfit-1.2.2/tests/test_nose.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pytest
 from scipy.optimize import rosen_der
 from uncertainties import ufloat
 
 from lmfit import Minimizer, Parameters, minimize
 from lmfit.lineshapes import gaussian
 from lmfit.minimizer import (HAS_EMCEE, SCALAR_METHODS, MinimizerResult,
-                             _nan_policy)
+                             coerce_float64)
 from lmfit.models import SineModel
 
 try:
     import numdifftools  # noqa: F401
     HAS_NUMDIFFTOOLS = True
 except ImportError:
     HAS_NUMDIFFTOOLS = False
@@ -415,15 +415,15 @@
         out = self.mini.scalar_minimize(method=self.minimizer)
 
         self.residual(out.params, self.x)
 
         for para, true_para in zip(out.params.values(), self.p_true.values()):
             check_wo_stderr(para, true_para.value, sig=sig)
 
-    def test_nan_policy(self):
+    def test_coerce_float64(self):
         # check that an error is raised if there are nan in
         # the data returned by userfcn
         self.data[0] = np.nan
 
         for method in SCALAR_METHODS:
             if method == 'cobyla' and sys.platform == 'darwin':
                 pytest.xfail("this aborts Python on macOS...")
@@ -440,25 +440,25 @@
         self.mini.nan_policy = 'omit'
         res = self.mini.minimize()
         assert_equal(res.ndata, np.size(self.data, 0) - 1)
 
         for para, true_para in zip(res.params.values(), self.p_true.values()):
             check_wo_stderr(para, true_para.value, sig=0.15)
 
-    def test_nan_policy_function(self):
+    def test_coerce_float64_function(self):
         a = np.array([0, 1, 2, 3, np.nan])
-        pytest.raises(ValueError, _nan_policy, a)
-        assert np.isnan(_nan_policy(a, nan_policy='propagate')[-1])
-        assert_equal(_nan_policy(a, nan_policy='omit'), [0, 1, 2, 3])
+        pytest.raises(ValueError, coerce_float64, a)
+        assert np.isnan(coerce_float64(a, nan_policy='propagate')[-1])
+        assert_equal(coerce_float64(a, nan_policy='omit'), [0, 1, 2, 3])
 
         a[-1] = np.inf
-        pytest.raises(ValueError, _nan_policy, a)
-        assert np.isposinf(_nan_policy(a, nan_policy='propagate')[-1])
-        assert_equal(_nan_policy(a, nan_policy='omit'), [0, 1, 2, 3])
-        assert_equal(_nan_policy(a, handle_inf=False), a)
+        pytest.raises(ValueError, coerce_float64, a)
+        assert np.isposinf(coerce_float64(a, nan_policy='propagate')[-1])
+        assert_equal(coerce_float64(a, nan_policy='omit'), [0, 1, 2, 3])
+        assert_equal(coerce_float64(a, handle_inf=False), a)
 
     def test_emcee(self):
         # test emcee
         if not HAS_EMCEE:
             return True
 
         np.random.seed(123456)
```

### Comparing `lmfit-1.2.1/tests/test_pandas.py` & `lmfit-1.2.2/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_parameter.py` & `lmfit-1.2.2/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.1/tests/test_parameters.py` & `lmfit-1.2.2/tests/test_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,15 +379,15 @@
 
 def test_parameters__repr_html_(parameters):
     """Test _repr_html method to generate HTML table for Parameters class."""
     pars, _, _ = parameters
     repr_html = pars._repr_html_()
 
     assert isinstance(repr_html, str)
-    assert '<table><tr><th> name </th><th> value </th>' in repr_html
+    assert '<table class="jp-toc-ignore"><caption>Parameters</caption>' in repr_html
 
 
 def test_parameters_add():
     """Tests for adding a Parameter to the Parameters class."""
     pars = lmfit.Parameters()
     pars_from_par = lmfit.Parameters()
```

### Comparing `lmfit-1.2.1/tests/test_printfuncs.py` & `lmfit-1.2.2/tests/test_printfuncs.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,17 +138,16 @@
     assert len(html_params) > 500
     assert 'brute' in html_params
     assert 'standard error' in html_params
     assert 'relative error' in html_params
 
     html_report = fitresult._repr_html_()
     assert len(html_report) > 1000
-    for header in report_headers:
-        header_title = header.replace('[', '').replace(']', '').strip()
-        assert header_title in html_report
+    for header in ('Model', 'Fit Statistics', 'Parameters', 'Correlations'):
+        assert header in html_report
 
 
 def test_fitreports_init_values(fitresult):
     """Verify that initial values are displayed as expected."""
     fitresult.params['sigma'].init_value = None
     report_split = fitresult.fit_report().split('\n')
     indx = [i for i, val in enumerate(report_split) if 'sigma' in val][0]
```

### Comparing `lmfit-1.2.1/tests/test_shgo.py` & `lmfit-1.2.2/tests/test_shgo.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,21 +24,14 @@
 
 def test_shgo_scipy_vs_lmfit():
     """Test SHGO algorithm in lmfit versus SciPy."""
     bounds = [(-512, 512), (-512, 512)]
     result_scipy = scipy.optimize.shgo(eggholder, bounds, n=30,
                                        sampling_method='sobol')
 
-    # in SciPy v1.7.0: "sobol was fixed and is now using scipy.stats.qmc.Sobol"
-    # FIXME: clean this up after we require SciPy >= 1.7.0
-    if int(scipy_version.split('.')[1]) < 7:
-        assert len(result_scipy.xl) == 13
-    else:
-        assert len(result_scipy.xl) == 6
-
     pars = lmfit.Parameters()
     pars.add_many(('x0', 0, True, -512, 512), ('x1', 0, True, -512, 512))
     mini = lmfit.Minimizer(eggholder_lmfit, pars)
     result = mini.minimize(method='shgo', n=30, sampling_method='sobol')
     out_x = np.array([result.params['x0'].value, result.params['x1'].value])
 
     assert_allclose(result_scipy.fun, result.residual)
@@ -49,21 +42,14 @@
 
 def test_shgo_scipy_vs_lmfit_2():
     """Test SHGO algorithm in lmfit versus SciPy."""
     bounds = [(-512, 512), (-512, 512)]
     result_scipy = scipy.optimize.shgo(eggholder, bounds, n=60, iters=5,
                                        sampling_method='sobol')
 
-    # in SciPy v1.7.0: "sobol was fixed and is now using scipy.stats.qmc.Sobol"
-    # FIXME: clean this up after we require SciPy >= 1.7.0
-    if int(scipy_version.split('.')[1]) < 7:
-        assert len(result_scipy.xl) == 39
-    else:
-        assert len(result_scipy.xl) == 74
-
     pars = lmfit.Parameters()
     pars.add_many(('x0', 0, True, -512, 512), ('x1', 0, True, -512, 512))
     mini = lmfit.Minimizer(eggholder_lmfit, pars)
     result = mini.minimize(method='shgo', n=60, iters=5,
                            sampling_method='sobol')
     assert_allclose(result_scipy.fun, result.residual)
     assert_allclose(result_scipy.xl, result.shgo_xl)
@@ -110,15 +96,15 @@
                          ('x1', 1., True, 2.5, 7.5))
 
     out = minimizer_Alpine02.minimize(params=pars_bounds, method='shgo')
     assert 5.0 <= out.params['x0'].value <= 15.0
     assert 2.5 <= out.params['x1'].value <= 7.5
 
 
-def test_shgo_disp_true(minimizer_Alpine02, capsys):
+def abandoned_test_shgo_disp_true(minimizer_Alpine02, capsys):
     """Test SHGO algorithm with disp is True."""
     kws = {'disp': True}
     minimizer_Alpine02.minimize(method='shgo', options=kws)
     captured = capsys.readouterr()
     assert 'Splitting first generation' in captured.out
```

### Comparing `lmfit-1.2.1/tests/test_stepmodel.py` & `lmfit-1.2.2/tests/test_stepmodel.py`

 * *Files identical despite different names*

