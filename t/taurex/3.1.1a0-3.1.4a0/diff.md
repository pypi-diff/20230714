# Comparing `tmp/taurex-3.1.1a0.tar.gz` & `tmp/taurex-3.1.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taurex-3.1.1a0.tar", last modified: Wed Sep 15 17:23:47 2021, max compression
+gzip compressed data, was "taurex-3.1.4a0.tar", last modified: Fri Jul 14 18:43:46 2023, max compression
```

## Comparing `taurex-3.1.1a0.tar` & `taurex-3.1.4a0.tar`

### file list

```diff
@@ -1,405 +1,405 @@
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.731835 taurex-3.1.1a0/
--rw-r--r--   0 ahmed      (501) staff       (20)      546 2021-09-15 17:23:41.000000 taurex-3.1.1a0/.bumpversion.cfg
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.571239 taurex-3.1.1a0/.github/
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.586461 taurex-3.1.1a0/.github/workflows/
--rw-r--r--   0 ahmed      (501) staff       (20)     1336 2021-09-15 17:17:08.000000 taurex-3.1.1a0/.github/workflows/test-taurex.yml
--rw-r--r--   0 ahmed      (501) staff       (20)     1244 2021-09-15 17:17:08.000000 taurex-3.1.1a0/.github/workflows/upload-test.yml
--rw-r--r--   0 ahmed      (501) staff       (20)     1526 2021-09-15 17:17:08.000000 taurex-3.1.1a0/.gitignore
--rw-r--r--   0 ahmed      (501) staff       (20)      581 2021-07-01 10:26:34.000000 taurex-3.1.1a0/.readthedocs.yaml
--rw-r--r--   0 ahmed      (501) staff       (20)      829 2021-09-15 17:17:08.000000 taurex-3.1.1a0/CHANGELOG
--rw-r--r--   0 ahmed      (501) staff       (20)     2822 2021-07-01 10:26:34.000000 taurex-3.1.1a0/CONTRIBUTING.md
--rw-r--r--   0 ahmed      (501) staff       (20)     1579 2021-07-01 10:26:34.000000 taurex-3.1.1a0/LICENSE
--rw-r--r--   0 ahmed      (501) staff       (20)     2383 2021-09-15 17:23:47.732065 taurex-3.1.1a0/PKG-INFO
--rw-r--r--   0 ahmed      (501) staff       (20)      853 2021-09-15 17:23:41.000000 taurex-3.1.1a0/README.md
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.587121 taurex-3.1.1a0/doc/
--rw-r--r--   0 ahmed      (501) staff       (20)      584 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/Makefile
--rw-r--r--   0 ahmed      (501) staff       (20)      791 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/make.bat
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.589080 taurex-3.1.1a0/doc/source/
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.589405 taurex-3.1.1a0/doc/source/_static/
--rw-r--r--   0 ahmed      (501) staff       (20)    45894 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/_static/taurex_logo.png
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.598198 taurex-3.1.1a0/doc/source/api/
--rw-r--r--   0 ahmed      (501) staff       (20)      436 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/api/modules.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      904 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/api/taurex.binning.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      484 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/api/taurex.cache.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     1474 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/api/taurex.chemistry.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      449 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/api/taurex.cia.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     1352 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/api/taurex.contributions.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      435 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/api/taurex.core.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      345 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/api/taurex.instrument.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      270 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/api/taurex.log.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      228 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/api/taurex.mixin.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      752 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/api/taurex.model.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      128 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/api/taurex.mpi.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      846 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/api/taurex.opacity.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      856 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/api/taurex.optimizer.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      603 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/api/taurex.output.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      540 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/api/taurex.parameter.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      469 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/api/taurex.pressure.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      951 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/api/taurex.spectrum.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      478 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/api/taurex.stellar.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     1289 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/api/taurex.temperature.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      591 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/api/taurex.util.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     1773 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/citation.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     5959 2021-09-15 17:23:41.000000 taurex-3.1.1a0/doc/source/conf.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.602462 taurex-3.1.1a0/doc/source/devel/
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.606084 taurex-3.1.1a0/doc/source/devel/_static/
--rw-r--r--   0 ahmed      (501) staff       (20)   321804 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/devel/_static/Taurex3-framework2.png
--rw-r--r--   0 ahmed      (501) staff       (20)    68298 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/devel/_static/bbnoise.png
--rw-r--r--   0 ahmed      (501) staff       (20)    76263 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/devel/_static/phoenixa.png
--rw-r--r--   0 ahmed      (501) staff       (20)    69794 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/devel/_static/phoenixb.png
--rw-r--r--   0 ahmed      (501) staff       (20)    64456 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/devel/_static/phoenixdenoise.png
--rw-r--r--   0 ahmed      (501) staff       (20)    73381 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/devel/_static/phoenixnoise.png
--rw-r--r--   0 ahmed      (501) staff       (20)    64391 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/devel/_static/random_tp_500.png
--rw-r--r--   0 ahmed      (501) staff       (20)    10764 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/devel/basics.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     5513 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/devel/components.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     2010 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/devel/fittingparameters.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     3353 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/devel/guidelines.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      319 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/devel/index.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     8232 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/devel/mixins.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      843 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/devel/overview.rst
--rw-r--r--   0 ahmed      (501) staff       (20)    10847 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/devel/plugins.rst
--rw-r--r--   0 ahmed      (501) staff       (20)       24 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/devel/recipes.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     1623 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/index.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     3071 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/plugins_cata.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     1296 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/requirements.txt
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.608501 taurex-3.1.1a0/doc/source/user/
--rw-r--r--   0 ahmed      (501) staff       (20)      445 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/user/index.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     2645 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/user/installation.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      639 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/introduction.rst
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.609191 taurex-3.1.1a0/doc/source/user/library/
--rw-r--r--   0 ahmed      (501) staff       (20)      201 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/library/index.rst
--rw-r--r--   0 ahmed      (501) staff       (20)  1523112 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/library/quickstart.ipynb
--rw-r--r--   0 ahmed      (501) staff       (20)     2509 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/user/mpi.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     4242 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/user/plugins.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     1307 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/user/support_data_formats.rst
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.619118 taurex-3.1.1a0/doc/source/user/taurex/
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.629887 taurex-3.1.1a0/doc/source/user/taurex/_static/
--rw-r--r--   0 ahmed      (501) staff       (20)    38787 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/ch4_and_h2o.png
--rw-r--r--   0 ahmed      (501) staff       (20)    41972 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/co2_and_h2o.png
--rw-r--r--   0 ahmed      (501) staff       (20)    31809 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/constantgas.png
--rw-r--r--   0 ahmed      (501) staff       (20)    64142 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/contrib.png
--rw-r--r--   0 ahmed      (501) staff       (20)    30797 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/firstfm.png
--rw-r--r--   0 ahmed      (501) staff       (20)    36070 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/fm_and_obs.png
--rw-r--r--   0 ahmed      (501) staff       (20)    41996 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/fm_obs_bin.png
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.631835 taurex-3.1.1a0/doc/source/user/taurex/_static/fm_plots/
--rw-r--r--   0 ahmed      (501) staff       (20)     8815 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/fm_plots/fm_plots-0.png
--rw-r--r--   0 ahmed      (501) staff       (20)    10791 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/fm_plots/fm_plots-1.png
--rw-r--r--   0 ahmed      (501) staff       (20)    50123 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/fm_plots/fm_plots-2.png
--rw-r--r--   0 ahmed      (501) staff       (20)    26947 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/fm_plots/fm_plots-3.png
--rw-r--r--   0 ahmed      (501) staff       (20)     8122 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/fm_plots/fm_plots-4.png
--rw-r--r--   0 ahmed      (501) staff       (20)    78197 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/full_contrib.png
--rw-r--r--   0 ahmed      (501) staff       (20)    21636 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/guillot.png
--rw-r--r--   0 ahmed      (501) staff       (20)    41408 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/h2o_only.png
--rw-r--r--   0 ahmed      (501) staff       (20)    30839 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/isothermal.png
--rw-r--r--   0 ahmed      (501) staff       (20)    22886 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/npoint.png
--rw-r--r--   0 ahmed      (501) staff       (20)    66169 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/random_tp.png
--rw-r--r--   0 ahmed      (501) staff       (20)    64391 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/random_tp_500.png
--rw-r--r--   0 ahmed      (501) staff       (20)   289658 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/random_tp_posterior.png
--rw-r--r--   0 ahmed      (501) staff       (20)    40802 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/ray_and_cia.png
--rw-r--r--   0 ahmed      (501) staff       (20)    41655 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/retrieval.png
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.634667 taurex-3.1.1a0/doc/source/user/taurex/_static/retrieval_plots/
--rw-r--r--   0 ahmed      (501) staff       (20)     8874 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-0.png
--rw-r--r--   0 ahmed      (501) staff       (20)    13793 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-1.png
--rw-r--r--   0 ahmed      (501) staff       (20)    66947 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-2.png
--rw-r--r--   0 ahmed      (501) staff       (20)    56661 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-3.png
--rw-r--r--   0 ahmed      (501) staff       (20)    27146 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-4.png
--rw-r--r--   0 ahmed      (501) staff       (20)     8901 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-5.png
--rw-r--r--   0 ahmed      (501) staff       (20)    25222 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/rodgers.png
--rw-r--r--   0 ahmed      (501) staff       (20)    20339 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/twolayerabundance.png
--rw-r--r--   0 ahmed      (501) staff       (20)    23288 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/_static/twopointgas.png
--rw-r--r--   0 ahmed      (501) staff       (20)     2925 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/binning.rst
--rw-r--r--   0 ahmed      (501) staff       (20)    10362 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/user/taurex/chemistry.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     7803 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/user/taurex/custom.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     6995 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/user/taurex/derived.rst
--rw-r--r--   0 ahmed      (501) staff       (20)    10584 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/user/taurex/fitting.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     1443 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/user/taurex/global.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      792 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/user/taurex/index.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     4306 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/user/taurex/inputfile.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     1636 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/instrument.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     1717 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/user/taurex/mixins.rst
--rw-r--r--   0 ahmed      (501) staff       (20)    10053 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/user/taurex/models.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     2001 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/observation.rst
--rw-r--r--   0 ahmed      (501) staff       (20)      791 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/optimizer.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     2427 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/planet.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     3214 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/plotting.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     2089 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/user/taurex/pressure.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     9179 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/user/taurex/quickstart.rst
--rw-r--r--   0 ahmed      (501) staff       (20)     4301 2021-07-01 10:26:34.000000 taurex-3.1.1a0/doc/source/user/taurex/star.rst
--rw-r--r--   0 ahmed      (501) staff       (20)    12566 2021-09-15 17:17:08.000000 taurex-3.1.1a0/doc/source/user/taurex/temperature.rst
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.573702 taurex-3.1.1a0/examples/
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.636465 taurex-3.1.1a0/examples/library/
--rw-r--r--   0 ahmed      (501) staff       (20)      442 2021-07-01 10:26:34.000000 taurex-3.1.1a0/examples/library/chemistry_randomizer.par
--rw-r--r--   0 ahmed      (501) staff       (20)     2717 2021-07-01 10:26:34.000000 taurex-3.1.1a0/examples/library/chemistry_randomizer.py
--rw-r--r--   0 ahmed      (501) staff       (20)     6401 2021-09-15 17:17:08.000000 taurex-3.1.1a0/examples/library/example_chem.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1704 2021-07-01 10:26:34.000000 taurex-3.1.1a0/examples/library/example_inst.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2773 2021-07-01 10:26:34.000000 taurex-3.1.1a0/examples/library/example_temp.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.636811 taurex-3.1.1a0/examples/notebooks/
--rw-r--r--   0 ahmed      (501) staff       (20)  1523112 2021-07-01 10:26:34.000000 taurex-3.1.1a0/examples/notebooks/quickstart.ipynb
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.643048 taurex-3.1.1a0/examples/parfiles/
--rw-r--r--   0 ahmed      (501) staff       (20)     1153 2021-07-01 10:26:34.000000 taurex-3.1.1a0/examples/parfiles/custom_chemistry.par
--rw-r--r--   0 ahmed      (501) staff       (20)      604 2021-07-01 10:26:34.000000 taurex-3.1.1a0/examples/parfiles/custom_selfretrieval.par
--rw-r--r--   0 ahmed      (501) staff       (20)     1123 2021-07-01 10:26:34.000000 taurex-3.1.1a0/examples/parfiles/custom_temp.par
--rw-r--r--   0 ahmed      (501) staff       (20)      948 2021-07-01 10:26:34.000000 taurex-3.1.1a0/examples/parfiles/emission_secondary.par
--rw-r--r--   0 ahmed      (501) staff       (20)     1156 2021-07-01 10:26:34.000000 taurex-3.1.1a0/examples/parfiles/multinest.par
--rw-r--r--   0 ahmed      (501) staff       (20)     1018 2021-07-01 10:26:34.000000 taurex-3.1.1a0/examples/parfiles/nestle.par
--rw-r--r--   0 ahmed      (501) staff       (20)    10752 2021-07-01 10:26:34.000000 taurex-3.1.1a0/examples/parfiles/quickstart.dat
--rw-r--r--   0 ahmed      (501) staff       (20)      668 2021-07-01 10:26:34.000000 taurex-3.1.1a0/examples/parfiles/quickstart.par
--rw-r--r--   0 ahmed      (501) staff       (20)     1048 2021-07-01 10:26:34.000000 taurex-3.1.1a0/examples/parfiles/transmission_equil.par
--rw-r--r--   0 ahmed      (501) staff       (20)     1145 2021-07-01 10:26:34.000000 taurex-3.1.1a0/examples/parfiles/transmission_model.par
--rw-r--r--   0 ahmed      (501) staff       (20)      101 2021-09-15 17:17:08.000000 taurex-3.1.1a0/requirements.txt
--rw-r--r--   0 ahmed      (501) staff       (20)      145 2021-09-15 17:23:47.732862 taurex-3.1.1a0/setup.cfg
--rw-r--r--   0 ahmed      (501) staff       (20)     2087 2021-09-15 17:23:41.000000 taurex-3.1.1a0/setup.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.649297 taurex-3.1.1a0/taurex/
--rw-r--r--   0 ahmed      (501) staff       (20)      107 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)      577 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/_citation.py
--rw-r--r--   0 ahmed      (501) staff       (20)       38 2021-09-15 17:23:41.000000 taurex-3.1.1a0/taurex/_version.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.654543 taurex-3.1.1a0/taurex/binning/
--rw-r--r--   0 ahmed      (501) staff       (20)      203 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/binning/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     4437 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/binning/binner.py
--rw-r--r--   0 ahmed      (501) staff       (20)     5774 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/binning/fluxbinner.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1786 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/binning/lightcurvebinner.py
--rw-r--r--   0 ahmed      (501) staff       (20)      903 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/binning/nativebinner.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2853 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/binning/simplebinner.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.656979 taurex-3.1.1a0/taurex/cache/
--rw-r--r--   0 ahmed      (501) staff       (20)      184 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/cache/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     7288 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/cache/ciaacache.py
--rw-r--r--   0 ahmed      (501) staff       (20)      472 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/cache/globalcache.py
--rw-r--r--   0 ahmed      (501) staff       (20)     8306 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/cache/ktablecache.py
--rw-r--r--   0 ahmed      (501) staff       (20)    11804 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/cache/opacitycache.py
--rw-r--r--   0 ahmed      (501) staff       (20)      524 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/cache/singleton.py
--rw-r--r--   0 ahmed      (501) staff       (20)      466 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/chemistry.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.658779 taurex-3.1.1a0/taurex/cia/
--rw-r--r--   0 ahmed      (501) staff       (20)      177 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/cia/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     4017 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/cia/cia.py
--rw-r--r--   0 ahmed      (501) staff       (20)    12432 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/cia/hitrancia.py
--rw-r--r--   0 ahmed      (501) staff       (20)     3990 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/cia/picklecia.py
--rw-r--r--   0 ahmed      (501) staff       (20)      732 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/constants.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.662676 taurex-3.1.1a0/taurex/contributions/
--rw-r--r--   0 ahmed      (501) staff       (20)      424 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/contributions/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     4867 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/contributions/absorption.py
--rw-r--r--   0 ahmed      (501) staff       (20)     4400 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/contributions/cia.py
--rw-r--r--   0 ahmed      (501) staff       (20)     6974 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/contributions/contribution.py
--rw-r--r--   0 ahmed      (501) staff       (20)     4070 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/contributions/flatmie.py
--rw-r--r--   0 ahmed      (501) staff       (20)    10591 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/contributions/hm.py
--rw-r--r--   0 ahmed      (501) staff       (20)     7576 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/contributions/leemie.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1794 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/contributions/rayleigh.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2429 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/contributions/simpleclouds.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.663718 taurex-3.1.1a0/taurex/core/
--rw-r--r--   0 ahmed      (501) staff       (20)      709 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/core/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2587 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/core/priors.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.665201 taurex-3.1.1a0/taurex/data/
--rw-r--r--   0 ahmed      (501) staff       (20)       26 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/data/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2751 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/citation.py
--rw-r--r--   0 ahmed      (501) staff       (20)    11744 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/fittable.py
--rw-r--r--   0 ahmed      (501) staff       (20)     8929 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/planet.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.665588 taurex-3.1.1a0/taurex/data/profiles/
--rw-r--r--   0 ahmed      (501) staff       (20)       89 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/data/profiles/__init__.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.668475 taurex-3.1.1a0/taurex/data/profiles/chemistry/
--rw-r--r--   0 ahmed      (501) staff       (20)      290 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/chemistry/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     3289 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/chemistry/autochemistry.py
--rw-r--r--   0 ahmed      (501) staff       (20)     8439 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/chemistry/chemistry.py
--rw-r--r--   0 ahmed      (501) staff       (20)      957 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/chemistry/filechemistry.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.671097 taurex-3.1.1a0/taurex/data/profiles/chemistry/gas/
--rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/data/profiles/chemistry/gas/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1722 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/chemistry/gas/arraygas.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1932 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/chemistry/gas/constantgas.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2552 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/chemistry/gas/gas.py
--rw-r--r--   0 ahmed      (501) staff       (20)     7833 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/chemistry/gas/powergas.py
--rw-r--r--   0 ahmed      (501) staff       (20)     6686 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/chemistry/gas/twolayergas.py
--rw-r--r--   0 ahmed      (501) staff       (20)     3804 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/chemistry/gas/twopointgas.py
--rw-r--r--   0 ahmed      (501) staff       (20)    13886 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/chemistry/taurexchemistry.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.672617 taurex-3.1.1a0/taurex/data/profiles/pressure/
--rw-r--r--   0 ahmed      (501) staff       (20)      162 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/pressure/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)      930 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/pressure/arraypressure.py
--rw-r--r--   0 ahmed      (501) staff       (20)      636 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/pressure/filepressure.py
--rw-r--r--   0 ahmed      (501) staff       (20)     5286 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/pressure/pressureprofile.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.675954 taurex-3.1.1a0/taurex/data/profiles/temperature/
--rw-r--r--   0 ahmed      (501) staff       (20)      202 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/data/profiles/temperature/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1360 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/temperature/file.py
--rw-r--r--   0 ahmed      (501) staff       (20)     6614 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/temperature/guillot.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1276 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/temperature/isothermal.py
--rw-r--r--   0 ahmed      (501) staff       (20)     9284 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/temperature/npoint.py
--rw-r--r--   0 ahmed      (501) staff       (20)     4474 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/temperature/rodgers.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2081 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/temperature/temparray.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1948 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/profiles/temperature/tprofile.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.679634 taurex-3.1.1a0/taurex/data/spectrum/
--rw-r--r--   0 ahmed      (501) staff       (20)      203 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/data/spectrum/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2922 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/spectrum/array.py
--rw-r--r--   0 ahmed      (501) staff       (20)      934 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/spectrum/iraclis.py
--rw-r--r--   0 ahmed      (501) staff       (20)     4126 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/spectrum/lightcurve.py
--rw-r--r--   0 ahmed      (501) staff       (20)      715 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/spectrum/observed.py
--rw-r--r--   0 ahmed      (501) staff       (20)     3068 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/spectrum/spectrum.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1449 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/spectrum/taurex.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.680906 taurex-3.1.1a0/taurex/data/stellar/
--rw-r--r--   0 ahmed      (501) staff       (20)      134 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/data/stellar/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)    11544 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/stellar/phoenix.py
--rw-r--r--   0 ahmed      (501) staff       (20)     3317 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/data/stellar/star.py
--rw-r--r--   0 ahmed      (501) staff       (20)       51 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/exceptions.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.682531 taurex-3.1.1a0/taurex/instruments/
--rw-r--r--   0 ahmed      (501) staff       (20)      109 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/instruments/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)      996 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/instruments/instrument.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1579 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/instruments/instrumentfile.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1213 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/instruments/snr.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.683790 taurex-3.1.1a0/taurex/log/
--rw-r--r--   0 ahmed      (501) staff       (20)      466 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/log/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2664 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/log/logger.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.684907 taurex-3.1.1a0/taurex/mixin/
--rw-r--r--   0 ahmed      (501) staff       (20)      275 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/mixin/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     3287 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/mixin/core.py
--rw-r--r--   0 ahmed      (501) staff       (20)     8839 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/mixin/mixins.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.687060 taurex-3.1.1a0/taurex/model/
--rw-r--r--   0 ahmed      (501) staff       (20)      197 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/model/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2667 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/model/directimage.py
--rw-r--r--   0 ahmed      (501) staff       (20)    12997 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/model/emission.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.688245 taurex-3.1.1a0/taurex/model/lightcurve/
--rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/model/lightcurve/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)    15103 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/model/lightcurve/lightcurve.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2837 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/model/lightcurve/lightcurvedata.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2982 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/model/model.py
--rw-r--r--   0 ahmed      (501) staff       (20)    20456 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/model/simplemodel.py
--rw-r--r--   0 ahmed      (501) staff       (20)     5160 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/model/transmission.py
--rw-r--r--   0 ahmed      (501) staff       (20)     4597 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/mpi.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.691080 taurex-3.1.1a0/taurex/opacity/
--rw-r--r--   0 ahmed      (501) staff       (20)      203 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/opacity/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     3281 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/opacity/exotransmit.py
--rw-r--r--   0 ahmed      (501) staff       (20)      982 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/opacity/fakeopacity.py
--rw-r--r--   0 ahmed      (501) staff       (20)     4007 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/opacity/hdf5opacity.py
--rw-r--r--   0 ahmed      (501) staff       (20)     5986 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/opacity/interpolateopacity.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.693231 taurex-3.1.1a0/taurex/opacity/ktables/
--rw-r--r--   0 ahmed      (501) staff       (20)      142 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/opacity/ktables/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     3759 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/opacity/ktables/hdfktable.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1254 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/opacity/ktables/ktable.py
--rw-r--r--   0 ahmed      (501) staff       (20)     5870 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/opacity/ktables/nemesisktables.py
--rw-r--r--   0 ahmed      (501) staff       (20)     3051 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/opacity/ktables/picklektable.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1939 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/opacity/opacity.py
--rw-r--r--   0 ahmed      (501) staff       (20)     3229 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/opacity/pickleopacity.py
--rw-r--r--   0 ahmed      (501) staff       (20)     4157 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/opacity/radisopacity.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.696416 taurex-3.1.1a0/taurex/optimizer/
--rw-r--r--   0 ahmed      (501) staff       (20)      315 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/optimizer/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     5374 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/optimizer/dypolychord.py
--rw-r--r--   0 ahmed      (501) staff       (20)    16262 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/optimizer/multinest.py
--rw-r--r--   0 ahmed      (501) staff       (20)     7706 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/optimizer/nestle.py
--rw-r--r--   0 ahmed      (501) staff       (20)    26516 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/optimizer/optimizer.py
--rw-r--r--   0 ahmed      (501) staff       (20)    13077 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/optimizer/polychord.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.699924 taurex-3.1.1a0/taurex/output/
--rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/output/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2905 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/output/hdf5.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1423 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/output/output.py
--rw-r--r--   0 ahmed      (501) staff       (20)       70 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/output/writeable.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.701450 taurex-3.1.1a0/taurex/parameter/
--rw-r--r--   0 ahmed      (501) staff       (20)       44 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/parameter/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)    16366 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/parameter/classfactory.py
--rw-r--r--   0 ahmed      (501) staff       (20)    15314 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/parameter/factory.py
--rw-r--r--   0 ahmed      (501) staff       (20)    14455 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/parameter/parameterparser.py
--rw-r--r--   0 ahmed      (501) staff       (20)       77 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/planet.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.702402 taurex-3.1.1a0/taurex/plot/
--rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/plot/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)    21741 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/plot/corner.py
--rw-r--r--   0 ahmed      (501) staff       (20)    37950 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/plot/plotter.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.702827 taurex-3.1.1a0/taurex/plugins/
--rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/plugins/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)      125 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/pressure.py
--rw-r--r--   0 ahmed      (501) staff       (20)      363 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/spectrum.py
--rw-r--r--   0 ahmed      (501) staff       (20)      109 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/stellar.py
--rw-r--r--   0 ahmed      (501) staff       (20)    22960 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/taurex.py
--rw-r--r--   0 ahmed      (501) staff       (20)      389 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/taurexdefs.py
--rw-r--r--   0 ahmed      (501) staff       (20)      310 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/temperature.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.706877 taurex-3.1.1a0/taurex/util/
--rw-r--r--   0 ahmed      (501) staff       (20)      137 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/util/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2895 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/util/emission.py
--rw-r--r--   0 ahmed      (501) staff       (20)      729 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/util/fitting.py
--rw-r--r--   0 ahmed      (501) staff       (20)     8887 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/util/fortran.py
--rw-r--r--   0 ahmed      (501) staff       (20)     5791 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/util/geometry.py
--rw-r--r--   0 ahmed      (501) staff       (20)     6859 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/util/hdf5.py
--rw-r--r--   0 ahmed      (501) staff       (20)    10513 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/util/math.py
--rw-r--r--   0 ahmed      (501) staff       (20)      732 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/util/module.py
--rw-r--r--   0 ahmed      (501) staff       (20)     9965 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/util/output.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2203 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/util/scattering.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1610 2021-07-01 10:26:34.000000 taurex-3.1.1a0/taurex/util/spectrum.py
--rw-r--r--   0 ahmed      (501) staff       (20)    16668 2021-09-15 17:17:08.000000 taurex-3.1.1a0/taurex/util/util.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.652087 taurex-3.1.1a0/taurex.egg-info/
--rwxr-xr-x   0 ahmed      (501) staff       (20)     2383 2021-09-15 17:23:47.000000 taurex-3.1.1a0/taurex.egg-info/PKG-INFO
--rwxr-xr-x   0 ahmed      (501) staff       (20)    10967 2021-09-15 17:23:47.000000 taurex-3.1.1a0/taurex.egg-info/SOURCES.txt
--rwxr-xr-x   0 ahmed      (501) staff       (20)        1 2021-09-15 17:23:47.000000 taurex-3.1.1a0/taurex.egg-info/dependency_links.txt
--rwxr-xr-x   0 ahmed      (501) staff       (20)       93 2021-09-15 17:23:47.000000 taurex-3.1.1a0/taurex.egg-info/entry_points.txt
--rwxr-xr-x   0 ahmed      (501) staff       (20)       91 2021-09-15 17:23:47.000000 taurex-3.1.1a0/taurex.egg-info/requires.txt
--rwxr-xr-x   0 ahmed      (501) staff       (20)       13 2021-09-15 17:23:47.000000 taurex-3.1.1a0/taurex.egg-info/top_level.txt
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.710274 taurex-3.1.1a0/tests/
--rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-07-01 10:26:34.000000 taurex-3.1.1a0/tests/__init__.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.713469 taurex-3.1.1a0/tests/benchmark/
--rw-r--r--   0 ahmed      (501) staff       (20)      941 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/benchmark/test_bb.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2798 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/benchmark/test_bilinear_interps.py
--rw-r--r--   0 ahmed      (501) staff       (20)     3935 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/benchmark/test_contrib_funcs.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1077 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/benchmark/test_emission_funcs.py
--rw-r--r--   0 ahmed      (501) staff       (20)      903 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/benchmark/test_forward_model.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1499 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/benchmark/test_linear_interps.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.715427 taurex-3.1.1a0/tests/chemistry/
--rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/chemistry/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2685 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/chemistry/test_chemistry.py
--rw-r--r--   0 ahmed      (501) staff       (20)      906 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/chemistry/test_constantgas.py
--rw-r--r--   0 ahmed      (501) staff       (20)     4890 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/chemistry/test_free_chemistry.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2310 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/chemistry/test_powergas.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.716085 taurex-3.1.1a0/tests/cia/
--rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/cia/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2796 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/cia/test_cia.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.716827 taurex-3.1.1a0/tests/citation/
--rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/citation/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)      382 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/citation/test_citation.py
--rw-r--r--   0 ahmed      (501) staff       (20)       81 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/conftest.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.718304 taurex-3.1.1a0/tests/factory/
--rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/factory/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)      911 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/factory/test_classfactory.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1898 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/factory/test_factories.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2280 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/factory/test_mixin.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.718717 taurex-3.1.1a0/tests/fixtures/
--rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/fixtures/__init__.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.719516 taurex-3.1.1a0/tests/fixtures/opacities/
--rw-r--r--   0 ahmed      (501) staff       (20)      361 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/fixtures/opacities/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)      757 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/fixtures/opacities/genopacs.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.719990 taurex-3.1.1a0/tests/fixtures/profiles/
--rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/fixtures/profiles/__init__.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.720271 taurex-3.1.1a0/tests/fixtures/spectra/
--rw-r--r--   0 ahmed      (501) staff       (20)      349 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/fixtures/spectra/__init__.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.720655 taurex-3.1.1a0/tests/model/
--rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/model/__init__.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.721869 taurex-3.1.1a0/tests/optimizer/
--rw-r--r--   0 ahmed      (501) staff       (20)     1850 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/optimizer/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)      820 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/optimizer/test_nestle.py
--rw-r--r--   0 ahmed      (501) staff       (20)     4360 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/optimizer/test_optimizer.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.722239 taurex-3.1.1a0/tests/output/
--rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/output/__init__.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.722956 taurex-3.1.1a0/tests/parameter/
--rw-r--r--   0 ahmed      (501) staff       (20)        2 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/parameter/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2696 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/parameter/test_keywords.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.724034 taurex-3.1.1a0/tests/priors/
--rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/priors/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2721 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/priors/test_nonuniform.py
--rw-r--r--   0 ahmed      (501) staff       (20)      468 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/priors/test_priors.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.724713 taurex-3.1.1a0/tests/spectrum/
--rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/spectrum/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)    12076 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/spectrum/test_spectrum.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.726278 taurex-3.1.1a0/tests/stellar/
--rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/stellar/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)      662 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/stellar/test_blackbody.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1783 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/stellar/test_phoenix.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.726739 taurex-3.1.1a0/tests/strategies/
--rw-r--r--   0 ahmed      (501) staff       (20)     7761 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/strategies/__init__.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.728331 taurex-3.1.1a0/tests/temperature/
--rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/temperature/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2782 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/temperature/test_guillot.py
--rw-r--r--   0 ahmed      (501) staff       (20)      848 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/temperature/test_isothermal.py
--rw-r--r--   0 ahmed      (501) staff       (20)     4613 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/temperature/test_npoint.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1106 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/test_binning.py
--rw-r--r--   0 ahmed      (501) staff       (20)     3866 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/test_core.py
--rw-r--r--   0 ahmed      (501) staff       (20)    16461 2021-07-01 10:26:34.000000 taurex-3.1.1a0/tests/test_modelload.py
--rw-r--r--   0 ahmed      (501) staff       (20)     4533 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/test_opac.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2363 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/test_pressure.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.730483 taurex-3.1.1a0/tests/util/
--rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/util/__init__.py
--rw-r--r--   0 ahmed      (501) staff       (20)     1231 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/util/test_emission.py
--rw-r--r--   0 ahmed      (501) staff       (20)      942 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/util/test_fitting.py
--rw-r--r--   0 ahmed      (501) staff       (20)     3192 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/util/test_math.py
--rw-r--r--   0 ahmed      (501) staff       (20)     5842 2021-09-15 17:17:08.000000 taurex-3.1.1a0/tests/util/test_util.py
-drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2021-09-15 17:23:47.731330 taurex-3.1.1a0/tools/
--rw-r--r--   0 ahmed      (501) staff       (20)     4610 2021-07-01 10:26:34.000000 taurex-3.1.1a0/tools/exocross_to_hdf5.py
--rw-r--r--   0 ahmed      (501) staff       (20)     2133 2021-07-01 10:26:34.000000 taurex-3.1.1a0/tools/pickle_to_properformat.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.910729 taurex-3.1.4a0/
+-rw-r--r--   0 ahmed      (501) staff       (20)      546 2023-07-14 18:39:11.000000 taurex-3.1.4a0/.bumpversion.cfg
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:45.261242 taurex-3.1.4a0/.github/
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:45.446096 taurex-3.1.4a0/.github/workflows/
+-rw-r--r--   0 ahmed      (501) staff       (20)     1336 2023-07-14 18:36:43.000000 taurex-3.1.4a0/.github/workflows/test-taurex.yml
+-rw-r--r--   0 ahmed      (501) staff       (20)     1244 2023-07-14 18:36:43.000000 taurex-3.1.4a0/.github/workflows/upload-test.yml
+-rw-r--r--   0 ahmed      (501) staff       (20)     1526 2023-07-14 18:36:43.000000 taurex-3.1.4a0/.gitignore
+-rw-r--r--   0 ahmed      (501) staff       (20)      581 2021-07-01 10:26:34.000000 taurex-3.1.4a0/.readthedocs.yaml
+-rw-r--r--   0 ahmed      (501) staff       (20)      829 2023-07-14 18:36:43.000000 taurex-3.1.4a0/CHANGELOG
+-rw-r--r--   0 ahmed      (501) staff       (20)     2822 2021-07-01 10:26:34.000000 taurex-3.1.4a0/CONTRIBUTING.md
+-rw-r--r--   0 ahmed      (501) staff       (20)     1579 2021-07-01 10:26:34.000000 taurex-3.1.4a0/LICENSE
+-rw-r--r--   0 ahmed      (501) staff       (20)     1847 2023-07-14 18:43:46.911250 taurex-3.1.4a0/PKG-INFO
+-rw-r--r--   0 ahmed      (501) staff       (20)      853 2023-07-14 18:39:11.000000 taurex-3.1.4a0/README.md
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:45.453445 taurex-3.1.4a0/doc/
+-rw-r--r--   0 ahmed      (501) staff       (20)      584 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/Makefile
+-rw-r--r--   0 ahmed      (501) staff       (20)      791 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/make.bat
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:45.463012 taurex-3.1.4a0/doc/source/
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:45.464778 taurex-3.1.4a0/doc/source/_static/
+-rw-r--r--   0 ahmed      (501) staff       (20)    45894 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/_static/taurex_logo.png
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:45.516152 taurex-3.1.4a0/doc/source/api/
+-rw-r--r--   0 ahmed      (501) staff       (20)      436 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/api/modules.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      904 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/api/taurex.binning.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      484 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/api/taurex.cache.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     1474 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/api/taurex.chemistry.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      449 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/api/taurex.cia.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     1352 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/api/taurex.contributions.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      435 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/api/taurex.core.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      345 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/api/taurex.instrument.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      270 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/api/taurex.log.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      228 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/api/taurex.mixin.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      752 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/api/taurex.model.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      128 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/api/taurex.mpi.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      846 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/api/taurex.opacity.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      856 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/api/taurex.optimizer.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      603 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/api/taurex.output.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      540 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/api/taurex.parameter.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      469 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/api/taurex.pressure.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      951 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/api/taurex.spectrum.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      478 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/api/taurex.stellar.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     1289 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/api/taurex.temperature.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      591 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/api/taurex.util.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     1773 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/citation.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     5959 2023-07-14 18:39:11.000000 taurex-3.1.4a0/doc/source/conf.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:45.738371 taurex-3.1.4a0/doc/source/devel/
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:45.763473 taurex-3.1.4a0/doc/source/devel/_static/
+-rw-r--r--   0 ahmed      (501) staff       (20)   321804 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/devel/_static/Taurex3-framework2.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    68298 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/devel/_static/bbnoise.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    76263 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/devel/_static/phoenixa.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    69794 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/devel/_static/phoenixb.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    64456 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/devel/_static/phoenixdenoise.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    73381 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/devel/_static/phoenixnoise.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    64391 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/devel/_static/random_tp_500.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    10764 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/devel/basics.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     5513 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/devel/components.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     2010 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/devel/fittingparameters.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     3353 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/devel/guidelines.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      319 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/devel/index.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     8232 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/devel/mixins.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      843 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/devel/overview.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)    10847 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/devel/plugins.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)       24 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/devel/recipes.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     1623 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/index.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     2454 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/plugins_cata.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     1303 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/requirements.txt
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:45.775161 taurex-3.1.4a0/doc/source/user/
+-rw-r--r--   0 ahmed      (501) staff       (20)      445 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/user/index.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     2645 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/user/installation.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      639 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/introduction.rst
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:45.779285 taurex-3.1.4a0/doc/source/user/library/
+-rw-r--r--   0 ahmed      (501) staff       (20)      201 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/library/index.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)  1523112 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/library/quickstart.ipynb
+-rw-r--r--   0 ahmed      (501) staff       (20)     2509 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/user/mpi.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     4242 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/user/plugins.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     1307 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/user/support_data_formats.rst
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:45.857584 taurex-3.1.4a0/doc/source/user/taurex/
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:45.930921 taurex-3.1.4a0/doc/source/user/taurex/_static/
+-rw-r--r--   0 ahmed      (501) staff       (20)    38787 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/ch4_and_h2o.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    41972 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/co2_and_h2o.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    31809 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/constantgas.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    64142 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/contrib.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    30797 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/firstfm.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    36070 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/fm_and_obs.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    41996 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/fm_obs_bin.png
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:45.965277 taurex-3.1.4a0/doc/source/user/taurex/_static/fm_plots/
+-rw-r--r--   0 ahmed      (501) staff       (20)     8815 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/fm_plots/fm_plots-0.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    10791 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/fm_plots/fm_plots-1.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    50123 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/fm_plots/fm_plots-2.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    26947 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/fm_plots/fm_plots-3.png
+-rw-r--r--   0 ahmed      (501) staff       (20)     8122 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/fm_plots/fm_plots-4.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    78197 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/full_contrib.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    21636 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/guillot.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    41408 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/h2o_only.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    30839 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/isothermal.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    22886 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/npoint.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    66169 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/random_tp.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    64391 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/random_tp_500.png
+-rw-r--r--   0 ahmed      (501) staff       (20)   289658 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/random_tp_posterior.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    40802 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/ray_and_cia.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    41655 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/retrieval.png
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:45.981912 taurex-3.1.4a0/doc/source/user/taurex/_static/retrieval_plots/
+-rw-r--r--   0 ahmed      (501) staff       (20)     8874 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-0.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    13793 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-1.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    66947 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-2.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    56661 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-3.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    27146 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-4.png
+-rw-r--r--   0 ahmed      (501) staff       (20)     8901 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-5.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    25222 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/rodgers.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    20339 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/twolayerabundance.png
+-rw-r--r--   0 ahmed      (501) staff       (20)    23288 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/_static/twopointgas.png
+-rw-r--r--   0 ahmed      (501) staff       (20)     2925 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/binning.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)    10362 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/user/taurex/chemistry.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     7803 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/user/taurex/custom.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     6995 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/user/taurex/derived.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)    10584 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/user/taurex/fitting.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     1443 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/user/taurex/global.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      792 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/user/taurex/index.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     4306 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/user/taurex/inputfile.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     1636 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/instrument.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     1717 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/user/taurex/mixins.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)    10053 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/user/taurex/models.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     2001 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/observation.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)      791 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/optimizer.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     2427 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/planet.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     3214 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/plotting.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     2089 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/user/taurex/pressure.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     9179 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/user/taurex/quickstart.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)     4301 2021-07-01 10:26:34.000000 taurex-3.1.4a0/doc/source/user/taurex/star.rst
+-rw-r--r--   0 ahmed      (501) staff       (20)    12566 2023-07-14 18:36:43.000000 taurex-3.1.4a0/doc/source/user/taurex/temperature.rst
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:45.298671 taurex-3.1.4a0/examples/
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:45.993404 taurex-3.1.4a0/examples/library/
+-rw-r--r--   0 ahmed      (501) staff       (20)      442 2021-07-01 10:26:34.000000 taurex-3.1.4a0/examples/library/chemistry_randomizer.par
+-rw-r--r--   0 ahmed      (501) staff       (20)     2717 2021-07-01 10:26:34.000000 taurex-3.1.4a0/examples/library/chemistry_randomizer.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     6401 2023-07-14 18:36:43.000000 taurex-3.1.4a0/examples/library/example_chem.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1704 2021-07-01 10:26:34.000000 taurex-3.1.4a0/examples/library/example_inst.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2773 2021-07-01 10:26:34.000000 taurex-3.1.4a0/examples/library/example_temp.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:45.996154 taurex-3.1.4a0/examples/notebooks/
+-rw-r--r--   0 ahmed      (501) staff       (20)  1523112 2021-07-01 10:26:34.000000 taurex-3.1.4a0/examples/notebooks/quickstart.ipynb
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.031877 taurex-3.1.4a0/examples/parfiles/
+-rw-r--r--   0 ahmed      (501) staff       (20)     1153 2021-07-01 10:26:34.000000 taurex-3.1.4a0/examples/parfiles/custom_chemistry.par
+-rw-r--r--   0 ahmed      (501) staff       (20)      604 2021-07-01 10:26:34.000000 taurex-3.1.4a0/examples/parfiles/custom_selfretrieval.par
+-rw-r--r--   0 ahmed      (501) staff       (20)     1123 2021-07-01 10:26:34.000000 taurex-3.1.4a0/examples/parfiles/custom_temp.par
+-rw-r--r--   0 ahmed      (501) staff       (20)      948 2021-07-01 10:26:34.000000 taurex-3.1.4a0/examples/parfiles/emission_secondary.par
+-rw-r--r--   0 ahmed      (501) staff       (20)     1156 2021-07-01 10:26:34.000000 taurex-3.1.4a0/examples/parfiles/multinest.par
+-rw-r--r--   0 ahmed      (501) staff       (20)     1018 2021-07-01 10:26:34.000000 taurex-3.1.4a0/examples/parfiles/nestle.par
+-rw-r--r--   0 ahmed      (501) staff       (20)    10752 2021-07-01 10:26:34.000000 taurex-3.1.4a0/examples/parfiles/quickstart.dat
+-rw-r--r--   0 ahmed      (501) staff       (20)      668 2021-07-01 10:26:34.000000 taurex-3.1.4a0/examples/parfiles/quickstart.par
+-rw-r--r--   0 ahmed      (501) staff       (20)     1048 2021-07-01 10:26:34.000000 taurex-3.1.4a0/examples/parfiles/transmission_equil.par
+-rw-r--r--   0 ahmed      (501) staff       (20)     1145 2021-07-01 10:26:34.000000 taurex-3.1.4a0/examples/parfiles/transmission_model.par
+-rw-r--r--   0 ahmed      (501) staff       (20)      101 2023-07-14 18:36:43.000000 taurex-3.1.4a0/requirements.txt
+-rw-r--r--   0 ahmed      (501) staff       (20)      145 2023-07-14 18:43:46.915545 taurex-3.1.4a0/setup.cfg
+-rw-r--r--   0 ahmed      (501) staff       (20)     2087 2023-07-14 18:39:11.000000 taurex-3.1.4a0/setup.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.062598 taurex-3.1.4a0/taurex/
+-rw-r--r--   0 ahmed      (501) staff       (20)      107 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      577 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/_citation.py
+-rw-r--r--   0 ahmed      (501) staff       (20)       38 2023-07-14 18:39:11.000000 taurex-3.1.4a0/taurex/_version.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.134761 taurex-3.1.4a0/taurex/binning/
+-rw-r--r--   0 ahmed      (501) staff       (20)      203 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/binning/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     4437 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/binning/binner.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     5774 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/binning/fluxbinner.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1786 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/binning/lightcurvebinner.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      903 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/binning/nativebinner.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2853 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/binning/simplebinner.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.154661 taurex-3.1.4a0/taurex/cache/
+-rw-r--r--   0 ahmed      (501) staff       (20)      184 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/cache/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     7288 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/cache/ciaacache.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      472 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/cache/globalcache.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     8306 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/cache/ktablecache.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    11804 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/cache/opacitycache.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      524 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/cache/singleton.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      466 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/chemistry.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.189723 taurex-3.1.4a0/taurex/cia/
+-rw-r--r--   0 ahmed      (501) staff       (20)      177 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/cia/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     4017 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/cia/cia.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    12512 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/cia/hitrancia.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     3990 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/cia/picklecia.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      732 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/constants.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.244864 taurex-3.1.4a0/taurex/contributions/
+-rw-r--r--   0 ahmed      (501) staff       (20)      424 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/contributions/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     4867 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/contributions/absorption.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     4400 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/contributions/cia.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     6974 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/contributions/contribution.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     4070 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/contributions/flatmie.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    10824 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/contributions/hm.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     7576 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/contributions/leemie.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1794 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/contributions/rayleigh.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2429 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/contributions/simpleclouds.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.249651 taurex-3.1.4a0/taurex/core/
+-rw-r--r--   0 ahmed      (501) staff       (20)      709 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/core/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2587 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/core/priors.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.259257 taurex-3.1.4a0/taurex/data/
+-rw-r--r--   0 ahmed      (501) staff       (20)       26 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/data/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     3445 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/citation.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    11744 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/fittable.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     8929 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/planet.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.261459 taurex-3.1.4a0/taurex/data/profiles/
+-rw-r--r--   0 ahmed      (501) staff       (20)       89 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/data/profiles/__init__.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.273079 taurex-3.1.4a0/taurex/data/profiles/chemistry/
+-rw-r--r--   0 ahmed      (501) staff       (20)      290 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/chemistry/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     3289 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/chemistry/autochemistry.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     8439 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/chemistry/chemistry.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      957 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/chemistry/filechemistry.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.390528 taurex-3.1.4a0/taurex/data/profiles/chemistry/gas/
+-rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/data/profiles/chemistry/gas/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1722 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/chemistry/gas/arraygas.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1932 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/chemistry/gas/constantgas.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2552 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/chemistry/gas/gas.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     7833 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/chemistry/gas/powergas.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     6686 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/chemistry/gas/twolayergas.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     3804 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/chemistry/gas/twopointgas.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    13886 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/chemistry/taurexchemistry.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.404441 taurex-3.1.4a0/taurex/data/profiles/pressure/
+-rw-r--r--   0 ahmed      (501) staff       (20)      162 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/pressure/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      930 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/pressure/arraypressure.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      636 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/pressure/filepressure.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     5286 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/pressure/pressureprofile.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.453595 taurex-3.1.4a0/taurex/data/profiles/temperature/
+-rw-r--r--   0 ahmed      (501) staff       (20)      202 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/data/profiles/temperature/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1360 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/temperature/file.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     6614 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/temperature/guillot.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1276 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/temperature/isothermal.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     9284 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/temperature/npoint.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     4474 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/temperature/rodgers.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2081 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/temperature/temparray.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1948 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/profiles/temperature/tprofile.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.507112 taurex-3.1.4a0/taurex/data/spectrum/
+-rw-r--r--   0 ahmed      (501) staff       (20)      203 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/data/spectrum/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2922 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/spectrum/array.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      934 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/spectrum/iraclis.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     4126 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/spectrum/lightcurve.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      715 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/spectrum/observed.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     3326 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/spectrum/spectrum.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1449 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/spectrum/taurex.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.535466 taurex-3.1.4a0/taurex/data/stellar/
+-rw-r--r--   0 ahmed      (501) staff       (20)      134 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/data/stellar/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    11544 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/stellar/phoenix.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     3317 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/data/stellar/star.py
+-rw-r--r--   0 ahmed      (501) staff       (20)       51 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/exceptions.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.545205 taurex-3.1.4a0/taurex/instruments/
+-rw-r--r--   0 ahmed      (501) staff       (20)      109 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/instruments/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      996 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/instruments/instrument.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1579 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/instruments/instrumentfile.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1213 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/instruments/snr.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.551934 taurex-3.1.4a0/taurex/log/
+-rw-r--r--   0 ahmed      (501) staff       (20)      466 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/log/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2664 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/log/logger.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.560737 taurex-3.1.4a0/taurex/mixin/
+-rw-r--r--   0 ahmed      (501) staff       (20)      275 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/mixin/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     3287 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/mixin/core.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     8839 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/mixin/mixins.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.629640 taurex-3.1.4a0/taurex/model/
+-rw-r--r--   0 ahmed      (501) staff       (20)      197 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/model/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2667 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/model/directimage.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    12997 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/model/emission.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.645644 taurex-3.1.4a0/taurex/model/lightcurve/
+-rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/model/lightcurve/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    15103 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/model/lightcurve/lightcurve.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2837 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/model/lightcurve/lightcurvedata.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2982 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/model/model.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    21166 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/model/simplemodel.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     5160 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/model/transmission.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     4597 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/mpi.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.671301 taurex-3.1.4a0/taurex/opacity/
+-rw-r--r--   0 ahmed      (501) staff       (20)      203 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/opacity/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     4247 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/opacity/exotransmit.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      982 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/opacity/fakeopacity.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     6516 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/opacity/hdf5opacity.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     5986 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/opacity/interpolateopacity.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.684575 taurex-3.1.4a0/taurex/opacity/ktables/
+-rw-r--r--   0 ahmed      (501) staff       (20)      142 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/opacity/ktables/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     3759 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/opacity/ktables/hdfktable.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1254 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/opacity/ktables/ktable.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     5870 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/opacity/ktables/nemesisktables.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     3051 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/opacity/ktables/picklektable.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2240 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/opacity/opacity.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     3229 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/opacity/pickleopacity.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     4979 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/opacity/radisopacity.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.695547 taurex-3.1.4a0/taurex/optimizer/
+-rw-r--r--   0 ahmed      (501) staff       (20)      315 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/optimizer/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     5374 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/optimizer/dypolychord.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    16529 2023-07-14 18:40:19.000000 taurex-3.1.4a0/taurex/optimizer/multinest.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     7706 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/optimizer/nestle.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    29330 2023-07-14 18:40:19.000000 taurex-3.1.4a0/taurex/optimizer/optimizer.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    13077 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/optimizer/polychord.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.702098 taurex-3.1.4a0/taurex/output/
+-rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/output/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2905 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/output/hdf5.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1423 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/output/output.py
+-rw-r--r--   0 ahmed      (501) staff       (20)       70 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/output/writeable.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.709094 taurex-3.1.4a0/taurex/parameter/
+-rw-r--r--   0 ahmed      (501) staff       (20)       44 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/parameter/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    16366 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/parameter/classfactory.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    15314 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/parameter/factory.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    14455 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/parameter/parameterparser.py
+-rw-r--r--   0 ahmed      (501) staff       (20)       77 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/planet.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.715380 taurex-3.1.4a0/taurex/plot/
+-rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/plot/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    21741 2022-04-11 10:54:49.000000 taurex-3.1.4a0/taurex/plot/corner.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    37950 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/plot/plotter.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.717194 taurex-3.1.4a0/taurex/plugins/
+-rw-r--r--   0 ahmed      (501) staff       (20)        0 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/plugins/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      125 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/pressure.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      363 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/spectrum.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      109 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/stellar.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    23748 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/taurex.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      389 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/taurexdefs.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      310 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/temperature.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.735371 taurex-3.1.4a0/taurex/util/
+-rw-r--r--   0 ahmed      (501) staff       (20)      137 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/util/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2895 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/util/emission.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      729 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/util/fitting.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     8887 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/util/fortran.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     5791 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/util/geometry.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     6859 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/util/hdf5.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    10513 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/util/math.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      732 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/util/module.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     9965 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/util/output.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2203 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/util/scattering.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1610 2021-07-01 10:26:34.000000 taurex-3.1.4a0/taurex/util/spectrum.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    16668 2023-07-14 18:36:43.000000 taurex-3.1.4a0/taurex/util/util.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.101554 taurex-3.1.4a0/taurex.egg-info/
+-rwxr-xr-x   0 ahmed      (501) staff       (20)     1847 2023-07-14 18:43:44.000000 taurex-3.1.4a0/taurex.egg-info/PKG-INFO
+-rwxr-xr-x   0 ahmed      (501) staff       (20)    10967 2023-07-14 18:43:45.000000 taurex-3.1.4a0/taurex.egg-info/SOURCES.txt
+-rwxr-xr-x   0 ahmed      (501) staff       (20)        1 2023-07-14 18:43:44.000000 taurex-3.1.4a0/taurex.egg-info/dependency_links.txt
+-rwxr-xr-x   0 ahmed      (501) staff       (20)       92 2023-07-14 18:43:44.000000 taurex-3.1.4a0/taurex.egg-info/entry_points.txt
+-rwxr-xr-x   0 ahmed      (501) staff       (20)       91 2023-07-14 18:43:44.000000 taurex-3.1.4a0/taurex.egg-info/requires.txt
+-rwxr-xr-x   0 ahmed      (501) staff       (20)       13 2023-07-14 18:43:44.000000 taurex-3.1.4a0/taurex.egg-info/top_level.txt
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.749789 taurex-3.1.4a0/tests/
+-rw-r--r--   0 ahmed      (501) staff       (20)        0 2021-07-01 10:26:34.000000 taurex-3.1.4a0/tests/__init__.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.758475 taurex-3.1.4a0/tests/benchmark/
+-rw-r--r--   0 ahmed      (501) staff       (20)      941 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/benchmark/test_bb.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2798 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/benchmark/test_bilinear_interps.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     3935 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/benchmark/test_contrib_funcs.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1077 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/benchmark/test_emission_funcs.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      903 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/benchmark/test_forward_model.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1499 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/benchmark/test_linear_interps.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.765371 taurex-3.1.4a0/tests/chemistry/
+-rw-r--r--   0 ahmed      (501) staff       (20)        0 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/chemistry/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2685 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/chemistry/test_chemistry.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      906 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/chemistry/test_constantgas.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     4890 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/chemistry/test_free_chemistry.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2310 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/chemistry/test_powergas.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.768179 taurex-3.1.4a0/tests/cia/
+-rw-r--r--   0 ahmed      (501) staff       (20)        0 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/cia/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2796 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/cia/test_cia.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.771710 taurex-3.1.4a0/tests/citation/
+-rw-r--r--   0 ahmed      (501) staff       (20)        0 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/citation/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      382 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/citation/test_citation.py
+-rw-r--r--   0 ahmed      (501) staff       (20)       81 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/conftest.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.777119 taurex-3.1.4a0/tests/factory/
+-rw-r--r--   0 ahmed      (501) staff       (20)        0 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/factory/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      911 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/factory/test_classfactory.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1898 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/factory/test_factories.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2280 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/factory/test_mixin.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.780008 taurex-3.1.4a0/tests/fixtures/
+-rw-r--r--   0 ahmed      (501) staff       (20)        0 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/fixtures/__init__.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.790072 taurex-3.1.4a0/tests/fixtures/opacities/
+-rw-r--r--   0 ahmed      (501) staff       (20)      361 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/fixtures/opacities/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      757 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/fixtures/opacities/genopacs.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.793811 taurex-3.1.4a0/tests/fixtures/profiles/
+-rw-r--r--   0 ahmed      (501) staff       (20)        0 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/fixtures/profiles/__init__.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.806380 taurex-3.1.4a0/tests/fixtures/spectra/
+-rw-r--r--   0 ahmed      (501) staff       (20)      349 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/fixtures/spectra/__init__.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.813568 taurex-3.1.4a0/tests/model/
+-rw-r--r--   0 ahmed      (501) staff       (20)        0 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/model/__init__.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.828014 taurex-3.1.4a0/tests/optimizer/
+-rw-r--r--   0 ahmed      (501) staff       (20)     2764 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/optimizer/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      820 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/optimizer/test_nestle.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     6377 2023-07-14 18:39:11.000000 taurex-3.1.4a0/tests/optimizer/test_optimizer.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.830022 taurex-3.1.4a0/tests/output/
+-rw-r--r--   0 ahmed      (501) staff       (20)        0 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/output/__init__.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.842276 taurex-3.1.4a0/tests/parameter/
+-rw-r--r--   0 ahmed      (501) staff       (20)        2 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/parameter/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2696 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/parameter/test_keywords.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.855197 taurex-3.1.4a0/tests/priors/
+-rw-r--r--   0 ahmed      (501) staff       (20)        0 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/priors/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2721 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/priors/test_nonuniform.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      468 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/priors/test_priors.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.859955 taurex-3.1.4a0/tests/spectrum/
+-rw-r--r--   0 ahmed      (501) staff       (20)        0 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/spectrum/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    12076 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/spectrum/test_spectrum.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.866622 taurex-3.1.4a0/tests/stellar/
+-rw-r--r--   0 ahmed      (501) staff       (20)        0 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/stellar/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      662 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/stellar/test_blackbody.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1783 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/stellar/test_phoenix.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.868740 taurex-3.1.4a0/tests/strategies/
+-rw-r--r--   0 ahmed      (501) staff       (20)     7761 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/strategies/__init__.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.883010 taurex-3.1.4a0/tests/temperature/
+-rw-r--r--   0 ahmed      (501) staff       (20)        0 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/temperature/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2782 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/temperature/test_guillot.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      848 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/temperature/test_isothermal.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     4613 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/temperature/test_npoint.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1106 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/test_binning.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     3866 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/test_core.py
+-rw-r--r--   0 ahmed      (501) staff       (20)    16461 2021-07-01 10:26:34.000000 taurex-3.1.4a0/tests/test_modelload.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     4533 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/test_opac.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2363 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/test_pressure.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.900861 taurex-3.1.4a0/tests/util/
+-rw-r--r--   0 ahmed      (501) staff       (20)        0 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/util/__init__.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     1231 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/util/test_emission.py
+-rw-r--r--   0 ahmed      (501) staff       (20)      942 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/util/test_fitting.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     3192 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/util/test_math.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     5842 2023-07-14 18:36:43.000000 taurex-3.1.4a0/tests/util/test_util.py
+drwxr-xr-x   0 ahmed      (501) staff       (20)        0 2023-07-14 18:43:46.909677 taurex-3.1.4a0/tools/
+-rw-r--r--   0 ahmed      (501) staff       (20)     4610 2021-07-01 10:26:34.000000 taurex-3.1.4a0/tools/exocross_to_hdf5.py
+-rw-r--r--   0 ahmed      (501) staff       (20)     2133 2021-07-01 10:26:34.000000 taurex-3.1.4a0/tools/pickle_to_properformat.py
```

### Comparing `taurex-3.1.1a0/.bumpversion.cfg` & `taurex-3.1.4a0/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 3.1.1-alpha
+current_version = 3.1.4-alpha
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}
 	{major}.{minor}.{patch}
 	{major}.{minor}
```

### Comparing `taurex-3.1.1a0/.github/workflows/test-taurex.yml` & `taurex-3.1.4a0/.github/workflows/test-taurex.yml`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/.github/workflows/upload-test.yml` & `taurex-3.1.4a0/.github/workflows/upload-test.yml`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/.gitignore` & `taurex-3.1.4a0/.gitignore`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/.readthedocs.yaml` & `taurex-3.1.4a0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/CHANGELOG` & `taurex-3.1.4a0/CHANGELOG`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/CONTRIBUTING.md` & `taurex-3.1.4a0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/LICENSE` & `taurex-3.1.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/PKG-INFO` & `taurex-3.1.4a0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,84 +1,16 @@
 Metadata-Version: 2.1
 Name: taurex
-Version: 3.1.1a0
+Version: 3.1.4a0
 Summary: TauREx 3 retrieval framework
 Home-page: https://github.com/ucl-exoplanets/TauREx3_public/
 Author: Ahmed Faris Al-Refaie
 Author-email: ahmed.al-refaie.12@ucl.ac.uk
 License: BSD
-Description: # TauREx 3
-        
-        ![Python package](https://github.com/ucl-exoplanets/TauREx3/workflows/Python%20package/badge.svg)
-        
-        TauREx 3 is the newest version of the TauREx retrieval code.
-        
-        Documentation can be found [here](https://taurex3-public.readthedocs.io/en/latest/)
-        
-        Current build: 3.1.1-alpha
-        
-        ## Prerequisites
-        
-        * numpy
-        
-        
-        
-        ## Installing from PyPi
-        
-        
-        You can install it by doing
-        
-        ```
-        pip install taurex
-        ```
-        
-        
-        ## Installing from source
-        
-        
-        Clone the directory using:
-        
-        ```
-        git clone https://github.com/ucl-exoplanets/TauREx3_public.git
-        ```
-        
-        Move into the TauREx3 folder
-        
-        ```
-        cd TauREx3
-        ```
-        
-        Then install
-        
-        ```
-        pip install .
-        ```
-        
-        To build documentation do
-        
-        ```
-        python setup.py build_sphinx
-        ```
-        
-        
-        Try importing taurex:
-        
-        ```
-        python -c "import taurex; print(taurex.__version__)"
-        ```
-        
-        Or running taurex itself
-        
-        ```
-        taurex
-        ```
-        
-        If there are no errors then it was successful!
 Keywords: exoplanet,retrieval,taurex,taurex3,atmosphere,atmospheric
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
@@ -87,7 +19,76 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Provides: taurex
 Description-Content-Type: text/markdown
 Provides-Extra: Plot
+License-File: LICENSE
+
+# TauREx 3
+
+![Python package](https://github.com/ucl-exoplanets/TauREx3/workflows/Python%20package/badge.svg)
+
+TauREx 3 is the newest version of the TauREx retrieval code.
+
+Documentation can be found [here](https://taurex3-public.readthedocs.io/en/latest/)
+
+Current build: 3.1.4-alpha
+
+## Prerequisites
+
+* numpy
+
+
+
+## Installing from PyPi
+
+
+You can install it by doing
+
+```
+pip install taurex
+```
+
+
+## Installing from source
+
+
+Clone the directory using:
+
+```
+git clone https://github.com/ucl-exoplanets/TauREx3_public.git
+```
+
+Move into the TauREx3 folder
+
+```
+cd TauREx3
+```
+
+Then install
+
+```
+pip install .
+```
+
+To build documentation do
+
+```
+python setup.py build_sphinx
+```
+
+
+Try importing taurex:
+
+```
+python -c "import taurex; print(taurex.__version__)"
+```
+
+Or running taurex itself
+
+```
+taurex
+```
+
+If there are no errors then it was successful!
```

### Comparing `taurex-3.1.1a0/README.md` & `taurex-3.1.4a0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ![Python package](https://github.com/ucl-exoplanets/TauREx3/workflows/Python%20package/badge.svg)
 
 TauREx 3 is the newest version of the TauREx retrieval code.
 
 Documentation can be found [here](https://taurex3-public.readthedocs.io/en/latest/)
 
-Current build: 3.1.1-alpha
+Current build: 3.1.4-alpha
 
 ## Prerequisites
 
 * numpy
```

### Comparing `taurex-3.1.1a0/doc/Makefile` & `taurex-3.1.4a0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/make.bat` & `taurex-3.1.4a0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/_static/taurex_logo.png` & `taurex-3.1.4a0/doc/source/_static/taurex_logo.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/api/taurex.binning.rst` & `taurex-3.1.4a0/doc/source/api/taurex.binning.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/api/taurex.chemistry.rst` & `taurex-3.1.4a0/doc/source/api/taurex.chemistry.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/api/taurex.contributions.rst` & `taurex-3.1.4a0/doc/source/api/taurex.contributions.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/api/taurex.model.rst` & `taurex-3.1.4a0/doc/source/api/taurex.model.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/api/taurex.opacity.rst` & `taurex-3.1.4a0/doc/source/api/taurex.opacity.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/api/taurex.optimizer.rst` & `taurex-3.1.4a0/doc/source/api/taurex.optimizer.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/api/taurex.output.rst` & `taurex-3.1.4a0/doc/source/api/taurex.output.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/api/taurex.parameter.rst` & `taurex-3.1.4a0/doc/source/api/taurex.parameter.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/api/taurex.spectrum.rst` & `taurex-3.1.4a0/doc/source/api/taurex.spectrum.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/api/taurex.temperature.rst` & `taurex-3.1.4a0/doc/source/api/taurex.temperature.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/api/taurex.util.rst` & `taurex-3.1.4a0/doc/source/api/taurex.util.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/citation.rst` & `taurex-3.1.4a0/doc/source/citation.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/conf.py` & `taurex-3.1.4a0/doc/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 project = 'TauREx'
 copyright = '2019, Ahmed Al-Refaie, Quentin Changeat, Ingo Waldmann, Giovanna Tinetti'
 author = 'Ahmed Al-Refaie'
 
 # The short X.Y version
 sys.path.insert(0, os.path.abspath('../../'))
 # The full version, including alpha/beta/rc tags
-release = '3.1.1-alpha'
+release = '3.1.4-alpha'
 version = '.'.join(release.split('.')[:2])
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `taurex-3.1.1a0/doc/source/devel/_static/Taurex3-framework2.png` & `taurex-3.1.4a0/doc/source/devel/_static/Taurex3-framework2.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/devel/_static/bbnoise.png` & `taurex-3.1.4a0/doc/source/devel/_static/bbnoise.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/devel/_static/phoenixa.png` & `taurex-3.1.4a0/doc/source/devel/_static/phoenixa.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/devel/_static/phoenixb.png` & `taurex-3.1.4a0/doc/source/devel/_static/phoenixb.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/devel/_static/phoenixdenoise.png` & `taurex-3.1.4a0/doc/source/devel/_static/phoenixdenoise.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/devel/_static/phoenixnoise.png` & `taurex-3.1.4a0/doc/source/devel/_static/phoenixnoise.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/devel/_static/random_tp_500.png` & `taurex-3.1.4a0/doc/source/devel/_static/random_tp_500.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/devel/basics.rst` & `taurex-3.1.4a0/doc/source/devel/basics.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/devel/components.rst` & `taurex-3.1.4a0/doc/source/devel/components.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/devel/fittingparameters.rst` & `taurex-3.1.4a0/doc/source/devel/fittingparameters.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/devel/guidelines.rst` & `taurex-3.1.4a0/doc/source/devel/guidelines.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/devel/mixins.rst` & `taurex-3.1.4a0/doc/source/devel/mixins.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/devel/overview.rst` & `taurex-3.1.4a0/doc/source/devel/overview.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/devel/plugins.rst` & `taurex-3.1.4a0/doc/source/devel/plugins.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/index.rst` & `taurex-3.1.4a0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/requirements.txt` & `taurex-3.1.4a0/doc/source/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -64,7 +64,8 @@
 tornado==6.0.3
 traitlets==4.3.3
 urllib3==1.25.7
 wcwidth==0.1.7
 webencodings==0.5.1
 widgetsnbextension==3.5.1
 zipp==0.6.0
+taurex
```

### Comparing `taurex-3.1.1a0/doc/source/user/installation.rst` & `taurex-3.1.4a0/doc/source/user/installation.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/introduction.rst` & `taurex-3.1.4a0/doc/source/user/introduction.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/library/quickstart.ipynb` & `taurex-3.1.4a0/doc/source/user/library/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/mpi.rst` & `taurex-3.1.4a0/doc/source/user/mpi.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/plugins.rst` & `taurex-3.1.4a0/doc/source/user/plugins.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/support_data_formats.rst` & `taurex-3.1.4a0/doc/source/user/support_data_formats.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/ch4_and_h2o.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/ch4_and_h2o.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/co2_and_h2o.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/co2_and_h2o.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/constantgas.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/constantgas.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/contrib.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/contrib.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/firstfm.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/firstfm.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/fm_and_obs.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/fm_and_obs.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/fm_obs_bin.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/fm_obs_bin.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/fm_plots/fm_plots-0.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/fm_plots/fm_plots-0.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/fm_plots/fm_plots-1.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/fm_plots/fm_plots-1.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/fm_plots/fm_plots-2.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/fm_plots/fm_plots-2.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/fm_plots/fm_plots-3.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/fm_plots/fm_plots-3.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/fm_plots/fm_plots-4.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/fm_plots/fm_plots-4.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/full_contrib.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/full_contrib.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/guillot.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/guillot.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/h2o_only.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/h2o_only.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/isothermal.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/isothermal.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/npoint.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/npoint.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/random_tp.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/random_tp.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/random_tp_500.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/random_tp_500.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/random_tp_posterior.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/random_tp_posterior.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/ray_and_cia.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/ray_and_cia.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/retrieval.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/retrieval.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-0.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-0.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-1.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-1.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-2.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-2.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-3.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-3.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-4.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-4.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-5.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/retrieval_plots/retrieval_plots-5.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/rodgers.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/rodgers.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/twolayerabundance.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/twolayerabundance.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/_static/twopointgas.png` & `taurex-3.1.4a0/doc/source/user/taurex/_static/twopointgas.png`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/binning.rst` & `taurex-3.1.4a0/doc/source/user/taurex/binning.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/chemistry.rst` & `taurex-3.1.4a0/doc/source/user/taurex/chemistry.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/custom.rst` & `taurex-3.1.4a0/doc/source/user/taurex/custom.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/derived.rst` & `taurex-3.1.4a0/doc/source/user/taurex/derived.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/fitting.rst` & `taurex-3.1.4a0/doc/source/user/taurex/fitting.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/global.rst` & `taurex-3.1.4a0/doc/source/user/taurex/global.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/index.rst` & `taurex-3.1.4a0/doc/source/user/taurex/index.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/inputfile.rst` & `taurex-3.1.4a0/doc/source/user/taurex/inputfile.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/instrument.rst` & `taurex-3.1.4a0/doc/source/user/taurex/instrument.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/mixins.rst` & `taurex-3.1.4a0/doc/source/user/taurex/mixins.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/models.rst` & `taurex-3.1.4a0/doc/source/user/taurex/models.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/observation.rst` & `taurex-3.1.4a0/doc/source/user/taurex/observation.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/optimizer.rst` & `taurex-3.1.4a0/doc/source/user/taurex/optimizer.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/planet.rst` & `taurex-3.1.4a0/doc/source/user/taurex/planet.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/plotting.rst` & `taurex-3.1.4a0/doc/source/user/taurex/plotting.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/pressure.rst` & `taurex-3.1.4a0/doc/source/user/taurex/pressure.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/quickstart.rst` & `taurex-3.1.4a0/doc/source/user/taurex/quickstart.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/star.rst` & `taurex-3.1.4a0/doc/source/user/taurex/star.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/doc/source/user/taurex/temperature.rst` & `taurex-3.1.4a0/doc/source/user/taurex/temperature.rst`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/examples/library/chemistry_randomizer.py` & `taurex-3.1.4a0/examples/library/chemistry_randomizer.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/examples/library/example_chem.py` & `taurex-3.1.4a0/examples/library/example_chem.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/examples/library/example_inst.py` & `taurex-3.1.4a0/examples/library/example_inst.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/examples/library/example_temp.py` & `taurex-3.1.4a0/examples/library/example_temp.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/examples/notebooks/quickstart.ipynb` & `taurex-3.1.4a0/examples/notebooks/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/examples/parfiles/custom_chemistry.par` & `taurex-3.1.4a0/examples/parfiles/custom_chemistry.par`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/examples/parfiles/custom_selfretrieval.par` & `taurex-3.1.4a0/examples/parfiles/custom_selfretrieval.par`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/examples/parfiles/custom_temp.par` & `taurex-3.1.4a0/examples/parfiles/custom_temp.par`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/examples/parfiles/emission_secondary.par` & `taurex-3.1.4a0/examples/parfiles/emission_secondary.par`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/examples/parfiles/multinest.par` & `taurex-3.1.4a0/examples/parfiles/multinest.par`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/examples/parfiles/nestle.par` & `taurex-3.1.4a0/examples/parfiles/nestle.par`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/examples/parfiles/quickstart.dat` & `taurex-3.1.4a0/examples/parfiles/quickstart.dat`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/examples/parfiles/quickstart.par` & `taurex-3.1.4a0/examples/parfiles/quickstart.par`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/examples/parfiles/transmission_equil.par` & `taurex-3.1.4a0/examples/parfiles/transmission_equil.par`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/examples/parfiles/transmission_model.par` & `taurex-3.1.4a0/examples/parfiles/transmission_model.par`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/setup.py` & `taurex-3.1.4a0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     'Operating System :: OS Independent',
     'Programming Language :: Python',
     'Topic :: Scientific/Engineering',
     'Topic :: Software Development :: Libraries',
 ]
 
 # Handle versioning
-version = '3.1.1-alpha'
+version = '3.1.4-alpha'
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='taurex',
       author='Ahmed Faris Al-Refaie',
       author_email='ahmed.al-refaie.12@ucl.ac.uk',
```

### Comparing `taurex-3.1.1a0/taurex/_citation.py` & `taurex-3.1.4a0/taurex/_citation.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/binning/binner.py` & `taurex-3.1.4a0/taurex/binning/binner.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/binning/fluxbinner.py` & `taurex-3.1.4a0/taurex/binning/fluxbinner.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/binning/lightcurvebinner.py` & `taurex-3.1.4a0/taurex/binning/lightcurvebinner.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/binning/nativebinner.py` & `taurex-3.1.4a0/taurex/binning/nativebinner.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/binning/simplebinner.py` & `taurex-3.1.4a0/taurex/binning/simplebinner.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/cache/ciaacache.py` & `taurex-3.1.4a0/taurex/cache/ciaacache.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/cache/ktablecache.py` & `taurex-3.1.4a0/taurex/cache/ktablecache.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/cache/opacitycache.py` & `taurex-3.1.4a0/taurex/cache/opacitycache.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/cache/singleton.py` & `taurex-3.1.4a0/taurex/cache/singleton.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/cia/cia.py` & `taurex-3.1.4a0/taurex/cia/cia.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/cia/hitrancia.py` & `taurex-3.1.4a0/taurex/cia/hitrancia.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module contains classes that handle loading of HITRAN cia files"""
 from .cia import CIA
 import numpy as np
 from taurex.util.math import interp_lin_only
+from taurex.log import Logger
 
 
 class EndOfHitranCIAException(Exception):
     """
     An exception that occurs when the end of a HITRAN file
     is reached
     """
@@ -15,15 +16,15 @@
 def hashwn(start_wn, end_wn):
     """
     Simple wavenumber hash function
     """
     return str(start_wn)+str(end_wn)
 
 
-class HitranCiaGrid(object):
+class HitranCiaGrid(Logger):
     """
     Class that handles a particular HITRAN cia wavenumber grid
     Since temperatures for CIA sometimes have different wavenumber grids this
     class helps to simplify managing them by only dealing with one at a time.
     These will help us unify into a single grid eventually
 
     Parameters
@@ -33,14 +34,15 @@
 
     wn_max : float
         The maximum wavenumber for this grid
 
     """
 
     def __init__(self, wn_min, wn_max):
+        super().__init__(self.__class__.__name__)
         self.wn = None
         self.Tsigma = []
 
     def add_temperature(self, T, sigma):
         """
         Adds a temeprature and crossection to this wavenumber grid
```

### Comparing `taurex-3.1.1a0/taurex/cia/picklecia.py` & `taurex-3.1.4a0/taurex/cia/picklecia.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/constants.py` & `taurex-3.1.4a0/taurex/constants.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/contributions/absorption.py` & `taurex-3.1.4a0/taurex/contributions/absorption.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/contributions/cia.py` & `taurex-3.1.4a0/taurex/contributions/cia.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/contributions/contribution.py` & `taurex-3.1.4a0/taurex/contributions/contribution.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/contributions/flatmie.py` & `taurex-3.1.4a0/taurex/contributions/flatmie.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/contributions/hm.py` & `taurex-3.1.4a0/taurex/contributions/hm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
  
 from .contribution import Contribution, contribute_tau
 import numpy as np
 from taurex.data.fittable import fitparam
 from taurex.exceptions import InvalidModelException
-
+import warnings
 
 class HydrogenIon(Contribution):
 
 
     def __init__(self):
         super().__init__('HydrogenIon')
         self.photo_thresh = 1.6419
@@ -17,27 +17,27 @@
     def build(self, model):
         pass
 
     def finalize(self, model):
         raise NotImplementedError
 
     def f(self, lamb):
-
         C_n = np.array([1, 52.519, 49.534, -118.858, 92.536, -34.194, 4.982])
         n = np.arange(C_n.shape[0])
-
-        return np.sum(C_n[...,None] * ((1 / lamb[None,...] - 1 / self.photo_thresh) ** (n[...,None] / 2)),axis=0)
-
-
-
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            to_ret = np.sum(C_n[...,None] * ((1 / lamb[None,...] - 1 / self.photo_thresh) ** (n[...,None] / 2)),axis=0)
+        return to_ret
         #return np.nan_to_num(sum([c * ((1 / lamb - 1 / self.photo_thresh) ** (n / 2)) for n, c in enumerate(C_n)]))
 
     def sigma_pd(self, lamb):
-
-        return np.nan_to_num(1e-18 * (lamb ** 3) * (1 / lamb - 1 / self.photo_thresh) ** (3 / 2) * self._f_res)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            to_ret = np.nan_to_num(1e-18 * (lamb ** 3) * (1 / lamb - 1 / self.photo_thresh) ** (3 / 2) * self._f_res)
+        return to_ret
 
     def k_bf(self, lamb, T):
         return 0.750 * T ** (-5 / 2) * np.exp(self.alpha / (self.photo_thresh * T)) * (
                     1 - np.exp(-self.alpha / (lamb * T))) * self.sigma_pd(lamb)
 
     def k_ff(self, lamb, T):
```

### Comparing `taurex-3.1.1a0/taurex/contributions/leemie.py` & `taurex-3.1.4a0/taurex/contributions/leemie.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/contributions/rayleigh.py` & `taurex-3.1.4a0/taurex/contributions/rayleigh.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/contributions/simpleclouds.py` & `taurex-3.1.4a0/taurex/contributions/simpleclouds.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/core/__init__.py` & `taurex-3.1.4a0/taurex/core/__init__.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/core/priors.py` & `taurex-3.1.4a0/taurex/core/priors.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/citation.py` & `taurex-3.1.4a0/taurex/data/citation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,46 @@
+from functools import lru_cache
+from urllib.error import HTTPError, URLError
 from pybtex.database import Entry
 
 
 def cleanup_string(string):
     return string.replace('{', '').replace('}', '').replace('\\', '')
 
+
 def recurse_bibtex(obj, entries):
     for b in obj.__class__.__bases__:
         if issubclass(b, Citable):
             entries.extend(b.BIBTEX_ENTRIES)
             recurse_bibtex(b, entries)
 
+
 def stringify_people(authors):
 
     return ', '.join([cleanup_string(str(p)) for p in authors])
 
+
 def unique_citations_only(citations):
 
     current_citations = []
     for c in citations:
         if c not in current_citations:
             current_citations.append(c)
     return current_citations
 
+
 def to_bibtex(citations):
     import uuid
     from pybtex.database import BibliographyData
     entries = {str(uuid.uuid4())[:8]: b for b in citations}
     bib_data = BibliographyData(entries=entries)
 
     return bib_data.to_string('bibtex')
 
 
-
 def handle_publication(fields):
     journal = []
     if 'journal' in fields:
         journal.append(cleanup_string(fields['journal']))
     elif 'booktitle' in fields:
         journal.append(cleanup_string(fields['booktitle']))
     elif 'archivePrefix' in fields:
@@ -58,14 +63,18 @@
 
 
 def construct_nice_printable_string(entry, indent=0):
 
     mystring = ''
     indent = ''.join(['\t']*indent)
     form = f'{indent}%s\n'
+    
+    if isinstance(entry, str):
+        return f'Found non bibtex citation: {entry}\n'
+
 
     if 'title' in entry.fields:
         mystring += form % cleanup_string(entry.fields['title'])
 
     people = entry.persons
     if 'author' in people:
         mystring += form % stringify_people(people['author'])
@@ -81,14 +90,15 @@
     information.
     """
 
     BIBTEX_ENTRIES = []
     """
     List of bibtext entries
     """
+
     def citations(self):
         entries = self.BIBTEX_ENTRIES[:]
         recurse_bibtex(self, entries)
         all_citations = [Entry.from_string(b, 'bibtex')
                          for b in entries]
 
         return unique_citations_only(all_citations)
@@ -98,7 +108,29 @@
         entries = self.citations()
 
         if len(entries) == 0:
             return ''
 
         return '\n'.join([construct_nice_printable_string(e)
                           for e in entries])
+
+
+@lru_cache(maxsize=100)
+def doi_to_bibtex(doi):
+    import urllib
+    BASE_URL = 'http://dx.doi.org/'
+    url = BASE_URL + doi
+
+    req = urllib.request.Request(url)
+    req.add_header('Accept', 'application/x-bibtex')
+    try:
+        with urllib.request.urlopen(req) as f:
+            return f.read().decode()
+    except HTTPError as e:
+        if e.code == 404:
+            print('DOI not found.')
+        else:
+            print('Service unavailable.')
+
+        return None
+    except URLError:
+        return None
```

### Comparing `taurex-3.1.1a0/taurex/data/fittable.py` & `taurex-3.1.4a0/taurex/data/fittable.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/planet.py` & `taurex-3.1.4a0/taurex/data/planet.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/chemistry/autochemistry.py` & `taurex-3.1.4a0/taurex/data/profiles/chemistry/autochemistry.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/chemistry/chemistry.py` & `taurex-3.1.4a0/taurex/data/profiles/chemistry/chemistry.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/chemistry/filechemistry.py` & `taurex-3.1.4a0/taurex/data/profiles/chemistry/filechemistry.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/chemistry/gas/arraygas.py` & `taurex-3.1.4a0/taurex/data/profiles/chemistry/gas/arraygas.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/chemistry/gas/constantgas.py` & `taurex-3.1.4a0/taurex/data/profiles/chemistry/gas/constantgas.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/chemistry/gas/gas.py` & `taurex-3.1.4a0/taurex/data/profiles/chemistry/gas/gas.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/chemistry/gas/powergas.py` & `taurex-3.1.4a0/taurex/data/profiles/chemistry/gas/powergas.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/chemistry/gas/twolayergas.py` & `taurex-3.1.4a0/taurex/data/profiles/chemistry/gas/twolayergas.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/chemistry/gas/twopointgas.py` & `taurex-3.1.4a0/taurex/data/profiles/chemistry/gas/twopointgas.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/chemistry/taurexchemistry.py` & `taurex-3.1.4a0/taurex/data/profiles/chemistry/taurexchemistry.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/pressure/arraypressure.py` & `taurex-3.1.4a0/taurex/data/profiles/pressure/arraypressure.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/pressure/filepressure.py` & `taurex-3.1.4a0/taurex/data/profiles/pressure/filepressure.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/pressure/pressureprofile.py` & `taurex-3.1.4a0/taurex/data/profiles/pressure/pressureprofile.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/temperature/file.py` & `taurex-3.1.4a0/taurex/data/profiles/temperature/file.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/temperature/guillot.py` & `taurex-3.1.4a0/taurex/data/profiles/temperature/guillot.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/temperature/isothermal.py` & `taurex-3.1.4a0/taurex/data/profiles/temperature/isothermal.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/temperature/npoint.py` & `taurex-3.1.4a0/taurex/data/profiles/temperature/npoint.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/temperature/rodgers.py` & `taurex-3.1.4a0/taurex/data/profiles/temperature/rodgers.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/temperature/temparray.py` & `taurex-3.1.4a0/taurex/data/profiles/temperature/temparray.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/profiles/temperature/tprofile.py` & `taurex-3.1.4a0/taurex/data/profiles/temperature/tprofile.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/spectrum/array.py` & `taurex-3.1.4a0/taurex/data/spectrum/array.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/spectrum/iraclis.py` & `taurex-3.1.4a0/taurex/data/spectrum/iraclis.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/spectrum/lightcurve.py` & `taurex-3.1.4a0/taurex/data/spectrum/lightcurve.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/spectrum/observed.py` & `taurex-3.1.4a0/taurex/data/spectrum/observed.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/spectrum/spectrum.py` & `taurex-3.1.4a0/taurex/data/spectrum/spectrum.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 
 """
 Contains the basic definition of an observed spectrum for TauRex 3
 """
 
 from taurex.log import Logger
 from taurex.output.writeable import Writeable
+from taurex.core import Fittable
 
 
-class BaseSpectrum(Logger, Writeable):
+class BaseSpectrum(Logger, Fittable, Writeable):
     """
 
     *Abstract class*
 
     A base class where spectrums are loaded (or later created). This
     is used to either plot against the forward model or passed into the 
     optimizer to be used to fit the forward model
@@ -21,15 +22,16 @@
 
     name : str
         Name to be used in logging
 
     """
 
     def __init__(self, name):
-        super().__init__(name)
+        Logger.__init__(self,name)
+        Fittable.__init__(self)
 
     def create_binner(self):
         """
         Creates the appropriate binning object
         """
         from taurex.binning import FluxBinner
 
@@ -136,14 +138,23 @@
         Raises
         ------
         NotImplementedError
 
         """
         raise NotImplementedError
 
+    @property
+    def fittingParameters(self):
+        return self.fitting_parameters()
+
+    @property
+    def derivedParameters(self):
+        return self.derived_parameters()
+
+
     def write(self, output):
         output.write_array('wlgrid', self.wavelengthGrid)
         output.write_array('spectrum', self.spectrum)
         output.write_array('binedges', self.binEdges)
         output.write_array('binwidths', self.binWidths)
         output.write_array('errorbars', self.errorBar)
```

### Comparing `taurex-3.1.1a0/taurex/data/spectrum/taurex.py` & `taurex-3.1.4a0/taurex/data/spectrum/taurex.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/stellar/phoenix.py` & `taurex-3.1.4a0/taurex/data/stellar/phoenix.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/data/stellar/star.py` & `taurex-3.1.4a0/taurex/data/stellar/star.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/instruments/instrument.py` & `taurex-3.1.4a0/taurex/instruments/instrument.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/instruments/instrumentfile.py` & `taurex-3.1.4a0/taurex/instruments/instrumentfile.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/instruments/snr.py` & `taurex-3.1.4a0/taurex/instruments/snr.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/log/logger.py` & `taurex-3.1.4a0/taurex/log/logger.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/mixin/core.py` & `taurex-3.1.4a0/taurex/mixin/core.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/mixin/mixins.py` & `taurex-3.1.4a0/taurex/mixin/mixins.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/model/directimage.py` & `taurex-3.1.4a0/taurex/model/directimage.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/model/emission.py` & `taurex-3.1.4a0/taurex/model/emission.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/model/lightcurve/lightcurve.py` & `taurex-3.1.4a0/taurex/model/lightcurve/lightcurve.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/model/lightcurve/lightcurvedata.py` & `taurex-3.1.4a0/taurex/model/lightcurve/lightcurvedata.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/model/model.py` & `taurex-3.1.4a0/taurex/model/model.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/model/simplemodel.py` & `taurex-3.1.4a0/taurex/model/simplemodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -282,14 +282,15 @@
                                                    Pl,
                                                    mu_profile)
         self.altitude_profile = z[:-1]
         self.scaleheight_profile = H[:-1]
         self.gravity_profile = g[:-1]
         self.altitude_boundaries = z
         self.deltaz = deltaz
+
     @property
     def pressureProfile(self):
         """
         Atmospheric pressure profile in Pa
         """
         return self.pressure.profile
 
@@ -378,19 +379,17 @@
         from taurex.exceptions import InvalidModelException
         from taurex.cache.opacitycache import OpacityCache
         from taurex.cache import GlobalCache
 
         cacher = OpacityCache()
 
         if GlobalCache()['opacity_method'] == 'ktables':
-            from taurex.cache.ktablecache import KTableCache 
+            from taurex.cache.ktablecache import KTableCache
             cacher = KTableCache()
 
-
-
         active_gases = self.chemistry.activeGases
 
         wavenumbergrid = \
             [cacher[gas].wavenumberGrid for gas in active_gases]
 
         current_grid = None
         for wn in wavenumbergrid:
@@ -531,26 +530,19 @@
         samples: 
 
         """
         from taurex.util.math import OnlineVariance
         tp_profiles = OnlineVariance()
         active_gases = OnlineVariance()
         inactive_gases = OnlineVariance()
-        cond = None
-
         has_condensates = self.chemistry.hasCondensates
 
-        if has_condensates:
-            cond = OnlineVariance()
-
+        cond = OnlineVariance() if has_condensates else None
 
-        if binner is not None:
-            binned_spectrum = OnlineVariance()
-        else:
-            binned_spectrum = None
+        binned_spectrum = OnlineVariance() if binner is not None else None
         native_spectrum = OnlineVariance()
 
         for weight in samples():
 
             native_grid, native, tau, _ = self.model(wngrid=wngrid,
                                                      cutoff_grid=False)
 
@@ -566,31 +558,29 @@
 
             native_spectrum.update(native, weight=weight)
 
             if binned_spectrum is not None:
                 binned = binner.bindown(native_grid, native)[1]
                 binned_spectrum.update(binned, weight=weight)
 
-        profile_dict = {}
-        spectrum_dict = {}
-
         tp_std = np.sqrt(tp_profiles.parallelVariance())
         active_std = np.sqrt(active_gases.parallelVariance())
         inactive_std = np.sqrt(inactive_gases.parallelVariance())
 
-        profile_dict['temp_profile_std'] = tp_std
-        profile_dict['active_mix_profile_std'] = active_std
-        profile_dict['inactive_mix_profile_std'] = inactive_std
+        profile_dict = {
+            'temp_profile_std': tp_std,
+            'active_mix_profile_std': active_std,
+            'inactive_mix_profile_std': inactive_std,
+        }
+
         if cond is not None:
             profile_dict['condensate_profile_std'] = \
                 np.sqrt(cond.parallelVariance())
 
-        spectrum_dict['native_std'] = \
-            np.sqrt(native_spectrum.parallelVariance())
-
+        spectrum_dict = {'native_std': np.sqrt(native_spectrum.parallelVariance())}
         if binned_spectrum is not None:
             spectrum_dict['binned_std'] = \
                 np.sqrt(binned_spectrum.parallelVariance())
 
         return profile_dict, spectrum_dict
 
     def path_integral(self, wngrid, return_contrib):
@@ -598,31 +588,62 @@
 
     def generate_profiles(self):
         from taurex.util.output import generate_profile_dict
         prof = generate_profile_dict(self)
         prof['mu_profile'] = self.chemistry.muProfile
         return prof
 
-
-
     def write(self, output):
         # Run a model if needed
         self.model()
 
         model = super().write(output)
 
         self._chemistry.write(model)
         self._temperature_profile.write(model)
         self.pressure.write(model)
         self._planet.write(model)
         self._star.write(model)
         return model
 
     def citations(self):
+        from taurex.cache import OpacityCache
+        from taurex.cache.ktablecache import KTableCache
+        from taurex.data.citation import unique_citations_only
+
         model_citations = super().citations()
         model_citations.extend(self.chemistry.citations())
         model_citations.extend(self.temperature.citations())
         model_citations.extend(self.pressure.citations())
         model_citations.extend(self.planet.citations())
         model_citations.extend(self.star.citations())
 
-        return model_citations
+        # Get cache citations
+        active_gases = self.chemistry.activeGases
+
+        opacitycache = OpacityCache()
+
+        # Do cross sections
+
+        for g in active_gases:
+
+            try:
+                xsec = opacitycache.opacity_dict[g]
+                model_citations.extend(
+                    xsec.citations()
+
+                )
+            except KeyError:
+                continue
+
+        # # Now Ktables
+        # for g in active_gases:
+
+        #     try:
+        #         model_citations.extend(
+        #             ktablecache.opacity_dict[g].citations()
+
+        #         )
+        #     except KeyError:
+        #         continue
+
+        return unique_citations_only(model_citations)
```

### Comparing `taurex-3.1.1a0/taurex/model/transmission.py` & `taurex-3.1.4a0/taurex/model/transmission.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/mpi.py` & `taurex-3.1.4a0/taurex/mpi.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/opacity/exotransmit.py` & `taurex-3.1.4a0/taurex/opacity/ktables/picklektable.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,114 +1,107 @@
-import pathlib
-from taurex.opacity.interpolateopacity import InterpolatingOpacity
+from ..interpolateopacity import InterpolatingOpacity
+import pickle
 import numpy as np
+import pathlib
+from .ktable import KTable
 
 
-class ExoTransmitOpacity(InterpolatingOpacity):
-
+class PickleKTable(KTable, InterpolatingOpacity):
+    """
+    This is the base class for computing opactities
+    """
 
     @classmethod
     def discover(cls):
         import os
         import glob
         import pathlib
         from taurex.cache import GlobalCache
         from taurex.util.util import sanitize_molecule_string
 
-        path = GlobalCache()['xsec_path']
+        path = GlobalCache()['ktable_path']
         if path is None:
             return []
-        path = os.path.join(path, '*.dat')
+        path = os.path.join(path, '*.pickle')
 
         files = glob.glob(path)
 
         discovery = []
 
         interp = GlobalCache()['xsec_interpolation'] or 'linear'
 
         for f in files:
-            mol_name = sanitize_molecule_string(pathlib.Path(f).stem[4:])
+            splits = pathlib.Path(f).stem.split('.')
+            mol_name = sanitize_molecule_string(splits[0])
+
             discovery.append((mol_name, [f, interp]))
 
         return discovery
 
-
     def __init__(self, filename, interpolation_mode='linear'):
-
-        super().__init__('ExoOpacity:{}'.format(
-                            pathlib.Path(filename).stem[4:]),
-                         interpolation_mode=interpolation_mode)
+        super().__init__('PickleKtable:{}'.format(pathlib.Path(filename).stem[0:10]),
+                        interpolation_mode=interpolation_mode)
 
         self._filename = filename
-        self._molecule_name = pathlib.Path(filename).stem[4:]
-        self._load_exo_transmit(filename)
+        self._molecule_name = None
+        self._spec_dict = None
+        self._resolution = None
+        self._load_pickle_file(filename)
+        
+        
+    @property
+    def moleculeName(self):
+        return self._molecule_name
 
-    def _load_exo_transmit(self, filename):
-        self.debug('Loading opacity from {}'.format(filename))
+    @property
+    def xsecGrid(self):
+        return self._xsec_grid
 
-        with open(filename, 'r') as f:
-            lines = f.readlines()
 
-        self._temperature_grid = np.array(
-            [float(l) for l in lines[0].split()])  # *t_conversion
+    def _load_pickle_file(self, filename):
 
-        self._pressure_grid = np.array(
-            [float(l) for l in lines[1].split()])*1e5
+        #Load the pickle file
+        self.info('Loading opacity from {}'.format(filename))
+        try:
+            with open(filename, 'rb') as f:
+                self._spec_dict = pickle.load(f)
+        except UnicodeDecodeError:
+            with open(filename, 'rb') as f:
+                self._spec_dict = pickle.load(f, encoding='latin1')       
+        
+        self._wavenumber_grid = self._spec_dict['bin_centers']
+        self._ngauss = self._spec_dict['ngauss']
+        self._temperature_grid = self._spec_dict['t']
+        self._pressure_grid = self._spec_dict['p']*1e5
+        self._xsec_grid = self._spec_dict['kcoeff']
+        self._weights = self._spec_dict['weights']
+        self._molecule_name = self._spec_dict['name']
 
         self._min_pressure = self._pressure_grid.min()
         self._max_pressure = self._pressure_grid.max()
         self._min_temperature = self._temperature_grid.min()
         self._max_temperature = self._temperature_grid.max()
+        self.clean_molecule_name()
 
-        wn_grid = []
-
-        for ln in lines[2:]:
-            arr = np.array([float(l) for l in ln.split()])
-            if arr.shape[0] == 1:
-                wn_grid.append(10000*1e-6/arr[0])
-
-        wn_grid = np.array(wn_grid)
-
-        grid_sort = wn_grid.argsort()
-        self._wavenumber_grid = wn_grid[grid_sort]
-
-        pressure_count = 0
-        lambda_count = -1
-        self._xsec_grid = np.empty(shape=(self.pressureGrid.shape[0],
-                                          self.temperatureGrid.shape[0],
-                                          self.wavenumberGrid.shape[0]))
-
-        for ln in lines[2:]:
-            arr = np.array([float(l) for l in ln.split()])
-            if arr.shape[0] == 1:
-                lambda_count += 1
-                pressure_count = 0
-            else:
-                self._xsec_grid[pressure_count, :,
-                                lambda_count] = arr[1:] + 1e-60
-                pressure_count += 1
-
-        self._xsec_grid = self._xsec_grid[:, :, grid_sort]*10000
+    def clean_molecule_name(self):
+        splits = self.moleculeName.split('_')
+        self._molecule_name = splits[0]
 
     @property
     def wavenumberGrid(self):
         return self._wavenumber_grid
 
     @property
     def temperatureGrid(self):
         return self._temperature_grid
-
+    
     @property
     def pressureGrid(self):
         return self._pressure_grid
 
     @property
     def resolution(self):
         return self._resolution
 
     @property
-    def moleculeName(self):
-        return self._molecule_name
-
-    @property
-    def xsecGrid(self):
-        return self._xsec_grid
+    def weights(self):
+        return self._weights
```

### Comparing `taurex-3.1.1a0/taurex/opacity/fakeopacity.py` & `taurex-3.1.4a0/taurex/opacity/fakeopacity.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/opacity/hdf5opacity.py` & `taurex-3.1.4a0/taurex/opacity/ktables/hdfktable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,132 +1,123 @@
-from .interpolateopacity import InterpolatingOpacity
-import pickle
+from ..interpolateopacity import InterpolatingOpacity
+import h5py
 import numpy as np
 import pathlib
-from taurex.mpi import allocate_as_shared
+from taurex.util.util import sanitize_molecule_string
+from .ktable import KTable
 
-class HDF5Opacity(InterpolatingOpacity):
-    """
-    This is the base class for computing opactities
 
+class HDF5KTable(KTable, InterpolatingOpacity):
     """
-
-    @classmethod
-    def priority(cls):
-        return 5
-
+    This is the base class for computing opactities using correlated k tables
+    """
+    
     @classmethod
     def discover(cls):
         import os
         import glob
         import pathlib
         from taurex.cache import GlobalCache
-        from taurex.util.util import sanitize_molecule_string
-
-        path = GlobalCache()['xsec_path']
+        
+        path = GlobalCache()['ktable_path']
         if path is None:
             return []
-        path = [os.path.join(path, '*.h5'), os.path.join(path, '*.hdf5')]
-        file_list = [f for glist in path for f in glob.glob(glist)]
+        path = os.path.join(path, '*.hdf5')
+
+        files = glob.glob(path) + \
+            glob.glob(os.path.join(GlobalCache()['ktable_path'], '*.h5'))
 
         discovery = []
 
         interp = GlobalCache()['xsec_interpolation'] or 'linear'
-        mem = GlobalCache()['xsec_in_memory'] or True
 
-        for f in file_list:
-            op = HDF5Opacity(f, interpolation_mode='linear', in_memory=False)
-            mol_name = op.moleculeName
-            discovery.append((mol_name, [f, interp, mem]))
-            #op._spec_dict.close()
-            del op
+        for f in files:
+            splits = pathlib.Path(f).stem.split('_')
+            mol_name = sanitize_molecule_string(splits[0])
+
+            discovery.append((mol_name, [f, interp]))
 
         return discovery
 
 
-    def __init__(self, filename, interpolation_mode='exp', in_memory=False):
-        super().__init__('HDF5Opacity:{}'.format(pathlib.Path(filename).stem[0:10]),
+    def __init__(self, filename, interpolation_mode='linear', in_memory=True):
+        self._molecule_name = sanitize_molecule_string(pathlib.Path(filename).stem.split('_')[0])
+        super().__init__('HDF5Ktable:{}'.format(self._molecule_name),
                          interpolation_mode=interpolation_mode)
-
+        self._molecule_name = sanitize_molecule_string(pathlib.Path(filename).stem.split('_')[0])
         self._filename = filename
-        self._molecule_name = None
         self._spec_dict = None
+
+        self._resolution = None
         self.in_memory = in_memory
-        self._load_hdf_file(filename)
+        self._load_pickle_file(filename)
 
     @property
     def moleculeName(self):
         return self._molecule_name
 
     @property
     def xsecGrid(self):
         return self._xsec_grid
 
-    def _load_hdf_file(self, filename):
-        import h5py
+    def _load_pickle_file(self, filename):
         import astropy.units as u
-        # Load the pickle file
-        self.debug('Loading opacity from {}'.format(filename))
-
-        self._spec_dict = h5py.File(filename, 'r')
+        #Load the pickle file
+        self.info('Loading opacity from {}'.format(filename))
 
-        self._wavenumber_grid = self._spec_dict['bin_edges'][:]
-
-        #temperature_units = self._spec_dict['t'].attrs['units']
-        #t_conversion = u.Unit(temperature_units).to(u.K).value
-
-        self._temperature_grid = self._spec_dict['t'][:]  # *t_conversion
+        self._spec_dict = h5py.File(filename, 'r')    
+        
+        self._wavenumber_grid = self._spec_dict['bin_centers'][...].astype(np.float64)
+        self._ngauss = self._spec_dict['ngauss'][()]
+        self._temperature_grid = self._spec_dict['t'][...].astype(np.float64)
 
         pressure_units = self._spec_dict['p'].attrs['units']
         try:
             p_conversion = u.Unit(pressure_units).to(u.Pa)
         except:
             p_conversion = u.Unit(pressure_units, format="cds").to(u.Pa)
 
-        self._pressure_grid = self._spec_dict['p'][:]*p_conversion
 
-        if self.in_memory:
-            self._xsec_grid = allocate_as_shared(self._spec_dict['xsecarr'][...], logger=self)
-        else:
-            self._xsec_grid = self._spec_dict['xsecarr']
+        self._pressure_grid = self._spec_dict['p'][...].astype(np.float64)*p_conversion
 
-        self._resolution = np.average(np.diff(self._wavenumber_grid))
-        self._molecule_name = self._spec_dict['mol_name'][()]
 
-        if isinstance(self._molecule_name, np.ndarray):
-            self._molecule_name = self._molecule_name[0]
-        
-        try:
-            self._molecule_name = self._molecule_name.decode()
-        except (UnicodeDecodeError, AttributeError,):
-            pass
 
-        from taurex.util.util import ensure_string_utf8
-
-        self._molecule_name = ensure_string_utf8(self._molecule_name)
+        if self.in_memory:
+            self._xsec_grid = self._spec_dict['kcoeff'][...].astype(np.float64)
+        else:
+            self._xsec_grid = self._spec_dict['kcoeff']
+        self._weights = self._spec_dict['weights'][...].astype(np.float64)
 
         self._min_pressure = self._pressure_grid.min()
         self._max_pressure = self._pressure_grid.max()
         self._min_temperature = self._temperature_grid.min()
         self._max_temperature = self._temperature_grid.max()
-
+        self.clean_molecule_name()
         if self.in_memory:
             self._spec_dict.close()
-        
+
+    def clean_molecule_name(self):
+        splits = self.moleculeName.split('_')
+        self._molecule_name = splits[0]
 
     @property
     def wavenumberGrid(self):
         return self._wavenumber_grid
 
     @property
     def temperatureGrid(self):
         return self._temperature_grid
-
+    
     @property
     def pressureGrid(self):
         return self._pressure_grid
 
     @property
     def resolution(self):
         return self._resolution
 
-        # return factor*(q_11*(Pmax-P)*(Tmax-T) + q_21*(P-Pmin)*(Tmax-T) + q_12*(Pmax-P)*(T-Tmin) + q_22*(P-Pmin)*(T-Tmin))
+    @property
+    def weights(self):
+        return self._weights
+
+
+        #return factor*(q_11*(Pmax-P)*(Tmax-T) + q_21*(P-Pmin)*(Tmax-T) + q_12*(Pmax-P)*(T-Tmin) + q_22*(P-Pmin)*(T-Tmin))
```

### Comparing `taurex-3.1.1a0/taurex/opacity/interpolateopacity.py` & `taurex-3.1.4a0/taurex/opacity/interpolateopacity.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/opacity/ktables/hdfktable.py` & `taurex-3.1.4a0/taurex/opacity/pickleopacity.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,123 +1,107 @@
-from ..interpolateopacity import InterpolatingOpacity
-import h5py
+from .interpolateopacity import InterpolatingOpacity
+import pickle
 import numpy as np
 import pathlib
 from taurex.util.util import sanitize_molecule_string
-from .ktable import KTable
+from taurex.mpi import allocate_as_shared
 
-
-class HDF5KTable(KTable, InterpolatingOpacity):
+class PickleOpacity(InterpolatingOpacity):
     """
-    This is the base class for computing opactities using correlated k tables
+    This is the base class for computing opactities
+
     """
-    
+
     @classmethod
     def discover(cls):
         import os
         import glob
         import pathlib
         from taurex.cache import GlobalCache
-        
-        path = GlobalCache()['ktable_path']
+        from taurex.util.util import sanitize_molecule_string
+
+        path = GlobalCache()['xsec_path']
         if path is None:
             return []
-        path = os.path.join(path, '*.hdf5')
+        path = os.path.join(path, '*.pickle')
 
-        files = glob.glob(path) + \
-            glob.glob(os.path.join(GlobalCache()['ktable_path'], '*.h5'))
+        files = glob.glob(path)
 
         discovery = []
 
         interp = GlobalCache()['xsec_interpolation'] or 'linear'
 
         for f in files:
-            splits = pathlib.Path(f).stem.split('_')
+            splits = pathlib.Path(f).stem.split('.')
             mol_name = sanitize_molecule_string(splits[0])
 
             discovery.append((mol_name, [f, interp]))
 
         return discovery
 
-
-    def __init__(self, filename, interpolation_mode='linear', in_memory=True):
-        self._molecule_name = sanitize_molecule_string(pathlib.Path(filename).stem.split('_')[0])
-        super().__init__('HDF5Ktable:{}'.format(self._molecule_name),
+    def __init__(self, filename, interpolation_mode='linear'):
+        super().__init__('PickleOpacity:{}'.format(pathlib.Path(filename).stem[0:10]),
                          interpolation_mode=interpolation_mode)
-        self._molecule_name = sanitize_molecule_string(pathlib.Path(filename).stem.split('_')[0])
+
         self._filename = filename
+        self._molecule_name = None
         self._spec_dict = None
-
         self._resolution = None
-        self.in_memory = in_memory
         self._load_pickle_file(filename)
 
     @property
     def moleculeName(self):
         return self._molecule_name
 
     @property
     def xsecGrid(self):
         return self._xsec_grid
 
     def _load_pickle_file(self, filename):
-        import astropy.units as u
-        #Load the pickle file
-        self.info('Loading opacity from {}'.format(filename))
 
-        self._spec_dict = h5py.File(filename, 'r')    
-        
-        self._wavenumber_grid = self._spec_dict['bin_centers'][...].astype(np.float64)
-        self._ngauss = self._spec_dict['ngauss'][()]
-        self._temperature_grid = self._spec_dict['t'][...].astype(np.float64)
-
-        pressure_units = self._spec_dict['p'].attrs['units']
+        # Load the pickle file
+        self.info('Loading opacity from {}'.format(filename))
         try:
-            p_conversion = u.Unit(pressure_units).to(u.Pa)
-        except:
-            p_conversion = u.Unit(pressure_units, format="cds").to(u.Pa)
-
-
-        self._pressure_grid = self._spec_dict['p'][...].astype(np.float64)*p_conversion
-
-
-
-        if self.in_memory:
-            self._xsec_grid = self._spec_dict['kcoeff'][...].astype(np.float64)
-        else:
-            self._xsec_grid = self._spec_dict['kcoeff']
-        self._weights = self._spec_dict['weights'][...].astype(np.float64)
+            with open(filename, 'rb') as f:
+                self._spec_dict = pickle.load(f)
+        except UnicodeDecodeError:
+            with open(filename, 'rb') as f:
+                self._spec_dict = pickle.load(f, encoding='latin1')
+
+        self._wavenumber_grid = self._spec_dict['wno']
+
+        self._temperature_grid = self._spec_dict['t']
+        self._pressure_grid = self._spec_dict['p']*1e5
+        self._xsec_grid = allocate_as_shared(self._spec_dict['xsecarr'], logger=self)
+        self._resolution = np.average(np.diff(self._wavenumber_grid))
+
+        splits = pathlib.Path(filename).stem.split('.')
+        mol_name = sanitize_molecule_string(splits[0])
+        self._molecule_name = mol_name
 
         self._min_pressure = self._pressure_grid.min()
         self._max_pressure = self._pressure_grid.max()
         self._min_temperature = self._temperature_grid.min()
         self._max_temperature = self._temperature_grid.max()
         self.clean_molecule_name()
-        if self.in_memory:
-            self._spec_dict.close()
 
     def clean_molecule_name(self):
         splits = self.moleculeName.split('_')
         self._molecule_name = splits[0]
 
     @property
     def wavenumberGrid(self):
         return self._wavenumber_grid
 
     @property
     def temperatureGrid(self):
         return self._temperature_grid
-    
+
     @property
     def pressureGrid(self):
         return self._pressure_grid
 
     @property
     def resolution(self):
         return self._resolution
 
-    @property
-    def weights(self):
-        return self._weights
-
-
-        #return factor*(q_11*(Pmax-P)*(Tmax-T) + q_21*(P-Pmin)*(Tmax-T) + q_12*(Pmax-P)*(T-Tmin) + q_22*(P-Pmin)*(T-Tmin))
+        # return factor*(q_11*(Pmax-P)*(Tmax-T) + q_21*(P-Pmin)*(Tmax-T) + q_12*(Pmax-P)*(T-Tmin) + q_22*(P-Pmin)*(T-Tmin))
```

### Comparing `taurex-3.1.1a0/taurex/opacity/ktables/ktable.py` & `taurex-3.1.4a0/taurex/opacity/ktables/ktable.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/opacity/ktables/nemesisktables.py` & `taurex-3.1.4a0/taurex/opacity/ktables/nemesisktables.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/opacity/opacity.py` & `taurex-3.1.4a0/taurex/opacity/opacity.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from taurex.log import Logger
+from taurex.core import Citable
 import numpy as np
 
 
-class Opacity(Logger):
+class Opacity(Logger, Citable):
     """
     This is the base class for computing opactities
 
     """
 
     @classmethod
     def discover(cls):
@@ -66,7 +67,21 @@
 
             # total_bins = self.wavenumberGrid[min_max].shape[0]
             # if total_bins > wngrid.shape[0]:
             #     return np.append(np.histogram(self.wavenumberGrid,wngrid, weights=orig)[0]/np.histogram(self.wavenumberGrid,wngrid)[0],0)
 
             # else:
             return np.interp(wngrid, self.wavenumberGrid[wngrid_filter], orig)
+
+    def opacityCitation(self):
+        """
+        Citation for the specific molecular opacity (linelist origin etc)
+
+
+        Returns
+        -------
+        list of str: 
+            List of string with reference information
+
+        """
+        return []
+
```

### Comparing `taurex-3.1.1a0/taurex/optimizer/dypolychord.py` & `taurex-3.1.4a0/taurex/optimizer/dypolychord.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/optimizer/multinest.py` & `taurex-3.1.4a0/taurex/optimizer/multinest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
                  num_params_cluster=None,
                  maximum_modes=100,
                  constant_efficiency_mode=False,
                  evidence_tolerance=0.5,
                  mode_tolerance=-1e90,
                  importance_sampling=False,
                  resume=False,
+                 n_iter_before_update=100,
                  multinest_prefix='1-',
                  verbose_output=True, sigma_fraction=0.1):
         super().__init__('Multinest', observed, model, sigma_fraction)
 
         # sampling chains directory
         self.nest_path = 'chains/'
         self.nclust_par = -1
@@ -34,14 +35,15 @@
         self.sampling_eff = sampling_efficiency
         # number of live points
         self.n_live_points = int(num_live_points)
         # maximum no. of iterations (0=inf)
         self.max_iter = int(max_iterations)
         # search for multiple modes
         self.multimodes = search_multi_modes
+        self.n_iter_before_update = int(n_iter_before_update)
         # parameters on which to cluster, e.g. if nclust_par = 3, it will
         # cluster on the first 3 parameters only.
         # if ncluster_par = -1 it clusters on all parameters
         self.nclust_par = num_params_cluster
         # maximum number of modes
         self.max_modes = int(maximum_modes)
         # run in constant efficiency mode
@@ -73,14 +75,16 @@
     def compute_fit(self):
         import pymultinest
         data = self._observed.spectrum
         datastd = self._observed.errorBar
         sqrtpi = np.sqrt(2*np.pi)
 
         def multinest_loglike(cube, ndim, nparams):
+            data = self._observed.spectrum
+            datastd = self._observed.errorBar
             # log-likelihood function called by multinest
             fit_params_container = np.array(
                 [cube[i] for i in range(len(self.fitting_parameters))])
             chi_t = self.chisq_trans(fit_params_container, data, datastd)
 
             # print('---------START---------')
             # print('chi_t',chi_t)
@@ -120,14 +124,15 @@
         self.info('Beginning fit......')
         pymultinest.run(LogLikelihood=multinest_loglike,
                         Prior=multinest_uniform_prior,
                         n_dims=ndim,
                         multimodal=self.multimodes,
                         n_clustering_params=ncluster,
                         max_modes=self.max_modes,
+                        n_iter_before_update=self.n_iter_before_update,
                         outputfiles_basename=os.path.join(self.dir_multinest,
                                                           self.multinest_prefix),
                         const_efficiency_mode=self.const_eff,
                         importance_nested_sampling=self.imp_sampling,
                         resume=self.resume,
                         verbose=self.verbose,
                         sampling_efficiency=self.sampling_eff,
@@ -330,18 +335,17 @@
             yield solution_idx, opt_map, opt_values, [
                 ('Statistics', {'local log-evidence': self._multinest_output['NEST_stats']['modes'][solution_idx]['local log-evidence'],
                                 'local log-evidence error': self._multinest_output['NEST_stats']['modes'][solution_idx]['local log-evidence error']}),
                 ('fit_params', v['fit_params']),
                 ('tracedata', v['tracedata']),
                 ('weights', v['weights'])]
 
-
     @classmethod
     def input_keywords(self):
-        return ['multinest','pymultinest', ]
+        return ['multinest', 'pymultinest', ]
 
     BIBTEX_ENTRIES = [
         """
         @article{ refId0,
         author = {{Buchner, J.} and {Georgakakis, A.} and {Nandra, K.} and {Hsu, L.} and {Rangel, C.} and {Brightman, M.} and {Merloni, A.} and {Salvato, M.} and {Donley, J.} and {Kocevski, D.}},
         title = {X-ray spectral modelling of the AGN obscuring region in the
             CDFS: Bayesian model selection and catalogue},
@@ -370,8 +374,8 @@
             eprint = {0809.3437},
         primaryClass = {astro-ph},
             adsurl = {https://ui.adsabs.harvard.edu/abs/2009MNRAS.398.1601F},
             adsnote = {Provided by the SAO/NASA Astrophysics Data System}
         }
         """
 
-    ]
+    ]
```

### Comparing `taurex-3.1.1a0/taurex/optimizer/nestle.py` & `taurex-3.1.4a0/taurex/optimizer/nestle.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/optimizer/optimizer.py` & `taurex-3.1.4a0/taurex/optimizer/optimizer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,50 @@
+from re import M
 from taurex.log import Logger, disableLogging, enableLogging
 import numpy as np
 import math
 from taurex import OutputSize
 from taurex.core.priors import PriorMode
 from taurex.data.citation import Citable
 
+
+def compile_params(fitparams, driveparams, fit_priors=None):
+    from taurex.core.priors import Uniform, LogUniform
+
+    fitting_parameters = []
+    fitting_priors = []
+    derived_parameters = []
+    _fit_priors = fit_priors or {}
+
+    for params in fitparams.values():
+        name, latex, fget, fset, mode, to_fit, bounds = params
+
+        #self.debug('Checking fitting parameter {}'.format(params))
+        if to_fit:
+            fitting_parameters.append(params)
+            if name not in _fit_priors:
+                prior = None
+                if mode == 'log':
+                    prior = LogUniform(lin_bounds=bounds)
+
+                else:
+                    prior = Uniform(bounds=bounds)
+                fitting_priors.append(prior)
+                _fit_priors[name] = prior
+            else:
+                fitting_priors.append(_fit_priors[name])
+
+    for params in driveparams.values():
+        name, latex, fget, compute = params
+        if compute:
+            derived_parameters.append(params)
+
+    return fitting_parameters, fitting_priors, _fit_priors, derived_parameters
+
+
 class Optimizer(Logger, Citable):
     """
     A base class that handles fitting and optimization of forward models.
     The class handles the compiling and management of fitting parameters in 
     forward models, in its current form it cannot fit and requires a class 
     derived from it to implement the :func:`compute_fit` function.
 
@@ -36,36 +72,38 @@
         self._model_callback = None
         self._sigma_fraction = sigma_fraction
         self._fit_priors = {}
         self.fitting_parameters = []
         self.fitting_priors = []
 
     def set_model(self, model):
+        from taurex.model import ForwardModel
         """
         Sets the model to be optimized/fit
 
         Parameters
         ----------
         model : :class:`~taurex.model.model.ForwardModel`
             The forward model we wish to optimize
 
         """
-        self._model = model
+        self._model: ForwardModel = model
 
     def set_observed(self, observed):
+        from taurex.spectrum import BaseSpectrum
         """
         Sets the observation to optimize the model to
 
         Parameters
         ----------
         observed : :class:`~taurex.data.spectrum.spectrum.BaseSpectrum`
             Observed spectrum we will optimize to
 
         """
-        self._observed = observed
+        self._observed: BaseSpectrum = observed
         if observed is not None:
             self._binner = observed.create_binner()
 
     def compile_params(self):
         from taurex.core.priors import Uniform, LogUniform
         """ 
         Goes through and compiles all parameters within the model that
@@ -77,37 +115,55 @@
         self.info('Initializing parameters')
         self.fitting_parameters = []
         self.derived_parameters = []
         self.fitting_priors = []
         # param_name,param_latex,
         #                 fget.__get__(self),fset.__get__(self),
         #                         default_fit,default_bounds
-        for params in self._model.fittingParameters.values():
-            name, latex, fget, fset, mode, to_fit, bounds = params
-
-            self.debug('Checking fitting parameter {}'.format(params))
-            if to_fit:
-                self.fitting_parameters.append(params)
-
-                if name not in self._fit_priors:
-                    prior = None
-                    if mode == 'log':
-                        prior = LogUniform(lin_bounds=bounds)
-                        
-                    else:
-                        prior = Uniform(bounds=bounds)
-                    self.fitting_priors.append(prior)
-                    self._fit_priors[name] = prior
-                else:
-                    self.fitting_priors.append(self._fit_priors[name])
+        # for params in self._model.fittingParameters.values():
 
-        for params in self._model.derivedParameters.values():
-            name, latex, fget, compute = params
-            if compute:
-                self.derived_parameters.append(params)
+        self.fitting_parameters, \
+            self.fitting_priors, \
+            _model_priors, \
+            self.derived_parameters = \
+            compile_params(self._model.fittingParameters,
+                           self._model.derivedParameters, self._fit_priors)
+
+        self._fit_priors.update(_model_priors)
+        obs_fit, obs_prior, _obs_priors, obs_deriv = \
+            compile_params(
+                self._observed.fittingParameters,
+                self._observed.derivedParameters, self._fit_priors
+            )
+        self.fitting_parameters.extend(obs_fit)
+        self.fitting_priors.extend(obs_prior)
+        self._fit_priors.update(_obs_priors)
+        self.derived_parameters.extend(obs_deriv)
+        #     name, latex, fget, fset, mode, to_fit, bounds = params
+
+        #     self.debug('Checking fitting parameter {}'.format(params))
+        #     if to_fit:
+        #         self.fitting_parameters.append(params)
+
+        #         if name not in self._fit_priors:
+        #             prior = None
+        #             if mode == 'log':
+        #                 prior = LogUniform(lin_bounds=bounds)
+
+        #             else:
+        #                 prior = Uniform(bounds=bounds)
+        #             self.fitting_priors.append(prior)
+        #             self._fit_priors[name] = prior
+        #         else:
+        #             self.fitting_priors.append(self._fit_priors[name])
+
+        # for params in self._model.derivedParameters.values():
+        #     name, latex, fget, compute = params
+        #     if compute:
+        #         self.derived_parameters.append(params)
 
         self.info('-------FITTING---------------')
         self.info('Parameters to be fit:')
         for params, priors in zip(self.fitting_parameters, self.fitting_priors):
             name, latex, fget, fset, mode, to_fit, bounds = params
             self.info('{}: Value: {} Type:{} Params:{}'.format(
                 name, fget(), priors.__class__.__name__, priors.params()))
@@ -130,15 +186,14 @@
             self.error('Trying to update model with more fitting parameters'
                        ' than enabled')
             self.error(f'No. enabled parameters:{len(self.fitting_parameters)}'
                        f' Update length: {len(fit_params)}')
             raise ValueError('Trying to update model with more fitting'
                              ' parameters than enabled')
 
-
         for value, param, priors in zip(fit_params, self.fitting_parameters, self.fitting_priors):
             name, latex, fget, fset, mode, to_fit, bounds = param
             # if mode == 'log':
             #     value = 10**value
             fset(priors.prior(value))
 
     @property
@@ -167,15 +222,15 @@
         Returns
         -------
         :obj:`list`:
             List of each value of a fitting parameter
 
         """
 
-        return [c[2]() if c[4] == 'linear' else math.log10(c[2]()) 
+        return [c[2]() if c[4] == 'linear' else math.log10(c[2]())
                 for c in self.fitting_parameters]
 
     @property
     def fit_boundaries(self):
         """
 
         Returns the fitting boundaries of the parameter
@@ -220,15 +275,14 @@
             List of parameter names in LaTeX format
 
 
         """
         return [c[1] if self._fit_priors[c[0]].priorMode is PriorMode.LINEAR else 'log({})'.format(c[1])
                 for c in self.fitting_parameters]
 
-
     @property
     def derived_names(self):
         """ 
 
         Returns a list of the current values of a fitting parameter. This 
         respects the ``mode`` setting
 
@@ -237,15 +291,14 @@
         :obj:`list`:
             List of each value of a fitting parameter
 
         """
 
         return [c[0] for c in self.derived_parameters]
 
-
     @property
     def derived_latex(self):
         """ 
 
         Returns a list of the current values of a fitting parameter. This 
         respects the ``mode`` setting
 
@@ -281,57 +334,71 @@
         Parameters
         ----------
         parameter : str
             Name of the parameter we want to fit
 
         """
 
+        obj = self._model if parameter in self._model.fittingParameters \
+            else self._observed
+
         name, latex, fget, fset, mode, to_fit, bounds = \
-            self._model.fittingParameters[parameter]
+            obj.fittingParameters[parameter]
 
         to_fit = True
 
-        self._model.fittingParameters[parameter] = (
+        obj.fittingParameters[parameter] = (
             name, latex, fget, fset, mode, to_fit, bounds)
 
     def enable_derived(self, parameter):
+
+        obj = self._model if parameter in self._model.derivedParameters \
+            else self._observed
+
         name, latex, fget, compute = \
-            self._model.derivedParameters[parameter]
+            obj.derivedParameters[parameter]
         compute = True
-        self._model.derivedParameters[parameter] = (
+        obj.derivedParameters[parameter] = (
             name, latex, fget, compute
         )
 
     def disable_fit(self, parameter):
         """
         Disables fitting of the parameter
 
         Parameters
         ----------
         parameter : str
             Name of the parameter we do not want to fit
 
         """
+
+        obj = self._model if parameter in self._model.fittingParameters \
+            else self._observed
+
         name, latex, fget, fset, mode, to_fit, bounds = \
-            self._model.fittingParameters[parameter]
+            obj.fittingParameters[parameter]
 
         to_fit = False
 
-        self._model.fittingParameters[parameter] = (
+        obj.fittingParameters[parameter] = (
             name, latex, fget, fset, mode, to_fit, bounds)
 
     def disable_derived(self, parameter):
+
+        obj = self._model if parameter in self._model.fittingParameters \
+            else self._observed
+
         name, latex, fget, compute = \
-            self._model.derivedParameters[parameter]
+            obj.derivedParameters[parameter]
         compute = False
-        self._model.derivedParameters[parameter] = (
+        obj.derivedParameters[parameter] = (
             name, latex, fget, compute
         )
 
-
     def set_boundary(self, parameter, new_boundaries):
         """
         Sets the boundary of the parameter
 
         Parameters
         ----------
         parameter : str
@@ -340,20 +407,23 @@
         new_boundaries : tuple of float
             New fitting boundaries, with the form
             ( ``bound_min`` , ``bound_max`` ). These should
             not take into account the ``mode`` setting of a fitting parameter.
 
 
         """
+
+        obj = self._model if parameter in self._model.fittingParameters \
+            else self._observed
         name, latex, fget, fset, mode, to_fit, bounds = \
-            self._model.fittingParameters[parameter]
+            obj.fittingParameters[parameter]
 
         bounds = new_boundaries
 
-        self._model.fittingParameters[parameter] = (
+        obj.fittingParameters[parameter] = (
             name, latex, fget, fset, mode, to_fit, bounds)
 
     def set_factor_boundary(self, parameter, factors):
         """
         Sets the boundary of the parameter based on a factor
 
         Parameters
@@ -364,23 +434,26 @@
         factor : tuple of float
             To be written
 
 
 
         """
 
+        obj = self._model if parameter in self._model.fittingParameters \
+            else self._observed
+
         name, latex, fget, fset, mode, to_fit, bounds = \
-            self._model.fittingParameters[parameter]
+            obj.fittingParameters[parameter]
 
         value = fget()
 
         new_boundaries = factors[0]*value, factors[1]*value
 
         bounds = new_boundaries
-        self._model.fittingParameters[parameter] = (
+        obj.fittingParameters[parameter] = (
             name, latex, fget, fset, mode, to_fit, bounds)
 
     def set_mode(self, parameter, new_mode):
         """
         Sets the fitting mode of a parameter
 
         Parameters
@@ -390,28 +463,34 @@
 
         new_mode : ``linear`` or ``log``
             Sets whether the parameter is fit in linear or log space
 
 
 
         """
+
+        obj = self._model if parameter in self._model.fittingParameters \
+            else self._observed
         new_mode = new_mode.lower()
 
         name, latex, fget, fset, mode, to_fit, bounds = \
-            self._model.fittingParameters[parameter]
+            obj.fittingParameters[parameter]
 
         if new_mode not in ('log', 'linear',):
             self.error('Incorrect mode set for fit parameter,')
             raise ValueError
 
-        self._model.fittingParameters[parameter] = (
+        obj.fittingParameters[parameter] = (
             name, latex, fget, fset, new_mode, to_fit, bounds)
 
     def set_prior(self, parameter, prior):
-        if parameter not in self._model.fittingParameters:
+
+        obj = self._model if parameter in self._model.fittingParameters \
+            else self._observed
+        if parameter not in obj.fittingParameters:
             self.error('Fitting parameter %s does not exist', parameter)
             raise ValueError('Fitting parameter does not exist')
 
         self._fit_priors[parameter] = prior
 
     def chisq_trans(self, fit_params, data, datastd):
         """
@@ -441,23 +520,26 @@
             chi-squared
 
 
         """
         from taurex.exceptions import InvalidModelException
         self.update_model(fit_params)
 
+        mydata = self._observed.spectrum
+        #myerror = self._observed.errorBar
+
         obs_bins = self._observed.wavenumberGrid
 
         try:
             _, final_model, _, _ = self._binner.bin_model(
                 self._model.model(wngrid=obs_bins))
         except InvalidModelException:
             return np.nan
 
-        res = (data.ravel() - final_model.ravel()) / datastd.ravel()
+        res = (mydata.ravel() - final_model.ravel()) / datastd.ravel()
         res = np.nansum(res*res)
         if res == 0:
             res = np.nan
 
         return res
 
     def compute_fit(self):
@@ -482,15 +564,15 @@
         """
         from tabulate import tabulate
         self.compile_params()
 
         fit_names = self.fit_names
 
         prior_type = [p.__class__.__name__ for p in self.fitting_priors]
-        args = [p.params() for p in self.fitting_priors] 
+        args = [p.params() for p in self.fitting_priors]
 
         fit_values = self.fit_values
         self.info('')
         self.info('-------------------------------------')
         self.info('------Retrieval Parameters-----------')
         self.info('-------------------------------------')
         self.info('')
@@ -543,25 +625,24 @@
 
         """
         output.write_string('optimizer', self.__class__.__name__)
         output.write_string_array('fit_parameter_names', self.fit_names)
         output.write_string_array('fit_parameter_latex', self.fit_latex)
         output.write_array('fit_boundary_low', np.array(
             [x.boundaries()[0] for x in self.fitting_priors]))
-        output.write_array('fit_boundary_high', np.array([x.boundaries()[1] for x in self.fitting_priors]))
+        output.write_array('fit_boundary_high', np.array(
+            [x.boundaries()[1] for x in self.fitting_priors]))
         if len(self.derived_names) > 0:
-            output.write_string_array('derived_parameter_names', self.derived_names)
-            output.write_string_array('derived_parameter_latex', self.derived_latex)
+            output.write_string_array(
+                'derived_parameter_names', self.derived_names)
+            output.write_string_array(
+                'derived_parameter_latex', self.derived_latex)
 
         return output
 
-
-
-
-
     def write_fit(self, output):
         """
         Writes basic fitting parameters into output
 
         Parameters
         ----------
         output : :class:`~taurex.output.output.Output` or :class:`~taurex.output.output.OutputGroup`
@@ -611,27 +692,26 @@
         enableLogging()
 
         self.info('I will only iterate through partitioned %s '
                   'points (the rest is in parallel)', len(sample_list)//size)
 
         disableLogging()
 
-
         def sample_iter():
             count = 0
             for parameters, weight in sample_list[rank::size]:
                 self.update_model(parameters)
                 enableLogging()
                 if rank == 0 and count % 10 == 0 and count > 0:
 
                     self.info('Progress {}%'.format(
                         count*100.0 / (len(sample_list)/size)))
                 disableLogging()
                 yield weight
-                count +=1
+                count += 1
 
         return self._model.compute_error(sample_iter, wngrid=binning,
                                          binner=self._binner)
 
     def generate_solution(self, output_size=OutputSize.heavy):
         """
         Generates a dictionary with all solutions and other useful parameters
@@ -639,15 +719,15 @@
         from taurex.util.output import generate_profile_dict, \
             store_contributions
 
         solution_dict = {}
 
         self.info('Post-processing - Generating spectra and profiles')
 
-        # Loop through each solution, grab optimized parameters and anything 
+        # Loop through each solution, grab optimized parameters and anything
         # else we want to store
         for solution, optimized_map, \
                 optimized_median, values in self.get_solution():
 
             enableLogging()
             self.info('Computing solution %s', solution)
             sol_values = {}
@@ -664,17 +744,18 @@
             sol_values['Spectra'] = self._binner.generate_spectrum_output(
                 opt_result, output_size=output_size)
 
             try:
                 sol_values['Spectra']['Contributions'] = store_contributions(
                     self._binner, self._model, output_size=output_size-3)
             except Exception as e:
-                self.warning('Not bothering to store contributions since its broken')
+                self.warning(
+                    'Not bothering to store contributions since its broken')
                 self.warning('%s ', str(e))
-    
+
             # Update with the optimized median
             self.update_model(optimized_median)
 
             self._model.model(cutoff_grid=False)
 
             # Store profiles here
             sol_values['Profiles'] = self._model.generate_profiles()
@@ -691,25 +772,25 @@
                 if k in sol_values['Spectra']:
                     sol_values['Spectra'][k].update(v)
                 else:
                     sol_values['Spectra'][k] = v
 
             solution_dict['solution{}'.format(solution)] = sol_values
 
-
         if len(self.derived_names) > 0:
             #solution_dict[f'solution{solution}']['derived_params'] = {}
             # Compute derived
             for solution, optimized_map, \
                     optimized_median, values in self.get_solution():
                 solution_dict[f'solution{solution}']['derived_params'] = {}
                 derived_dict = self.compute_derived_trace(solution)
                 if derived_dict is None:
                     continue
-                solution_dict[f'solution{solution}']['derived_params'].update(derived_dict)
+                solution_dict[f'solution{solution}']['derived_params'].update(
+                    derived_dict)
 
         enableLogging()
         self.info('Post-processing - Complete')
 
         return solution_dict
 
     def compute_derived_trace(self, solution):
@@ -724,15 +805,15 @@
 
         rank = mpi.get_rank()
 
         num_procs = mpi.nprocs()
 
         count = 0
 
-        derived_param = {p: ([],[]) for p in self.derived_names}
+        derived_param = {p: ([], []) for p in self.derived_names}
 
         weight_comb = []
 
         if len(self.derived_names) == 0:
             return
 
         self.info('Computing derived parameters......')
@@ -748,23 +829,25 @@
             parameters = samples[idx]
             weight = weights[idx]
             self.update_model(parameters)
             self._model.initialize_profiles()
             for p, v in zip(self.derived_names, self.derived_values):
                 derived_param[p][0].append(v)
                 derived_param[p][1].append(weight)
-            
+
         result_dict = {}
 
         sorted_weights = weights.argsort()
 
         for param, (trace, w) in derived_param.items():
-            
-            all_trace = np.array(mpi.allreduce(trace, op='SUM'))  # I cant remember why this works
-            all_weight = np.array(mpi.allreduce(w, op='SUM'))  # I cant remember why this works
+
+            # I cant remember why this works
+            all_trace = np.array(mpi.allreduce(trace, op='SUM'))
+            # I cant remember why this works
+            all_weight = np.array(mpi.allreduce(w, op='SUM'))
 
             all_weight_sort = all_weight.argsort()
 
             # Sort them into the right order
             all_weight[sorted_weights] = all_weight[all_weight_sort]
             all_trace[sorted_weights] = all_trace[all_weight_sort]
 
@@ -789,23 +872,23 @@
         Read traces and weights and return
         a random ``sigma_fraction`` sample of them
 
         Parameters
         ----------
         solution:
             a solution output from sampler
-        
+
         Yields
         ------
         traces: :obj:`array`
             Traces of a particular sample
 
         weight: float
             Weight of sample
-        
+
         """
         from taurex.util.util import random_int_iter
         samples = self.get_samples(solution)
         weights = self.get_weights(solution)
 
         iterator = random_int_iter(samples.shape[0], self._sigma_fraction)
         for x in iterator:
@@ -821,37 +904,36 @@
         median and MAP values
 
         Yields
         ------
 
         solution_no: int
             Solution number
-        
+
         map: :obj:`array`
             Map values
-        
+
         median: :obj:`array`
             Median values
-        
+
         extra: :obj:`list`
             List of tuples of extra information to store.
             Must be of form ``(name, data)``
-            
-        
+
+
 
         """
         raise NotImplementedError
 
     def get_samples(self, solution_id):
         raise NotImplementedError
 
     def get_weights(self, solution_id):
         raise NotImplementedError
 
-
     def write(self, output):
         """
         Creates 'Optimizer'
         them respectively
 
 
 
@@ -862,12 +944,10 @@
 
 
 
         """
         opt = output.create_group('Optimizer')
         self.write_optimizer(opt)
 
-
-
     @classmethod
     def input_keywords(self):
-        raise NotImplementedError
+        raise NotImplementedError
```

### Comparing `taurex-3.1.1a0/taurex/optimizer/polychord.py` & `taurex-3.1.4a0/taurex/optimizer/polychord.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/output/hdf5.py` & `taurex-3.1.4a0/taurex/output/hdf5.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/output/output.py` & `taurex-3.1.4a0/taurex/output/output.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/parameter/classfactory.py` & `taurex-3.1.4a0/taurex/parameter/classfactory.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/parameter/factory.py` & `taurex-3.1.4a0/taurex/parameter/factory.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/parameter/parameterparser.py` & `taurex-3.1.4a0/taurex/parameter/parameterparser.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/plot/corner.py` & `taurex-3.1.4a0/taurex/plot/corner.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/plot/plotter.py` & `taurex-3.1.4a0/taurex/plot/plotter.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/taurex.py` & `taurex-3.1.4a0/taurex/taurex.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         print('-----------------------------------------------')
         print('')
         table = [(' / '.join(c.input_keywords()),
                   f'{c.__name__}',
                   c.__module__.split('.')[0].split('_')[-1])
                  for c in cf.temperatureKlasses
                  if hasattr(c, 'input_keywords')]
-        print(tabulate.tabulate(table, 
+        print(tabulate.tabulate(table,
                                 headers=['profile_type', 'Class', 'Source'],
                                 tablefmt="fancy_grid"))
         print('\n')
     elif keywords in ('gas', ):
         print('')
         print('-----------------------------------------------')
         print('-------------Available Gas Profiles------------')
@@ -84,15 +84,15 @@
         print('-------------Available Priors------------------')
         print('-----------------------------------------------')
         print('')
         table = [(f'{c.__name__}',
                  c.__module__.split('.')[0].split('_')[-1])
                  for c in cf.priorKlasses
                  if hasattr(c, 'input_keywords')]
-        print(tabulate.tabulate(table, 
+        print(tabulate.tabulate(table,
                                 headers=['prior', 'Class', 'Source'],
                                 tablefmt="fancy_grid"))
         print('\n')
     elif keywords in ('model', ):
         print('')
         print('-----------------------------------------------')
         print('-------------Available Forward [Model]s--------')
@@ -111,15 +111,15 @@
         print('-------------Available [Pressure]s-------------')
         print('-----------------------------------------------')
         print('')
         table = [(' / '.join(c.input_keywords()), f'{c.__name__}',
                  c.__module__.split('.')[0].split('_')[-1])
                  for c in cf.pressureKlasses]
         print(tabulate.tabulate(table,
-                                headers=['profile_type', 'Class', 'Source'], 
+                                headers=['profile_type', 'Class', 'Source'],
                                 tablefmt="fancy_grid"))
         print('\n')
 
 
 def show_parameters(model):
     import tabulate
     print('')
@@ -194,32 +194,33 @@
         print(k)
 
     print('\n\nFailed plugins')
     print('---------------------------')
     for k, v in failed_plugins.items():
         print(k)
         print(f'Reason: {v}')
-    
+
     print('\n')
 
 
 def output_citations(model, instrument, optimizer):
+    from taurex.cache import OpacityCache
     from taurex.mpi import barrier, get_rank
 
     barrier()
     bib_tex = None
     citation_string = None
     if get_rank() == 0:
         print('\n\n----------------------------------------------------------')
         print('----------------------Bibiliography-----------------------')
         print('----------------------------------------------------------')
 
         print('If you use any of the results from this run please cite')
         print('the following publications:')
-        
+
         citation_string = ''
         all_citations = []
         print('\n')
         print('TauREx-Related')
         print('--------------\n')
         from taurex._citation import __citations__, taurex_citation
         citation_string += __citations__
@@ -248,33 +249,56 @@
             all_citations.extend(instrument.citations())
             if len(cite) > 0:
                 citation_string += cite
                 print('Instrument')
                 print('---------\n')
                 print(cite)
 
+        oc = OpacityCache()
+
+        active_gases = model.chemistry.activeGases
+
+        # Do cross sections
+
+        missing_citations = []
+
+        for g in active_gases:
+            try:
+                xsec = oc.opacity_dict[g]
+                if len(xsec.opacityCitation()) == 0:
+                    missing_citations.append(g)
+            except KeyError:
+                continue
+
+        if missing_citations:
+            print('Missing Opacity Citations')
+            print('------------------------\n')
+            print('These opacities do not have citation information, please')
+            print('determine their appropriate publications and cite them \n')
+            print(missing_citations)
+            print('\n')
         from taurex.core import to_bibtex
-        bib_tex = to_bibtex(all_citations)
-    
+        bib_tex = to_bibtex([a for a in all_citations if not isinstance(a, str)])
+
     barrier()
 
     return bib_tex, citation_string
 
+
 def only_bibtex(filename, pp):
     model = pp.generate_appropriate_model()
     instrument = pp.generate_instrument()[0]
     optimizer = pp.generate_optimizer()
 
     bib_tex, citation_string = output_citations(model, instrument, optimizer)
     if bib_tex:
         with open(filename, 'w') as f:
             f.write(bib_tex)
 
 
-
 def main():
     import argparse
     import datetime
 
     import logging
     from taurex.mpi import get_rank
     from taurex.log import setLogLevel
@@ -324,15 +348,15 @@
     parser.add_argument('-v', "--version", dest='version', default=False,
                         help="Display version", action='store_true')
 
     parser.add_argument("--plugins", dest='plugins', default=False,
                         help="Display plugins", action='store_true')
 
     parser.add_argument("--fitparams", dest='fitparams', default=False,
-                        help="Display available fitting params", 
+                        help="Display available fitting params",
                         action='store_true')
 
     parser.add_argument("--bibtex", dest='bibtex', type=str,
                         help="Output bibliography .bib to filepath")
 
     parser.add_argument("--only-bib", dest='no_run',
                         help="Do not run anything, only store bibtex (must have --bibtex)", default=False, action='store_true')
@@ -383,27 +407,24 @@
         return only_bibtex(args.bibtex, pp)
 
     # Get the spectrum
     observation = pp.generate_observation()
 
     binning = pp.generate_binning()
 
-
     # Generate a model from the input
     model = pp.generate_appropriate_model(obs=observation)
 
     # build the model
     model.build()
 
     if args.fitparams:
         show_parameters(model)
         return
 
-
-
     wngrid = None
 
     if binning == 'observed' and observation is None:
         logging.critical('Binning selected from Observation yet None provided')
         quit()
 
     if binning is None:
@@ -530,15 +551,15 @@
                 spectrum['instrument_wnwidth'] = inst_result[-1]
                 spectrum['instrument_wlgrid'] = 10000/inst_result[0]
                 spectrum['instrument_spectrum'] = inst_result[1]
                 spectrum['instrument_noise'] = inst_result[2]
 
             try:
                 spectrum['Contributions'] = \
-                    store_contributions(binning, model, 
+                    store_contributions(binning, model,
                                         output_size=output_size-3)
             except Exception:
                 pass
 
             if solution is not None:
                 out.store_dictionary(solution, group_name='Solutions')
                 priors = {}
```

### Comparing `taurex-3.1.1a0/taurex/util/emission.py` & `taurex-3.1.4a0/taurex/util/emission.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/util/fitting.py` & `taurex-3.1.4a0/taurex/util/fitting.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/util/fortran.py` & `taurex-3.1.4a0/taurex/util/fortran.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/util/geometry.py` & `taurex-3.1.4a0/taurex/util/geometry.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/util/hdf5.py` & `taurex-3.1.4a0/taurex/util/hdf5.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/util/math.py` & `taurex-3.1.4a0/taurex/util/math.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/util/module.py` & `taurex-3.1.4a0/taurex/util/module.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/util/output.py` & `taurex-3.1.4a0/taurex/util/output.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/util/scattering.py` & `taurex-3.1.4a0/taurex/util/scattering.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/util/spectrum.py` & `taurex-3.1.4a0/taurex/util/spectrum.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex/util/util.py` & `taurex-3.1.4a0/taurex/util/util.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/taurex.egg-info/PKG-INFO` & `taurex-3.1.4a0/taurex.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,84 +1,16 @@
 Metadata-Version: 2.1
 Name: taurex
-Version: 3.1.1a0
+Version: 3.1.4a0
 Summary: TauREx 3 retrieval framework
 Home-page: https://github.com/ucl-exoplanets/TauREx3_public/
 Author: Ahmed Faris Al-Refaie
 Author-email: ahmed.al-refaie.12@ucl.ac.uk
 License: BSD
-Description: # TauREx 3
-        
-        ![Python package](https://github.com/ucl-exoplanets/TauREx3/workflows/Python%20package/badge.svg)
-        
-        TauREx 3 is the newest version of the TauREx retrieval code.
-        
-        Documentation can be found [here](https://taurex3-public.readthedocs.io/en/latest/)
-        
-        Current build: 3.1.1-alpha
-        
-        ## Prerequisites
-        
-        * numpy
-        
-        
-        
-        ## Installing from PyPi
-        
-        
-        You can install it by doing
-        
-        ```
-        pip install taurex
-        ```
-        
-        
-        ## Installing from source
-        
-        
-        Clone the directory using:
-        
-        ```
-        git clone https://github.com/ucl-exoplanets/TauREx3_public.git
-        ```
-        
-        Move into the TauREx3 folder
-        
-        ```
-        cd TauREx3
-        ```
-        
-        Then install
-        
-        ```
-        pip install .
-        ```
-        
-        To build documentation do
-        
-        ```
-        python setup.py build_sphinx
-        ```
-        
-        
-        Try importing taurex:
-        
-        ```
-        python -c "import taurex; print(taurex.__version__)"
-        ```
-        
-        Or running taurex itself
-        
-        ```
-        taurex
-        ```
-        
-        If there are no errors then it was successful!
 Keywords: exoplanet,retrieval,taurex,taurex3,atmosphere,atmospheric
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
@@ -87,7 +19,76 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Provides: taurex
 Description-Content-Type: text/markdown
 Provides-Extra: Plot
+License-File: LICENSE
+
+# TauREx 3
+
+![Python package](https://github.com/ucl-exoplanets/TauREx3/workflows/Python%20package/badge.svg)
+
+TauREx 3 is the newest version of the TauREx retrieval code.
+
+Documentation can be found [here](https://taurex3-public.readthedocs.io/en/latest/)
+
+Current build: 3.1.4-alpha
+
+## Prerequisites
+
+* numpy
+
+
+
+## Installing from PyPi
+
+
+You can install it by doing
+
+```
+pip install taurex
+```
+
+
+## Installing from source
+
+
+Clone the directory using:
+
+```
+git clone https://github.com/ucl-exoplanets/TauREx3_public.git
+```
+
+Move into the TauREx3 folder
+
+```
+cd TauREx3
+```
+
+Then install
+
+```
+pip install .
+```
+
+To build documentation do
+
+```
+python setup.py build_sphinx
+```
+
+
+Try importing taurex:
+
+```
+python -c "import taurex; print(taurex.__version__)"
+```
+
+Or running taurex itself
+
+```
+taurex
+```
+
+If there are no errors then it was successful!
```

### Comparing `taurex-3.1.1a0/taurex.egg-info/SOURCES.txt` & `taurex-3.1.4a0/taurex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/benchmark/test_bb.py` & `taurex-3.1.4a0/tests/benchmark/test_bb.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/benchmark/test_bilinear_interps.py` & `taurex-3.1.4a0/tests/benchmark/test_bilinear_interps.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/benchmark/test_contrib_funcs.py` & `taurex-3.1.4a0/tests/benchmark/test_contrib_funcs.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/benchmark/test_emission_funcs.py` & `taurex-3.1.4a0/tests/benchmark/test_emission_funcs.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/benchmark/test_forward_model.py` & `taurex-3.1.4a0/tests/benchmark/test_forward_model.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/benchmark/test_linear_interps.py` & `taurex-3.1.4a0/tests/benchmark/test_linear_interps.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/chemistry/test_chemistry.py` & `taurex-3.1.4a0/tests/chemistry/test_chemistry.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/chemistry/test_constantgas.py` & `taurex-3.1.4a0/tests/chemistry/test_constantgas.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/chemistry/test_free_chemistry.py` & `taurex-3.1.4a0/tests/chemistry/test_free_chemistry.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/chemistry/test_powergas.py` & `taurex-3.1.4a0/tests/chemistry/test_powergas.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/cia/test_cia.py` & `taurex-3.1.4a0/tests/cia/test_cia.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/factory/test_classfactory.py` & `taurex-3.1.4a0/tests/factory/test_classfactory.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/factory/test_factories.py` & `taurex-3.1.4a0/tests/factory/test_factories.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/factory/test_mixin.py` & `taurex-3.1.4a0/tests/factory/test_mixin.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/fixtures/opacities/genopacs.py` & `taurex-3.1.4a0/tests/fixtures/opacities/genopacs.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/optimizer/__init__.py` & `taurex-3.1.4a0/tests/optimizer/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         Creates the appropriate binning object
         """
         from taurex.binning import NativeBinner
 
         return NativeBinner()
 
     def __init__(self, m, c, N):
+        super().__init__('LineObs')
         self._m = m
         self._c = c
         self._x = np.linspace(1, 100, N)
         self._y = self._m*self._x + self._c
         self._yerr = 0.1+0.1*np.random.rand(N)
         self._y += self._yerr * np.random.randn(N)
 
@@ -80,7 +81,49 @@
     @property
     def wavenumberGrid(self):
         return self._x
 
     @property
     def errorBar(self):
         return self._yerr
+
+
+
+class LineObsWithParams(BaseSpectrum):
+
+    def create_binner(self):
+        """
+        Creates the appropriate binning object
+        """
+        from taurex.binning import NativeBinner
+
+        return NativeBinner()
+
+    def __init__(self, m, c, N):
+        super().__init__('LineObs')
+        self._m = m
+        self._c = c
+        self._lol = 40
+        self._x = np.linspace(1, 100, N)
+        self._y = self._m*self._x + self._c
+        self._yerr = 0.1+0.1*np.random.rand(N)
+        self._y += self._yerr * np.random.randn(N)
+
+    @property
+    def spectrum(self):
+        return self._y
+
+    @property
+    def wavenumberGrid(self):
+        return self._x
+
+    @property
+    def errorBar(self):
+        return self._yerr
+
+    @fitparam(param_name='lol')
+    def lol(self):
+        return self._lol
+
+    @lol.setter
+    def lol(self, value):
+        self._lol = value
```

### Comparing `taurex-3.1.1a0/tests/optimizer/test_nestle.py` & `taurex-3.1.4a0/tests/optimizer/test_nestle.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/optimizer/test_optimizer.py` & `taurex-3.1.4a0/tests/optimizer/test_optimizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from . import LineModel, LineObs
+from . import LineModel, LineObs, LineObsWithParams
 from hypothesis import given, note,strategies as st
 from taurex.optimizer import Optimizer
 from taurex.core.priors import Uniform, LogUniform
 import math
 
 @given(m=st.floats(0.1, 100, allow_nan=False),
        c=st.floats(0.1, 100, allow_nan=False))
@@ -41,14 +41,89 @@
     assert 'm' in opt.fit_names
     assert opt.fit_values[opt.fit_names.index('c')] == c
     assert opt.fit_values[opt.fit_names.index('m')] == m
 
 
 @given(m=st.floats(0.1, 100, allow_nan=False),
        c=st.floats(0.1, 100, allow_nan=False))
+def test_optimizer_fittingparams_with_obs(m, c):
+
+    lm = LineModel()
+    lm.m = m
+    lm.c = c
+    lo = LineObsWithParams(m=m, c=c, N=10)
+
+    opt = Optimizer('test', observed=lo, model=lm)
+
+    opt.enable_fit('m')
+    opt.enable_fit('lol')
+    opt.compile_params()
+
+    assert 'm' in opt.fit_names
+    assert 'lol' in opt.fit_names
+    assert 'c' not in opt.fit_names
+    assert opt.fit_values[opt.fit_names.index('m')] == m
+
+    opt.enable_fit('c')
+    opt.disable_fit('m')
+    opt.compile_params()
+    assert 'c' in opt.fit_names
+    assert 'm' not in opt.fit_names
+    assert 'lol' in opt.fit_names
+    assert opt.fit_values[opt.fit_names.index('c')] == c
+
+    opt.enable_fit('c')
+    opt.disable_fit('m')
+    opt.disable_fit('lol')
+    opt.compile_params()
+    assert 'c' in opt.fit_names
+    assert 'm' not in opt.fit_names
+    assert 'lol' not in opt.fit_names
+    assert opt.fit_values[opt.fit_names.index('c')] == c
+
+    opt.disable_fit('m')
+    opt.disable_fit('c')
+    opt.disable_fit('lol')
+    opt.compile_params()
+
+    opt.enable_fit('c')
+    opt.enable_fit('m')
+    opt.enable_fit('lol')
+    opt.compile_params()
+    assert 'c' in opt.fit_names
+    assert 'm' in opt.fit_names
+    assert 'lol' in opt.fit_names
+    assert opt.fit_values[opt.fit_names.index('c')] == c
+    assert opt.fit_values[opt.fit_names.index('m')] == m
+
+def test_optimizer_setprior():
+    from taurex.core.priors import Uniform, LogUniform, Gaussian
+    lm = LineModel()
+    lm.m = 1.0
+    lm.c = 10.0
+    lo = LineObs(m=1.0, c=10.0, N=10)
+
+    opt = Optimizer('test', observed=lo, model=lm)
+
+
+    opt.set_prior('m', Uniform([0.1, 100]))
+    opt.set_prior('c', Gaussian(0.1, 100))
+
+
+
+    opt.enable_fit('m')
+    opt.enable_fit('c')
+    opt.compile_params()
+    assert isinstance(opt.fitting_priors[opt.fit_names.index('m')], Uniform)
+    assert isinstance(opt.fitting_priors[opt.fit_names.index('c')], Gaussian)
+
+
+
+@given(m=st.floats(0.1, 100, allow_nan=False),
+       c=st.floats(0.1, 100, allow_nan=False))
 def test_optimizer_updatemodel(m, c):
 
     lm = LineModel()
     lm.m = 1.0
     lm.c = 10.0
     lo = LineObs(m=m, c=c, N=10)
```

### Comparing `taurex-3.1.1a0/tests/parameter/test_keywords.py` & `taurex-3.1.4a0/tests/parameter/test_keywords.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/priors/test_nonuniform.py` & `taurex-3.1.4a0/tests/priors/test_nonuniform.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/spectrum/test_spectrum.py` & `taurex-3.1.4a0/tests/spectrum/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/stellar/test_blackbody.py` & `taurex-3.1.4a0/tests/stellar/test_blackbody.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/stellar/test_phoenix.py` & `taurex-3.1.4a0/tests/stellar/test_phoenix.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/strategies/__init__.py` & `taurex-3.1.4a0/tests/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/temperature/test_guillot.py` & `taurex-3.1.4a0/tests/temperature/test_guillot.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/temperature/test_isothermal.py` & `taurex-3.1.4a0/tests/temperature/test_isothermal.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/temperature/test_npoint.py` & `taurex-3.1.4a0/tests/temperature/test_npoint.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/test_binning.py` & `taurex-3.1.4a0/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/test_core.py` & `taurex-3.1.4a0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/test_modelload.py` & `taurex-3.1.4a0/tests/test_modelload.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/test_opac.py` & `taurex-3.1.4a0/tests/test_opac.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/test_pressure.py` & `taurex-3.1.4a0/tests/test_pressure.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/util/test_emission.py` & `taurex-3.1.4a0/tests/util/test_emission.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/util/test_fitting.py` & `taurex-3.1.4a0/tests/util/test_fitting.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/util/test_math.py` & `taurex-3.1.4a0/tests/util/test_math.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tests/util/test_util.py` & `taurex-3.1.4a0/tests/util/test_util.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tools/exocross_to_hdf5.py` & `taurex-3.1.4a0/tools/exocross_to_hdf5.py`

 * *Files identical despite different names*

### Comparing `taurex-3.1.1a0/tools/pickle_to_properformat.py` & `taurex-3.1.4a0/tools/pickle_to_properformat.py`

 * *Files identical despite different names*

