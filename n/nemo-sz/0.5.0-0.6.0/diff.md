# Comparing `tmp/nemo-sz-0.5.0.tar.gz` & `tmp/nemo-sz-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemo-sz-0.5.0.tar", last modified: Wed Nov 17 08:16:16 2021, max compression
+gzip compressed data, was "nemo-sz-0.6.0.tar", last modified: Fri Jul 14 12:08:04 2023, max compression
```

## Comparing `nemo-sz-0.5.0.tar` & `nemo-sz-0.6.0.tar`

### file list

```diff
@@ -1,156 +1,155 @@
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2021-11-17 08:16:16.720290 nemo-sz-0.5.0/
--rw-rw-r--   0 matty     (1000) matty     (1000)     1820 2021-08-18 14:14:27.000000 nemo-sz-0.5.0/INSTALL.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)      343 2021-11-17 08:09:46.000000 nemo-sz-0.5.0/MANIFEST.in
--rw-rw-r--   0 matty     (1000) matty     (1000)      801 2021-11-17 08:16:16.720290 nemo-sz-0.5.0/PKG-INFO
--rw-rw-r--   0 matty     (1000) matty     (1000)     2116 2021-11-17 06:29:58.000000 nemo-sz-0.5.0/README.rst
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2021-11-17 08:16:16.700289 nemo-sz-0.5.0/bin/
--rw-rw-r--   0 matty     (1000) matty     (1000)    14617 2021-08-04 12:24:32.000000 nemo-sz-0.5.0/bin/nemo
--rw-rw-r--   0 matty     (1000) matty     (1000)     5336 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/bin/nemoCatalogCheck
--rw-rw-r--   0 matty     (1000) matty     (1000)    21274 2020-10-01 09:44:19.000000 nemo-sz-0.5.0/bin/nemoCosmo
--rw-rw-r--   0 matty     (1000) matty     (1000)    20809 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/bin/nemoMass
--rw-rw-r--   0 matty     (1000) matty     (1000)     3848 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/bin/nemoMock
--rw-rw-r--   0 matty     (1000) matty     (1000)    12257 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/bin/nemoModel
--rw-rw-r--   0 matty     (1000) matty     (1000)     4133 2021-02-17 13:10:21.000000 nemo-sz-0.5.0/bin/nemoSelFn
--rw-rw-r--   0 matty     (1000) matty     (1000)     6385 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/bin/nemoSpec
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2021-11-17 08:16:16.700289 nemo-sz-0.5.0/docs/
--rw-rw-r--   0 matty     (1000) matty     (1000)      580 2019-02-24 16:16:40.000000 nemo-sz-0.5.0/docs/Makefile
--rw-rw-r--   0 matty     (1000) matty     (1000)     3317 2021-03-04 16:41:54.000000 nemo-sz-0.5.0/docs/advanced.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)     2804 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/docs/commands.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)     5724 2021-02-17 13:10:21.000000 nemo-sz-0.5.0/docs/conf.py
--rw-rw-r--   0 matty     (1000) matty     (1000)    39720 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/docs/config.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)     2874 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/docs/development.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)      261 2021-02-17 13:10:21.000000 nemo-sz-0.5.0/docs/dr3_tutorial.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)      225 2021-03-08 15:45:50.000000 nemo-sz-0.5.0/docs/dr5_tutorial.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)      634 2021-10-01 12:20:40.000000 nemo-sz-0.5.0/docs/index.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)       89 2021-02-17 13:10:21.000000 nemo-sz-0.5.0/docs/install.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)     6167 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/docs/outputs.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)      194 2021-02-17 16:06:52.000000 nemo-sz-0.5.0/docs/quickstart.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)     1041 2020-06-17 07:51:59.000000 nemo-sz-0.5.0/docs/reference.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)      253 2021-02-17 13:10:21.000000 nemo-sz-0.5.0/docs/sosims_tutorial.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)       79 2020-11-11 10:23:57.000000 nemo-sz-0.5.0/docs/testing.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)      218 2021-02-17 13:10:21.000000 nemo-sz-0.5.0/docs/tilec_tutorial.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)      123 2021-02-17 13:10:21.000000 nemo-sz-0.5.0/docs/tutorials.rst
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2021-11-17 08:16:16.696289 nemo-sz-0.5.0/examples/
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2021-11-17 08:16:16.712290 nemo-sz-0.5.0/examples/ACT-DR3-clusters/
--rw-rw-r--   0 matty     (1000) matty     (1000)  8743680 2021-11-17 06:54:24.000000 nemo-sz-0.5.0/examples/ACT-DR3-clusters/ACTPol_clusters.fits
--rw-rw-r--   0 matty     (1000) matty     (1000)  9696960 2021-11-17 06:54:24.000000 nemo-sz-0.5.0/examples/ACT-DR3-clusters/ACTPol_redshifts.fits
--rw-rw-r--   0 matty     (1000) matty     (1000)    74880 2021-11-17 06:54:24.000000 nemo-sz-0.5.0/examples/ACT-DR3-clusters/E-D56Clusters.fits
--rw-rw-r--   0 matty     (1000) matty     (1000)     8262 2021-11-17 06:54:24.000000 nemo-sz-0.5.0/examples/ACT-DR3-clusters/README.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)     7063 2021-11-17 06:54:24.000000 nemo-sz-0.5.0/examples/ACT-DR3-clusters/equD56.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     3816 2021-11-17 06:54:24.000000 nemo-sz-0.5.0/examples/ACT-DR3-clusters/equD56_quick.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)   412359 2021-11-17 06:54:24.000000 nemo-sz-0.5.0/examples/ACT-DR3-clusters/pointSourceMask.fits.gz
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2021-11-17 08:16:16.712290 nemo-sz-0.5.0/examples/ACT-DR3-clusters/profiles_ACT/
--rw-rw-r--   0 matty     (1000) matty     (1000)   240000 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/ACT-DR3-clusters/profiles_ACT/profile_AR1_2009_pixwin_130224.txt
--rw-rw-r--   0 matty     (1000) matty     (1000)     4538 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/ACT-DR3-clusters/selFnExample.py
--rw-rw-r--   0 matty     (1000) matty     (1000)   138534 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/ACT-DR3-clusters/surveyMask.fits.gz
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2021-11-17 08:16:16.712290 nemo-sz-0.5.0/examples/ACT-DR5-clusters/
--rw-rw-r--   0 matty     (1000) matty     (1000)      249 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/ACT-DR5-clusters/DR5ClusterSearch.slurm
--rw-rw-r--   0 matty     (1000) matty     (1000)     6163 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/ACT-DR5-clusters/DR5ClusterSearch.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)      712 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/ACT-DR5-clusters/FETCH_MAPS.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)     3004 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/ACT-DR5-clusters/README.rst
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2021-11-17 08:16:16.716290 nemo-sz-0.5.0/examples/SOSims/
--rw-rw-r--   0 matty     (1000) matty     (1000)      824 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/HEALPIX_TO_CAR.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)      224 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/MAKE_BEAMS.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)       56 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/MAKE_MOCKS_SMALL.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)       56 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/MAKE_MOCKS_TILES.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)     6258 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/MFMF_SOSim_3freq_small.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     6618 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/MFMF_SOSim_3freq_tiles.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     3132 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/NzCheck.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     9122 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/README.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)      583 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/cobayaConf_SOSims_fixedScalingRelation.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     1475 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/combineComponentMaps.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     1457 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/createSurveyMask.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     3443 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/healpix2CAR.py
--rw-rw-r--   0 matty     (1000) matty     (1000)      876 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/makeGaussianBeam.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     1429 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/makeRedshiftsCatalog.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     2081 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/readWebSkyInputCatalog.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     4554 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/selFnExample.py
--rw-rw-r--   0 matty     (1000) matty     (1000)      203 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/slurm_cosmo.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)      205 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/slurm_mass.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)      273 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/slurm_nemo.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)      292 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/slurm_small_cosmo.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)     1255 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/surveyMask.reg
--rw-rw-r--   0 matty     (1000) matty     (1000)     1237 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/template_AdvACT.txt
--rw-rw-r--   0 matty     (1000) matty     (1000)      542 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/template_E-D56.txt
--rw-rw-r--   0 matty     (1000) matty     (1000)     1236 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/template_small.txt
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2021-11-17 08:16:16.716290 nemo-sz-0.5.0/examples/SOSims/validationScripts/
--rw-rw-r--   0 matty     (1000) matty     (1000)      542 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/validationScripts/README.md
--rw-rw-r--   0 matty     (1000) matty     (1000)     5366 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/validationScripts/checkMassRecovery.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     5188 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/validationScripts/checkMassRecovery_M200m.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     6703 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/validationScripts/makeMassFunctionPlotsCCL.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     6787 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/SOSims/validationScripts/makeMassFunctionPlotsCCL_recovered.py
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2021-11-17 08:16:16.716290 nemo-sz-0.5.0/examples/TILe-C/
--rw-rw-r--   0 matty     (1000) matty     (1000)     1030 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/TILe-C/README.md
--rw-rw-r--   0 matty     (1000) matty     (1000)     4238 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/TILe-C/y_f090beam.yml
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2021-11-17 08:16:16.716290 nemo-sz-0.5.0/examples/clustercal/
--rw-rw-r--   0 matty     (1000) matty     (1000)       22 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/clustercal/README.md
--rw-rw-r--   0 matty     (1000) matty     (1000)     9692 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/clustercal/clustercal.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     6420 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/clustercal/makeConfigs.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     5375 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/clustercal/template_singlefreq.yml
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2021-11-17 08:16:16.716290 nemo-sz-0.5.0/examples/quickstart/
--rw-rw-r--   0 matty     (1000) matty     (1000)     2900 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/quickstart/README.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)     4966 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/quickstart/quickstart-clusters.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     1823 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/quickstart/quickstart-sources.yml
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2021-11-17 08:16:16.716290 nemo-sz-0.5.0/examples/sources/
--rw-rw-r--   0 matty     (1000) matty     (1000)     1410 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/sources/PSExample_E-D56.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     1385 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/sources/PSExample_deep56_s15_f090.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     1541 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/sources/PSExample_deep8.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     8852 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/sources/PS_S16_f090_nightOnly.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     8870 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/sources/PS_S16_nightOnly.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     2813 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/sources/PS_S18d_f090_202006_2pass.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     2814 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/sources/PS_S18d_f150_202006_2pass.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)      168 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/sources/PS_S18d_f220_202006.sh
--rw-rw-r--   0 matty     (1000) matty     (1000)     7784 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/sources/PS_S18d_f220_202006.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     2814 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/sources/PS_S18d_f220_202006_2pass.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     7960 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/sources/PS_f150_act+planck_day+night.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     8901 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/sources/PS_f220_nightOnly.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)      183 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/sources/README.md
--rw-rw-r--   0 matty     (1000) matty     (1000)      172 2021-11-17 06:54:25.000000 nemo-sz-0.5.0/examples/sources/RUN_PS.sh
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2021-11-17 08:16:16.720290 nemo-sz-0.5.0/nemo/
--rw-rw-r--   0 matty     (1000) matty     (1000)    27793 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/nemo/MockSurvey.py
--rw-rw-r--   0 matty     (1000) matty     (1000)      499 2020-01-29 14:51:01.000000 nemo-sz-0.5.0/nemo/__init__.py
--rw-rw-r--   0 matty     (1000) matty     (1000)      497 2021-11-17 08:16:16.720290 nemo-sz-0.5.0/nemo/_version.py
--rw-rw-r--   0 matty     (1000) matty     (1000)    36755 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/nemo/catalogs.py
--rw-rw-r--   0 matty     (1000) matty     (1000)    79168 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/nemo/completeness.py
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2021-11-17 08:16:16.716290 nemo-sz-0.5.0/nemo/data/
--rw-rw-r--   0 matty     (1000) matty     (1000)   140701 2019-03-11 10:14:35.000000 nemo-sz-0.5.0/nemo/data/planck_lensedCls.dat
--rw-rw-r--   0 matty     (1000) matty     (1000)    67722 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/nemo/filters.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     4464 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/nemo/gnfw.py
--rw-rw-r--   0 matty     (1000) matty     (1000)   116957 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/nemo/maps.py
--rw-rw-r--   0 matty     (1000) matty     (1000)    12237 2019-09-17 14:28:39.000000 nemo-sz-0.5.0/nemo/nemoCython.pyx
--rw-rw-r--   0 matty     (1000) matty     (1000)    25956 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/nemo/photometry.py
--rw-rw-r--   0 matty     (1000) matty     (1000)    52854 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/nemo/pipelines.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     1516 2019-04-10 08:18:42.000000 nemo-sz-0.5.0/nemo/plotSettings.py
--rw-rw-r--   0 matty     (1000) matty     (1000)    64438 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/nemo/signals.py
--rw-rw-r--   0 matty     (1000) matty     (1000)    21064 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/nemo/startUp.py
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2021-11-17 08:16:16.720290 nemo-sz-0.5.0/nemo_sz.egg-info/
--rw-rw-r--   0 matty     (1000) matty     (1000)      801 2021-11-17 08:16:16.000000 nemo-sz-0.5.0/nemo_sz.egg-info/PKG-INFO
--rw-rw-r--   0 matty     (1000) matty     (1000)     4173 2021-11-17 08:16:16.000000 nemo-sz-0.5.0/nemo_sz.egg-info/SOURCES.txt
--rw-rw-r--   0 matty     (1000) matty     (1000)        1 2021-11-17 08:16:16.000000 nemo-sz-0.5.0/nemo_sz.egg-info/dependency_links.txt
--rw-rw-r--   0 matty     (1000) matty     (1000)      127 2021-11-17 08:16:16.000000 nemo-sz-0.5.0/nemo_sz.egg-info/requires.txt
--rw-rw-r--   0 matty     (1000) matty     (1000)       16 2021-11-17 08:16:16.000000 nemo-sz-0.5.0/nemo_sz.egg-info/top_level.txt
--rw-rw-r--   0 matty     (1000) matty     (1000)       78 2020-11-10 16:42:01.000000 nemo-sz-0.5.0/pyproject.toml
--rw-rw-r--   0 matty     (1000) matty     (1000)      192 2021-11-17 08:16:16.720290 nemo-sz-0.5.0/setup.cfg
--rw-rw-r--   0 matty     (1000) matty     (1000)     2048 2021-09-13 10:02:49.000000 nemo-sz-0.5.0/setup.py
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2021-11-17 08:16:16.720290 nemo-sz-0.5.0/tests/
--rw-rw-r--   0 matty     (1000) matty     (1000)      977 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/tests/README.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)     2157 2021-09-07 15:31:52.000000 nemo-sz-0.5.0/tests/clusters.robot
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2021-11-17 08:16:16.720290 nemo-sz-0.5.0/tests/configs/
--rw-rw-r--   0 matty     (1000) matty     (1000)     1236 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/tests/configs/MPITestSurveyMaskHeader.txt
--rw-rw-r--   0 matty     (1000) matty     (1000)     1324 2021-09-07 15:31:52.000000 nemo-sz-0.5.0/tests/configs/PSTest_E-D56.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     1430 2021-09-07 15:31:52.000000 nemo-sz-0.5.0/tests/configs/PSTest_south2008.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     1233 2021-09-07 15:31:52.000000 nemo-sz-0.5.0/tests/configs/PSTest_south2008_fourier.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)      255 2021-09-07 15:31:52.000000 nemo-sz-0.5.0/tests/configs/README.rst
--rw-rw-r--   0 matty     (1000) matty     (1000)     3442 2021-09-07 15:31:52.000000 nemo-sz-0.5.0/tests/configs/equD56_quick_fourier.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     5932 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/tests/configs/sim_cl_A10_MFMF_tiles.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     5727 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/tests/configs/sim_cl_B12_MFMF_tiles.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     6033 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/tests/configs/sim_cl_MFMF.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     6102 2021-09-16 09:23:07.000000 nemo-sz-0.5.0/tests/configs/sim_cl_MFMF_pass2.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     1253 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/tests/configs/sim_ptsrc_f090.yml
--rw-rw-r--   0 matty     (1000) matty     (1000)     1236 2021-09-07 15:31:52.000000 nemo-sz-0.5.0/tests/configs/smallTestSurveyMaskHeader.txt
--rw-rw-r--   0 matty     (1000) matty     (1000)     1227 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/tests/debug.py
-drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2021-11-17 08:16:16.720290 nemo-sz-0.5.0/tests/lib/
--rw-rw-r--   0 matty     (1000) matty     (1000)    17534 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/tests/lib/NemoTests.py
--rw-rw-r--   0 matty     (1000) matty     (1000)     2422 2021-09-07 15:31:52.000000 nemo-sz-0.5.0/tests/point_sources.robot
--rw-rw-r--   0 matty     (1000) matty     (1000)     5493 2021-11-17 06:29:36.000000 nemo-sz-0.5.0/tests/quick.robot
--rw-rw-r--   0 matty     (1000) matty     (1000)    70144 2021-02-17 13:10:21.000000 nemo-sz-0.5.0/versioneer.py
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.267146 nemo-sz-0.6.0/
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1694 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/INSTALL.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1531 2020-11-05 07:18:13.000000 nemo-sz-0.6.0/LICENSE
+-rw-rw-r--   0 matty     (1000) matty     (1000)      343 2021-11-17 08:09:46.000000 nemo-sz-0.6.0/MANIFEST.in
+-rw-rw-r--   0 matty     (1000) matty     (1000)      776 2023-07-14 12:08:04.267146 nemo-sz-0.6.0/PKG-INFO
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2132 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/README.rst
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.231145 nemo-sz-0.6.0/bin/
+-rw-rw-r--   0 matty     (1000) matty     (1000)     8401 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/bin/nemo
+-rw-rw-r--   0 matty     (1000) matty     (1000)     5336 2021-11-17 06:29:36.000000 nemo-sz-0.6.0/bin/nemoCatalogCheck
+-rw-rw-r--   0 matty     (1000) matty     (1000)    23560 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/bin/nemoMass
+-rw-rw-r--   0 matty     (1000) matty     (1000)     4274 2022-08-24 09:10:58.000000 nemo-sz-0.6.0/bin/nemoMock
+-rw-rw-r--   0 matty     (1000) matty     (1000)    18345 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/bin/nemoModel
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6385 2021-11-17 06:29:36.000000 nemo-sz-0.6.0/bin/nemoSpec
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.231145 nemo-sz-0.6.0/docs/
+-rw-rw-r--   0 matty     (1000) matty     (1000)      580 2019-02-24 16:16:40.000000 nemo-sz-0.6.0/docs/Makefile
+-rw-rw-r--   0 matty     (1000) matty     (1000)     3317 2021-03-04 16:41:54.000000 nemo-sz-0.6.0/docs/advanced.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2310 2022-08-26 03:53:41.000000 nemo-sz-0.6.0/docs/commands.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)     5731 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/docs/conf.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)    38946 2022-01-11 13:00:45.000000 nemo-sz-0.6.0/docs/config.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2874 2021-11-17 06:29:36.000000 nemo-sz-0.6.0/docs/development.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)      261 2021-02-17 13:10:21.000000 nemo-sz-0.6.0/docs/dr3_tutorial.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)      225 2021-03-08 15:45:50.000000 nemo-sz-0.6.0/docs/dr5_tutorial.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)      634 2021-10-01 12:20:40.000000 nemo-sz-0.6.0/docs/index.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)       89 2021-02-17 13:10:21.000000 nemo-sz-0.6.0/docs/install.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6167 2021-11-17 06:29:36.000000 nemo-sz-0.6.0/docs/outputs.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)      194 2021-02-17 16:06:52.000000 nemo-sz-0.6.0/docs/quickstart.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)      976 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/docs/reference.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)      253 2021-02-17 13:10:21.000000 nemo-sz-0.6.0/docs/sosims_tutorial.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)       79 2020-11-11 10:23:57.000000 nemo-sz-0.6.0/docs/testing.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)      123 2021-02-17 13:10:21.000000 nemo-sz-0.6.0/docs/tutorials.rst
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.231145 nemo-sz-0.6.0/examples/
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.251145 nemo-sz-0.6.0/examples/ACT-DR3-clusters/
+-rw-rw-r--   0 matty     (1000) matty     (1000)  8743680 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/ACTPol_clusters.fits
+-rw-rw-r--   0 matty     (1000) matty     (1000)  9696960 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/ACTPol_redshifts.fits
+-rw-rw-r--   0 matty     (1000) matty     (1000)    74880 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/E-D56Clusters.fits
+-rw-rw-r--   0 matty     (1000) matty     (1000)     8262 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/README.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)     7063 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/equD56.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     3816 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/equD56_quick.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)   412359 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/pointSourceMask.fits.gz
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.251145 nemo-sz-0.6.0/examples/ACT-DR3-clusters/profiles_ACT/
+-rw-rw-r--   0 matty     (1000) matty     (1000)   240000 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/profiles_ACT/profile_AR1_2009_pixwin_130224.txt
+-rw-rw-r--   0 matty     (1000) matty     (1000)     4656 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/selFnExample.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)   138534 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR3-clusters/surveyMask.fits.gz
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.251145 nemo-sz-0.6.0/examples/ACT-DR5-clusters/
+-rw-rw-r--   0 matty     (1000) matty     (1000)      220 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR5-clusters/DR5ClusterSearch.slurm
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6184 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR5-clusters/DR5ClusterSearch.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)      712 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR5-clusters/FETCH_MAPS.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)     3429 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/ACT-DR5-clusters/README.rst
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.255146 nemo-sz-0.6.0/examples/SOSims/
+-rw-rw-r--   0 matty     (1000) matty     (1000)      824 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/HEALPIX_TO_CAR.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)      224 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/MAKE_BEAMS.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)       56 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/MAKE_MOCKS_SMALL.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)       56 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/MAKE_MOCKS_TILES.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6258 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/MFMF_SOSim_3freq_small.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6618 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/MFMF_SOSim_3freq_tiles.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     3132 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/NzCheck.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     9122 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/README.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)      583 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/cobayaConf_SOSims_fixedScalingRelation.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1475 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/combineComponentMaps.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1457 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/createSurveyMask.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     3443 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/healpix2CAR.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)      876 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/makeGaussianBeam.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1429 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/makeRedshiftsCatalog.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2081 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/readWebSkyInputCatalog.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     4554 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/selFnExample.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)      203 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/slurm_cosmo.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)      205 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/slurm_mass.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)      273 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/slurm_nemo.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)      292 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/slurm_small_cosmo.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1255 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/surveyMask.reg
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1237 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/template_AdvACT.txt
+-rw-rw-r--   0 matty     (1000) matty     (1000)      542 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/template_E-D56.txt
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1236 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/template_small.txt
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.255146 nemo-sz-0.6.0/examples/SOSims/validationScripts/
+-rw-rw-r--   0 matty     (1000) matty     (1000)      542 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/validationScripts/README.md
+-rw-rw-r--   0 matty     (1000) matty     (1000)     5366 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/validationScripts/checkMassRecovery.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     5188 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/validationScripts/checkMassRecovery_M200m.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6703 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/validationScripts/makeMassFunctionPlotsCCL.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6787 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/SOSims/validationScripts/makeMassFunctionPlotsCCL_recovered.py
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.255146 nemo-sz-0.6.0/examples/TILe-C/
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1030 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/TILe-C/README.md
+-rw-rw-r--   0 matty     (1000) matty     (1000)     4238 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/TILe-C/y_f090beam.yml
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.259146 nemo-sz-0.6.0/examples/clustercal/
+-rw-rw-r--   0 matty     (1000) matty     (1000)       22 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/clustercal/README.md
+-rw-rw-r--   0 matty     (1000) matty     (1000)     9692 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/clustercal/clustercal.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6420 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/clustercal/makeConfigs.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     5375 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/clustercal/template_singlefreq.yml
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.259146 nemo-sz-0.6.0/examples/quickstart/
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2900 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/quickstart/README.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)     4966 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/quickstart/quickstart-clusters.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1823 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/quickstart/quickstart-sources.yml
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.259146 nemo-sz-0.6.0/examples/sources/
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1410 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PSExample_E-D56.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1385 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PSExample_deep56_s15_f090.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1541 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PSExample_deep8.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     8852 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PS_S16_f090_nightOnly.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     8870 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PS_S16_nightOnly.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2813 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PS_S18d_f090_202006_2pass.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2814 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PS_S18d_f150_202006_2pass.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)      168 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PS_S18d_f220_202006.sh
+-rw-rw-r--   0 matty     (1000) matty     (1000)     7784 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PS_S18d_f220_202006.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2814 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PS_S18d_f220_202006_2pass.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     7960 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PS_f150_act+planck_day+night.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     8901 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/PS_f220_nightOnly.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)      183 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/README.md
+-rw-rw-r--   0 matty     (1000) matty     (1000)      172 2023-07-14 10:39:55.000000 nemo-sz-0.6.0/examples/sources/RUN_PS.sh
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.267146 nemo-sz-0.6.0/nemo/
+-rw-rw-r--   0 matty     (1000) matty     (1000)    31319 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/nemo/MockSurvey.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)      499 2020-01-29 14:51:01.000000 nemo-sz-0.6.0/nemo/__init__.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)      497 2023-07-14 12:08:04.267146 nemo-sz-0.6.0/nemo/_version.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)    39014 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/nemo/catalogs.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)    88877 2023-07-14 12:02:44.000000 nemo-sz-0.6.0/nemo/completeness.py
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.263146 nemo-sz-0.6.0/nemo/data/
+-rw-rw-r--   0 matty     (1000) matty     (1000)   140701 2019-03-11 10:14:35.000000 nemo-sz-0.6.0/nemo/data/planck_lensedCls.dat
+-rw-rw-r--   0 matty     (1000) matty     (1000)    67692 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/nemo/filters.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     4464 2021-11-17 06:29:36.000000 nemo-sz-0.6.0/nemo/gnfw.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)   127604 2023-07-14 12:05:05.000000 nemo-sz-0.6.0/nemo/maps.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)    26084 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/nemo/photometry.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)    55311 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/nemo/pipelines.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1576 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/nemo/plotSettings.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)    72242 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/nemo/signals.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)    40957 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/nemo/startUp.py
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.263146 nemo-sz-0.6.0/nemo_sz.egg-info/
+-rw-rw-r--   0 matty     (1000) matty     (1000)      776 2023-07-14 12:08:04.000000 nemo-sz-0.6.0/nemo_sz.egg-info/PKG-INFO
+-rw-rw-r--   0 matty     (1000) matty     (1000)     4198 2023-07-14 12:08:04.000000 nemo-sz-0.6.0/nemo_sz.egg-info/SOURCES.txt
+-rw-rw-r--   0 matty     (1000) matty     (1000)        1 2023-07-14 12:08:04.000000 nemo-sz-0.6.0/nemo_sz.egg-info/dependency_links.txt
+-rw-rw-r--   0 matty     (1000) matty     (1000)      121 2023-07-14 12:08:04.000000 nemo-sz-0.6.0/nemo_sz.egg-info/requires.txt
+-rw-rw-r--   0 matty     (1000) matty     (1000)        5 2023-07-14 12:08:04.000000 nemo-sz-0.6.0/nemo_sz.egg-info/top_level.txt
+-rw-rw-r--   0 matty     (1000) matty     (1000)       81 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/pyproject.toml
+-rw-rw-r--   0 matty     (1000) matty     (1000)      192 2023-07-14 12:08:04.267146 nemo-sz-0.6.0/setup.cfg
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2019 2023-07-13 15:43:22.000000 nemo-sz-0.6.0/setup.py
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.263146 nemo-sz-0.6.0/tests/
+-rw-rw-r--   0 matty     (1000) matty     (1000)      977 2021-11-17 06:29:36.000000 nemo-sz-0.6.0/tests/README.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2157 2021-09-07 15:31:52.000000 nemo-sz-0.6.0/tests/clusters.robot
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.267146 nemo-sz-0.6.0/tests/configs/
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1236 2021-11-17 06:29:36.000000 nemo-sz-0.6.0/tests/configs/MPITestSurveyMaskHeader.txt
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1324 2021-09-07 15:31:52.000000 nemo-sz-0.6.0/tests/configs/PSTest_E-D56.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1430 2021-09-07 15:31:52.000000 nemo-sz-0.6.0/tests/configs/PSTest_south2008.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1233 2021-09-07 15:31:52.000000 nemo-sz-0.6.0/tests/configs/PSTest_south2008_fourier.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)      255 2021-09-07 15:31:52.000000 nemo-sz-0.6.0/tests/configs/README.rst
+-rw-rw-r--   0 matty     (1000) matty     (1000)     3442 2021-09-07 15:31:52.000000 nemo-sz-0.6.0/tests/configs/equD56_quick_fourier.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6660 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/tests/configs/quickstart-multipass.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     5937 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/tests/configs/sim_cl_A10_MFMF_tiles.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     5937 2022-11-15 08:06:49.000000 nemo-sz-0.6.0/tests/configs/sim_cl_A10_MFMF_tiles_multipass.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     5732 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/tests/configs/sim_cl_B12_MFMF_tiles.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6038 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/tests/configs/sim_cl_MFMF.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     6107 2022-11-15 08:07:19.000000 nemo-sz-0.6.0/tests/configs/sim_cl_MFMF_pass2.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1365 2022-01-11 13:00:45.000000 nemo-sz-0.6.0/tests/configs/sim_ptsrc_f090.yml
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1236 2021-09-07 15:31:52.000000 nemo-sz-0.6.0/tests/configs/smallTestSurveyMaskHeader.txt
+-rw-rw-r--   0 matty     (1000) matty     (1000)     1227 2021-11-17 06:29:36.000000 nemo-sz-0.6.0/tests/debug.py
+drwxrwxr-x   0 matty     (1000) matty     (1000)        0 2023-07-14 12:08:04.267146 nemo-sz-0.6.0/tests/lib/
+-rw-rw-r--   0 matty     (1000) matty     (1000)    17643 2022-01-21 15:05:26.000000 nemo-sz-0.6.0/tests/lib/NemoTests.py
+-rw-rw-r--   0 matty     (1000) matty     (1000)     2422 2021-09-07 15:31:52.000000 nemo-sz-0.6.0/tests/point_sources.robot
+-rw-rw-r--   0 matty     (1000) matty     (1000)     5896 2023-07-13 13:29:55.000000 nemo-sz-0.6.0/tests/quick.robot
+-rw-rw-r--   0 matty     (1000) matty     (1000)    70144 2021-02-17 13:10:21.000000 nemo-sz-0.6.0/versioneer.py
```

### Comparing `nemo-sz-0.5.0/INSTALL.rst` & `nemo-sz-0.6.0/INSTALL.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 **Nemo** is written in `Python <https://www.python.org/>`_ (3.6+), and requires the
 following additional modules to be installed (currently used versions are given in
 brackets, later versions also probably work):
 
-* numpy (1.13.3)
+* numpy (1.19)
 * scipy (1.3.0)
 * matplotlib (2.1.1)
 * astLib (0.11.7)
-* `pixell <https://github.com/simonsobs/pixell/>`_ (0.6.3 or git version)
+* `pixell <https://github.com/simonsobs/pixell/>`_ (0.17 or later)
 * Pillow (5.1.0)
 * astropy (4.0)
-* Cython (0.24.1)
 * PyYAML (3.12)
 * `CCL <https://github.com/LSSTDESC/CCL>`_ (2.1 or later)
 * mpi4py (3.0.0)
 * colorcet (1.0.0; https://github.com/bokeh/colorcet/releases)
 
 The latest tagged version of **Nemo** can be installed using ``pip``:
     
 .. code-block::
 
    pip install nemo-sz
 
-Note that you will need to have ``cython`` and ``numpy`` installed already (for the moment).
-Other dependencies will be installed by ``pip``, except for ``pyccl`` and ``mpi4py``.
+Dependencies will be installed by ``pip``, except for ``pyccl`` and ``mpi4py``.
 
 You may also install using the standard ``setup.py`` script, e.g., as root:
 
 .. code-block::
 
    sudo python setup.py install
```

### Comparing `nemo-sz-0.5.0/PKG-INFO` & `nemo-sz-0.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: nemo-sz
-Version: 0.5.0
+Version: 0.6.0
 Summary: Millimeter-wave galaxy cluster and source detection package.
 Home-page: https://nemo-sz.readthedocs.io
 Author: Matt Hilton + Nemo Contributors
 Author-email: hiltonm@ukzn.ac.za
-License: UNKNOWN
-Description: Millimeter-wave map filtering and Sunyaev-Zel'dovich galaxy cluster/source detection package. Originally developed for the Atacama Cosmology Telescope project.
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Astronomy
+License-File: LICENSE
+
+Millimeter-wave map filtering and Sunyaev-Zel'dovich galaxy cluster/source detection package. Originally developed for the Atacama Cosmology Telescope project.
```

### Comparing `nemo-sz-0.5.0/README.rst` & `nemo-sz-0.6.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 `Atacama Cosmology Telescope <https://act.princeton.edu/>`_ project,
 and capable of analyzing maps that will be produced by the
 `Simons Observatory <https://simonsobservatory.org/>`_.
 
 * **Documentation:** https://nemo-sz.readthedocs.io
 * **License:** `BSD 3-Clause <LICENSE>`_
 * **Authors:** Matt Hilton, with contributions from Simone Aiola, David Alonso,
-  Matthew Hasselfield, Kevin Huffenberger, Toby Marriage, Sigurd Naess, and Cristóbal Sifón
-  (not all reflected on GitHub).
+  Matthew Hasselfield, Kevin Huffenberger, Toby Marriage, Niall MacCrann,
+  Sigurd Naess, and Cristóbal Sifón (not all reflected on GitHub).
 * **Installation:** ``pip install nemo-sz``
 * **Support:** Please use the `GitHub issues page <https://github.com/simonsobs/nemo/issues>`_, 
   and/or contact `Matt Hilton <mailto:matt.hilton@mykolab.com>`_.
 
 **Nemo** is written in `Python <https://www.python.org/>`_ and
 provides `several modules <https://nemo-sz.readthedocs.io/en/latest/reference.html>`_ that
 may be useful for analyzing ACT/SO data, in addition to the command-line programs provided
```

### Comparing `nemo-sz-0.5.0/bin/nemoCatalogCheck` & `nemo-sz-0.6.0/bin/nemoCatalogCheck`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/bin/nemoMass` & `nemo-sz-0.6.0/bin/nemoMass`

 * *Files 14% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 from nemo import maps
 from nemo import filters
 from nemo import MockSurvey
 from nemo import photometry
 from nemo import startUp
 from nemo import completeness
 from nemo import pipelines
+on_rtd=os.environ.get('READTHEDOCS', None)
+if on_rtd is None:
+    import pyccl as ccl
 import argparse
 import astropy.io.fits as pyfits
 import time
 import yaml
 
 #------------------------------------------------------------------------------------------------------------
 def addForcedPhotometry(pathToCatalog, config, zColumnName = None, zErrColumnName = None):
@@ -93,42 +96,56 @@
     tab=forcedMatched
     tab.add_column(zMatched['redshift'])
     tab.add_column(zMatched['redshiftErr'])
     
     return tab
 
 #------------------------------------------------------------------------------------------------------------
-def calcMass(tab, massOptions, QFit, fRelWeightsDict, mockSurvey):
+def calcMass(tab, massOptions, QFit, fRelWeightsDict, mockSurvey, otherMassEstimates = []):
     """Calculates masses for cluster data in table.
     
     """
 
+    try:
+        refMassDef=ccl.halos.MassDef(massOptions['delta'], massOptions['rhoType'],
+                                     c_m_relation = massOptions['concMassRelation'])
+    except:
+        refMassDef=ccl.halos.MassDef(massOptions['delta'], massOptions['rhoType'])
+
     if 'relativisticCorrection' not in massOptions.keys():
         massOptions['relativisticCorrection']=True
         
     # Experimenting with E(z)^gamma instead of E(z)^2
     if 'Ez_gamma' not in massOptions.keys():
         massOptions['Ez_gamma']=2
 
     # Experimenting with arbitrary (1+z)^something
     if 'onePlusRedshift_power' not in massOptions.keys():
         massOptions['onePlusRedshift_power']=0.0
     
     print("massOptions", massOptions)
-        
-    label=mockSurvey.mdefLabel
-    colNames=['%s' % (label), '%sUncorr' % (label)]
-    if 'rescaleFactor' in massOptions.keys():
-        colNames.append('%sCal' % (label))
-    colNames=colNames+["M200m", "M200mUncorr"] # We will generalize fully later so user can choose mass defs
-    for c in colNames:
-        tab['%s' % (c)]=np.zeros(len(tab))
-        tab['%s_errPlus' % (c)]=np.zeros(len(tab))
-        tab['%s_errMinus' % (c)]=np.zeros(len(tab))
-    
+
+    # Add all columns for all used mass definitions
+    labels=['M%d%s' % (massOptions['delta'], massOptions['rhoType'][0])]
+    for massDefDict in otherMassEstimates:
+        labels.append('M%d%s' % (massDefDict['delta'], massDefDict['rhoType'][0]))
+    for l in labels:
+        colNames=['%s' % (l), '%sUncorr' % (l)]
+        if 'rescaleFactor' in massOptions.keys():
+            colNames.append('%sCal' % (l))
+        colNames=colNames+["M200m", "M200mUncorr"] # We will generalize fully later so user can choose mass defs
+        for c in colNames:
+            tab['%s' % (c)]=np.zeros(len(tab))
+            tab['%s_errPlus' % (c)]=np.zeros(len(tab))
+            tab['%s_errMinus' % (c)]=np.zeros(len(tab))
+            if l == labels[0]:
+                tab['Q']=np.zeros(len(tab))
+    label=labels[0]
+    assert(label == mockSurvey.mdefLabel)
+
     count=0
     for row in tab:
         count=count+1
         print("... rank %d; %d/%d; %s (%.3f +/- %.3f) ..." % (config.rank, count, len(tab), row['name'], 
                                                               row['redshift'], row['redshiftErr']))
 
         tileName=row['tileName']
@@ -148,14 +165,15 @@
                                             applyMFDebiasCorrection = True,
                                             applyRelativisticCorrection = massOptions['relativisticCorrection'],
                                             fRelWeightsDict = fRelWeightsDict[tileName],
                                             tileName = tileName)
             row['%s' % (label)]=massDict['%s' % (label)]
             row['%s_errPlus' % (label)]=massDict['%s_errPlus' % (label)]
             row['%s_errMinus' % (label)]=massDict['%s_errMinus' % (label)]
+            row['Q']=massDict['Q']
             # Uncorrected for mass function steepness
             unCorrMassDict=signals.calcMass(row['fixed_y_c']*1e-4, row['fixed_err_y_c']*1e-4, 
                                                     row['redshift'], row['redshiftErr'],
                                                     tenToA0 = massOptions['tenToA0'],
                                                     B0 = massOptions['B0'], 
                                                     Mpivot = massOptions['Mpivot'], 
                                                     sigma_int = massOptions['sigma_int'],
@@ -165,31 +183,44 @@
                                                     applyMFDebiasCorrection = False,
                                                     applyRelativisticCorrection = massOptions['relativisticCorrection'],
                                                     fRelWeightsDict = fRelWeightsDict,
                                                     tileName = tileName)
             row['%sUncorr' % (label)]=unCorrMassDict['%s' % (label)]
             row['%sUncorr_errPlus' % (label)]=unCorrMassDict['%s_errPlus' % (label)]
             row['%sUncorr_errMinus' % (label)]=unCorrMassDict['%s_errMinus' % (label)]
-            # Mass conversion -  remove later when fully generalized
-            row['M200m']=signals.convertM500cToM200m(massDict['M500c']*1e14, row['redshift'])/1e14
-            row['M200m_errPlus']=(row['M500c_errPlus']/row['M500c'])*row['M200m']
-            row['M200m_errMinus']=(row['M500c_errMinus']/row['M500c'])*row['M200m']
-            row['M200mUncorr']=signals.convertM500cToM200m(unCorrMassDict['M500c']*1e14, row['redshift'])/1e14
-            row['M200mUncorr_errPlus']=(row['M500cUncorr_errPlus']/row['M500cUncorr'])*row['M200mUncorr']
-            row['M200mUncorr_errMinus']=(row['M500cUncorr_errMinus']/row['M500cUncorr'])*row['M200mUncorr']
             # Re-scaling (e.g., using richness-based weak-lensing mass calibration)
             if 'rescaleFactor' in massOptions.keys():
-                row['%sCal' % (label)]=massDict['%s' % (label)]/massOptions['rescaleFactor']        
+                row['%sCal' % (label)]=massDict['%s' % (label)]/massOptions['rescaleFactor']
                 row['%sCal_errPlus' % (label)]=np.sqrt(np.power(row['%s_errPlus' % (label)]/row['%s' % (label)], 2) + \
                                                        np.power(massOptions['rescaleFactorErr']/massOptions['rescaleFactor'], 2))*row['%sCal' % (label)]
                 row['%sCal_errMinus' % (label)]=np.sqrt(np.power(row['%s_errMinus' % (label)]/row['%s' % (label)], 2) + \
                                                         np.power(massOptions['rescaleFactorErr']/massOptions['rescaleFactor'], 2))*row['%sCal' % (label)]
-            #row['M200mCal']=signals.convertM500cToM200m(row['M500Cal']*1e14, row['redshift'])/1e14
-            #row['M200mCal_errPlus']=(row['M500Cal_errPlus']/row['M500Cal'])*row['M200mCal']
-            #row['M200mCal_errMinus']=(row['M500Cal_errMinus']/row['M500Cal'])*row['M200mCal']
+                calMassDict={label: row['%sCal' % (label)],
+                             label+'_errPlus': row['%sCal_errPlus' % (label)],
+                             label+'_errMinus': row['%sCal_errMinus' % (label)]}
+
+            # CCL-based mass conversions
+            resultsList=[massDict, unCorrMassDict]
+            suffixList=['', 'Uncorr']
+            if 'rescaleFactor' in massOptions.keys():
+                resultsList.append(calMassDict)
+                suffixList.append('Cal')
+            for resultDict, suffix in zip(resultsList, suffixList):
+                for massDefDict in otherMassEstimates:
+                    if 'concMassRelation' not in massDefDict.keys():
+                        massDefDict['concMassRelation']=None
+                    thisLabel='M%d%s' % (massDefDict['delta'], massDefDict['rhoType'][0])
+                    try:
+                        thisMassDef=ccl.halos.MassDef(massDefDict['delta'], massDefDict['rhoType'], c_m_relation = massDefDict['concMassRelation'])
+                    except:
+                        thisMassDef=ccl.halos.MassDef(massDefDict['delta'], massDefDict['rhoType'])
+                    thisMass=signals.MDef1ToMDef2(resultDict[label]*1e14, row['redshift'], refMassDef, thisMassDef, mockSurvey.cosmoModel)/1e14
+                    row[thisLabel+suffix]=thisMass
+                    row[thisLabel+suffix+'_errPlus']=(row[label+suffix+'_errPlus']/row[label+suffix])*row[thisLabel+suffix]
+                    row[thisLabel+suffix+'_errMinus']=(row[label+suffix+'_errMinus']/row[label+suffix])*row[thisLabel+suffix]
 
     return tab
 
 #------------------------------------------------------------------------------------------------------------
 def makeParser():
     
     parser=argparse.ArgumentParser("nemoMass")
@@ -199,14 +230,22 @@
                         redshift, redshiftErr. If the catalog contains fixed_y_c, fixed_err_y_c columns,\
                         then these will be used to infer mass estimates. If not, 'forced photometry' mode \
                         will be enabled, and the fixed_y_c, fixed_err_y_c values will be extracted from the\
                         filtered maps.", default = None)
     parser.add_argument("-o", "--output", dest="outFileName", help = "Output catalog file name \
                         (.fits format). If not given, the name of the output catalog file will be based on\
                         either configFileName or catFileName.", default = None)
+    parser.add_argument("-Q", "--Q-source", dest="QSource", help = "Source of the Q function data - either\
+                        'fit' (the 'classic' method), 'injection' (for Q based on source injection test\
+                        results), or 'hybrid' (uses the 'fit' method for scales smaller than the reference\
+                        filter scale, and the 'injection' method for scales larger than the reference filter\
+                        scale).", default = 'fit')
+    parser.add_argument("-x", "--x-match-arcmin", dest="xMatchArcmin", default = 2.5,
+                        help = "Specifies the cross-match radius (in arcmin) to use when matching the redshift\
+                        catalog onto the cluster candidate catalog.")
     parser.add_argument("-z", "--z-column", dest="zColumnName", help = "Specifies the name of the redshift\
                         column in the input catalog.", default = None)
     parser.add_argument("-e", "--z-error-column", dest="zErrColumnName", help = "Specifies the name of the \
                         redshift uncertainty column in the input catalog.", default = None)
     parser.add_argument("-F", "--forced-photometry", dest="forcedPhotometry", help = "Perform forced photometry.\
                         This is automatically enabled if the catalog does not contain the fixed_y_c, \
                         fixed_err_y_c columns. Use this switch to force using this mode even if the \
@@ -231,29 +270,37 @@
     parser = makeParser()
     args = parser.parse_args()
     
     parDictFileName=args.configFileName
     catFileName=args.catFileName
     outFileName=args.outFileName
     forcedPhotometry=args.forcedPhotometry
+    QSource=args.QSource
+    if QSource not in ['fit', 'injection', 'hybrid']:
+        raise Exception("QSource must be either 'fit', 'injection', or 'hybrid'")
     
     if args.noStrictMPIExceptions == True:
         strictMPIExceptions=False
     else:
         strictMPIExceptions=True
     
     # Load the nemo catalog and match against the z catalog
     # NOTE: This is now done using coord matching (nearest within some maximum tolerance), rather than names
     if catFileName is None:
         config=startUp.NemoConfig(parDictFileName, MPIEnabled = args.MPIEnabled, divideTilesByProcesses = False,
-                                  setUpMaps = False, verbose = False, strictMPIExceptions = strictMPIExceptions)
+                                  makeOutputDirs = False, setUpMaps = False, verbose = False,
+                                  strictMPIExceptions = strictMPIExceptions)
         optimalCatalogFileName=config.rootOutDir+os.path.sep+"%s_optimalCatalog.fits" % (os.path.split(config.rootOutDir)[-1])           
         nemoTab=atpy.Table().read(optimalCatalogFileName)
         zTab=atpy.Table().read(config.parDict['massOptions']['redshiftCatalog'])
-        nemoTab, zTab, rDeg=catalogs.crossMatch(nemoTab, zTab, radiusArcmin = 2.5)
+        if args.xMatchArcmin != 'act':
+            xMatchArcmin=float(args.xMatchArcmin)
+            nemoTab, zTab, rDeg=catalogs.crossMatch(nemoTab, zTab, radiusArcmin = xMatchArcmin)
+        else:
+            raise Exception("Fancier cross-matching not implemented yet.")
         nemoTab['redshift']=zTab['redshift']
         if 'redshiftErr' in zTab.keys():
             nemoTab['redshiftErr']=zTab['redshiftErr']
         else:
             print("... WARNING: no redshiftErr column found in '%s' - assuming redshiftErr = 0 for all clusters ..." %  (config.parDict['massOptions']['redshiftCatalog']))
             nemoTab['redshiftErr']=0
         tab=nemoTab
@@ -276,17 +323,23 @@
                 forcedPhotometry=True
         config=startUp.NemoConfig(parDictFileName, MPIEnabled = args.MPIEnabled, divideTilesByProcesses = False,
                                   setUpMaps = forcedPhotometry, writeTileDir = False, verbose = False,
                                   strictMPIExceptions = strictMPIExceptions)
     
     # Remaining set-up
     massOptions=config.parDict['massOptions']
-    Q=signals.QFit(config)    
+    Q=signals.QFit(QSource, selFnDir = config.selFnDir)
     fRelWeightsDict=signals.getFRelWeights(config)
     
+    if 'otherMassEstimates' in config.parDict.keys() and config.parDict['massOptions'] is not None:
+        otherMassEstimates=config.parDict['otherMassEstimates']
+    else:
+        # Default to match older versions of Nemo
+        otherMassEstimates=[{'delta': 200, 'rhoType': 'matter', 'concMassRelation': "Bhattacharya13"}]
+
     # Forced photometry (if enabled) - modifying table in place
     # NOTE: Move this up if/when we make it run under MPI
     if forcedPhotometry == True:
         tab=addForcedPhotometry(catFileName, config, args.zColumnName, args.zErrColumnName)
     
     # Set cosmological parameters for e.g. E(z) calc if these are set in .par file
     # We set them after the Q calc, because the Q calc needs to be for the fiducial cosmology
@@ -296,49 +349,35 @@
     # Hence minMass here needs to be set well below the survey mass limit
     # areaDeg2 we don't care about here
     minMass=1e13
     areaDeg2=700.
     zMin=0.0
     zMax=2.0
     # H0, Om0, Ol0 used for E(z), theta500 calcs in Q - these are updated when we call create mockSurvey
-    if 'H0' in list(massOptions.keys()):
-        H0=massOptions['H0']
-    else:
-        H0=70.
-    if 'Om0' in list(massOptions.keys()):
-        Om0=massOptions['Om0']
-    else:
-        Om0=0.3
-    # OmegaB0, sigma8 only used for mass function Eddington bias correction
-    if 'Ob0' in list(massOptions.keys()):
-        Ob0=massOptions['Ob0']
-    else:
-        Ob0=0.05
-    if 'sigma8' in list(massOptions.keys()):
-        sigma8=massOptions['sigma8']
-    else:
-        sigma8=0.8
-    if 'ns' in list(massOptions.keys()):
-        ns=massOptions['ns']
-    else:
-        ns=0.95
-    mockSurvey=MockSurvey.MockSurvey(minMass, areaDeg2, zMin, zMax, H0, Om0, Ob0, sigma8, ns)
+    # NOTE: startUp now sets defaults for these if not given in config
+    H0=massOptions['H0']
+    Om0=massOptions['Om0']
+    Ob0=massOptions['Ob0']
+    sigma8=massOptions['sigma8']
+    ns=massOptions['ns']
+    mockSurvey=MockSurvey.MockSurvey(minMass, areaDeg2, zMin, zMax, H0, Om0, Ob0, sigma8, ns,
+                                     rhoType = massOptions['rhoType'], delta = massOptions['delta'])
         
     # Seems like multiprocessing doesn't work under slurm...   
     # So use MPI instead: just divide up catalog among processes
     tab.add_column(atpy.Column(np.arange(len(tab)), "sortIndex"))
     if config.MPIEnabled == True:
         numRowsPerProcess=int(np.ceil(len(tab)/config.size))
         startIndex=config.rank*numRowsPerProcess
         endIndex=startIndex+numRowsPerProcess
         if config.rank == config.size-1:
             endIndex=len(tab)
         tab=tab[startIndex:endIndex]
         
-    tab=calcMass(tab, massOptions, Q, fRelWeightsDict, mockSurvey)
+    tab=calcMass(tab, massOptions, Q, fRelWeightsDict, mockSurvey, otherMassEstimates = otherMassEstimates)
     
     if config.MPIEnabled == True:
         tabList=config.comm.gather(tab, root = 0)
         if config.rank != 0:
             assert tabList is None
             print("... MPI rank %d finished ..." % (config.rank))
             sys.exit()
@@ -349,14 +388,15 @@
     tab.sort('sortIndex')
     tab.remove_column('sortIndex')
     
     outDir=os.path.split(outFileName)[0]
     if outDir != '':
         os.makedirs(outDir, exist_ok = True)
     tab.meta['NEMOVER']=nemo.__version__
+    tab.meta['QSOURCE']=QSource
     tab.write(outFileName, overwrite = True)
     
     # Detect if testing a mock catalog, and write some stats on recovered masses
     if 'true_M500' in tab.keys():
         # Noise sources in mocks
         if 'applyPoissonScatter' in config.parDict.keys():
             applyPoissonScatter=config.parDict['applyPoissonScatter']
```

### Comparing `nemo-sz-0.5.0/bin/nemoMock` & `nemo-sz-0.6.0/bin/nemoMock`

 * *Files 11% similar despite different names*

```diff
@@ -48,14 +48,17 @@
     parser.add_argument("-C", "--combine-mocks", dest="combineMocks", action="store_true", 
                         help="Combine the mocks into one large catalog (use this to make oversampled\
                         mock catalogs).", default = False)
     #parser.add_argument("-f", "--footprint", dest = "footprint", help="""Footprint to use, e.g., DES,
                         #HSC, KiDS (default: full).""", default = None)
     parser.add_argument("-S", "--SNR-cut", dest = "SNRCut", help="Include only clusters with\
                         fixed_SNR > this value.", default = 4.0, type = float)
+    parser.add_argument("-Q", "--Q-source", dest="QSource", help = "Source of the Q function data - either\
+                        'fit' (the 'classic' method) or 'injection' (for Q based on source injection test\
+                        results.", default = 'fit')
     #parser.add_argument("-M", "--mpi", dest="MPIEnabled", action="store_true", help="""Enable MPI. If you 
                         #want to use this, run with e.g., mpiexec -np 4 nemoMock selFnDir mocksDir -M""", 
                         #default = False)
     
     return parser
     
 #------------------------------------------------------------------------------------------------------------
@@ -69,14 +72,17 @@
     configFileName=args.configFileName
     numMocksToMake=args.numMocks
     combineMocks=args.combineMocks
     SNRCut=args.SNRCut
     MPIEnabled=False
     #zStep=args.zStep
     #footprintLabel=args.footprint
+    QSource=args.QSource
+    if QSource not in ['fit', 'injection']:
+        raise Exception("QSource must be either 'fit' or 'injection'")
 
     if configFileName is None:
         configFileName=args.selFnDir+os.path.sep+"config.yml"
     config=startUp.NemoConfig(configFileName, MPIEnabled = MPIEnabled, makeOutputDirs = False, 
                               selFnDir = selFnDir, setUpMaps = False, verbose = False)
     config.mocksDir=mocksDir
     config.parDict['thresholdSigma']=args.SNRCut
@@ -88,8 +94,8 @@
             numMocksToMake=1
 
     # Remove this once we re-jig for MPI
     if config.MPIEnabled == True and numMocksToMake > 1:
         raise Exception("NemoMock needs to be adapted for MPI if making multiple mocks - not done yet.")
 
     pipelines.makeMockClusterCatalog(config, numMocksToMake = numMocksToMake, combineMocks = combineMocks,
-                                     writeCatalogs = True, verbose = True)
+                                     writeCatalogs = True, verbose = True, QSource = QSource)
```

### Comparing `nemo-sz-0.5.0/bin/nemoModel` & `nemo-sz-0.6.0/bin/nemoModel`

 * *Files 22% similar despite different names*

```diff
@@ -8,29 +8,33 @@
 
 import os
 import sys
 import numpy as np
 import astropy.table as atpy
 import astropy.io.fits as pyfits
 from astLib import *
-from nemo import startUp
-from nemo import maps
-from nemo import catalogs
+from nemo import startUp, maps, catalogs, signals
 import argparse
 import astropy.io.fits as pyfits
+on_rtd=os.environ.get('READTHEDOCS', None)
+if on_rtd is None:
+    import pyccl as ccl
 
 #------------------------------------------------------------------------------------------------------------
 def makeParser():
     
     parser=argparse.ArgumentParser("nemoModel")
     parser.add_argument("catalog", help = "Either the path to a Nemo FITS-table format catalog,\
                         or 'pointsources-N' (to generate a test catalog of N point sources that will be\
                         inserted into the map, e.g., pointsources-1000 will insert 1000 sources). If\
                         the latter, the catalog will be written to outputFileName_inputCatalog.fits\
-                        (with the .fits extension stripped from outputFileName).")
+                        (with the .fits extension stripped from outputFileName). If the former,\
+                        cosmological parameters may be specified in the FITS header using the\
+                        OM0, OB0, H0, SIGMA8, NS keywords (used only for cluster models at the\
+                        moment).")
     parser.add_argument("maskFileName", help = "A FITS image file, containing a mask of the desired sky\
                         area. Non-zero values in the mask are used to define tiles (typically 10 x 5 deg),\
                         which are processed in parallel if MPI is enabled (see -M switch). The output sky\
                         model image will have the same pixelization as the mask image.")
     parser.add_argument("beamFileName", help = "A file containing the beam profile, in the standard format\
                         used by ACT.")
     parser.add_argument("outputFileName", help = "The name of the output file that will contain the sky\
@@ -54,17 +58,33 @@
                         --cmb-seed to set the random seed to the same value if creating sets of maps at\
                         different frequencies. Note that this is very memory intensive for large maps,\
                         and is a serial operation.")
     parser.add_argument("-S", "--seed", dest = "seed", type = int, default = None,
                         help = "Random seed used only for generating (optional) cosmic microwave\
                         background or source catalog realizations (i.e., the seed is not used for\
                         noise realizations).")
-    parser.add_argument("-N", "--add-white-noise", dest = "addWhiteNoise", type = float, default = 0.0,
+    parser.add_argument("-N", "--add-noise", dest = "addNoise", default = 0.0,
                         help = "If a random cosmic microwave background realization had been added, add\
-                        uniform per-pixel white noise at the specified level.")
+                        white noise. If a number is given, uniform per-pixel white noise at the specified\
+                        level is added. If a number followed by 'sb' is given (e.g., 40sb), then constant\
+                        surface brightness noise (per square arcmin) is added, adjusting for varying pixel\
+                        scale across the map (if present). Otherwise, a path to an inverse variance map\
+                        can be given (must have the same pixelization as the supplied mask).")
+    parser.add_argument("-k", "--lknee", dest = "lKnee", default = None, type = float,
+                        help = "Must be used with -N (--add-noise) and -C (--add-cmb). If given,\
+                        1/f noise with power spectrum N_l = (1 + l/lknee)^-3) will be generated and added\
+                        to the map (see Appendix A of MacCrann et al. 2023). Reasonable values to use\
+                        are 2000 for ACT f090, and 3000 for ACT f150.")
+    parser.add_argument("-A", "--add-map", dest = "addMap", default = None,
+                        help = "Path to a FITS map (same pixelization as the input mask) that will be\
+                        added to the output sim map. Useful if you want to add extra pre-computed signals\
+                        to the map (e.g., Galactic dust, large scale noise components etc.). Amplitudes\
+                        can be modified with the --add-map-scaling parameter.")
+    parser.add_argument("--add-map-scaling", dest = "addMapScaling", default = 1.0,
+                        help = "If given, multiply the map pointed to by --add-map by this factor.")
     parser.add_argument("--split-noise-test", dest = "splitNoiseTest", action = "store_true",
                         help = "If set, and -N and -C switches are used, split the map into two\
                         sections, with the white noise level doubled in one half of the map.")
     parser.add_argument("-T", "--break-map-into-tiles", dest = "breakIntoTiles", action = "store_true",
                         help = "Break large maps into tiles using the autotiler function in Nemo.\
                         This will be turned on automatically if MPI is enabled (using -M).", 
                         default = False)
@@ -83,46 +103,77 @@
                         to the Exception handling in mpi4py.", default = False)
     
     return parser
 
 #------------------------------------------------------------------------------------------------------------
 if __name__ == '__main__':
 
-    parser = makeParser()
-    args = parser.parse_args()
+    parser=makeParser()
+    args=parser.parse_args()
     
     if args.noStrictMPIExceptions == True:
         strictMPIExceptions=False
     else:
         strictMPIExceptions=True
 
+    if args.addMap is not None:
+        assert(os.path.exists(args.addMap) == True)
+
     # Create a stub config (then we can use existing start-up stuff to dish out the tiles)
     print(">>> Setting up ...")
     parDict={}
     mapDict={}
     mapDict['mapFileName']=args.maskFileName
     mapDict['obsFreqGHz']=args.obsFreqGHz
     mapDict['beamFileName']=args.beamFileName
     parDict['unfilteredMaps']=[mapDict]
     parDict['mapFilters']=[]
+    parDict['useTiling']=False
+    parDict['reprojectToTan']=False
     if args.MPIEnabled == True or args.breakIntoTiles == True:
-        parDict['makeTileDir']=True
+        parDict['useTiling']=True
         parDict['tileOverlapDeg']=1.0
-        parDict['tileDefLabel']='auto'
         parDict['tileDefinitions']={'mask': args.maskFileName,
                                     'targetTileWidthDeg': 10.0, 'targetTileHeightDeg': 5.0}
 
     config=startUp.NemoConfig(parDict, MPIEnabled = args.MPIEnabled, divideTilesByProcesses = True,
-                              makeOutputDirs = False, setUpMaps = True, writeTileDir = False, 
+                              makeOutputDirs = False, setUpMaps = True, writeTileInfo = False,
                               verbose = False, strictMPIExceptions = strictMPIExceptions)
     
     baseDir, fileName=os.path.split(args.outputFileName)
     if baseDir != '':
         os.makedirs(baseDir, exist_ok = True)
-    
+
+    # Noise:
+    # - if number, uniform white noise level per pixel
+    # - if number with sb suffix, uniform white noise level per square arcmin
+    # - if string, a path to ivar map
+    if config.rank == 0:
+        if type(args.addNoise) == str and args.addNoise[-2:] == 'sb':
+            addNoise=float(args.addNoise.split('sb')[0])
+            noiseMode='perSquareArcmin'
+        else:
+            noiseMode='perPixel'
+            try:
+                addNoise=float(args.addNoise)
+            except:
+                # Assumed inv var map path
+                with pyfits.open(args.addNoise) as img:
+                    if img[0].data.ndim == 2:
+                        sigma=img[0].data
+                    else:
+                        sigma=img[0].data[0]
+                    addNoiseWCS=astWCS.WCS(img[0].header, mode = 'pyfits')
+                valid=sigma > 1e-7
+                sigma[valid]=np.sqrt(1/sigma[valid])
+                addNoise=sigma
+    else:
+        addNoise=None
+        noiseMode=None
+
     if args.catalog[:12] == 'pointsources':
         try:
             numSources=int(args.catalog.split("-")[-1])
         except:
             raise Exception("Use format pointsources-N, e.g., pointsources-100 will generate a test catalog of 100 sources.")
         with pyfits.open(args.maskFileName) as img:
             for extName in img:
@@ -133,33 +184,48 @@
             if numSources > 0:
                 tab=catalogs.generateRandomSourcesCatalog(data, wcs, numSources, seed = args.seed)
                 tab.write(args.outputFileName.replace(".fits", "_inputCatalog.fits"), overwrite = True)
             else:
                 tab=atpy.Table(names = ('RADeg', 'decDeg'))
     else:
         tab=atpy.Table().read(args.catalog)
-    
+
+    # Optionally override the fiducial cosmology (only useful for cluster sims)
+    keywords=['OM0', 'OB0', 'H0', 'SIGMA8', 'NS']
+    keyCount=0
+    for key in keywords:
+        if key in tab.meta.keys():
+            keyCount=keyCount+1
+    if keyCount == len(keywords):
+        print(">>> Using cosmology specified in header for catalog %s [only affects painted cluster sizes]" % (args.catalog))
+        cosmoModel=ccl.Cosmology(Omega_c = tab.meta['OM0']-tab.meta['OB0'], Omega_b = tab.meta['OB0'],
+                                 h = 0.01*tab.meta['H0'], sigma8 = tab.meta['SIGMA8'], n_s = tab.meta['NS'],
+                                 transfer_function = signals.transferFunction)
+    else:
+        print(">>> Using fiducial cosmology")
+        cosmoModel=signals.fiducialCosmoModel
+
     # Optional signal scaling (useful for diff alpha sims)
     if 'y_c' in tab.keys():
         tab['y_c']=tab['y_c']*args.scale
     
     # Build a dictionary containing the model images which we'll stich together at the end
     print(">>> Building models in tiles ...")
     modelsDict={}
     for tileName in config.tileNames:
         print("... %s ..." % (tileName))
         shape=(config.tileCoordsDict[tileName]['clippedSection'][3]-config.tileCoordsDict[tileName]['clippedSection'][2], 
                config.tileCoordsDict[tileName]['clippedSection'][1]-config.tileCoordsDict[tileName]['clippedSection'][0])
         wcs=astWCS.WCS(config.tileCoordsDict[tileName]['header'], mode = 'pyfits')
         try:
-            modelsDict[tileName]=maps.makeModelImage(shape, wcs, tab, args.beamFileName, 
+            modelsDict[tileName]=maps.makeModelImage(shape, wcs, tab, args.beamFileName,
                                                      obsFreqGHz = args.obsFreqGHz,
                                                      validAreaSection = config.tileCoordsDict[tileName]['areaMaskInClipSection'],
                                                      TCMBAlpha = args.TCMBAlpha,
-                                                     profile = args.profile)
+                                                     profile = args.profile, cosmoModel = cosmoModel)
         except:
             raise Exception("makeModelImage failed on tile '%s'" % (tileName))
 
     # Gathering
     #if config.MPIEnabled == True:
         #config.comm.barrier()
         #gathered_modelsDicts=config.comm.gather(modelsDict, root = 0)
@@ -191,22 +257,58 @@
     if config.rank == 0:
         d=np.zeros([config.origWCS.header['NAXIS2'], config.origWCS.header['NAXIS1']])
         wcs=config.origWCS
         for tileName in modelsDict.keys():
             print("... %s ..." % (tileName))
             minX, maxX, minY, maxY=config.tileCoordsDict[tileName]['clippedSection']
             if modelsDict[tileName] is not None:
-                d[minY:maxY, minX:maxX]=d[minY:maxY, minX:maxX]+modelsDict[tileName]
+                d[minY:maxY, minX:maxX]=d[minY:maxY, minX:maxX]+np.array(modelsDict[tileName])
         # Optionally add CMB
         if args.addCMB == True:
+            # Save tSZ-only map for debugging
+            astImages.saveFITS(args.outputFileName.replace(".fits", "_signalOnly.fits"), d, wcs)
             shape=(d.shape)
-            d=d+maps.simCMBMap(shape, wcs, noiseLevel = args.addWhiteNoise, beamFileName = args.beamFileName, 
+            # Split adding CMB and noise to enable more tests
+            d=d+maps.simCMBMap(shape, wcs, noiseLevel = None, beam = args.beamFileName,
                                seed = args.seed)
+            astImages.saveFITS(args.outputFileName.replace(".fits", "_signalAndCMB.fits"), d, wcs)
+            # Support trimming of inv var map, if we have one that doesn't match area mask
+            # NOTE: As it's noise, we don't actually care about matching RA, dec coords strictly
+            # So we don't worry about +/-1 pixel offsets here
+            # But we do have to deal with RA wrapping, and whether RAMax needs to increase/decrease
+            if type(addNoise) == np.ndarray and shape != addNoise.shape:
+                RAMin, RAMax, decMin, decMax=wcs.getImageMinMaxWCSCoords()
+                clipOk=False
+                count=0
+                lastWidth=None
+                direction=1
+                while clipOk is False:
+                    count=count+1
+                    clip=astImages.clipUsingRADecCoords(addNoise, addNoiseWCS, RAMin, RAMax, decMin, decMax)
+                    if lastWidth is not None:
+                        if lastWidth > clip['data'].shape[1]:
+                            direction=direction*-1
+                    lastWidth=clip['data'].shape[1]
+                    if clip['data'].shape[0] < d.shape[0]:
+                        decMax=decMax+0.01
+                    if clip['data'].shape[1] < d.shape[1]:
+                        RAMax=RAMax+0.01*direction
+                    if clip['data'].shape[0] >= d.shape[0] and clip['data'].shape[1] >= d.shape[1]:
+                        clipOk=True
+                    if count > 20:
+                        raise Exception("Clipping ivar map to suitable size failed to converge quickly enough.")
+                addNoise=clip['data'][:d.shape[0], :d.shape[1]]
+                # raise Exception("Given inv var map does not have the same dimensions as the output sim map - should match the given mask")
+            d=d+maps.simNoiseMap(shape, addNoise, wcs = wcs, lKnee = args.lKnee, noiseMode = noiseMode)
             # For testing abrupt noise changes
             if args.splitNoiseTest == True:
-                d[:int(d.shape[0]/2)]=d[:int(d.shape[0]/2)]+np.random.normal(0, 2*args.addWhiteNoise, [int(d.shape[0]/2), d.shape[1]])
+                d[:int(d.shape[0]/2)]=d[:int(d.shape[0]/2)]+np.random.normal(0, 2*args.addNoise, [int(d.shape[0]/2), d.shape[1]])
                 # Doesn't really matter about absolute scaling of this
-                weights=np.ones(d.shape)*args.addWhiteNoise
+                weights=np.ones(d.shape)*args.addNoise
                 weights[:int(d.shape[0]/2)]=weights[:int(d.shape[0]/2)]*2
                 weights=np.power(weights, -2)
                 astImages.saveFITS(args.outputFileName.replace(".fits", ".ivar.fits"), weights, wcs)
+        # Optionally add another component (e.g., large scale noise, to start with)
+        if args.addMap is not None:
+            with pyfits.open(args.addMap) as img:
+                d=d+float(args.addMapScaling)*img[0].data
         astImages.saveFITS(args.outputFileName, d, wcs)
```

### Comparing `nemo-sz-0.5.0/bin/nemoSpec` & `nemo-sz-0.6.0/bin/nemoSpec`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/docs/Makefile` & `nemo-sz-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/docs/advanced.rst` & `nemo-sz-0.6.0/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/docs/commands.rst` & `nemo-sz-0.6.0/docs/commands.rst`

 * *Files 20% similar despite different names*

```diff
@@ -32,31 +32,14 @@
    :prog: nemoMass
    
    :program:`nemoMass` infers cluster masses based on their SZ signal as measured by
    :program:`nemo`. Cosmological and scaling relation parameters are set in the
    YAML-format configuration file.
 
 
-.. _nemoSelFnCommand:
-   
-nemoSelFn
----------
-   
-.. argparse::
-   :filename: ../bin/nemoSelFn
-   :func: makeParser
-   :prog: nemoSelFn
-
-   :program:`nemoSelFn` calculates mass completeness summary statistics and generates
-   files needed to compute the selection function from the results of a :program:`nemo`
-   cluster detection run. Usually this command is not needed as :program:`nemo` can be
-   set to do this task by setting `calcSelFn: True` in the YAML-format
-   configuration file.
-
-
 .. _nemoMockCommand:
 
 nemoMock
 ---------
    
 .. argparse::
    :filename: ../bin/nemoMock
```

### Comparing `nemo-sz-0.5.0/docs/conf.py` & `nemo-sz-0.6.0/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 autoclass_content = 'both'
 add_module_names = False
 autodoc_mock_imports = ["pyccl", "mpi4py"]
 
 # -- Project information -----------------------------------------------------
 
 project = 'nemo'
-copyright = '2020, Nemo Contributors (Atacama Cosmology Telescope + Simons Observatory)'
+copyright = '2020 - 2023, Nemo Contributors (Atacama Cosmology Telescope + Simons Observatory)'
 author = 'Nemo Contributors (Atacama Cosmology Telescope + Simons Observatory)'
 
 # The short X.Y version
 version = __version__
 # The full version, including alpha/beta/rc tags
 release = __version__
 
@@ -65,15 +65,15 @@
 master_doc = 'index'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `nemo-sz-0.5.0/docs/config.rst` & `nemo-sz-0.6.0/docs/config.rst`

 * *Files 5% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
 RADecSection
 ^^^^^^^^^^^^
 
     If given, cut all maps and masks to include only this rectangular section. This is
     specified as a list in the form ``[RAMin, RAMax, decMin, decMax]``, with all
     coordinates in decimal degrees. This option is useful for testing purposes, but it
-    should not be used for maps that are broken into tiles (see `makeTileDir`_).
+    should not be used for maps that are broken into tiles (see `Tiling`_).
     
     *Example:*
     
     .. code-block:: yaml
 
        RADecSection: [330.0, 355.0, -10.0, 5.0]
 
@@ -187,50 +187,25 @@
 
 
 .. _Tiling:
 
 Tiling
 ======
 
-makeTileDir
-^^^^^^^^^^^
+useTiling:
+^^^^^^^^^^
     
     If True, break the map into tiles according to the settings specified in
-    `tileDefinitions`_. For each map and mask used by :ref:`nemoCommand`,
-    a directory with prefix ``tileDir_`` followed by the map filename will be
-    created (see also `tileDefLabel`_ below). The individual tiles cut 
-    from each map can be found within, in subdirectories labeled according to
-    the tile name. This is done such that on subsequent :ref:`nemoCommand` 
-    runs, each process (if running in parallel under MPI) can read its data
-    from disk without any bottleneck, if using a cluster file system
-    (e.g., `Lustre <https://www.lustre.org/>`_).
-
-    .. note::  If you modify your config file or the map to be tiled, then
-               **Nemo** should detect this and re-make the ``tileDir_*``
-               directories. If you have any doubts, you can always delete
-               the ``tileDir_*`` directories to force them to be re-made
-               from scratch the next time you run :ref:`nemoCommand`.
-
-    *Example:*
-    
-    .. code-block:: yaml
-    
-       makeTileDir: True
-       
+    `tileDefinitions`_.
 
-tileDefLabel
-^^^^^^^^^^^^    
-    This is used to label ``tileDir`` directories, i.e., directories will be
-    created with names in the format ``tileDir_tileDefLabel_<map file name>``.
-    
     *Example:*
     
     .. code-block:: yaml
     
-       tileDefLabel: 'auto'
+       useTiling: True
 
     
 tileDefinitions
 ^^^^^^^^^^^^^^^
     
     This sets how the map is broken into tiles, which is how **Nemo** handles
     parallel processing through MPI (dividing the tiles up as equally as
@@ -1147,14 +1122,29 @@
     *Example:*
     
     .. code-block:: yaml
     
        sourcesPerTile: 50
 
 
+sourceInjectionAmplitudeRange
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+    Sets the minimum and maximum of the range of injected source or
+    cluster model amplitudes. For sources, the amplitudes are specified
+    as ΔT (μK), while for clusters the amplitudes are specified in terms
+    of the central Comptonization parameter, y\ :sub:`0`.
+
+    *Example:*
+
+    .. code-block:: yaml
+
+       sourceInjectionAmplitudeRange: [1, 1000]
+
+
 sourceInjectionModels
 ^^^^^^^^^^^^^^^^^^^^^
     
     For cluster injection tests. This is a list that specifies the shapes
     of clusters to be inserted, with each run inserting cluster signals
     of random amplitude but the same profile.
     The `Arnaud et al. (2010) <https://ui.adsabs.harvard.edu/abs/2010A%26A...517A..92A/abstract>`_
```

### Comparing `nemo-sz-0.5.0/docs/development.rst` & `nemo-sz-0.6.0/docs/development.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/docs/index.rst` & `nemo-sz-0.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/docs/outputs.rst` & `nemo-sz-0.6.0/docs/outputs.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/docs/reference.rst` & `nemo-sz-0.6.0/docs/reference.rst`

 * *Files 7% similar despite different names*

```diff
@@ -42,21 +42,14 @@
 MockSurvey
 ----------
 
 .. automodule:: nemo.MockSurvey
    :members:
 
 
-nemoCython
-----------
-
-.. automodule:: nemoCython
-   :members:
-
-
 photometry
 ----------
 
 .. automodule:: nemo.photometry
    :members:
```

### Comparing `nemo-sz-0.5.0/examples/ACT-DR3-clusters/ACTPol_clusters.fits` & `nemo-sz-0.6.0/examples/ACT-DR3-clusters/ACTPol_clusters.fits`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/ACT-DR3-clusters/ACTPol_redshifts.fits` & `nemo-sz-0.6.0/examples/ACT-DR3-clusters/ACTPol_redshifts.fits`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/ACT-DR3-clusters/E-D56Clusters.fits` & `nemo-sz-0.6.0/examples/ACT-DR3-clusters/E-D56Clusters.fits`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/ACT-DR3-clusters/README.rst` & `nemo-sz-0.6.0/examples/ACT-DR3-clusters/README.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/ACT-DR3-clusters/equD56.yml` & `nemo-sz-0.6.0/examples/ACT-DR3-clusters/equD56.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/ACT-DR3-clusters/equD56_quick.yml` & `nemo-sz-0.6.0/examples/ACT-DR3-clusters/equD56_quick.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/ACT-DR3-clusters/pointSourceMask.fits.gz` & `nemo-sz-0.6.0/examples/ACT-DR3-clusters/pointSourceMask.fits.gz`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/ACT-DR3-clusters/profiles_ACT/profile_AR1_2009_pixwin_130224.txt` & `nemo-sz-0.6.0/examples/ACT-DR3-clusters/profiles_ACT/profile_AR1_2009_pixwin_130224.txt`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/ACT-DR3-clusters/selFnExample.py` & `nemo-sz-0.6.0/examples/SOSims/selFnExample.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 from scipy import interpolate
 from nemo import completeness
 import argparse
 import time
 import IPython
 
 #------------------------------------------------------------------------------------------------------------
-def printNumClusters(H0, Om0, Ob0, sigma_8, n_s, scalingRelationDict = None):
+def printNumClusters(H0, Om0, Ob0, sigma8, ns, scalingRelationDict = None):
     """Example of how to update selection function.
     
     """
     
     # This function has to be called every time a parameter value is changed
-    selFn.update(H0, Om0, Ob0, sigma_8, n_s, scalingRelationDict = scalingRelationDict)
+    selFn.update(H0, Om0, Ob0, sigma8, ns, scalingRelationDict = scalingRelationDict)
     
-    print(">>> H0 = %.2f km/s/Mpc Om0 = %.2f Ob0 = %.2f sigma_8 = %.2f tenToA0 = %.3e sigma_int = %.2f" \
-        % (selFn.mockSurvey.H0, selFn.mockSurvey.Om0, selFn.mockSurvey.Ob0, selFn.mockSurvey.sigma8, 
-           selFn.scalingRelationDict['tenToA0'], selFn.scalingRelationDict['sigma_int']))
+    print(">>> H0 = %.2f km/s/Mpc Om0 = %.2f Ob0 = %.2f sigma8 = %.2f ns = %.3f tenToA0 = %.3e sigma_int = %.2f" \
+        % (selFn.mockSurvey.H0, selFn.mockSurvey.Om0, selFn.mockSurvey.Ob0, selFn.mockSurvey.sigma8,
+           selFn.mockSurvey.ns, selFn.scalingRelationDict['tenToA0'], selFn.scalingRelationDict['sigma_int']))
     numClusters=selFn.mockSurvey.calcNumClustersExpected(compMz = selFn.compMz)
     print("... number of clusters expected = %.2f (in %.2f square degrees) ..." %  (numClusters, selFn.totalAreaDeg2))
     
 #------------------------------------------------------------------------------------------------------------
 if __name__ == '__main__':
 
     parser=argparse.ArgumentParser("selFnExample.py")
@@ -60,38 +60,38 @@
                              footprintLabel = footprintLabel, zStep = zStep)
 
     # If we want to play with scaling relation also
     scalingRelationDict=selFn.scalingRelationDict
     
     # Default parameters    
     t0=time.time()
-    H0, Om0, Ob0, sigma_8, n_s = 70.0, 0.30, 0.05, 0.80, 0.96
-    printNumClusters(H0, Om0, Ob0, sigma_8, n_s, scalingRelationDict = scalingRelationDict)
+    H0, Om0, Ob0, sigma8, ns = 70.0, 0.30, 0.05, 0.80, 0.95   
+    printNumClusters(H0, Om0, Ob0, sigma8, ns, scalingRelationDict = scalingRelationDict)
     t1=time.time()
     print("... iteration took %.3f sec ..." % (t1-t0))
     completeness.makeMzCompletenessPlot(selFn.compMz, selFn.mockSurvey.log10M, selFn.mockSurvey.z, "test0", "test0_Mz.pdf")
     
     # A complete iteration of changing cosmological parameters    
     t0=time.time()
-    H0, Om0, Ob0, sigma_8, n_s = 72.0, 0.27, 0.05, 0.74, 1.00
-    printNumClusters(H0, Om0, Ob0, sigma_8, n_s, scalingRelationDict = scalingRelationDict)
+    H0, Om0, Ob0, sigma8, ns = 72.0, 0.27, 0.05, 0.74, 0.95
+    printNumClusters(H0, Om0, Ob0, sigma8, ns, scalingRelationDict = scalingRelationDict)
     t1=time.time()
     print("... iteration took %.3f sec ..." % (t1-t0))
     completeness.makeMzCompletenessPlot(selFn.compMz, selFn.mockSurvey.log10M, selFn.mockSurvey.z, "test1", "test1_Mz.pdf")
     
     # Changing the scaling relation normalisation
     t0=time.time()
     scalingRelationDict['tenToA0']=3e-5
-    printNumClusters(H0, Om0, Ob0, sigma_8, n_s, scalingRelationDict = scalingRelationDict)
+    printNumClusters(H0, Om0, Ob0, sigma8, ns, scalingRelationDict = scalingRelationDict)
     t1=time.time()
     print("... iteration took %.3f sec ..." % (t1-t0))
     completeness.makeMzCompletenessPlot(selFn.compMz, selFn.mockSurvey.log10M, selFn.mockSurvey.z, "test2", "test2_Mz.pdf")
 
     # Changing the scaling relation intrinsic scatter
     t0=time.time()
     scalingRelationDict['tenToA0']=4.95e-5
     scalingRelationDict['sigma_int']=0.001
-    printNumClusters(H0, Om0, Ob0, sigma_8, n_s, scalingRelationDict = scalingRelationDict)
+    printNumClusters(H0, Om0, Ob0, sigma8, ns, scalingRelationDict = scalingRelationDict)
     t1=time.time()
     print("... iteration took %.3f sec ..." % (t1-t0))
     completeness.makeMzCompletenessPlot(selFn.compMz, selFn.mockSurvey.log10M, selFn.mockSurvey.z, "test3", "test3_Mz.pdf")
```

### Comparing `nemo-sz-0.5.0/examples/ACT-DR3-clusters/surveyMask.fits.gz` & `nemo-sz-0.6.0/examples/ACT-DR3-clusters/surveyMask.fits.gz`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/ACT-DR5-clusters/DR5ClusterSearch.yml` & `nemo-sz-0.6.0/examples/ACT-DR5-clusters/DR5ClusterSearch.yml`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 useInterpolator: True
 rejectBorder: 0
 objIdent: 'ACT-CL'
 longNames: False
 
 # Photometry options
 photFilter: 'Arnaud_M2e14_z0p4' # Defines the reference filter for cluster selection / mass estimates
+fitQ: True
 
 # Optionally override the GNFW parameters - if not present, Arnaud et al. (2010) parameters are used
 # The example below is for the Planck Pressure Profile (PPP)
 #GNFWParams: {P0: 6.41, c500: 1.81, gamma: 0.31, alpha: 1.33, beta: 4.13, tol: 1e-7, npts: 100}
 
 # Mass measurement options - used by nemoMass
 # redshiftCatalog:  A .fits table containing name, RADeg, decDeg, redshift, redshiftErr columns
@@ -54,25 +55,27 @@
               redshiftCatalog: "redshifts_confirmed_v1.1.fits"}
 
 # Selection function options - this calculation can also be enabled with the nemo -S switch
 # NOTE: could eventually add 'completenessFraction' to 'massLimitMaps', which is why that's a dictionary list
 # Use selFnFootprints to calculate average completeness in given sky areas - e.g., overlap with optical surveys
 calcSelFn: True
 selFnOptions: {fixedSNRCut: 5.0,
-               method: 'montecarlo',
+               method: 'fast',
                numIterations: 1000, 
                massLimitMaps: [{z: 0.5}]}
                
-#selFnFootprints: 
+# selFnFootprints: 
 #    - {label: "HSC",
 #       maskList: ["HSCCheckAndSelFn/s19a_fdfc_CAR_contarea_ziy-gt-5.fits"]}
 #    - {label: "KiDS",
 #       maskList: ["KiDSSelFn/mask_KiDSN.fits", "KiDSSelFn/mask_KiDSS.fits"]}
 #    - {label: "DES",
 #       maskList: ["DESY3/AdvACT_y3a2_footprint_griz_1exp_v2.0.fits"]}
+#    - {label: "DECaLS",
+#       maskList: ["DECaLS_DR8_mask.fits"]}
 
 # Filter definitions:
 # allFilters is a dictionary of parameters that will be copied into all mapFilters
 # (these can be overridden by keys with the same name in mapFilters)
 allFilters: {class: "ArnaudModelMatchedFilter",
              params: {noiseParams: {method: "dataMap",
                                     noiseGridArcmin: 40.},
@@ -119,29 +122,27 @@
        params: {M500MSun: 2.0e+14, z: 1.2}}
     - {label: "Arnaud_M4e14_z1p2",
        params: {M500MSun: 4.0e+14, z: 1.2}}
     - {label: "Arnaud_M8e14_z1p2",
        params: {M500MSun: 8.0e+14, z: 1.2}}
 
 # Source injection test - this can also be enabled with the nemo -I switch
-#sourceInjectionTest: False
-sourceInjectionIterations: 200
+sourceInjectionIterations: 9
 sourcesPerTile: 50
 sourceInjectionModels:
     - {redshift: 0.8, M500: 2.0e+14}
     - {redshift: 0.4, M500: 2.0e+14}
     - {redshift: 0.2, M500: 2.0e+14}
     - {redshift: 0.1, M500: 2.0e+14}
 
-# tileDir options - cut-up each map into smaller sections
-makeTileDir: True
+# Tiling options - cut-up each map into smaller sections
+useTiling: True
 makeQuickLookMaps: False
 stitchTiles: True
 tileOverlapDeg: 1.0
-tileDefLabel: 'auto'
 tileDefinitions: {mask: 'dr5_masking/AdvACTSurveyMask_v7_S18.fits',
                   targetTileWidthDeg: 10.0, 
                   targetTileHeightDeg: 5.0}
 
 # If this is given, only the named tiles will be processed (useful for testing)
 #tileNameList:
     #- '1_10_7'
```

### Comparing `nemo-sz-0.5.0/examples/ACT-DR5-clusters/FETCH_MAPS.sh` & `nemo-sz-0.6.0/examples/ACT-DR5-clusters/FETCH_MAPS.sh`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/ACT-DR5-clusters/README.rst` & `nemo-sz-0.6.0/examples/ACT-DR5-clusters/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Here we provide a guide to reproducing the 
 `ACT DR5 cluster catalog <https://ui.adsabs.harvard.edu/abs/2020arXiv200911043H/abstract>`_.
 
 .. note::  The config files and scripts needed for this tutorial can be
            found in the `examples/ACT-DR5-clusters <https://github.com/simonsobs/nemo/tree/main/examples/ACT-DR5-clusters>`_
            directory of the **Nemo** source distribution.
 
+.. note::  The `released ACT DR5 cluster catalog v1.1 <https://lambda.gsfc.nasa.gov/product/act/actpol_dr5_szcluster_catalog_get.html>`_
+           was produced with code that is closest (but not identical) to
+           `Nemo v0.5.0 <https://github.com/simonsobs/nemo/releases/tag/v0.5.0>`_.
+           Later versions of **Nemo** may produce slightly different output as the
+           code is improved and bugs are fixed.
+
 
 Downloading maps and other needed files
 =======================================
 
 The first step is to download the ACT DR5 maps, described in 
 `Naess et al. (2020) <https://ui.adsabs.harvard.edu/abs/2020JCAP...12..046N/abstract>`_,
 from `LAMBDA <https://lambda.gsfc.nasa.gov/product/act/actpol_prod_table.cfm>`_. In
```

### Comparing `nemo-sz-0.5.0/examples/SOSims/HEALPIX_TO_CAR.sh` & `nemo-sz-0.6.0/examples/SOSims/HEALPIX_TO_CAR.sh`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/MFMF_SOSim_3freq_small.yml` & `nemo-sz-0.6.0/examples/SOSims/MFMF_SOSim_3freq_small.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/MFMF_SOSim_3freq_tiles.yml` & `nemo-sz-0.6.0/examples/SOSims/MFMF_SOSim_3freq_tiles.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/NzCheck.py` & `nemo-sz-0.6.0/examples/SOSims/NzCheck.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/README.rst` & `nemo-sz-0.6.0/examples/SOSims/README.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/cobayaConf_SOSims_fixedScalingRelation.yml` & `nemo-sz-0.6.0/examples/SOSims/cobayaConf_SOSims_fixedScalingRelation.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/combineComponentMaps.py` & `nemo-sz-0.6.0/examples/SOSims/combineComponentMaps.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/createSurveyMask.py` & `nemo-sz-0.6.0/examples/SOSims/createSurveyMask.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/healpix2CAR.py` & `nemo-sz-0.6.0/examples/SOSims/healpix2CAR.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/makeGaussianBeam.py` & `nemo-sz-0.6.0/examples/SOSims/makeGaussianBeam.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/makeRedshiftsCatalog.py` & `nemo-sz-0.6.0/examples/SOSims/makeRedshiftsCatalog.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/readWebSkyInputCatalog.py` & `nemo-sz-0.6.0/examples/SOSims/readWebSkyInputCatalog.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/selFnExample.py` & `nemo-sz-0.6.0/examples/ACT-DR3-clusters/selFnExample.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 from scipy import interpolate
 from nemo import completeness
 import argparse
 import time
 import IPython
 
 #------------------------------------------------------------------------------------------------------------
-def printNumClusters(H0, Om0, Ob0, sigma8, ns, scalingRelationDict = None):
+def printNumClusters(H0, Om0, Ob0, sigma_8, n_s, scalingRelationDict = None):
     """Example of how to update selection function.
     
     """
     
     # This function has to be called every time a parameter value is changed
-    selFn.update(H0, Om0, Ob0, sigma8, ns, scalingRelationDict = scalingRelationDict)
+    selFn.update(H0, Om0, Ob0, sigma_8, n_s, scalingRelationDict = scalingRelationDict)
     
-    print(">>> H0 = %.2f km/s/Mpc Om0 = %.2f Ob0 = %.2f sigma8 = %.2f ns = %.3f tenToA0 = %.3e sigma_int = %.2f" \
-        % (selFn.mockSurvey.H0, selFn.mockSurvey.Om0, selFn.mockSurvey.Ob0, selFn.mockSurvey.sigma8,
-           selFn.mockSurvey.ns, selFn.scalingRelationDict['tenToA0'], selFn.scalingRelationDict['sigma_int']))
+    print(">>> H0 = %.2f km/s/Mpc Om0 = %.2f Ob0 = %.2f sigma_8 = %.2f tenToA0 = %.3e sigma_int = %.2f" \
+        % (selFn.mockSurvey.H0, selFn.mockSurvey.Om0, selFn.mockSurvey.Ob0, selFn.mockSurvey.sigma8, 
+           selFn.scalingRelationDict['tenToA0'], selFn.scalingRelationDict['sigma_int']))
     numClusters=selFn.mockSurvey.calcNumClustersExpected(compMz = selFn.compMz)
     print("... number of clusters expected = %.2f (in %.2f square degrees) ..." %  (numClusters, selFn.totalAreaDeg2))
     
 #------------------------------------------------------------------------------------------------------------
 if __name__ == '__main__':
 
     parser=argparse.ArgumentParser("selFnExample.py")
@@ -42,56 +42,57 @@
                         this is not given, the config.yml file in selFnDir will be used.""",
                         default = None)
     parser.add_argument("-f", "--footprint", dest = "footprint", help="""Footprint to use, e.g., DES,
                         HSC, KiDS (default: full).""", default = None)
     parser.add_argument("-S", "--SNR-cut", dest = "SNRCut", help="""Use only clusters with fixed_SNR > 
                         this value.""", default = 5.0, type = float)
     parser.add_argument("-z", "--z-step", dest = "zStep", help="""Redshift bin width (default: 0.1).""", 
-                        default = 0.1, type = float)
+                        default = 0.02, type = float)
     args = parser.parse_args()
     
     configFileName=args.configFileName
     selFnDir=args.selFnDir
     SNRCut=args.SNRCut
     zStep=args.zStep
     footprintLabel=args.footprint
     
     print(">>> Setting up SNR > %.2f selection function ..." % (SNRCut))
     selFn=completeness.SelFn(selFnDir, SNRCut, configFileName = configFileName, 
-                             footprintLabel = footprintLabel, zStep = zStep)
+                             footprint = footprintLabel, zStep = zStep)
+    massLabel="M%d%s" % (selFn.mockSurvey.delta, selFn.mockSurvey.rhoType[0])
 
     # If we want to play with scaling relation also
     scalingRelationDict=selFn.scalingRelationDict
     
     # Default parameters    
     t0=time.time()
-    H0, Om0, Ob0, sigma8, ns = 70.0, 0.30, 0.05, 0.80, 0.95   
-    printNumClusters(H0, Om0, Ob0, sigma8, ns, scalingRelationDict = scalingRelationDict)
+    H0, Om0, Ob0, sigma_8, n_s = 70.0, 0.30, 0.05, 0.80, 0.96
+    printNumClusters(H0, Om0, Ob0, sigma_8, n_s, scalingRelationDict = scalingRelationDict)
     t1=time.time()
     print("... iteration took %.3f sec ..." % (t1-t0))
-    completeness.makeMzCompletenessPlot(selFn.compMz, selFn.mockSurvey.log10M, selFn.mockSurvey.z, "test0", "test0_Mz.pdf")
+    completeness.makeMzCompletenessPlot(selFn.compMz, selFn.mockSurvey.log10M, selFn.mockSurvey.z, "test0", massLabel, "test0_Mz.pdf")
     
     # A complete iteration of changing cosmological parameters    
     t0=time.time()
-    H0, Om0, Ob0, sigma8, ns = 72.0, 0.27, 0.05, 0.74, 0.95
-    printNumClusters(H0, Om0, Ob0, sigma8, ns, scalingRelationDict = scalingRelationDict)
+    H0, Om0, Ob0, sigma_8, n_s = 72.0, 0.27, 0.05, 0.74, 1.00
+    printNumClusters(H0, Om0, Ob0, sigma_8, n_s, scalingRelationDict = scalingRelationDict)
     t1=time.time()
     print("... iteration took %.3f sec ..." % (t1-t0))
-    completeness.makeMzCompletenessPlot(selFn.compMz, selFn.mockSurvey.log10M, selFn.mockSurvey.z, "test1", "test1_Mz.pdf")
+    completeness.makeMzCompletenessPlot(selFn.compMz, selFn.mockSurvey.log10M, selFn.mockSurvey.z, "test1", massLabel, "test1_Mz.pdf")
     
     # Changing the scaling relation normalisation
     t0=time.time()
     scalingRelationDict['tenToA0']=3e-5
-    printNumClusters(H0, Om0, Ob0, sigma8, ns, scalingRelationDict = scalingRelationDict)
+    printNumClusters(H0, Om0, Ob0, sigma_8, n_s, scalingRelationDict = scalingRelationDict)
     t1=time.time()
     print("... iteration took %.3f sec ..." % (t1-t0))
-    completeness.makeMzCompletenessPlot(selFn.compMz, selFn.mockSurvey.log10M, selFn.mockSurvey.z, "test2", "test2_Mz.pdf")
+    completeness.makeMzCompletenessPlot(selFn.compMz, selFn.mockSurvey.log10M, selFn.mockSurvey.z, "test2", massLabel, "test2_Mz.pdf")
 
     # Changing the scaling relation intrinsic scatter
     t0=time.time()
     scalingRelationDict['tenToA0']=4.95e-5
     scalingRelationDict['sigma_int']=0.001
-    printNumClusters(H0, Om0, Ob0, sigma8, ns, scalingRelationDict = scalingRelationDict)
+    printNumClusters(H0, Om0, Ob0, sigma_8, n_s, scalingRelationDict = scalingRelationDict)
     t1=time.time()
     print("... iteration took %.3f sec ..." % (t1-t0))
-    completeness.makeMzCompletenessPlot(selFn.compMz, selFn.mockSurvey.log10M, selFn.mockSurvey.z, "test3", "test3_Mz.pdf")
+    completeness.makeMzCompletenessPlot(selFn.compMz, selFn.mockSurvey.log10M, selFn.mockSurvey.z, "test3", massLabel, "test3_Mz.pdf")
```

### Comparing `nemo-sz-0.5.0/examples/SOSims/surveyMask.reg` & `nemo-sz-0.6.0/examples/SOSims/surveyMask.reg`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/template_AdvACT.txt` & `nemo-sz-0.6.0/examples/SOSims/template_AdvACT.txt`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/template_E-D56.txt` & `nemo-sz-0.6.0/examples/SOSims/template_E-D56.txt`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/template_small.txt` & `nemo-sz-0.6.0/examples/SOSims/template_small.txt`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/validationScripts/README.md` & `nemo-sz-0.6.0/examples/SOSims/validationScripts/README.md`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/validationScripts/checkMassRecovery.py` & `nemo-sz-0.6.0/examples/SOSims/validationScripts/checkMassRecovery.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/validationScripts/checkMassRecovery_M200m.py` & `nemo-sz-0.6.0/examples/SOSims/validationScripts/checkMassRecovery_M200m.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/validationScripts/makeMassFunctionPlotsCCL.py` & `nemo-sz-0.6.0/examples/SOSims/validationScripts/makeMassFunctionPlotsCCL.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/SOSims/validationScripts/makeMassFunctionPlotsCCL_recovered.py` & `nemo-sz-0.6.0/examples/SOSims/validationScripts/makeMassFunctionPlotsCCL_recovered.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/TILe-C/README.md` & `nemo-sz-0.6.0/examples/TILe-C/README.md`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/TILe-C/y_f090beam.yml` & `nemo-sz-0.6.0/examples/TILe-C/y_f090beam.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/clustercal/clustercal.py` & `nemo-sz-0.6.0/examples/clustercal/clustercal.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/clustercal/makeConfigs.py` & `nemo-sz-0.6.0/examples/clustercal/makeConfigs.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/clustercal/template_singlefreq.yml` & `nemo-sz-0.6.0/examples/clustercal/template_singlefreq.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/quickstart/README.rst` & `nemo-sz-0.6.0/examples/quickstart/README.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/quickstart/quickstart-clusters.yml` & `nemo-sz-0.6.0/examples/quickstart/quickstart-clusters.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/quickstart/quickstart-sources.yml` & `nemo-sz-0.6.0/examples/quickstart/quickstart-sources.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/sources/PSExample_E-D56.yml` & `nemo-sz-0.6.0/examples/sources/PSExample_E-D56.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/sources/PSExample_deep56_s15_f090.yml` & `nemo-sz-0.6.0/examples/sources/PSExample_deep56_s15_f090.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/sources/PSExample_deep8.yml` & `nemo-sz-0.6.0/examples/sources/PSExample_deep8.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/sources/PS_S16_f090_nightOnly.yml` & `nemo-sz-0.6.0/examples/sources/PS_S16_f090_nightOnly.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/sources/PS_S16_nightOnly.yml` & `nemo-sz-0.6.0/examples/sources/PS_S16_nightOnly.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/sources/PS_S18d_f090_202006_2pass.yml` & `nemo-sz-0.6.0/examples/sources/PS_S18d_f090_202006_2pass.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/sources/PS_S18d_f150_202006_2pass.yml` & `nemo-sz-0.6.0/examples/sources/PS_S18d_f150_202006_2pass.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/sources/PS_S18d_f220_202006.yml` & `nemo-sz-0.6.0/examples/sources/PS_S18d_f220_202006.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/sources/PS_S18d_f220_202006_2pass.yml` & `nemo-sz-0.6.0/examples/sources/PS_S18d_f220_202006_2pass.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/sources/PS_f150_act+planck_day+night.yml` & `nemo-sz-0.6.0/examples/sources/PS_f150_act+planck_day+night.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/examples/sources/PS_f220_nightOnly.yml` & `nemo-sz-0.6.0/examples/sources/PS_f220_nightOnly.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/nemo/MockSurvey.py` & `nemo-sz-0.6.0/nemo/MockSurvey.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import subprocess
 from astropy.cosmology import FlatLambdaCDM
 on_rtd=os.environ.get('READTHEDOCS', None)
 if on_rtd is None:
     import pyccl as ccl
 from . import signals
 from . import catalogs
+from . import maps
 import pickle
 from scipy import interpolate
 from scipy import integrate
 from scipy.interpolate import InterpolatedUnivariateSpline as _spline
 from scipy import stats
 from astLib import *
 import time
@@ -58,15 +59,15 @@
             limit.
         numClustersByRedshift (:obj:`np.ndarray`): Number of clusters in the survey area above the
             minimum mass limit, as a function of redshift.
     
     """
     def __init__(self, minMass, areaDeg2, zMin, zMax, H0, Om0, Ob0, sigma8, ns, zStep = 0.01, 
                  enableDrawSample = False, delta = 500, rhoType = 'critical', 
-                 transferFunction = 'boltzmann_camb'):
+                 transferFunction = 'boltzmann_camb', massFunction = 'Tinker08'):
         """Create a MockSurvey object, for performing calculations of cluster counts or generating mock
         catalogs. The Tinker et al. (2008) halo mass function is used (hardcoded at present, but in 
         principle this can easily be swapped for any halo mass function supported by CCL).
         
         Args:
             minMass (:obj:`float`): The minimum mass, in MSun. This should be set considerably lower than
                 the actual survey completeness limit, otherwise completeness calculations will be wrong.
@@ -82,76 +83,100 @@
             zStep (:obj:`float`, optional): Sets the linear spacing between redshift bins.
             enableDrawSample (:obj:`bool`, optional): This needs to be set to True to enable use of the
                 :func:`self.drawSample` function. Setting this to False avoids some overhead.
             delta (:obj:``float`): Overdensity parameter, used for mass definition (e.g., 200, 500).
             rhoType (:obj:`str`): Density definition, either 'matter' or 'critical', used for mass definition.
             transferFunction (:obj:`str`): Transfer function to use, as understood by CCL (e.g., 'eisenstein_hu', 
                 'boltzmann_camb').
+            massFunction (:obj:`str`): Name of the mass function to use, currently either 'Tinker08' or
+                'Tinker10'. Mass function calculations are done by CCL.
                 
         """
         
         if areaDeg2 == 0:
             raise Exception("Cannot create a MockSurvey object with zero area")
+        self.areaDeg2=areaDeg2
+        self.areaSr=np.radians(np.sqrt(areaDeg2))**2
 
         zRange=np.arange(zMin, zMax+zStep, zStep)
-        areaSr=np.radians(np.sqrt(areaDeg2))**2
-        self.areaSr=areaSr
-        self.areaDeg2=areaDeg2
         self.zBinEdges=zRange
         self.z=(zRange[:-1]+zRange[1:])/2.
         self.a=1./(1+self.z)
         
         self.delta=delta
         self.rhoType=rhoType
         if self.delta == 200:
             c_m_relation='Bhattacharya13'
         else:
             c_m_relation=None
         self.mdef=ccl.halos.MassDef(self.delta, self.rhoType, c_m_relation = c_m_relation)
         self.transferFunction=transferFunction
+        self.massFuncName=massFunction
         
         # Just for convenience when used elsewhere
         self.mdefLabel="M%d%s" % (self.delta, self.rhoType[0])
         
         self.H0=-1
         self.Om0=-1
         self.Ob0=-1
         self.sigma8=-1
         self.ns=-1
         self._get_new_cosmo(H0, Om0, Ob0, sigma8, ns)
 
         # NOTE: These are just MSun now (NOT MSun/h); always defined according to mdef
-        self.log10M=np.arange(13, 16, 0.01)
+        self.log10M=np.arange(np.log10(minMass), 16, 0.01)
         self.M=np.power(10, self.log10M)
         self.log10MBinEdges=np.linspace(self.log10M.min()-(self.log10M[1]-self.log10M[0])/2, 
                                         self.log10M.max()+(self.log10M[1]-self.log10M[0])/2, len(self.log10M)+1)  
 
         # Below is needed for Q calc when not using M500c definition (for now at least)
         self._M500cDef=ccl.halos.MassDef(500, "critical")
 
         self.enableDrawSample=enableDrawSample
         self.update(H0, Om0, Ob0, sigma8, ns)
 
 
+    def setSurveyArea(self, areaDeg2):
+        """Change the area of the survey to a user-specified value, updating the cluster
+        counts accordingly.
+
+        Args:
+            areaDeg2 (:obj:`float`): Area of the survey in square degrees.
+
+        """
+
+        if areaDeg2 == 0:
+            raise Exception("Cannot create a MockSurvey object with zero area")
+        areaSr=np.radians(np.sqrt(areaDeg2))**2
+        if areaDeg2 != self.areaDeg2:
+            self.areaSr=areaSr
+            self.areaDeg2=areaDeg2
+            self._doClusterCount()
+
+
     def _get_new_cosmo(self, H0, Om0, Ob0, sigma8, ns):
         if ((self.H0 != H0) or (self.Om0 != Om0) or
             (self.Ob0 != Ob0) or (self.sigma8 != sigma8)):
             self.H0=H0
             self.Om0=Om0
             self.Ob0=Ob0
             self.sigma8=sigma8
             self.ns=ns
             self.cosmoModel = ccl.Cosmology(Omega_c=Om0-Ob0,
                                             Omega_b=Ob0,
                                             h=0.01*H0,
                                             sigma8=sigma8,
                                             n_s=ns,
                                             transfer_function=self.transferFunction)
-            self.mfunc = ccl.halos.MassFuncTinker08(self.cosmoModel,
-                                                    self.mdef)
+            if self.massFuncName == 'Tinker10':
+                self.mfunc=ccl.halos.MassFuncTinker10(self.cosmoModel,
+                                                      self.mdef)
+            elif self.massFuncName == 'Tinker08':
+                self.mfunc=ccl.halos.MassFuncTinker08(self.cosmoModel,
+                                                      self.mdef)
 
             
     def update(self, H0, Om0, Ob0, sigma8, ns):
         """Recalculate cluster counts for the updated cosmological parameters given.
         
         Args:
             H0 (:obj:`float`): The Hubble constant at redshift 0, in km/s/Mpc.
@@ -172,22 +197,23 @@
         self.Ez=ccl.h_over_h0(self.cosmoModel,self.a)
         self.Ez2=np.power(self.Ez, 2)
         self.DAz=ccl.angular_diameter_distance(self.cosmoModel,self.a)
         self.criticalDensity=ccl.physical_constants.RHO_CRITICAL*(self.Ez*self.cosmoModel['h'])**2
         for k in range(len(self.z)):
             # NOTE: Q fit uses theta500, as does fRel (hardcoded M500 - T relation in there)
             # This bit here may not be strictly necessary, since we don't need to map on to binning
-            if self.delta != 500 or self.rhoType != "critical":
+            if self.delta == 500 and self.rhoType == "critical":
+                interpLim_minLog10M500c=self.log10M.min()
+                interpLim_maxLog10M500c=self.log10M.max()
+            else:
                 interpLim_minLog10M500c=np.log10(self.mdef.translate_mass(self.cosmoModel, self.M.min(), 
                                                                           self.a[k], self._M500cDef))
                 interpLim_maxLog10M500c=np.log10(self.mdef.translate_mass(self.cosmoModel, self.M.max(), 
                                                                           self.a[k], self._M500cDef))
-            else:
-                interpLim_minLog10M500c=self.log10M.min()
-                interpLim_maxLog10M500c=self.log10M.max()
+
             zk=self.z[k]
             interpPoints=100
             fitM500s=np.power(10, np.linspace(interpLim_minLog10M500c, interpLim_maxLog10M500c, interpPoints))
             fitTheta500s=np.zeros(len(fitM500s))
             fitFRels=np.zeros(len(fitM500s))
             criticalDensity=self.criticalDensity[k]
             DA=self.DAz[k]
@@ -214,14 +240,15 @@
             # And we may as well have E(z), DA on the z grid also
             self.log10MRollers=[]
             for i in range(len(self.z)):
                 ngtm=self._cumulativeNumberDensity(self.z[i])
                 mask=ngtm > 0
                 self.log10MRollers.append(_spline((ngtm[mask] / ngtm[0])[::-1], np.log10(self.M[mask][::-1]), k=3))
     
+
     def _cumulativeNumberDensity(self, z):
         """Returns N > M (per cubic Mpc).
         
         """
 
         h=self.cosmoModel['h']
         dndlnM=self.mfunc.get_mass_function(self.cosmoModel,
@@ -246,14 +273,16 @@
 
         
     def _doClusterCount(self):
         """Updates cluster count etc. after mass function object is updated.
         
         """
 
+        assert(self.areaSr == np.radians(np.sqrt(self.areaDeg2))**2)
+
         zRange=self.zBinEdges
         h = self.cosmoModel['h']
         self.M=np.power(10, self.log10M) # in M_sun
         norm_mfunc=1. / np.log(10)
 
         # Number density by z and total cluster count (in redshift shells)
         # Can use to make P(m, z) plane
@@ -325,33 +354,34 @@
         """
         numberDensity=self._cumulativeNumberDensity(z)
         PLog10M=numberDensity/np.trapz(numberDensity, self.M)
 
         return PLog10M
 
 
-    def drawSample(self, y0Noise, scalingRelationDict, QFit, wcs = None, photFilterLabel = None, 
-                   tileName = None, SNRLimit = None, makeNames = False, z = None, numDraws = None,
-                   areaDeg2 = None, applySNRCut = False, applyPoissonScatter = True, 
-                   applyIntrinsicScatter = True, applyNoiseScatter = True):
+    def drawSample(self, y0Noise, scalingRelationDict, QFit = None, wcs = None, photFilterLabel = None,\
+                   tileName = None, SNRLimit = None, makeNames = False, z = None, numDraws = None,\
+                   areaDeg2 = None, applySNRCut = False, applyPoissonScatter = True,\
+                   applyIntrinsicScatter = True, applyNoiseScatter = True,\
+                   applyRelativisticCorrection = True, verbose = False):
         """Draw a cluster sample from the mass function, generating mock y0~ values (called `fixed_y_c` in
         Nemo catalogs) by applying the given scaling relation parameters, and then (optionally) applying
         a survey selection function.
         
         Args:
             y0Noise (:obj:`float` or :obj:`np.ndarray`): Either a single number (if using e.g., a survey
-                average) or a noise map (2d array). A noise map must be provided here if you want the
-                output catalog to contain RA, dec coordinates (in addition, a WCS object must also be
-                provided - see below).
+                average), an RMS table (with columns 'areaDeg2' and 'y0RMS'), or a noise map (2d array).
+                A noise map must be provided here if you want the output catalog to contain RA, dec
+                coordinates (in addition, a WCS object must also be provided - see below).
             scalingRelationDict (:obj:`dict`): A dictionary containing keys 'tenToA0', 'B0', 'Mpivot',
                 'sigma_int' that describes the scaling relation between y0~ and mass (this is the
                 format of `massOptions` in Nemo .yml config files).
-            tckQFitDict (:obj:`dict`): A dictionary of interpolation spline knots indexed by tileName,
-                that can be used to estimate Q, the filter mismatch function (see 
-                :func:`nemo.signals.loadQ`).
+            QFit (:obj:`nemo.signals.QFit`, optional): Object that handles the filter mismatch
+                function, *Q*. If not given, the output catalog will not contain `fixed_y_c` columns,
+                only `true_y_c` columns.
             wcs (:obj:`astWCS.WCS`, optional): WCS object corresponding to `y0Noise`, if `y0Noise` is
                 as noise map (2d image array). Needed if you want the output catalog to contain RA, dec
                 coordinates.
             photFilterLabel (:obj:`str`, optional): Name of the reference filter (as defined in the
                 Nemo .yml config file) that is used to define y0~ (`fixed_y_c`) and the filter mismatch 
                 function, Q.
             tileName (:obj:`str`, optional): Name of the tile for which the sample will be generated.
@@ -374,14 +404,16 @@
                 counts (implemented by modifiying the number of draws from the mass function).
             applyIntrinsicScatter (:obj:`bool`, optional): If True, apply intrinsic scatter to the
                 SZ measurements (`fixed_y_c`), as set by the `sigma_int` parameter in 
                 `scalingRelationDict`.
             applyNoiseScatter (:obj:`bool`, optional): If True, apply measurement noise, generated
                 from the given noise level or noise map (`y0Noise`), to the output SZ measurements
                 (`fixed_y_c`).
+            applyRelativisticCorrection (:obj:`bool`, optional): If True, apply the relativistic
+                correction.
                 
         Returns:
             A catalog as an :obj:`astropy.table.Table` object, in the same format as produced by
             the main `nemo` script.
         
         Notes:
             If both `applyIntrinsicScatter`, `applyNoiseScatter` are set to False, then the output
@@ -415,30 +447,59 @@
         numClusters=numClustersByRedshift.sum()
             
         if numDraws is not None:
             numClusters=numDraws            
 
         tenToA0, B0, Mpivot, sigma_int=[scalingRelationDict['tenToA0'], scalingRelationDict['B0'], 
                                         scalingRelationDict['Mpivot'], scalingRelationDict['sigma_int']]
-                    
+
         # If given y0Noise as RMSMap, draw coords (assuming clusters aren't clustered - which they are...)
         # NOTE: switched to using valid part of RMSMap here rather than areaMask - we need to fix the latter to same area
         # It isn't a significant issue though
         if type(y0Noise) == np.ndarray and y0Noise.ndim == 2:
+            # This generates even density RA, dec coords on the whole sky taking into account the projection
+            # Consequently, this is inefficient if fed individual tiles rather than a full sky noise map
+            assert(wcs is not None)
             RMSMap=y0Noise
-            ysInMask, xsInMask=np.where(RMSMap != 0)
-            coordIndices=np.random.randint(0, len(xsInMask), numClusters)
-            ys=ysInMask[coordIndices]
-            xs=xsInMask[coordIndices]
-            if wcs is not None:
-                RADecCoords=wcs.pix2wcs(xs, ys)
-                RADecCoords=np.array(RADecCoords)
-                RAs=RADecCoords[:, 0]
-                decs=RADecCoords[:, 1]
+            xsList=[]
+            ysList=[]
+            maxCount=10000
+            count=0
+            while(len(xsList) < numClusters):
+                count=count+1
+                if count > maxCount:
+                    raise Exception("Failed to generate enough random coords in %d iterations" % (maxCount))
+                theta=np.degrees(np.pi*2*np.random.uniform(0, 1, numClusters))
+                phi=np.degrees(np.arccos(2*np.random.uniform(0, 1, numClusters)-1))-90
+                xyCoords=np.array(wcs.wcs2pix(theta, phi))
+                xs=np.array(np.round(xyCoords[:, 0]), dtype = int)
+                ys=np.array(np.round(xyCoords[:, 1]), dtype = int)
+                mask=np.logical_and(np.logical_and(xs >= 0, xs < RMSMap.shape[1]), np.logical_and(ys >= 0, ys < RMSMap.shape[0]))
+                xs=xs[mask]
+                ys=ys[mask]
+                mask=RMSMap[ys, xs] > 0
+                xsList=xsList+xs[mask].tolist()
+                ysList=ysList+ys[mask].tolist()
+            xs=np.array(xsList)[:numClusters]
+            ys=np.array(ysList)[:numClusters]
+            del xsList, ysList
+            RADecCoords=wcs.pix2wcs(xs, ys)
+            RADecCoords=np.array(RADecCoords)
+            RAs=RADecCoords[:, 0]
+            decs=RADecCoords[:, 1]
             y0Noise=RMSMap[ys, xs]
+        elif type(y0Noise) == atpy.Table:
+            noisetck=interpolate.splrep(np.cumsum(y0Noise['areaDeg2']/y0Noise['areaDeg2'].sum()), y0Noise['y0RMS'], k = 1)
+            rnd=np.random.uniform(0, 1, numClusters)
+            vals=interpolate.splev(rnd, noisetck, ext = 3)
+            if np.any(vals < 0) or np.any(vals == np.nan):
+                raise Exception("Failed to make interpolating spline for RMSTab in tileName = %s" % (tileName))
+            y0Noise=vals
+            RAs=np.zeros(numClusters)
+            decs=np.zeros(numClusters)
         else:
             y0Noise=np.ones(numClusters)*y0Noise
             RAs=np.zeros(numClusters)
             decs=np.zeros(numClusters)
         
         # Fancy names or not?
         if makeNames == True:
@@ -448,21 +509,26 @@
         else:
             names=np.arange(numClusters)+1
                 
         # New way - on the redshift grid
         t0=time.time()
         currentIndex=0
         log10Ms=np.random.random_sample(y0Noise.shape) # These will be converted from random numbers to masses below
-        log10M500c=np.zeros(y0Noise.shape)
+        log10M500cs=np.zeros(y0Noise.shape)
         zs=np.zeros(y0Noise.shape)
         zErrs=np.zeros(y0Noise.shape)
         Ez2s=np.zeros(y0Noise.shape)
         Qs=np.zeros(y0Noise.shape)
         fRels=np.zeros(y0Noise.shape)
+        if verbose:
+            print(">>> Generating mock sample in redshift slices")
         for k in range(len(zRange)):
+
+            if verbose:
+                print("... z = %.3f [%d/%d]" % (zRange[k], k+1, len(zRange)))
             
             t00=time.time()
             zk=zRange[k]
             zIndex=np.argmin(abs(zk-self.z))      
             if numDraws is not None:
                 numClusters_zk=int(round(numDraws/len(zRange)))
             else:
@@ -482,39 +548,44 @@
             currentIndex=nextIndex
             t22=time.time()
             
             log10Ms[mask]=self.log10MRollers[k](log10Ms[mask])
             
             # We generalised mass definitions, but still need M500c, theta500c for Q, fRel calc
             # So... we may as well convert and add that to output (below) as well
-            if self.delta != 500 or self.rhoType != "critical":
-                log10M500c=np.log10(self.mdef.translate_mass(self.cosmoModel, np.power(10, log10Ms[mask]),
-                                                                1/(1+zk), self._M500cDef))
+            if self.delta == 500 and self.rhoType == "critical":
+                log10M500cs[mask]=log10Ms[mask]
             else:
-                log10M500c=log10Ms[mask]
+                log10M500cs[mask]=np.log10(self.mdef.translate_mass(self.cosmoModel, np.power(10, log10Ms[mask]),
+                                                                1/(1+zk), self._M500cDef))
 
-            theta500s=interpolate.splev(log10M500c, self.theta500Splines[k], ext = 3)
-            Qs[mask]=QFit.getQ(theta500s, z = zk, tileName = tileName)
-            fRels[mask]=interpolate.splev(log10M500c, self.fRelSplines[k], ext = 3)
+            theta500s=interpolate.splev(log10M500cs[mask], self.theta500Splines[k], ext = 3)
+            if QFit is not None:
+                Qs[mask]=QFit.getQ(theta500s, z = zk, tileName = tileName)
+            else:
+                Qs[mask]=1.0
+            fRels[mask]=interpolate.splev(log10M500cs[mask], self.fRelSplines[k], ext = 3)
             Ez2s[mask]=self.Ez2[k]
             zs[mask]=zk
       
         # For some cosmo parameters, splined masses can end up outside of valid range, so catch this
         log10Ms[log10Ms < self.log10M.min()]=self.log10M.min()
         log10Ms[log10Ms > self.log10M.max()]=self.log10M.max()
         
         # For some cosmo parameters, fRel can wander outside its range for crazy masses
         # So we just cap it at 0.1 here just to avoid -ve in log
         fRels[fRels <= 0]=0.1
         fRels[fRels > 1]=1.0
         try:
-            true_y0s=tenToA0*Ez2s*np.power(np.power(10, log10Ms)/Mpivot, 1+B0)*Qs*fRels
+            true_y0s=tenToA0*Ez2s*np.power(np.power(10, log10Ms)/Mpivot, 1+B0)*Qs
         except:
             raise Exception("Negative y0 values (probably spline related) for H0 = %.6f Om0 = %.6f sigma8 = %.6f at z = %.3f" % (self.H0, self.Om0, self.sigma8, zk))
-            
+        if applyRelativisticCorrection == True:
+            true_y0s=true_y0s*fRels
+
         # Add noise and intrinsic scatter everywhere
         if applyIntrinsicScatter == True:
             scattered_y0s=np.exp(np.random.normal(np.log(true_y0s), sigma_int, len(true_y0s)))
         else:
             scattered_y0s=true_y0s
         if applyNoiseScatter == True:
             measured_y0s=np.random.normal(scattered_y0s, y0Noise)
@@ -526,19 +597,23 @@
         massColLabel="true_M%d%s" % (self.delta, self.rhoType[0])
         tab=atpy.Table()
         tab.add_column(atpy.Column(names, 'name'))
         tab.add_column(atpy.Column(RAs, 'RADeg'))
         tab.add_column(atpy.Column(decs, 'decDeg'))
         tab.add_column(atpy.Column(np.power(10, log10Ms)/1e14, massColLabel))
         if 'true_M500c' not in tab.keys():
-            tab.add_column(atpy.Column(np.power(10, log10M500c)/1e14, 'true_M500c'))
-        tab.add_column(atpy.Column(Qs, 'true_Q'))
-        tab.add_column(atpy.Column(true_y0s/1e-4, 'true_fixed_y_c'))
-        tab.add_column(atpy.Column(measured_y0s/1e-4, 'fixed_y_c'))
-        tab.add_column(atpy.Column(y0Noise/1e-4, 'fixed_err_y_c'))
+            tab.add_column(atpy.Column(np.power(10, log10M500cs)/1e14, 'true_M500c'))
+        if QFit is None:
+            tab.add_column(atpy.Column(true_y0s/1e-4, 'true_y_c'))
+        else:
+            tab.add_column(atpy.Column(Qs, 'true_Q'))
+            tab.add_column(atpy.Column(true_y0s/1e-4, 'true_fixed_y_c'))
+            tab.add_column(atpy.Column(measured_y0s/1e-4, 'fixed_y_c'))
+            tab.add_column(atpy.Column(y0Noise/1e-4, 'fixed_err_y_c'))
+
         tab.add_column(atpy.Column(measured_y0s/y0Noise, 'fixed_SNR'))
         tab.add_column(atpy.Column(zs, 'redshift'))
         tab.add_column(atpy.Column(zErrs, 'redshiftErr'))
         if photFilterLabel is not None and tileName is not None:
             tab.add_column(atpy.Column([photFilterLabel]*len(tab), 'template'))
             tab.add_column(atpy.Column([tileName]*len(tab), 'tileName'))
```

### Comparing `nemo-sz-0.5.0/nemo/catalogs.py` & `nemo-sz-0.6.0/nemo/catalogs.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import sys
 import time
 import astropy.table as atpy
 from astropy.coordinates import SkyCoord
 from astropy.coordinates import match_coordinates_sky
 import astropy.io.fits as pyfits
 from scipy import ndimage
+from . import maps
 
 # For adding meta data to output
 import datetime
 import nemo
 
 #------------------------------------------------------------------------------------------------------------
 XMATCH_RADIUS_DEG=1.4/60.0  # catalog matching radius, for sim comparisons
@@ -28,14 +29,15 @@
 COLUMN_NAMES    = ['name', 
                    'RADeg', 
                    'decDeg', 
                    'SNR', 
                    'numSigPix', 
                    'template', 
                    'tileName',
+                   'flags',
                    'galacticLatDeg',
                    'deltaT_c',
                    'err_deltaT_c',
                    'y_c',
                    'err_y_c',
                    'Y500_sr',
                    'err_Y500_sr',
@@ -53,14 +55,15 @@
 COLUMN_FORMATS  = ['%s',
                    '%.6f',
                    '%.6f',
                    '%.1f',
                    '%d',
                    '%s',
                    '%s',
+                   '%d',
                    '%.6f',
                    '%.3f',
                    '%.3f',
                    '%.3e',
                    '%.3e',
                    '%.3e',
                    '%.3e',
@@ -177,15 +180,15 @@
                     if index != xIndices[xMatchIndex]:
                         mergedCatalog['toRemove'][index]=1
         mergedCatalog=mergedCatalog[mergedCatalog['toRemove'] == 0]
         mergedCatalog.remove_column('toRemove')
         mergedCatalog.sort(['RADeg', 'decDeg'])
         mergedCatalog=selectFromCatalog(mergedCatalog, constraintsList)
     else:
-        mergedCatalog=atpy.Table(names=('SNR','RADeg','decDeg'))
+        mergedCatalog=atpy.Table(names=('SNR', 'RADeg', 'decDeg'))
     
     return mergedCatalog
 
 #------------------------------------------------------------------------------------------------------------
 def catalog2DS9(catalog, outFileName, constraintsList = [], addInfo = [], idKeyToUse = 'name', 
                 RAKeyToUse = 'RADeg', decKeyToUse = 'decDeg', color = "cyan", showNames = True,
                 writeNemoInfo = True, coordSys = 'fk5', regionShape = 'point', width = 1):
@@ -290,25 +293,27 @@
     
 #------------------------------------------------------------------------------------------------------------
 def _makeRA(myRADeg):
     """Makes RA part of ACT names.
     
     """
     hours=(myRADeg/360)*24
+    strHours=("%.10f" % (hours))
     if hours<10:
-        sHours="0"+str(hours)[0]
+        sHours="0"+strHours[0]
     else:
-        sHours=str(hours)[:2]
+        sHours=strHours[:2]
     
-    mins=float(str(hours)[str(hours).index("."):])*60
-    if mins<10:
-        sMins="0"+str(mins)[:3]
+    mins=float(strHours[strHours.index("."):])*60
+    strMins=("%.10f" % (mins))
+    if mins < 10:
+        sMins="0"+strMins[:3]
     else:
-        sMins=str(mins)[:4]
-        
+        sMins=strMins[:4]
+
     return (sHours+sMins)#[:-2] # Trims off .x as not used in ACT names
         
 #------------------------------------------------------------------------------------------------------------
 def _makeDec(myDecDeg):
     """Makes dec part of ACT names
     
     """
@@ -655,15 +660,16 @@
         np.random.seed()
         
     return tab
 
 #------------------------------------------------------------------------------------------------------------
 def generateTestCatalog(config, numSourcesPerTile, amplitudeColumnName = 'fixed_y_c', 
                         amplitudeRange = [0.001, 1], amplitudeDistribution = 'linear', selFn = None,
-                        avoidanceRadiusArcmin = 20.0, maskDilationPix = 0):
+                        avoidanceRadiusArcmin = 20.0, maskDilationPix = 0,
+                        tileNames = None):
     """Generate a catalog of objects with random positions and amplitudes. This is for testing purposes - 
     see, e.g., :meth:`nemo.maps.sourceInjectionTest`.
     
     Args:
         config (:obj:`nemo.startup.NemoConfig`): Nemo configuration object.
         numSourcesPerTile (:obj:`int`): The maximum number of sources to insert into each tile. The number 
             of sources actually inserted may be less than this depending on the value of 
@@ -687,20 +693,24 @@
     Returns:
         An :obj:`astropy.table.Table` object containing the catalog.
         
     """
     
     if selFn is None:
         selFn=completeness.SelFn(config.selFnDir, 4.0, configFileName = config.configFileName, 
-                                 enableCompletenessCalc = False, setUpAreaMask = True)
+                                 enableCompletenessCalc = False, setUpAreaMask = True,
+                                 tileNames = tileNames)
+    if tileNames is None:
+        tileNames=selFn.tileNames
 
     RAs=[]
     decs=[]
     amps=[]
-    for tileName in config.tileNames:
+    catTileNames=[]
+    for tileName in tileNames:
         mapData=selFn.areaMaskDict[tileName]
         if mapData.sum() == 0:  # Skip any empty/blank tile
             continue
         wcs=selFn.WCSDict[tileName]
         # Dilate mask to avoid putting objects close to borders or holes
         for i in range(maskDilationPix):
             mapData=1-ndimage.binary_dilation(1-mapData)
@@ -725,29 +735,34 @@
                 keepObj=True
             if keepObj == True:
                 tileRAs.append(rai)
                 tileDecs.append(deci)
                 keepIndices.append(i)
             if len(keepIndices) == numSourcesPerTile:
                 break
+        # Edge case where we have tiny but non-zero area and didn't manage to insert anything
+        if len(coords) == 0:
+            continue
         RAs=RAs+coords[keepIndices, 0].tolist()
         decs=decs+coords[keepIndices, 1].tolist()
         if amplitudeDistribution == 'linear':
             amp=np.random.uniform(amplitudeRange[0], amplitudeRange[1], len(keepIndices))
         elif amplitudeDistribution == 'log':
             amp=np.power(10, np.random.uniform(np.log10(amplitudeRange)[0], np.log10(amplitudeRange)[1], len(keepIndices)))
         else:
             raise Exception("Must be either 'linear' or 'log'.")
         amps=amps+amp.tolist()
+        catTileNames=catTileNames+[tileName]*len(amp.tolist())
     
     tab=atpy.Table()
     tab.add_column(atpy.Column(np.arange(0, len(amps))+1, "name"))
     tab.add_column(atpy.Column(RAs, "RADeg"))
     tab.add_column(atpy.Column(decs, "decDeg"))
     tab.add_column(atpy.Column(amps, amplitudeColumnName))
+    tab.add_column(atpy.Column(catTileNames, 'tileName'))
 
     return tab
 
 #------------------------------------------------------------------------------------------------------------
 def crossMatch(refCatalog, matchCatalog, radiusArcmin = 2.5):
     """Cross matches `matchCatalog` onto `refCatalog` for objects found within some angular radius 
     (specified in arcmin).
@@ -852,24 +867,58 @@
             this image mask.
     
     Returns:
         An astropy Table containing the subset of objects within the image.
     
     """
     
-    xyCoords=wcs.wcs2pix(tab['RADeg'].tolist(), tab['decDeg'].tolist())
-    xyCoords=np.array(xyCoords, dtype = int)
+    xyCoords=np.array(wcs.wcs2pix(tab['RADeg'].tolist(), tab['decDeg'].tolist()))
     selected=[]
     for i in range(len(tab)):
         x, y=xyCoords[i][0], xyCoords[i][1]
+        if np.isnan(x) == True or np.isnan(y) == True:
+            selected.append(False)
+            continue
         if x >= 0 and x < shape[1]-1 and y >= 0 and y < shape[0]-1:
             if mask is not None:
                 if mask[int(round(y)), int(round(x))] == 1:
                     selected.append(True)
                 else:
                     selected.append(False)
             else:
                 selected.append(True)
         else:
             selected.append(False)
     
     return tab[selected]
+
+#------------------------------------------------------------------------------------------------------------
+def addFootprintColumnToCatalog(tab, label, areaMask, wcs):
+    """Add `footprint_label` column to the catalog, flagging objects found within the valid area of the given
+    mask.
+
+    Args:
+        tab (:obj:`astropy.table.Table`): Catalog, as an astropy Table object. Must have columns called
+            'RADeg', 'decDeg' that contain object coordinates in decimal degrees.
+        label (:obj:`str`): A column named `footprint_label` will be added to the catalog. Objects in the
+            catalog that fall within the valid area of the given area mask will have `footprint_label`
+            set to True.
+        areaMask (:obj:`np.ndarray`): Mask image defining the footprint corresponding to the given WCS.
+            Pixels with value = 1 indicate valid area, and pixels with value = 0 are considered to be
+            outside the mask.
+        wcs (:obj:`astWCS.WCS`): WCS of the area mask that defines the footprint.
+
+    Returns:
+        An astropy Table with `footprint_label` column added.
+
+    """
+
+    inMask=np.zeros(len(tab['RADeg'].data), dtype = bool)
+    coords=wcs.wcs2pix(tab['RADeg'].data, tab['decDeg'].data)
+    coords=np.array(np.round(coords), dtype = int)
+    mask1=np.logical_and(coords[:, 0] >= 0, coords[:, 1] >= 0)
+    mask2=np.logical_and(coords[:, 0] < areaMask.shape[1], coords[:, 1] < areaMask.shape[0])
+    mask=np.logical_and(mask1, mask2)
+    inMask[mask]=inMask[mask]+areaMask[coords[:, 1][mask], coords[:, 0][mask]]
+    tab['footprint_%s' % (label)]=inMask
+
+    return tab
```

### Comparing `nemo-sz-0.5.0/nemo/completeness.py` & `nemo-sz-0.6.0/nemo/completeness.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from scipy import optimize
 import nemo
 from . import signals
 from . import maps
 from . import MockSurvey
 from . import plotSettings
 from . import startUp
+from . import catalogs
 from collections import OrderedDict
 import colorcet
 import types
 import pickle
 import astropy.io.fits as pyfits
 import time
 import shutil
@@ -34,14 +35,18 @@
 from decimal import Decimal
 
 # If want to catch warnings as errors...
 #import warnings
 #warnings.filterwarnings('error')
 
 #------------------------------------------------------------------------------------------------------------
+class FootprintError(Exception):
+    pass
+
+#------------------------------------------------------------------------------------------------------------
 class SelFn(object):
     """An object that describes the survey selection function. It uses the output in the ``selFn/`` directory
     (produced by the :ref:`nemoCommand` command) to calculate the survey completeness for a given
     signal-to-noise cut on a (log\ :sub:`10` mass, z) grid for a given set of cosmological and scaling
     relation parameters.
        
     Args:
@@ -50,15 +55,15 @@
             and information needed to construct the filter mismatch function, `Q`, used in mass
             modeling.
         SNRCut (:obj:`float`): Completeness will be computed relative to this signal-to-noise selection
             cut (labelled as `fixed_SNR` in the catalogs produced by :ref:`nemoCommand`).
         configFileName (:obj:`str`, optional): Path to a Nemo configuration file. If not given, this
             will be read from ``selFnDir/config.yml``, which is the config file for the 
             :ref:`nemoCommand` run that produced the ``selFn`` directory.
-        footprintLabel (:obj:`str`, optional): Use this to specify a footprint, if any are defined in the
+        footprint (:obj:`str`, optional): Use this to specify a footprint, if any are defined in the
             Nemo config used to produce the ``selFn`` dir (e.g., 'DES', 'HSC', 'KiDS' etc.). The default
             value of ``None`` uses the whole survey footprint.
         zStep (:obj:`float`, optional): Use this to set the binning in redshift for completeness
             calculations.
         tileNames (:obj:`list`, optional): If given, restrict the :class:`SelFn` object to use only these
             tiles.
         enableDrawSample (:obj:`bool`, optional): This only needs to be set to `True` for generating mock
@@ -72,24 +77,35 @@
             correction of mass estimates. Probably only useful for debugging.
         applyRelativisticCorrection (:obj:`bool`, optional): Set to `False` to disable inclusion of
             the relativistic correction in completeness calculations.
         setupAreaMask (:obj:`bool`, optional): If `True`, read in the area masks so that quick position
             checks can be done (e.g., by :meth:`SelFn.checkCoordsAreInMask`).
         enableCompletenessCalc (:obj:`bool`, optional): If `True`, set up the machinery needed to do
             completeness calculations.
+        massFunction (:obj:`str`, optional): Name of the mass function to use, currently either
+            'Tinker08' or 'Tinker10'. Mass function calculations are done by CCL.
+        maxTheta500Arcmin (:obj:`float`, optional): If given, exclude clusters with expected angular size
+            greater than this from the cluster counts (set their completeness to 0).
+        method (:obj:`str`, optional): The method for calculating completeness. Options are: 'fast'
+            (using a simple model based on the noise and the expected cluster signals), or 'injection'
+            (directly using the results of end-to-end cluster injection and recovery sims).
+        QSource (:obj:`str`, optional): The source to use for Q (the filter mismatch function) - either
+            'fit' (to use results from the original Q-fitting routine) or 'injection' (to use Q derived
+            from source injection simulations).
 
     Attributes:
         SNRCut (:obj:`float`): Completeness will be computed relative to this signal-to-noise selection cut
             (labelled as `fixed_SNR` in the catalogs produced by :ref:`nemoCommand`).
-        footprintLabel (:obj:`str`): Use this to specify a footprint, if any are defined in the Nemo config
+        footprint (:obj:`str`): Use this to specify a footprint, if any are defined in the Nemo config
             used to produce the ``selFn`` dir (e.g., 'DES', 'HSC', 'KiDS' etc.). The default of ``None``
             uses the whole survey footprint.
         applyMFDebiasCorrection (:obj:`bool`): Set to `False` to disable the Eddington bias correction of
             mass estimates. Probably only useful for debugging.
         zStep (:obj:`float`): Use this to set the binning in redshift for completeness calculations.
+        zMax (:obj:`float`): Sets the maximum z used for completeness calculations.
         tileNames (:obj:`list`): The list of tiles used by the SelFn object (default of None uses all tiles).
         WCSDict (:obj:`dict`): A dictionary indexed by `tileName`, containing :obj:`astWCS.WCS` objects
             that describe the mapping between pixel coords and (RA, dec) coords in each tile.
         areaMaskDict (:obj:`dict`): A dictionary containing the survey area masks, indexed by tileName.
             Values > 0 in these masks define the cluster or source search area.
         scalingRelationDict (:obj:`dict`): A dictionary of scaling relation parameters (see example Nemo
             config files for the format).
@@ -103,133 +119,180 @@
         fRelDict (:obj:`dict`): A dictionary of weights used for relativistic corrections, indexed by
             `tileName`.
         mockSurvey (:class:`nemo.MockSurvey.MockSurvey`): A :class:`MockSurvey` object, used for halo mass function 
             calculations and generating mock catalogs.
 
     Note: 
         Some of the methods of this class are experimental and not necessarily well tested.
+
+    Note:
+        Once SNRCut is set for this object, it cannot be changed later (well, it can... but changing
+        self.SNRCut will not update anything, for the moment).
             
     """
         
-    def __init__(self, selFnDir, SNRCut, configFileName = None, footprintLabel = None, zStep = 0.01, 
-                 tileNames = None, enableDrawSample = False, mockOversampleFactor = 1.0, 
+    def __init__(self, selFnDir, SNRCut, configFileName = None, footprint = None, zStep = 0.01,
+                 zMax = 3.0, tileNames = None, enableDrawSample = False, mockOversampleFactor = 1.0,
                  downsampleRMS = True, applyMFDebiasCorrection = True, applyRelativisticCorrection = True,
-                 setUpAreaMask = False, enableCompletenessCalc = True, delta = 500, rhoType = 'critical'):
+                 setUpAreaMask = False, enableCompletenessCalc = True, delta = 500, rhoType = 'critical',
+                 massFunction = 'Tinker08', maxTheta500Arcmin = None, method = 'fast',
+                 QSource = 'fit', noiseCut = None):
         
         self.SNRCut=SNRCut
-        self.footprintLabel=footprintLabel
+        if footprint == 'full':
+            footprint=None
+        self.footprint=footprint
         self.downsampleRMS=downsampleRMS
         self.applyMFDebiasCorrection=applyMFDebiasCorrection
         self.applyRelativisticCorrection=applyRelativisticCorrection
         self.selFnDir=selFnDir
         self.zStep=zStep
+        self.maxTheta500Arcmin=maxTheta500Arcmin
 
         if configFileName is None:
             configFileName=self.selFnDir+os.path.sep+"config.yml"
             if os.path.exists(configFileName) == False:
                 raise Exception("No config .yml file found in selFnDir and no other location given.")
-        parDict=startUp.parseConfigFile(configFileName)
-        maps.addAutoTileDefinitions(parDict, DS9RegionFileName = self.selFnDir+os.path.sep+"tiles.reg",
-                                    cacheFileName = self.selFnDir+os.path.sep+"tileDefinitions.yml")
-
-        if tileNames == None:
-            self.tileNames=[]
-            if 'tileDefinitions' not in parDict.keys():
-                self.tileNames.append('PRIMARY')
-            else:
-                for tileDef in parDict['tileDefinitions']:
-                    self.tileNames.append(tileDef['tileName'])
-        else:
+        self._config=startUp.NemoConfig(configFileName, makeOutputDirs = False, setUpMaps = False, verbose = False,
+                                        selFnDir = self.selFnDir)
+        parDict=self._config.parDict
+
+        if tileNames is not None:
             self.tileNames=tileNames
+        else:
+            self.tileNames=self._config.tileNames
         
+        deprecatedMethods=['montecarlo']
+        if method in deprecatedMethods:
+            raise Exception("Selection function completeness calculation method '%s' is deprecated - use a valid method (e.g., 'injection')" % (method))
+        self.method=method
+
         # Needed for generating mock samples directly
-        self.photFilterLabel=parDict['photFilter']
+        self.photFilterLabel=self._config.parDict['photFilter']
             
-        # Sanity check that any given footprint is defined - if not, give a useful error message
-        if footprintLabel is not None:
+        # Check that any given footprint is defined - if not, give a useful error message
+        if footprint is not None:
             if 'selFnFootprints' not in parDict.keys():
                 raise Exception("No footprints defined in .yml config file")
             else:
                 labelsList=[]
                 for footprintDict in parDict['selFnFootprints']:
                     labelsList.append(footprintDict['label'])
-                if footprintLabel not in labelsList:
+                if footprint not in labelsList:
                     raise Exception("Footprint '%s' not found in selFnFootprints - check .yml config file" % (footprintLabel))
         
         # Load area masks
         if setUpAreaMask == True:
             self._setUpAreaMask()
         else:
             self.tileTab=None
             self.WCSDict=None
             self.areaMaskDict=None
                 
         if enableCompletenessCalc == True:
             
             self.scalingRelationDict=parDict['massOptions']
-            self.Q=signals.QFit(self.selFnDir+os.path.sep+"QFit.fits", tileNames = tileNames)
-            
+
+            # If the config didn't give cosmological parameters, put in defaults
+            defaults={'H0': 70.0, 'Om0': 0.30, 'Ob0': 0.05, 'sigma8': 0.8, 'ns': 0.95}
+            for key in defaults:
+                if key not in self.scalingRelationDict.keys():
+                    self.scalingRelationDict[key]=defaults[key]
+
             # We should be able to do everything (except clustering) with this
             # NOTE: Some tiles may be empty, so we'll exclude them from tileNames list here
             RMSTabFileName=self.selFnDir+os.path.sep+"RMSTab.fits"
-            if footprintLabel is not None:
-                RMSTabFileName=RMSTabFileName.replace(".fits", "_%s.fits" % (footprintLabel))
+            if footprint is not None:
+                RMSTabFileName=RMSTabFileName.replace(".fits", "_%s.fits" % (footprint))
+            if os.path.exists(RMSTabFileName) == False:
+                raise FootprintError
             self.RMSTab=atpy.Table().read(RMSTabFileName)
+            # Sanitise just in case [this is an edge case that has happened on one sim]
+            self.RMSTab=self.RMSTab[self.RMSTab['areaDeg2'] > 0]
+            if noiseCut is not None:
+                self.RMSTab=self.RMSTab[self.RMSTab['y0RMS'] < noiseCut]
             self.RMSDict={}
             tileNames=[]
+            totalAreaDeg2=0.0 # Doing it this way so that tileNames can be chosen and fed into selFn
             for tileName in self.tileNames:
                 tileTab=self.RMSTab[self.RMSTab['tileName'] == tileName]
                 if downsampleRMS == True and len(tileTab) > 0:
                     tileTab=downsampleRMSTab(tileTab) 
                 if len(tileTab) > 0:    # We may have some blank tiles...
                     self.RMSDict[tileName]=tileTab
                     tileNames.append(tileName)
+                    totalAreaDeg2=totalAreaDeg2+tileTab['areaDeg2'].sum()
             self.tileNames=tileNames
-            self.totalAreaDeg2=self.RMSTab['areaDeg2'].sum()
-            
+            self.totalAreaDeg2=totalAreaDeg2
+            # If want a plot of noise distribution
+            # plt.hist(self.RMSTab['y0RMS'], weights = self.RMSTab['areaDeg2'], bins  = 100, density=True)
+
             # For weighting - arrays where entries correspond with tileNames list
             tileAreas=[]    
             for tileName in self.tileNames:
                 areaDeg2=self.RMSTab[self.RMSTab['tileName'] == tileName]['areaDeg2'].sum()
                 tileAreas.append(areaDeg2)
             self.tileAreas=np.array(tileAreas)
             self.fracArea=self.tileAreas/self.totalAreaDeg2
 
+            # Check of area consistency
+            #checkAreaDeg2=0
+            #for tileName in self.tileNames:
+                #checkAreaDeg2=checkAreaDeg2+(self.areaMaskDict[tileName]*maps.getPixelAreaArcmin2Map(self.areaMaskDict[tileName].shape, self.WCSDict[tileName])/(60**2)).sum()
+
             # For quick sample generation
             self.mockOversampleFactor=mockOversampleFactor
             self.y0NoiseAverageDict={}
             for tileName in self.tileNames:
                 RMSTab=self.RMSDict[tileName]
                 areaWeights=RMSTab['areaDeg2'].data/RMSTab['areaDeg2'].data.sum()
                 if areaWeights.sum() > 0:
                     self.y0NoiseAverageDict[tileName]=np.average(RMSTab['y0RMS'].data, 
                                                                  weights = areaWeights)            
             assert(len(self.tileNames) == len(self.tileAreas))
             assert(len(self.tileNames) == len(self.y0NoiseAverageDict.keys()))
 
             # For relativistic corrections
             self.fRelDict=signals.loadFRelWeights(self.selFnDir+os.path.sep+"fRelWeights.fits")
-            
+
+            # Stuff from the source injection sims (now required for completeness calculation)
+            if self.method == 'injection':
+                injDataPath=self.selFnDir+os.path.sep+"sourceInjectionData.fits"
+                inputDataPath=self.selFnDir+os.path.sep+"sourceInjectionInputCatalog.fits"
+                if os.path.exists(injDataPath) == False or os.path.exists(inputDataPath) == False:
+                    raise Exception("%s not found - run a source injection test to generate (now required for completeness calculations)." % (injDataPath))
+                injTab=atpy.Table().read(injDataPath)
+                inputTab=atpy.Table().read(inputDataPath)
+                if footprint is not None:
+                    injTab=self.cutCatalogToSurveyArea(injTab)
+                    inputTab=self.cutCatalogToSurveyArea(inputTab)
+                theta500s, binCentres, compThetaGrid, thetaQ=_parseSourceInjectionData(injTab, inputTab, self.SNRCut)
+                self.compThetaInterpolator=interpolate.RectBivariateSpline(theta500s, binCentres,
+                                                                        compThetaGrid, kx = 3, ky = 3)
+
+            # Q can now either be from the 'classic' fit or the source injection sims
+            self.Q=signals.QFit(QSource = QSource, selFnDir = self.selFnDir, tileNames = tileNames)
+
             # Initial cosmology set-up
             minMass=5e13
             zMin=0.0
-            zMax=2.0
-            H0=70.
-            Om0=0.30
-            Ob0=0.05
-            sigma8=0.8
-            ns=0.95
+            H0=self.scalingRelationDict['H0']
+            Om0=self.scalingRelationDict['Om0']
+            Ob0=self.scalingRelationDict['Ob0']
+            sigma8=self.scalingRelationDict['sigma8']
+            ns=self.scalingRelationDict['ns']
             self.mockSurvey=MockSurvey.MockSurvey(minMass, self.totalAreaDeg2, zMin, zMax, H0, Om0, Ob0, sigma8, ns,
                                                   zStep = self.zStep, enableDrawSample = enableDrawSample,
-                                                  delta = delta, rhoType = rhoType)
+                                                  delta = delta, rhoType = rhoType, massFunction = massFunction)
             self.update(H0, Om0, Ob0, sigma8, ns)
 
 
     def _setUpAreaMask(self):
-        """Sets-up WCS info and loads area masks - needed for quick position checks etc.
+        """Sets-up WCS info and loads area masks (taking into account the footprint, if specified)
+        - needed for quick position checks etc.
         
         """
         
         # This takes ~20 sec to set-up - we could cache, or it's overhead when initialising SelFn
         # We could do a lot of this by just making the area mask, mass limit maps etc. MEFs
         # But then we wouldn't want to lazily load them (probably)
         self.tileTab=atpy.Table()
@@ -237,27 +300,47 @@
         self.tileTab.add_column(atpy.Column(np.zeros(len(self.tileNames)), 'RAMin'))
         self.tileTab.add_column(atpy.Column(np.zeros(len(self.tileNames)), 'RAMax'))
         self.tileTab.add_column(atpy.Column(np.zeros(len(self.tileNames)), 'decMin'))
         self.tileTab.add_column(atpy.Column(np.zeros(len(self.tileNames)), 'decMax'))
         self.WCSDict={}
         self.areaMaskDict={}
         for row in self.tileTab:
-            areaMap, wcs=loadAreaMask(row['tileName'], self.selFnDir)
+            if self.footprint is None:
+                areaMap, wcs=loadAreaMask(row['tileName'], self.selFnDir)
+            else:
+                areaMap, wcs=loadIntersectionMask(row['tileName'], self.selFnDir, self.footprint)
             self.WCSDict[row['tileName']]=wcs.copy()
             self.areaMaskDict[row['tileName']]=areaMap
             ra0, dec0=self.WCSDict[row['tileName']].pix2wcs(0, 0)
             ra1, dec1=self.WCSDict[row['tileName']].pix2wcs(wcs.header['NAXIS1'], wcs.header['NAXIS2'])
             if ra1 > ra0:
                 ra1=-(360-ra1)
             row['RAMin']=min([ra0, ra1])
             row['RAMax']=max([ra0, ra1])
             row['decMin']=min([dec0, dec1])
             row['decMax']=max([dec0, dec1])
             
-            
+
+    def cutCatalogToSurveyArea(self, catalog):
+        """Checks that the coordinates of objects in the given catalog are within the survey area
+        (taking into account a footprint, if specified) and cuts the catalog accordingly.
+
+        Args:
+            catalog (:obj:`astropy.table.Table`): The input catalog, as an astropy Table.
+
+        Returns:
+            A catalog (:obj:`astropy.table.Table`), cut to the survey area.
+
+        """
+
+        RAKey, decKey=catalogs.getTableRADecKeys(catalog)
+        mask=self.checkCoordsInAreaMask(catalog[RAKey], catalog[decKey])
+        return catalog[mask]
+
+
     def checkCoordsInAreaMask(self, RADeg, decDeg):
         """Checks if the given RA, dec coords are in valid regions of the map.
         
         Args:
             RADeg (:obj:`float` or :obj:`np.ndarray`): RA in decimal degrees.
             decDeg (:obj:`float` or :obj:`np.ndarray`): Dec in decimal degrees.
         
@@ -268,46 +351,31 @@
 
         if self.tileTab is None:
             self._setUpAreaMask()
 
         RADeg=np.array(RADeg)
         decDeg=np.array(decDeg)
         if RADeg.shape == ():
-            RADeg=[RADeg]
+            RADeg=np.array([RADeg])
         if decDeg.shape == ():
-            decDeg=[decDeg]
-        inMaskList=[]
-        for ra, dec in zip(RADeg, decDeg):
-            inMask=False
-            # Inside footprint check
-            # NOTE: Tiles may have -ve RAMin coords
-            raMask=np.logical_and(np.greater_equal(ra, self.tileTab['RAMin']), np.less(ra, self.tileTab['RAMax']))
-            negRAMask=np.logical_and(np.greater_equal(-(360-ra), self.tileTab['RAMin']), np.less(-(360-ra), self.tileTab['RAMax']))
-            raMask=np.logical_or(raMask, negRAMask)
-            decMask=np.logical_and(np.greater_equal(dec, self.tileTab['decMin']), np.less(dec, self.tileTab['decMax']))
-            tileMask=np.logical_and(raMask, decMask)
-            # This is just dealing with bytes versus strings in python3
-            matchTilesList=[]
-            for item in self.tileTab['tileName'][tileMask].tolist():
-                if type(item) == bytes:
-                    matchTilesList.append(item.decode('utf-8'))
-                else:
-                    matchTilesList.append(str(item))
-            for tileName in matchTilesList:
-                x, y=self.WCSDict[tileName].wcs2pix(ra, dec)
-                x=int(round(x)); y=int(round(y))
-                if x < self.WCSDict[tileName].header['NAXIS1'] and y < self.WCSDict[tileName].header['NAXIS2'] \
-                    and self.areaMaskDict[tileName][y, x] > 0:
-                    inMask=True
-            inMaskList.append(inMask)
-        
-        if len(inMaskList) > 1:
-            return np.array(inMaskList)
-        else:
-            return inMaskList[0]
+            decDeg=np.array([decDeg])
+        inMask=np.zeros(len(RADeg), dtype = bool)
+        tabList=[]
+        for tileName in self.tileNames:
+            wcs=self.WCSDict[tileName]
+            areaMask=self.areaMaskDict[tileName]
+            if areaMask.sum() > 0:
+                coords=wcs.wcs2pix(RADeg, decDeg)
+                coords=np.array(np.round(coords), dtype = int)
+                mask1=np.logical_and(coords[:, 0] >= 0, coords[:, 1] >= 0)
+                mask2=np.logical_and(coords[:, 0] < areaMask.shape[1], coords[:, 1] < areaMask.shape[0])
+                mask=np.logical_and(mask1, mask2)
+                inMask[mask]=inMask[mask]+areaMask[coords[:, 1][mask], coords[:, 0][mask]]
+
+        return inMask
         
 
     def update(self, H0, Om0, Ob0, sigma8, ns, scalingRelationDict = None):
         """Re-calculates the survey-average selection function for a given set of cosmological and scaling
         relation parameters.
         
         Returns:
@@ -316,78 +384,116 @@
 
         """
 
         if scalingRelationDict is not None:
             self.scalingRelationDict=scalingRelationDict
         
         self.mockSurvey.update(H0, Om0, Ob0, sigma8, ns)
-        
-        #---
-        # New - as well as completeness, get y0 grid to map between cluster counts <-> y0
         zRange=self.mockSurvey.z
-        y0GridCube=[]
-        compMzCube=[]
-        for tileName in self.RMSDict.keys():
-            tenToA0, B0, Mpivot, sigma_int=[self.scalingRelationDict['tenToA0'], self.scalingRelationDict['B0'], 
-                                            self.scalingRelationDict['Mpivot'], self.scalingRelationDict['sigma_int']]
-            y0Grid=np.zeros([zRange.shape[0], self.mockSurvey.clusterCount.shape[1]])
+        if self.method == 'injection':
+
+            # WARNING: Here there is no Q, and y0 is true y0, NOT y0~
+            # These grids are purely mapping 'input' signals to M, z via the scaling relation
+            y0Grid, theta500Grid=self._makeSignalGrids(applyQ = False)
+
+            compMz=np.zeros(y0Grid.shape)
             for i in range(len(zRange)):
-                zk=zRange[i]
-                k=np.argmin(abs(self.mockSurvey.z-zk))
-                if self.mockSurvey.delta != 500 or self.mockSurvey.rhoType != "critical":
-                    log10M500s=np.log10(self.mockSurvey.mdef.translate_mass(self.mockSurvey.cosmoModel, 
-                                                                            self.mockSurvey.M, 
-                                                                            self.mockSurvey.a[k], 
-                                                                            self.mockSurvey._M500cDef))
-                else:
-                    log10M500s=self.mockSurvey.log10M
-                theta500s_zk=interpolate.splev(log10M500s, self.mockSurvey.theta500Splines[k])
-                Qs_zk=self.Q.getQ(theta500s_zk, zk, tileName = tileName)
-                true_y0s_zk=tenToA0*np.power(self.mockSurvey.Ez[k], 2)*np.power(np.power(10, self.mockSurvey.log10M)/Mpivot,
-                                                                                1+B0)*Qs_zk
-                if self.applyRelativisticCorrection == True:
-                    fRels_zk=interpolate.splev(log10M500s, self.mockSurvey.fRelSplines[k])
-                    true_y0s_zk=true_y0s_zk*fRels_zk
-                y0Grid[i]=true_y0s_zk
-                
-            # For some cosmological parameters, we can still get the odd -ve y0
-            y0Grid[y0Grid <= 0] = 1e-9
-        
-            # Calculate completeness using area-weighted average
-            # NOTE: RMSTab that is fed in here can be downsampled in noise resolution for speed
-            RMSTab=self.RMSDict[tileName]
-            areaWeights=RMSTab['areaDeg2']/RMSTab['areaDeg2'].sum()
-            log_y0Lim=np.log(self.SNRCut*RMSTab['y0RMS'])
-            log_y0=np.log(y0Grid)
-            compMz=np.zeros(log_y0.shape)
-            for i in range(len(RMSTab)):
-                SNRGrid=y0Grid/RMSTab['y0RMS'][i]
-                SNRGrid=SNRGrid
-                log_y0Err=1/SNRGrid
-                log_y0Err[SNRGrid < self.SNRCut]=1/self.SNRCut
-                log_totalErr=np.sqrt(log_y0Err**2 + sigma_int**2)
-                compMz=compMz+stats.norm.sf(log_y0Lim[i], loc = log_y0, scale = log_totalErr)*areaWeights[i]
-            compMzCube.append(compMz)
-            y0GridCube.append(y0Grid)
-        compMzCube=np.array(compMzCube)
-        y0GridCube=np.array(y0GridCube)
-        self.compMz=np.average(compMzCube, axis = 0, weights = self.fracArea)
-        self.y0Grid=np.average(y0GridCube, axis = 0, weights = self.fracArea)
-
-        #---
-        # Old
-        #compMzCube=[]
-        #for tileName in self.RMSDict.keys():
-            #compMzCube.append(calcCompleteness(self.RMSDict[tileName], self.SNRCut, tileName, 
-                                               #self.mockSurvey, self.scalingRelationDict, self.tckQFitDict))
-            #if np.any(np.isnan(compMzCube[-1])) == True:
-                #raise Exception("NaNs in compMz for tile '%s'" % (tileName))
-        #compMzCube=np.array(compMzCube)
-        #self.compMz=np.average(compMzCube, axis = 0, weights = self.fracArea)
-        
+                try:
+                    compMz[i]=np.diag(self.compThetaInterpolator(theta500Grid[i], y0Grid[i]/1e-04))
+                except:
+                    # If above fails, it's because relativistic correction is on, and y0 doesn't always increase
+                    for j in range(y0Grid[i].shape[0]):
+                        compMz[i][j]=self.compThetaInterpolator(theta500Grid[i][j], y0Grid[i][j]/1e-04)
+            compMz[compMz < 0]=0
+            compMz[compMz > 1]=1
+            self.compMz=compMz
+            self.y0TildeGrid=self.Q.getQ(theta500Grid)*y0Grid
+
+            if self.scalingRelationDict['sigma_int'] > 0:
+                # Fiddling with Gaussian filter params has no effect
+                mode='nearest'
+                truncate=4.0
+                logy0Grid=np.log(y0Grid)
+                for i in range(logy0Grid.shape[0]):
+                    dy=np.mean(np.gradient(logy0Grid[i]))
+                    if dy > 0:
+                        npix=self.scalingRelationDict['sigma_int']/dy
+                        npix=npix*0.8   # Making this correction seems to work but not sure why yet
+                        self.mockSurvey.clusterCount[i]=ndimage.gaussian_filter1d(self.mockSurvey.clusterCount[i], npix,
+                                                                                  mode = mode, truncate = truncate)
+
+        elif self.method == 'fast':
+            y0GridCube=[]
+            compMzCube=[]
+            theta500Cube=[]
+            for tileName in self.RMSDict.keys():
+                y0Grid, theta500Grid=self._makeSignalGrids(tileName = tileName)
+                # Calculate completeness using area-weighted average
+                # NOTE: RMSTab that is fed in here can be downsampled in noise resolution for speed
+                RMSTab=self.RMSDict[tileName]
+                areaWeights=RMSTab['areaDeg2']/RMSTab['areaDeg2'].sum()
+                y0Lim=self.SNRCut*RMSTab['y0RMS']
+                log_y0Lim=np.log(self.SNRCut*RMSTab['y0RMS'])
+                log_y0=np.log(y0Grid)
+                compMz=np.zeros(log_y0.shape)
+                for i in range(len(RMSTab)):
+                    # With intrinsic scatter [may not be quite right, but a good approximation]
+                    totalLogErr=np.sqrt((RMSTab['y0RMS'][i]/y0Grid)**2 + self.scalingRelationDict['sigma_int']**2)
+                    sfi=stats.norm.sf(y0Lim[i], loc = y0Grid, scale = totalLogErr*y0Grid)
+                    compMz=compMz+sfi*areaWeights[i]
+                    # No intrinsic scatter, Gaussian noise
+                    #sfi=stats.norm.sf(y0Lim[i], loc = y0Grid, scale = RMSTab['y0RMS'][i])
+                    #compMz=compMz+sfi*areaWeights[i]
+                if self.maxTheta500Arcmin is not None:
+                    compMz=compMz*np.array(theta500Grid < self.maxTheta500Arcmin, dtype = float)
+                compMzCube.append(compMz)
+                y0GridCube.append(y0Grid)
+            compMzCube=np.array(compMzCube)
+            y0GridCube=np.array(y0GridCube)
+            self.compMz=np.average(compMzCube, axis = 0, weights = self.fracArea)
+            self.y0TildeGrid=np.average(y0GridCube, axis = 0, weights = self.fracArea)
+
+
+    def _makeSignalGrids(self, applyQ = True, tileName = None):
+        """Returns y0~ and theta500 grid. tileName here is optional and only used for Q.
+
+        """
+        zRange=self.mockSurvey.z
+        tenToA0, B0, Mpivot, sigma_int=[self.scalingRelationDict['tenToA0'], self.scalingRelationDict['B0'],
+                                        self.scalingRelationDict['Mpivot'], self.scalingRelationDict['sigma_int']]
+        y0Grid=np.zeros([zRange.shape[0], self.mockSurvey.clusterCount.shape[1]])
+        theta500Grid=np.zeros([zRange.shape[0], self.mockSurvey.clusterCount.shape[1]])
+        for i in range(len(zRange)):
+            zk=zRange[i]
+            k=np.argmin(abs(self.mockSurvey.z-zk))
+            if self.mockSurvey.delta != 500 or self.mockSurvey.rhoType != "critical":
+                log10M500s=np.log10(self.mockSurvey.mdef.translate_mass(self.mockSurvey.cosmoModel,
+                                                                        self.mockSurvey.M,
+                                                                        self.mockSurvey.a[k],
+                                                                        self.mockSurvey._M500cDef))
+            else:
+                log10M500s=self.mockSurvey.log10M
+            theta500s_zk=interpolate.splev(log10M500s, self.mockSurvey.theta500Splines[k])
+            Qs_zk=self.Q.getQ(theta500s_zk, zk, tileName = tileName)
+            #Qs_zk=self.compQInterpolator(theta500s_zk) # Survey-averaged Q from injection sims
+            true_y0s_zk=tenToA0*np.power(self.mockSurvey.Ez[k], 2)*np.power(np.power(10, self.mockSurvey.log10M)/Mpivot,
+                                                                            1+B0)
+            if applyQ == True:
+                true_y0s_zk=true_y0s_zk*Qs_zk
+            if self.applyRelativisticCorrection == True:
+                fRels_zk=interpolate.splev(log10M500s, self.mockSurvey.fRelSplines[k])
+                true_y0s_zk=true_y0s_zk*fRels_zk
+            y0Grid[i]=true_y0s_zk #*0.95
+            theta500Grid[i]=theta500s_zk
+
+        # For some cosmological parameters, we can still get the odd -ve y0
+        y0Grid[y0Grid <= 0] = 1e-9
+
+        return y0Grid, theta500Grid
+
 
     def projectCatalogToMz(self, tab):
         """Project a Nemo cluster catalog (an astropy Table) into the (log\ :sub:`10` mass, z) grid, taking
         into account the uncertainties on y0, and redshift. Note that if the redshift error is non-zero, this
         is a lot slower.
         
         Args:
@@ -477,35 +583,42 @@
         for i in range(len(Pdet)):
             Pdet[i]=stats.norm.sf(log_y0Lim[i], loc = log_y0[i], scale = log_totalErr[i])
         tab['Pdet']=Pdet
         
         return tab
 
     
-    def generateMockSample(self):
+    def generateMockSample(self, mockOversampleFactor = None, applyPoissonScatter = True):
         """Returns a mock catalog (but with no object coordinate information).
         
-        Note:
-            This currently uses the average noise level in each tile, rather than the full noise
-            distribution in each tile.
+        Args:
+            mockOversampleFactor (:obj:`float`, optional): Scale the number of objects in the mock by this
+                factor (e.g., this can be used to apply an overall area re-scaling). If given, this
+                overrides self.mockOversampleFactor.
+            applyPoissonScatter (:obj:`bool`, optional): If True, apply Poisson scatter to the cluster
+                number counts when generating the mock catalog.
         
         """
         
+        if mockOversampleFactor is None:
+            mockOversampleFactor=self.mockOversampleFactor
+
         mockTabsList=[]
         for tileName, areaDeg2 in zip(self.tileNames, self.tileAreas):
-            mockTab=self.mockSurvey.drawSample(self.y0NoiseAverageDict[tileName], self.scalingRelationDict, 
+            mockTab=self.mockSurvey.drawSample(self.RMSDict[tileName], self.scalingRelationDict,
                                                self.Q, wcs = None, 
                                                photFilterLabel = self.photFilterLabel, tileName = tileName, 
                                                makeNames = False,
                                                SNRLimit = self.SNRCut, applySNRCut = True,
-                                               areaDeg2 = areaDeg2*self.mockOversampleFactor,
-                                               applyPoissonScatter = True,
+                                               areaDeg2 = areaDeg2*mockOversampleFactor,
+                                               applyPoissonScatter = applyPoissonScatter,
                                                applyIntrinsicScatter = True,
-                                               applyNoiseScatter = True)
-            if mockTab is not None:
+                                               applyNoiseScatter = True,
+                                               applyRelativisticCorrection = self.applyRelativisticCorrection)
+            if mockTab is not None and len(mockTab) > 0:
                 mockTabsList.append(mockTab)
         tab=atpy.vstack(mockTabsList)
 
         return tab
     
     
     def getMassLimit(self, completenessFraction, zBinEdges = None):
@@ -526,14 +639,57 @@
         if zBinEdges is None:
             zBinEdges=self.mockSurvey.zBinEdges
             
         return calcMassLimit(completenessFraction, self.compMz, self.mockSurvey, zBinEdges)
 
     
 #------------------------------------------------------------------------------------------------------------
+def _parseSourceInjectionData(injTab, inputTab, SNRCut):
+    """Produce arrays for constructing interpolator objects from source injection test data.
+
+    Args:
+        injTab (:obj:`astropy.table.Table`): Output catalog produced by the source injection test.
+        inputTab (:obj:`astropy.table.Table`): Input catalog produced by the source injectio test.
+        SNRCut (:obj:`float`): Selection threshold in S/N to apply.
+
+    Returns:
+        theta500s, ycBinCentres, compThetaGrid, thetaQ
+
+    """
+
+    # Completeness given y0 (NOT y0~) and theta500 and the S/N cut as 2D spline
+    # We also derive survey-averaged Q here from the injection sim results [for y0 -> y0~ mapping]
+    # NOTE: This is a survey-wide average, doesn't respect footprints at the moment
+    # NOTE: This will need re-thinking for evolving, non-self-similar models?
+    theta500s=np.unique(inputTab['theta500Arcmin'])
+    binEdges=np.linspace(inputTab['inFlux'].min(), inputTab['inFlux'].max(), 101)
+    binCentres=(binEdges[1:]+binEdges[:-1])/2
+    compThetaGrid=np.zeros((theta500s.shape[0], binCentres.shape[0]))
+    thetaQ=np.zeros(len(theta500s))
+    #thetaQ_05=np.zeros(len(theta500s))
+    #thetaQ_95=np.zeros(len(theta500s))
+    for i in range(len(theta500s)):
+        t=theta500s[i]
+        injMask=np.logical_and(injTab['theta500Arcmin'] == t, injTab['SNR'] > SNRCut)
+        inputMask=inputTab['theta500Arcmin'] == t
+        injFlux=injTab['inFlux'][injMask]
+        outFlux=injTab['outFlux'][injMask]
+        inputFlux=inputTab['inFlux'][inputMask]
+        recN, binEdges=np.histogram(injFlux, bins = binEdges)
+        inpN, binEdges=np.histogram(inputFlux, bins = binEdges)
+        valid=inpN > 0
+        compThetaGrid[i][valid]=recN[valid]/inpN[valid]
+        if len(outFlux) > 0:
+            thetaQ[i]=np.median(outFlux/injFlux)
+            #thetaQ_05[i]=np.percentile(outFlux/injFlux, 5)
+            #thetaQ_95[i]=np.percentile(outFlux/injFlux, 95)
+
+    return theta500s, binCentres, compThetaGrid, thetaQ
+
+#------------------------------------------------------------------------------------------------------------
 def loadAreaMask(tileName, selFnDir):
     """Loads the survey area mask, i.e., the area searched for sources and clusters, for the given tile.
     
     Args:
         tileName (:obj:`str`): The name of the tile for which the area mask will be loaded.
         selFnDir (:obj:`str`): Path to a ``selFn/`` directory, as produced by the :ref:`nemoCommand`
             command. This directory contains information such as the survey noise maps, area masks,
@@ -545,14 +701,34 @@
     
     """
     
     areaMap, wcs=_loadTile(tileName, selFnDir, "areaMask", extension = 'fits')   
     return areaMap, wcs
 
 #------------------------------------------------------------------------------------------------------------
+def loadFlagMask(tileName, selFnDir):
+    """Loads the flag mask, i.e., areas flagged for reasons such as point source subtraction, for the given
+    tile.
+
+    Args:
+        tileName (:obj:`str`): The name of the tile for which the flag mask will be loaded.
+        selFnDir (:obj:`str`): Path to a ``selFn/`` directory, as produced by the :ref:`nemoCommand`
+            command. This directory contains information such as the survey noise maps, area masks,
+            and information needed to construct the filter mismatch function, `Q`, used in mass
+            modeling.
+
+    Returns:
+        Map array (2d :obj:`np.ndarray`), WCS object (:obj:`astWCS.WCS`)
+
+    """
+
+    areaMap, wcs=_loadTile(tileName, selFnDir, "flagMask", extension = 'fits')
+    return areaMap, wcs
+
+#------------------------------------------------------------------------------------------------------------
 def loadRMSMap(tileName, selFnDir, photFilter):
     """Loads the RMS (noise) map for the given tile.
     
     Args:
         tileName (:obj:`str`): The name of the tile for which the RMS (noise) map will be loaded.
         selFnDir (:obj:`str`): Path to a ``selFn/`` directory, as produced by the :ref:`nemoCommand`
             command. This directory contains information such as the survey noise maps, area masks,
@@ -618,14 +794,17 @@
     Returns map array, wcs
     
     """
     
     # After tidyUp is run, this will be a MEF file... during first run, it won't be (written under MPI)
     if os.path.exists(baseDir+os.path.sep+"%s#%s.%s" % (baseFileName, tileName, extension)):
         fileName=baseDir+os.path.sep+"%s#%s.%s" % (baseFileName, tileName, extension)
+    elif os.path.exists(baseDir+os.path.sep+tileName+os.path.sep+"%s#%s.%s" % (baseFileName, tileName, extension)):
+        # Lustre-friendlier: each tile has its own directory
+        fileName=baseDir+os.path.sep+tileName+os.path.sep+"%s#%s.%s" % (baseFileName, tileName, extension)
     else:
         fileName=baseDir+os.path.sep+"%s.%s" % (baseFileName, extension)
     with pyfits.open(fileName) as img:
         # If we find the tile - great. If not, we use first extension with data as it'll be compressed
         if tileName in img:
             extName=tileName
             data=img[extName].data
@@ -701,15 +880,15 @@
     # After tidyUp has run, there will be intersection mask MEF files
     intersectFileName=selFnDir+os.path.sep+"intersect_%s.fits" % (label)
     if os.path.exists(intersectFileName):
         intersectMask, wcs=loadIntersectionMask(tileName, selFnDir, label)
         return intersectMask
     
     # Otherwise, we may have a per-tile intersection mask
-    intersectFileName=selFnDir+os.path.sep+"intersect_%s#%s.fits" % (label, tileName)
+    intersectFileName=selFnDir+os.path.sep+tileName+os.path.sep+"intersect_%s#%s.fits" % (label, tileName)
     if os.path.exists(intersectFileName):
         intersectMask, wcs=loadIntersectionMask(tileName, selFnDir, label)
         return intersectMask
 
     # Otherwise... make it
     areaMap, wcs=loadAreaMask(tileName, selFnDir)
     RAMin, RAMax, decMin, decMax=wcs.getImageMinMaxWCSCoords()
@@ -751,16 +930,16 @@
         xMask=np.logical_and(xIn >= 0, xIn < maskData.shape[1])
         yMask=np.logical_and(yIn >= 0, yIn < maskData.shape[0])
         xOut=np.arange(intersectMask.shape[1])
         yOut=np.arange(intersectMask.shape[0])
         for i in yOut[yMask]:
             intersectMask[i][xMask]=maskData[yIn[i], xIn[xMask]]
     intersectMask=np.array(np.greater(intersectMask, 0.5), dtype = int)
-    maps.saveFITS(intersectFileName, intersectMask, wcs, compressed = True, compressionType = 'PLIO_1')
-        
+    maps.saveFITS(intersectFileName, intersectMask*areaMap, wcs, compressionType = 'PLIO_1')
+
     return intersectMask
 
 #------------------------------------------------------------------------------------------------------------
 def getRMSTab(tileName, photFilterLabel, selFnDir, footprintLabel = None):
     """Makes a table containing map area in the tile refered to by `tileName` against RMS (noise level)
     values, compressing the information in the RMS maps. Results are cached under `selFnDir`, and read from
     disk if found.
@@ -784,51 +963,41 @@
     # After tidyUp has run, we may have one global RMS table with an extra tileName column we can use
     RMSTabFileName=selFnDir+os.path.sep+"RMSTab.fits"
     if footprintLabel is not None:
         RMSTabFileName=RMSTabFileName.replace(".fits", "_%s.fits" % (footprintLabel))
     if os.path.exists(RMSTabFileName):
         tab=atpy.Table().read(RMSTabFileName)
         return tab[np.where(tab['tileName'] == tileName)]
-    
-    # Otherwise, we may have a per-tile RMS table
-    RMSTabFileName=selFnDir+os.path.sep+"RMSTab_%s.fits" % (tileName)
-    if footprintLabel != None:
-        RMSTabFileName=RMSTabFileName.replace(".fits", "_%s.fits" % (footprintLabel))
-    if os.path.exists(RMSTabFileName) == True:
-        return atpy.Table().read(RMSTabFileName)
-    
+
     # Table doesn't exist, so make it...
-    print(("... making %s ..." % (RMSTabFileName)))
+    print(("... making RMS table for tile = %s, footprint = %s" % (tileName, footprintLabel)))
     RMSMap, wcs=loadRMSMap(tileName, selFnDir, photFilterLabel)
     areaMap, wcs=loadAreaMask(tileName, selFnDir)
     areaMapSqDeg=(maps.getPixelAreaArcmin2Map(areaMap.shape, wcs)*areaMap)/(60**2)
 
     if footprintLabel != None:  
         intersectMask=makeIntersectionMask(tileName, selFnDir, footprintLabel)
         areaMapSqDeg=areaMapSqDeg*intersectMask        
         RMSMap=RMSMap*intersectMask
 
     RMSValues=np.unique(RMSMap[np.nonzero(RMSMap)])
-
     totalAreaDeg2=areaMapSqDeg.sum()
-    
     tileArea=np.zeros(len(RMSValues))
     for i in range(len(RMSValues)):
         tileArea[i]=areaMapSqDeg[np.equal(RMSMap, RMSValues[i])].sum()
     RMSTab=atpy.Table()
     RMSTab.add_column(atpy.Column(tileArea, 'areaDeg2'))
     RMSTab.add_column(atpy.Column(RMSValues, 'y0RMS'))
     # Checks - these should be impossible but we have seen (e.g., when messed up masks)
     tol=0.003
     if abs(RMSTab['areaDeg2'].sum()-areaMapSqDeg.sum()) > tol:
         raise Exception("Mismatch between area map and area in RMSTab for tile '%s'" % (tileName))
     if np.less(RMSTab['areaDeg2'], 0).sum() > 0:
         raise Exception("Negative area in tile '%s' - check your survey mask (and delete/remake tileDir files if necessary)." % (tileName))
     RMSTab.meta['NEMOVER']=nemo.__version__
-    RMSTab.write(RMSTabFileName)
 
     return RMSTab
 
 #------------------------------------------------------------------------------------------------------------
 def downsampleRMSTab(RMSTab, stepSize = 0.001*1e-4):
     """Downsamples `RMSTab` (see :meth:`getRMSTab`) in terms of noise resolution, binning by `stepSize`.
     
@@ -884,79 +1053,76 @@
     RMSValues=np.array(RMSTab['y0RMS'])
     tileArea=np.array(RMSTab['areaDeg2'])
     tileRMSValue=np.average(RMSValues, weights = tileArea)
 
     return tileRMSValue
 
 #------------------------------------------------------------------------------------------------------------
-def completenessByFootprint(selFnCollection, mockSurvey, diagnosticsDir, additionalLabel = ""):
-    """Write out the average (log\ :sub:`10` mass, z) grid over all survey footprints provided in 
-    `selFnCollection`, weighted by fraction of total survey area within the footprint. Also prints some
-    useful statistics and produces some plots that are written to the `diagnosticsDir` directory.
+def completenessByFootprint(config):
+    """Write out the average (log\ :sub:`10` mass, z) grid over all survey footprints defined in the config,
+    weighted by fraction of total survey area within the footprint. Also prints some useful statistics and
+    produces some plots that are written to the `diagnosticsDir` directory.
     
     Args:
-        selFnCollection (:obj:`dict`): A dictionary where each key points to a :class:`SelFn` object that
-            describes a given survey footprint. Here, "full" corresponds to the whole survey, while "DES"
-            may represent the DES footprint, if it has been defined in the :ref:`nemoCommand` config file
-            (see :ref:`selFnFootprints`).
-        mockSurvey (:class:`nemo.MockSurvey.MockSurvey`): A :class:`MockSurvey` object, used for halo mass
-            function calculations and generating mock catalogs.
-        diagnosticsDir (:obj:`str`): The path to the diagnostics directory, where the output from this
-            routine will be written.
-        additionalLabel (:obj:`str`, optional): This will be added to the output filenames (use this for
-            e.g., tagging with the :meth:`calcCompleteness` method used).
+        config (:class:`nemo.startUp.NemoConfig`): A NemoConfig object.
     
     Returns:
         None
         
     Note:
         Output is written to files named e.g. ``diagnosticsDir/MzCompleteness_label.npz``, where `label`
         is the footprint name (i.e., a key in `selFnCollection`); 'full' is the default (survey-wide
         average).
     
     """
-        
+
     zBinEdges=np.arange(0.05, 2.1, 0.1)
     zBinCentres=(zBinEdges[:-1]+zBinEdges[1:])/2.
-        
-    for footprintLabel in selFnCollection.keys():
-        print(">>> Survey-averaged results inside footprint: %s ..." % (footprintLabel))
-        selFnDictList=selFnCollection[footprintLabel]
-        tileAreas=[]
-        compMzCube=[]
-        completeness=[]
-        for selFnDict in selFnDictList:
-            tileAreas.append(selFnDict['tileAreaDeg2'])
-            massLimit_90Complete=calcMassLimit(0.9, selFnDict['compMz'], mockSurvey, zBinEdges = zBinEdges)
-            completeness.append(massLimit_90Complete)
-            compMzCube.append(selFnDict['compMz'])
-        tileAreas=np.array(tileAreas)
-        completeness=np.array(completeness)
-        if np.sum(tileAreas) == 0:
-            print("... no overlapping area with %s ..." % (footprintLabel))
+
+    footprintLabels=[None]
+    if 'selFnFootprints' in config.parDict.keys():
+        for footprintDict in config.parDict['selFnFootprints']:
+            footprintLabels.append(footprintDict['label'])
+
+    for footprintLabel in footprintLabels:
+
+        try:
+            selFn=SelFn(config.selFnDir, config.parDict['selFnOptions']['fixedSNRCut'],
+                        footprint = footprintLabel, zStep = 0.1,
+                        enableDrawSample = False, downsampleRMS = False,
+                        applyRelativisticCorrection = config.parDict['massOptions']['relativisticCorrection'],
+                        delta = config.parDict['massOptions']['delta'],
+                        rhoType = config.parDict['massOptions']['rhoType'],
+                        method = config.parDict['selFnOptions']['method'],
+                        QSource = config.parDict['selFnOptions']['QSource'])
+        except FootprintError:
             continue
-        fracArea=tileAreas/np.sum(tileAreas)
-        compMzCube=np.array(compMzCube)
-        compMz_surveyAverage=np.average(compMzCube, axis = 0, weights = fracArea)
-
-        outFileName=diagnosticsDir+os.path.sep+"MzCompleteness_%s%s.npz" % (footprintLabel, additionalLabel)
-        np.savez(outFileName, z = mockSurvey.z, log10M500c = mockSurvey.log10M, 
-                 M500Completeness = compMz_surveyAverage)
-        
-        makeMzCompletenessPlot(compMz_surveyAverage, mockSurvey.log10M, mockSurvey.z, footprintLabel, 
-                               diagnosticsDir+os.path.sep+"MzCompleteness_%s%s.pdf" % (footprintLabel, additionalLabel))
+            #print("... no overlapping area with footprint %s" % (footprintLabel))
+
+        massLabel=selFn.mockSurvey.mdefLabel
+
+        if footprintLabel is None:
+            footprintLabel="full"
+
+        massLimit_90Complete=calcMassLimit(0.9, selFn.compMz, selFn.mockSurvey, zBinEdges = zBinEdges)
+        outFileName=config.diagnosticsDir+os.path.sep+"MzCompleteness_%s_%s.npz" % (selFn.method, footprintLabel)
+        np.savez(outFileName, z = selFn.mockSurvey.z, log10M = selFn.mockSurvey.log10M, completeness = selFn.compMz)
+        makeMzCompletenessPlot(selFn.compMz, selFn.mockSurvey.log10M, selFn.mockSurvey.z, footprintLabel, massLabel,
+                               config.diagnosticsDir+os.path.sep+"MzCompleteness_%s_%s.pdf" % (selFn.method, footprintLabel))
 
         # 90% mass completeness limit and plots
-        massLimit_90Complete=np.average(completeness, axis = 0, weights = fracArea)  # agrees with full mass limit map
-        makeMassLimitVRedshiftPlot(massLimit_90Complete, zBinCentres, diagnosticsDir+os.path.sep+"completeness90Percent_%s%s.pdf" % (footprintLabel, additionalLabel), title = "footprint: %s" % (footprintLabel))
+        makeMassLimitVRedshiftPlot(massLimit_90Complete, zBinCentres,
+                                   config.diagnosticsDir+os.path.sep+"completeness90Percent_%s_%s.pdf" % (selFn.method, footprintLabel),
+                                   title = "footprint: %s" % (footprintLabel))
         zMask=np.logical_and(zBinCentres >= 0.2, zBinCentres < 1.0)
         averageMassLimit_90Complete=np.average(massLimit_90Complete[zMask])
-        print("... total survey area (after masking) = %.1f sq deg" % (np.sum(tileAreas)))
-        print("... survey-averaged 90%% mass completeness limit (z = 0.5) = %.1f x 10^14 MSun" % (massLimit_90Complete[np.argmin(abs(zBinCentres-0.5))]))
-        print("... survey-averaged 90%% mass completeness limit (0.2 < z < 1.0) = %.1f x 10^14 MSun" % (averageMassLimit_90Complete))
+        print(">>> Survey-averaged results inside footprint %s:" % (footprintLabel))
+        print("... total survey area (after masking) = %.1f sq deg" % (selFn.totalAreaDeg2))
+        print("... survey-averaged 90%% mass (%s) completeness limit (z = 0.5) = %.1f x 10^14 MSun" % (massLabel, massLimit_90Complete[np.argmin(abs(zBinCentres-0.5))]))
+        print("... survey-averaged 90%% mass (%s) completeness limit (0.2 < z < 1.0) = %.1f x 10^14 MSun" % (massLabel, averageMassLimit_90Complete))
 
 #------------------------------------------------------------------------------------------------------------
 def calcCompletenessContour(compMz, log10M, z, level = 0.90):
     """Calculates a completeness contour on the (log\ :sub:`10` mass, z) plane.
     
     Args:
         compMz (:obj:`np.ndarray`): Map (2d array) of completeness on the (log\ :sub:`10` mass, z) plane.
@@ -994,23 +1160,24 @@
     cont_z=np.array(cont_z)
     cont_log10M=np.array(cont_log10M)
     #cont_log10M=ndimage.uniform_filter(cont_log10M, int(np.ceil(len(cont_log10M)/20)))
     
     return cont_z, cont_log10M
     
 #------------------------------------------------------------------------------------------------------------
-def makeMzCompletenessPlot(compMz, log10M, z, title, outFileName):
+def makeMzCompletenessPlot(compMz, log10M, z, title, massLabel, outFileName):
     """Makes a (log\ :sub:`10` mass, z) completeness plot.
     
     Args:
         compMz (:obj:`np.ndarray`): Map (2d array) of completeness on the (log\ :sub:`10` mass, z) plane.
         log10M (:obj:`np.ndarray`): One dimensional array of log\ :sub:`10` mass values corresponding to
             `compMz`.
         z (:obj:`np.ndarray`): One dimensional arra of redshifts corresponding to `compMz`.
         title (:obj:`str`): Title that will be written at the top of the plot.
+        massLabel (:obj:`str`): Label for mass quantity (e.g., "M200c").
         outFileName (:obj:`str`): Path where the plot will be written to a file, with the format being
             determined by the file extension.
     
     Returns:
         None
         
     """
@@ -1020,22 +1187,24 @@
     # Actual plot
     plotSettings.update_rcParams()
     fig, ax = plt.subplots(figsize=(9.5,6.5))
 
     plt.imshow((compMz*100).transpose(), cmap = colorcet.m_rainbow, origin = 'lower', aspect = 'auto')
     
     y_tck=interpolate.splrep(log10M, np.arange(log10M.shape[0]))
-    plot_log10M=np.linspace(13.5, 15.5, 9)
+    plot_log10M=np.linspace(13.8, 15.4, 9)
     coords_log10M=interpolate.splev(plot_log10M, y_tck)
     labels_log10M=[]
     for lm in plot_log10M:
         labels_log10M.append("%.2f" % (lm))
     plt.yticks(interpolate.splev(plot_log10M, y_tck), labels_log10M)
     plt.ylim(coords_log10M.min(), coords_log10M.max())
-    plt.ylabel("log$_{10}$ ($M_{\\rm 500c} / M_{\odot}$)")
+    if massLabel[0] == "M":
+        massLabel=massLabel[1:]
+    plt.ylabel("log$_{10}$ ($M_{\\rm %s} / M_{\odot}$)" % (massLabel))
     
     x_tck=interpolate.splrep(z, np.arange(z.shape[0]))
     plot_z=np.linspace(0.0, 2.0, 11)
     coords_z=interpolate.splev(plot_z, x_tck)
     labels_z=[]
     for lz in plot_z:
         labels_z.append("%.1f" % (lz))
@@ -1084,36 +1253,36 @@
         for i in range(len(zBinEdges)-1):
             binnedMassLimit[i]=np.average(massLimit[np.logical_and(mockSurvey.z > zBinEdges[i], mockSurvey.z <= zBinEdges[i+1])])
         massLimit=binnedMassLimit
     
     return massLimit
     
 #------------------------------------------------------------------------------------------------------------
-def calcCompleteness(RMSTab, SNRCut, tileName, mockSurvey, scalingRelationDict, QFit,
-                     plotFileName = None, z = None, method = "fast", numDraws = 2000000, numIterations = 100):
+def calcCompleteness(RMSTab, SNRCut, tileName, mockSurvey, massOptions, QFit, plotFileName = None, z = None,
+                     method = "fast", numDraws = 2000000, numIterations = 100, verbose = False):
     """Calculate completeness as a function of (log\ :sub:`10` mass, z) on the mockSurvey grid at the given
     `SNRCut`. Intrinsic scatter in the scaling relation is taken into account.
     
     Args:
         RMSTab (:obj:`astropy.table.Table`): Table containing noise level by area, as returned by
             :meth:`getRMSTab`.
         SNRCut (:obj:`float`): Completeness will be calculated for objects relative to this cut in 
             ``fixed_SNR``.
         tileName (:obj:`str`): Name of the map tile.
         mockSurvey (:class:`nemo.MockSurvey.MockSurvey`): A :class:`MockSurvey` object, used for halo mass
             function calculations and generating mock catalogs.
-        scalingRelationDict (:obj:`dict`): A dictionary of scaling relation parameters (see example Nemo
-            config files for the format).
+        massOptions (:obj:`dict`): A dictionary of scaling relation, cosmological, and mass definition
+            parameters (see example Nemo config files for the format).
         QFit (:class:`nemo.signals.QFit`): An object for calculating the filter mismatch function, referred
             to as `Q` in the ACT papers from `Hasselfield et al. (2013) <http://adsabs.harvard.edu/abs/2013JCAP...07..008H>`_
             onwards.
         plotFileName (:obj:`str`, optional): If given, write a plot showing 90% completness limit to this
             path.
-        z (:obj:`np.ndarray`, optional): Redshifts at which the completeness calculation will be performed.
-            Alternatively, a single redshift can be specified as a :obj:`float` instead.
+        z (:obj:`float`, optional): Redshift at which the completeness calculation will be performed.
+            If None, the redshift range will be taken from the :class:`MockSurvey` object.
         method (:obj:`str`, optional): Two methods for doing the calculation are available: "fast" (applies
             the measurement errors and scatter to 'true' ỹ\ :sub:`0` values on a grid) and "montecarlo" (uses
             samples drawn from a mock catalog, generated on the fly, to estimate the completeness). Both
             methods should give consistent results.
         numDraws (:obj:`int`, optional): Used by the "montecarlo" method - sets the number of draws from the
             halo mass function on each iteration.
         numIterations (:obj:`int`, optional): Used by the "montecarlo" method - sets the number of iterations,
@@ -1127,57 +1296,72 @@
     if z is not None:
         zIndex=np.argmin(abs(mockSurvey.z-z))
         zRange=mockSurvey.z[zIndex:zIndex+1]
     else:
         zRange=mockSurvey.z
 
     trueMassCol="true_M%d%s" % (mockSurvey.delta, mockSurvey.rhoType[0])
-    
+
+    if verbose == True:
+        print("... calcuating completeness in tile %s using '%s' method" % (tileName, method))
+
     if method == "montecarlo":
+
+        #t0=time.time()
         # Need area-weighted average noise in the tile - we could change this to use entire RMS map instead
         areaWeights=RMSTab['areaDeg2'].data/RMSTab['areaDeg2'].data.sum()
         if areaWeights.sum() > 0:
             y0Noise=np.average(RMSTab['y0RMS'].data, weights = areaWeights)
             # Monte-carlo sims approach: slow - but can use to verify the other approach below
             halfBinWidth=(mockSurvey.log10M[1]-mockSurvey.log10M[0])/2.0
             binEdges_log10M=(mockSurvey.log10M-halfBinWidth).tolist()+[np.max(mockSurvey.log10M)+halfBinWidth]
             halfBinWidth=(mockSurvey.z[1]-mockSurvey.z[0])/2.0
             binEdges_z=(zRange-halfBinWidth).tolist()+[np.max(zRange)+halfBinWidth]
             allMz=np.zeros([mockSurvey.clusterCount.shape[1], mockSurvey.clusterCount.shape[0]])
             detMz=np.zeros([mockSurvey.clusterCount.shape[1], mockSurvey.clusterCount.shape[0]])
             for i in range(numIterations):
-                tab=mockSurvey.drawSample(y0Noise, scalingRelationDict, QFit, tileName = tileName, 
-                                        SNRLimit = SNRCut, applySNRCut = False, z = z, numDraws = numDraws)
+                tab=mockSurvey.drawSample(y0Noise, massOptions, QFit, tileName = tileName,
+                                          SNRLimit = SNRCut, applySNRCut = False, z = z, numDraws = numDraws,
+                                          applyRelativisticCorrection = massOptions['relativisticCorrection'])
                 allMz=allMz+np.histogram2d(np.log10(tab[trueMassCol]*1e14), tab['redshift'], [binEdges_log10M, binEdges_z])[0]
                 detMask=np.greater(tab['fixed_y_c']*1e-4, y0Noise*SNRCut)
                 detMz=detMz+np.histogram2d(np.log10(tab[trueMassCol][detMask]*1e14), tab['redshift'][detMask], [binEdges_log10M, binEdges_z])[0]
             mask=np.not_equal(allMz, 0)
             compMz=np.ones(detMz.shape)
             compMz[mask]=detMz[mask]/allMz[mask]
             compMz=compMz.transpose()
         else:
             compMz=np.zeros([mockSurvey.clusterCount.shape[0], mockSurvey.clusterCount.shape[1]])
         #astImages.saveFITS("test_compMz_MC_5000.fits", compMz.transpose(), None)
+        #t1=time.time()
 
     elif method == "fast":
-        
+
         # Using full noise distribution, weighted by fraction of area
         # NOTE: removed recMassBias and div parameters
-        #t0=time.time()
-        tenToA0, B0, Mpivot, sigma_int=[scalingRelationDict['tenToA0'], scalingRelationDict['B0'], 
-                                        scalingRelationDict['Mpivot'], scalingRelationDict['sigma_int']]
+        tenToA0, B0, Mpivot, sigma_int=[massOptions['tenToA0'], massOptions['B0'],
+                                        massOptions['Mpivot'], massOptions['sigma_int']]
         y0Grid=np.zeros([zRange.shape[0], mockSurvey.clusterCount.shape[1]])
         for i in range(len(zRange)):
             zk=zRange[i]
             k=np.argmin(abs(mockSurvey.z-zk))
-            theta500s_zk=interpolate.splev(mockSurvey.log10M, mockSurvey.theta500Splines[k])
+            # WARNING: the interpolates for theta500, fRel in MockSurvey work in terms of M500c
+            # mockSurvey.log10M is NOT necessarily M500c any more
+            if massOptions['delta'] == 500 and massOptions['rhoType'] == "critical":
+                log10M500cs=mockSurvey.log10M
+            else:
+                log10M500cs=np.log10(mockSurvey.mdef.translate_mass(mockSurvey.cosmoModel, np.power(10, mockSurvey.log10M),
+                                                                    1/(1+zk), mockSurvey._M500cDef))
+
+            theta500s_zk=interpolate.splev(log10M500cs, mockSurvey.theta500Splines[k])
             Qs_zk=QFit.getQ(theta500s_zk, z = zk, tileName = tileName)
-            fRels_zk=interpolate.splev(mockSurvey.log10M, mockSurvey.fRelSplines[k])
-            true_y0s_zk=tenToA0*np.power(mockSurvey.Ez[k], 2)*np.power(np.power(10, mockSurvey.log10M)/Mpivot, 1+B0)*Qs_zk*fRels_zk
-            #true_y0s_zk=tenToA0*np.power(mockSurvey.Ez[k], 2)*np.power((recMassBias*np.power(10, mockSurvey.log10M))/Mpivot, 1+B0)*Qs_zk*fRels_zk
+            true_y0s_zk=tenToA0*np.power(mockSurvey.Ez[k], 2)*np.power(np.power(10, mockSurvey.log10M)/Mpivot, 1+B0)*Qs_zk
+            if massOptions['relativisticCorrection'] == True:
+                fRels_zk=interpolate.splev(log10M500cs, mockSurvey.fRelSplines[k])
+                true_y0s_zk=true_y0s_zk*fRels_zk
             y0Grid[i]=true_y0s_zk
             
         # For some cosmological parameters, we can still get the odd -ve y0
         y0Grid[y0Grid <= 0] = 1e-9
         
         # Calculate completeness using area-weighted average
         # NOTE: RMSTab that is fed in here can be downsampled in noise resolution for speed
@@ -1202,15 +1386,18 @@
         #projImg=pyfits.open("projMz_SNR%.2f.fits" % (SNRCut))        
         #projMz=projImg[0].data.transpose()
         #projImg.close()
         #merit=np.sum(np.sqrt(np.power(projMz-predMz, 2)))
         #print(merit)
         #IPython.embed()
         #sys.exit()
-            
+
+    elif method is None:
+        return None
+
     else:
         raise Exception("calcCompleteness only has 'fast', and 'Monte Carlo' methods available")
             
     if plotFileName is not None:
         # Calculate 90% completeness as function of z
         zBinEdges=np.arange(0.05, 2.1, 0.1)
         zBinCentres=(zBinEdges[:-1]+zBinEdges[1:])/2.
@@ -1220,66 +1407,168 @@
         makeMassLimitVRedshiftPlot(massLimit_90Complete, zBinCentres, plotFileName, 
                                    title = "%s: $M_{\\rm %d%s}$ / $10^{14}$ M$_{\odot}$ > %.2f (0.2 < $z$ < 1)" % (tileName,
                                    mockSurvey.delta, mockSurvey.rhoType[0], averageMassLimit_90Complete))
             
     return compMz
       
 #------------------------------------------------------------------------------------------------------------
-def makeMassLimitMap(SNRCut, z, tileName, photFilterLabel, mockSurvey, scalingRelationDict, QFit, 
-                     diagnosticsDir, selFnDir):
-    """Makes a map of 90% mass completeness (for now, this fraction is fixed and not adjustable). The map
-    is written as a FITS file in the `diagnosticsDir` directory.
+def makeMassLimitMapsAndPlots(config):
+    """Makes maps of mass completeness and associated plots. Output is written to the the `diagnosticsDir`
+    directory). The maps to make are controlled by the ``massLimitMaps`` parameter in the ``selFnOptions``
+    dictionary in the Nemo config file.
     
     Args:
-        SNRCut (:obj:`float`): Completeness will be calculated for objects relative to this cut in
-            ``fixed_SNR``.
-        z (:obj:`float`): The redshift at which the mass limit map will be produced.
-        tileName (:obj:`str`): The name of the tile.
-        photFilterLabel (:obj:`str`): Name of the reference filter, as specified in, e.g., a 
-            :ref:`nemoCommand` config file (see :ref:`ConfigReference`).
-        mockSurvey (:class:`nemo.MockSurvey.MockSurvey`): A :class:`MockSurvey` object, used for halo mass function 
-            calculations and generating mock catalogs.
-        scalingRelationDict (:obj:`dict`): A dictionary of scaling relation parameters (see example Nemo
-            config files for the format).
-        QFit (:class:`nemo.signals.QFit`): An object for calculating the filter mismatch function, referred
-            to as `Q` in the ACT papers from `Hasselfield et al. (2013) <http://adsabs.harvard.edu/abs/2013JCAP...07..008H>`_
-            onwards.
-        diagnosticsDir (:obj:`str`): Path to the ``diagnostics/`` directory, as produced by the 
-            :ref:`nemoCommand` command.
-        selFnDir (:obj:`str`): Path to a ``selFn/`` directory, as produced by the :ref:`nemoCommand`
-            command. This directory contains information such as the survey noise maps, area masks,
-            and information needed to construct the filter mismatch function, `Q`, used in mass
-            modeling.
+        config (:class:`nemo.startUp.NemoConfig`): A NemoConfig object.
+
+    Returns:
+        None
     
     """
-        
-    RMSMap, wcs=loadRMSMap(tileName, selFnDir, photFilterLabel)
-    RMSTab=getRMSTab(tileName, photFilterLabel, selFnDir)
-    
-    # Downsampling for speed? 
-    # If this is done, also need the bin edges and then need to modify code below accordingly
-    #RMSTab=downsampleRMSTab(RMSTab)
-    
+
+    selFn=SelFn(config.selFnDir, config.parDict['selFnOptions']['fixedSNRCut'],
+                footprint = None, zStep = 0.1, setUpAreaMask = True,
+                enableDrawSample = False, downsampleRMS = False,
+                applyRelativisticCorrection = config.parDict['massOptions']['relativisticCorrection'],
+                delta = config.parDict['massOptions']['delta'],
+                rhoType = config.parDict['massOptions']['rhoType'],
+                method = config.parDict['selFnOptions']['method'],
+                QSource = config.parDict['selFnOptions']['QSource'])
+
+    if config.parDict['stitchTiles'] == True:
+        inFileName=config.selFnDir+os.path.sep+"stitched_RMSMap_%s.fits" % (config.parDict['photFilter'])
+    else:
+        inFileName=config.selFnDir+os.path.sep+"RMSMap_%s.fits" % (config.parDict['photFilter'])
+
+    d, wcs=maps.chunkLoadMask(inFileName, dtype = np.float32)
+    noiseLevels=np.unique(d)
+    noiseLevels=noiseLevels[noiseLevels > 0]
+
+    y0Grid, theta500Grid=selFn._makeSignalGrids()
+
     # Fill in blocks in map for each RMS value
-    outFileName=diagnosticsDir+os.path.sep+tileName+os.path.sep+"massLimitMap_z%s#%s.fits" % (str(z).replace(".", "p"), tileName)
-    if os.path.exists(outFileName) == False:
-        massLimMap=np.zeros(RMSMap.shape)
-        count=0
+    for massLimDict in config.parDict['selFnOptions']['massLimitMaps']:
         t0=time.time()
-        for y0Noise in RMSTab['y0RMS']:
-            count=count+1
-            #print(("... %d/%d (%.3e) ..." % (count, len(RMSTab), y0Noise)))
-            compMz=calcCompleteness(RMSTab[np.where(RMSTab['y0RMS'] == y0Noise)], SNRCut, tileName, mockSurvey, 
-                                    scalingRelationDict, QFit, z = z)
-            massLimMap[RMSMap == y0Noise]=mockSurvey.log10M[np.argmin(abs(compMz-0.9))]
-        t1=time.time()
-        mask=np.not_equal(massLimMap, 0)
-        massLimMap[mask]=np.power(10, massLimMap[mask])/1e14
-        maps.saveFITS(outFileName, massLimMap, wcs, compressed = True)
-        
+        # Need re-bin here to make this run in sensible amount of time
+        if 'numBins' not in massLimDict.keys():
+            numBins=50
+        else:
+            numBins=massLimDict['numBins']
+        if 'completenessFraction' not in massLimDict.keys():
+            completenessFraction=0.9
+        else:
+            completenessFraction=massLimDict['completenessFraction']
+        binEdges=np.linspace(noiseLevels.min(), noiseLevels.max(), numBins+1)
+        binCentres=(binEdges[1:]+binEdges[:-1])/2
+        zIndex=np.argmin(abs(selFn.mockSurvey.z-massLimDict['z']))
+        z=selFn.mockSurvey.z[zIndex]
+        outFileName=config.diagnosticsDir+os.path.sep+"massLimitMap_z%.2f_comp%.2f.fits" % (z, completenessFraction)
+        if os.path.exists(outFileName) == True:
+            print("... already made mass limit map %s" % (outFileName))
+            massLimMap, wcs=maps.chunkLoadMask(outFileName, dtype = np.float32)
+        else:
+            massLimMap=np.zeros(d.shape)
+            count=0
+            t0=time.time()
+            for i in range(len(binEdges)-1):
+                binMin=binEdges[i]
+                binMax=binEdges[i+1]
+                mask=np.logical_and(d > binMin, d <= binMax)
+                print("... %d/%d" % (i+1, len(binCentres)))
+                # No intrinsic scatter
+                #sfi=stats.norm.sf(selFn.SNRCut*binCentres[i], loc = y0Grid, scale = binCentres[i])
+                # With intrinsic scatter [see fast method in selFn.update]
+                totalLogErr=np.sqrt((binCentres[i]/y0Grid)**2 + selFn.scalingRelationDict['sigma_int']**2)
+                sfi=stats.norm.sf(selFn.SNRCut*binCentres[i], loc = y0Grid, scale = totalLogErr*y0Grid)
+                massLimMap[mask]=selFn.mockSurvey.log10M[np.argmin(abs(sfi[zIndex]-0.9))]
+            t1=time.time()
+            mask=np.not_equal(massLimMap, 0)
+            massLimMap[mask]=np.power(10, massLimMap[mask])/1e14
+            maps.saveFITS(outFileName, massLimMap, wcs, compressionType = "RICE_1")
+            print("... made mass limit map '%s' (time taken = %.3f sec)" % (outFileName, t1-t0))
+        del d, y0Grid, theta500Grid, noiseLevels
+
+        # Plots
+        plotSettings.update_rcParams()
+
+        # Map plot [this is only set-up really for large area maps]
+        massLimMap=np.ma.masked_where(massLimMap <1e-6, massLimMap)
+        fontSize=20.0
+        figSize=(16, 5.7)
+        axesLabels="sexagesimal"
+        axes=[0.08,0.15,0.91,0.88]
+        cutLevels=[2, int(np.median(massLimMap[np.nonzero(massLimMap)]))+2]
+        colorMapName=colorcet.m_rainbow
+        fig=plt.figure(figsize = figSize)
+        p=astPlots.ImagePlot(massLimMap, wcs, cutLevels = cutLevels, title = None, axes = axes,
+                             axesLabels = axesLabels, colorMapName = colorMapName, axesFontFamily = 'sans-serif',
+                             RATickSteps = {'deg': 30.0, 'unit': 'h'}, decTickSteps = {'deg': 20.0, 'unit': 'd'},
+                             axesFontSize = fontSize)
+        cbLabel="$M_{\\rm %d%s}$ (10$^{14}$ M$_{\odot}$) [%d%% complete]" % (selFn.mockSurvey.delta, selFn.mockSurvey.rhoType[0], int(100*completenessFraction))
+        cbShrink=0.7
+        cbAspect=40
+        cb=plt.colorbar(p.axes.images[0], ax = p.axes, orientation="horizontal", fraction = 0.05, pad = 0.18,
+                        shrink = cbShrink, aspect = cbAspect)
+        plt.figtext(0.53, 0.04, cbLabel, ha="center", va="center", fontsize = fontSize, family = "sans-serif")
+        plt.savefig(outFileName.replace(".fits", ".pdf"), dpi = 300)
+        plt.savefig(outFileName.replace(".fits", ".png"), dpi = 300)
+        plt.close()
+        del p
+
+        # Cumulative area info [note, compression drives up number of 'mass limits', so we rebin]
+        pixAreaMap=maps.getPixelAreaArcmin2Map(massLimMap.shape, wcs)
+        limits=np.unique(massLimMap)
+        limits=limits[limits > 0]
+        binEdges=np.linspace(limits.min(), limits.max(), 50)
+        binCentres=(binEdges[1:]+binEdges[:-1])/2
+        areas=[]
+        for i in range(len(binEdges)-1):
+            binMin=binEdges[i]
+            binMax=binEdges[i+1]
+            mask=np.logical_and(massLimMap > binMin, massLimMap <= binMax)
+            areas.append(pixAreaMap[mask].sum())
+        tab=atpy.Table()
+        tab['MLim']=binCentres
+        tab['areaDeg2']=areas
+        tab['areaDeg2']=tab['areaDeg2']/(60**2)
+        tab.sort('MLim')
+        del pixAreaMap, massLimMap, limits
+
+        # Full survey cumulative area plot
+        plt.figure(figsize=(9,6.5))
+        ax=plt.axes([0.155, 0.12, 0.82, 0.86])
+        plt.minorticks_on()
+        plt.plot(tab['MLim'], np.cumsum(tab['areaDeg2']), 'k-')
+        #plt.plot(plotMRange, plotCumArea, 'k-')
+        plt.ylabel("survey area < $M_{\\rm %d%s}$ limit (deg$^2$)" % (selFn.mockSurvey.delta, selFn.mockSurvey.rhoType[0]))
+        plt.xlabel("$M_{\\rm %d%s}$ (10$^{14}$ M$_{\odot}$) [%d%% complete]" % (selFn.mockSurvey.delta, selFn.mockSurvey.rhoType[0], int(100*completenessFraction)))
+        labelStr="total survey area = %.0f deg$^2$" % (np.cumsum(tab['areaDeg2']).max())
+        plt.ylim(0.0, 1.2*np.cumsum(tab['areaDeg2']).max())
+        plt.xlim(tab['MLim'].min(), tab['MLim'].max())
+        plt.figtext(0.2, 0.9, labelStr, ha="left", va="center")
+        plt.savefig(config.diagnosticsDir+os.path.sep+"cumulativeArea_massLimit_z%.2f_comp%.2f.pdf" % (z, completenessFraction))
+        plt.savefig(config.diagnosticsDir+os.path.sep+"cumulativeArea_massLimit_z%.2f_comp%.2f.png" % (z, completenessFraction))
+        plt.close()
+
+        # Deepest 20% cumulative area plot - we show a bit beyond this
+        totalAreaDeg2=tab['areaDeg2'].sum()
+        deepTab=tab[np.where(np.cumsum(tab['areaDeg2']) < 0.25 * totalAreaDeg2)]
+        plt.figure(figsize=(9,6.5))
+        ax=plt.axes([0.155, 0.12, 0.82, 0.86])
+        plt.minorticks_on()
+        plt.plot(tab['MLim'], np.cumsum(tab['areaDeg2']), 'k-')
+        plt.ylabel("survey area < $M_{\\rm %d%s}$ limit (deg$^2$)" % (selFn.mockSurvey.delta, selFn.mockSurvey.rhoType[0]))
+        plt.xlabel("$M_{\\rm %d%s}$ (10$^{14}$ M$_{\odot}$) [%d%% complete]" % (selFn.mockSurvey.delta, selFn.mockSurvey.rhoType[0], int(100*completenessFraction)))
+        labelStr="area of deepest 20%% = %.0f deg$^2$" % (0.2 * totalAreaDeg2)
+        plt.ylim(0.0, 1.2*np.cumsum(deepTab['areaDeg2']).max())
+        plt.xlim(deepTab['MLim'].min(), deepTab['MLim'].max())
+        plt.figtext(0.2, 0.9, labelStr, ha="left", va="center")
+        plt.savefig(config.diagnosticsDir+os.path.sep+"cumulativeArea_massLimit_z%.2f_comp%.2f_deepest20percent.pdf" % (z, completenessFraction))
+        plt.savefig(config.diagnosticsDir+os.path.sep+"cumulativeArea_massLimit_z%.2f_comp%.2f_deepest20percent.png" % (z, completenessFraction))
+        plt.close()
+
 #------------------------------------------------------------------------------------------------------------
 def makeMassLimitVRedshiftPlot(massLimit_90Complete, zRange, outFileName, title = None):
     """Makes a plot of 90%-completeness mass limit versus redshift. Uses spline interpolation.
     
     Args:
         massLimit_90Complete (:obj:`np.ndarray`): Mass limit at each redshift, corresponding to 90%
             completeness.
@@ -1309,103 +1598,14 @@
     labelStr="$M_{\\rm 500c}$ (10$^{14}$ M$_{\odot}$) [90% complete]"
     plt.ylabel(labelStr)
     plt.savefig(outFileName)
     if outFileName.find(".pdf") != -1:
         plt.savefig(outFileName.replace(".pdf", ".png"))
     plt.close()   
     
-#------------------------------------------------------------------------------------------------------------
-def cumulativeAreaMassLimitPlot(z, diagnosticsDir, selFnDir, tileNames):
-    """Makes cumulative plots of the 90%-completeness mass limit versus survey area, at the given redshift.
-    
-    Args:
-        z (:obj:`float`): The redshift at which the mass completeness is evaluated.
-        diagnosticsDir (:obj:`str`): Path to the ``diagnostics/`` directory, as produced by the 
-            :ref:`nemoCommand` command.
-        selFnDir (:obj:`str`): Path to a ``selFn/`` directory, as produced by the :ref:`nemoCommand`
-            command. This directory contains information such as the survey noise maps, area masks,
-            and information needed to construct the filter mismatch function, `Q`, used in mass
-            modeling.
-        tileNames (:obj:`list`): List of tiles to use.
-    
-    Note:
-        This routine writes plots into the `diagnosticsDir` directory (one for the cumulative mass
-        completeness limit over the whole survey area, and one for the deepest 20% only).
-    
-    Returns:
-        None
-        
-    """
-        
-    # NOTE: We truncate mass limits to 0.1 level here - differences beyond that are due to compression
-    allLimits=[]
-    allAreas=[]
-    for tileName in tileNames:
-        massLimMap, wcs=loadMassLimitMap(tileName, diagnosticsDir+os.path.sep+tileName, z)
-        areaMap, wcs=loadAreaMask(tileName, selFnDir)
-        areaMapSqDeg=(maps.getPixelAreaArcmin2Map(areaMap.shape, wcs)*areaMap)/(60**2)
-        limits=np.unique(massLimMap).tolist()
-        if limits[0] == 0:
-            limits=limits[1:]
-        areas=[]
-        truncLim=[]
-        for l in limits:
-            truncLim.append(round(l, 1))
-            #truncLim.append(float(Decimal(l).quantize(Decimal('0.1'))))
-            areas.append(areaMapSqDeg[np.where(massLimMap == l)].sum())
-        allLimits=allLimits+truncLim
-        allAreas=allAreas+areas
-    
-    # Reduce redundant mass limits
-    allLimits=np.array(allLimits)
-    allAreas=np.array(allAreas)
-    uniqLimits=np.unique(allLimits)
-    uniqAreas=[]
-    for u in uniqLimits:
-        uniqAreas.append(allAreas[allLimits == u].sum())
-    uniqAreas=np.array(uniqAreas)
-    tab=atpy.Table()
-    tab.add_column(atpy.Column(uniqLimits, 'MLim'))
-    tab.add_column(atpy.Column(uniqAreas, 'areaDeg2'))
-    tab.sort('MLim')
-        
-    plotSettings.update_rcParams()
-        
-    # Full survey plot
-    plt.figure(figsize=(9,6.5))
-    ax=plt.axes([0.155, 0.12, 0.82, 0.86])
-    plt.minorticks_on()
-    plt.plot(tab['MLim'], np.cumsum(tab['areaDeg2']), 'k-')
-    #plt.plot(plotMRange, plotCumArea, 'k-')
-    plt.ylabel("survey area < $M_{\\rm 500c}$ limit (deg$^2$)")
-    plt.xlabel("$M_{\\rm 500c}$ (10$^{14}$ M$_{\odot}$) [90% complete]")
-    labelStr="total survey area = %.0f deg$^2$" % (np.cumsum(tab['areaDeg2']).max())
-    plt.ylim(0.0, 1.2*np.cumsum(tab['areaDeg2']).max())
-    plt.xlim(tab['MLim'].min(), tab['MLim'].max())
-    plt.figtext(0.2, 0.9, labelStr, ha="left", va="center")
-    plt.savefig(diagnosticsDir+os.path.sep+"cumulativeArea_massLimit_z%s.pdf" % (str(z).replace(".", "p")))
-    plt.savefig(diagnosticsDir+os.path.sep+"cumulativeArea_massLimit_z%s.png" % (str(z).replace(".", "p")))
-    plt.close()
-    
-    # Deepest 20% - we show a bit beyond this
-    totalAreaDeg2=tab['areaDeg2'].sum()
-    deepTab=tab[np.where(np.cumsum(tab['areaDeg2']) < 0.25 * totalAreaDeg2)]
-    plt.figure(figsize=(9,6.5))
-    ax=plt.axes([0.155, 0.12, 0.82, 0.86])
-    plt.minorticks_on()
-    plt.plot(tab['MLim'], np.cumsum(tab['areaDeg2']), 'k-')
-    plt.ylabel("survey area < $M_{\\rm 500c}$ limit (deg$^2$)")
-    plt.xlabel("$M_{\\rm 500c}$ (10$^{14}$ M$_{\odot}$) [90% complete]")
-    labelStr="area of deepest 20%% = %.0f deg$^2$" % (0.2 * totalAreaDeg2)
-    plt.ylim(0.0, 1.2*np.cumsum(deepTab['areaDeg2']).max())
-    plt.xlim(deepTab['MLim'].min(), deepTab['MLim'].max())
-    plt.figtext(0.2, 0.9, labelStr, ha="left", va="center")
-    plt.savefig(diagnosticsDir+os.path.sep+"cumulativeArea_massLimit_z%s_deepest20Percent.pdf" % (str(z).replace(".", "p")))
-    plt.savefig(diagnosticsDir+os.path.sep+"cumulativeArea_massLimit_z%s_deepest20Percent.png" % (str(z).replace(".", "p")))
-    plt.close()
         
 #------------------------------------------------------------------------------------------------------------
 def makeFullSurveyMassLimitMapPlot(z, config):
     """Makes full area mass limit map by reprojecting the tile mass limit maps onto the full map pixelisation.
     Creates both a plot and a FITS image.
     
     Args:
@@ -1450,15 +1650,15 @@
                                 RATickSteps = {'deg': 30.0, 'unit': 'h'}, decTickSteps = {'deg': 20.0, 'unit': 'd'},
                                 axesFontSize = fontSize)
             cbLabel="$M_{\\rm 500c}$ (10$^{14}$ M$_{\odot}$) [90% complete]"
             cbShrink=0.7
             cbAspect=40
             cb=plt.colorbar(p.axes.images[0], ax = p.axes, orientation="horizontal", fraction = 0.05, pad = 0.18, 
                             shrink = cbShrink, aspect = cbAspect)
-            plt.figtext(0.53, 0.04, cbLabel, size = 20, ha="center", va="center", fontsize = fontSize, family = "sans-serif")
+            plt.figtext(0.53, 0.04, cbLabel, ha="center", va="center", fontsize = fontSize, family = "sans-serif")
             plt.savefig(outFileName.replace(".fits", ".pdf"), dpi = 300)
             plt.savefig(outFileName.replace(".fits", ".png"), dpi = 300)
             plt.close()
 
 #------------------------------------------------------------------------------------------------------------
 def tidyUp(config):
     """Tidies up the `selFn` directory, constructing multi-extension FITS files from individual tile images
@@ -1472,85 +1672,52 @@
     Returns:
         None
     
     """
     
     shutil.copy(config.configFileName, config.selFnDir+os.path.sep+"config.yml")
 
-    # Delete single tile Q fits (combined Q file should be made before this)
-    if 'photFilter' in config.parDict.keys() and config.parDict['photFilter'] is not None and config.parDict['fitQ'] == True:
-        #signals.makeCombinedQTable(config)
-        for tileName in config.allTileNames:
-            QFileName=config.selFnDir+os.path.sep+"QFit#%s.fits" % (tileName)
-            if os.path.exists(QFileName):
-                os.remove(QFileName)
-    
     # Make MEFs
-    MEFsToBuild=["areaMask", "RMSMap_%s" % (config.parDict['photFilter'])]
-    compressionTypes=["PLIO_1", "RICE_1"]
-    dtypes=[np.int32, np.float]
+    MEFsToBuild=["RMSMap_%s" % (config.parDict['photFilter'])]
+    compressionTypes=["RICE_1"]
+    dtypes=[np.float32]
     if 'selFnFootprints' in config.parDict.keys():
         for footprintDict in config.parDict['selFnFootprints']:
             MEFsToBuild.append("intersect_%s" % footprintDict['label'])
             compressionTypes.append("PLIO_1")
-            dtypes.append(np.int32)
+            dtypes.append(np.uint8)
+    assert(len(MEFsToBuild) == len(compressionTypes))
+    assert(len(MEFsToBuild) == len(dtypes))
     for MEFBaseName, compressionType, dtype in zip(MEFsToBuild, compressionTypes, dtypes):
         outFileName=config.selFnDir+os.path.sep+MEFBaseName+".fits"
         newImg=pyfits.HDUList()
         filesToRemove=[]
         for tileName in config.allTileNames:
-            fileName=config.selFnDir+os.path.sep+MEFBaseName+"#"+tileName+".fits"
+            fileName=config.selFnDir+os.path.sep+tileName+os.path.sep+MEFBaseName+"#"+tileName+".fits"
             if os.path.exists(fileName):
                 with pyfits.open(fileName) as img:
                     for extName in img:
                         if img[extName].data is not None:
                             break
                     hdu=pyfits.CompImageHDU(np.array(img[extName].data, dtype = dtype), img[extName].header, 
                                             name = tileName, compression_type = compressionType)
                 filesToRemove.append(fileName)
                 newImg.append(hdu)
         if len(newImg) > 0:
             newImg.writeto(outFileName, overwrite = True)
             for f in filesToRemove:
                 os.remove(f)
-            
-    # Combine RMSTab files (we can downsample further later if needed)
-    # We add a column for the tileName just in case want to select on this later
-    footprints=['']
-    if 'selFnFootprints' in config.parDict.keys():
-        for footprintDict in config.parDict['selFnFootprints']:
-            footprints.append(footprintDict['label'])
-    strLen=0
-    for tileName in config.allTileNames:
-        if len(tileName) > strLen:
-            strLen=len(tileName)
-    for footprint in footprints:
-        if footprint != "":
-            label="_"+footprint
-        else:
-            label=""
-        outFileName=config.selFnDir+os.path.sep+"RMSTab"+label+".fits"
-        tabList=[]
-        filesToRemove=[]
-        for tileName in config.allTileNames:
-            fileName=config.selFnDir+os.path.sep+"RMSTab_"+tileName+label+".fits"
-            if os.path.exists(fileName):
-                tileTab=atpy.Table().read(fileName)
-                tileTab.add_column(atpy.Column(np.array([tileName]*len(tileTab), dtype = '<U%d' % (strLen)), 
-                                               "tileName"))
-                tabList.append(tileTab)
-                filesToRemove.append(fileName)
-        if len(tabList) > 0:
-            tab=atpy.vstack(tabList)
-            tab.sort('y0RMS')
-            tab.meta['NEMOVER']=nemo.__version__
-            tab.write(outFileName, overwrite = True)
-            for f in filesToRemove:
-                os.remove(f)
-    
+
     # Write a table of tile areas for those that want it
     with open(config.selFnDir+os.path.sep+"tileAreas.txt", "w") as outFile:
         outFile.write("#tileName areaDeg2\n")
         for tileName in config.allTileNames:
             tileAreaDeg2=getTileTotalAreaDeg2(tileName, config.selFnDir)
             outFile.write("%s %.6f\n" % (tileName, tileAreaDeg2))
+
+    # Clean out any per-tile directories
+    for tileName in config.allTileNames:
+        if os.path.exists(config.selFnDir+os.path.sep+tileName) == True:
+            shutil.rmtree(config.selFnDir+os.path.sep+tileName)
+
+
```

### Comparing `nemo-sz-0.5.0/nemo/data/planck_lensedCls.dat` & `nemo-sz-0.6.0/nemo/data/planck_lensedCls.dat`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/nemo/filters.py` & `nemo-sz-0.6.0/nemo/filters.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,107 +32,78 @@
 from scipy import ndimage
 import astropy.io.fits as pyfits
 import astropy.stats as apyStats
 import copy
 import sys
 import glob
 import itertools
-import pyximport; pyximport.install()
-import nemoCython
 import nemo
 from . import maps
 from . import signals
 from . import photometry
 from . import catalogs
 from . import plotSettings
 from . import gnfw
 from . import completeness
 import astropy.table as atpy
 import time
 
 #-------------------------------------------------------------------------------------------------------------
-def filterMaps(unfilteredMapsDictList, filterParams, tileName, filteredMapsDir = '.', diagnosticsDir = '.', 
-               selFnDir = '.', verbose = True, undoPixelWindow = True, useCachedMaps = True,
+def filterMaps(unfilteredMapsDictList, filterParams, tileName, diagnosticsDir = '.', \
+               selFnDir = '.', verbose = True, undoPixelWindow = True, useCachedFilter = False, \
                returnFilter = False):
     """Builds and applies filters to the unfiltered map(s). 
     
     Args:
         unfilteredMapsDictList (:obj:`list`): A list of dictionaries, each of which describes a map of the sky
             at some frequency (see :ref:`InputMaps`).
         filterParams (:obj:`dict`): A dictionary containing filter settings (see :ref:`Filters`).
         tileName (:obj:`str`): The name of the tile.
-        filteredMapsDir (:obj:`str`, optional): The path to the directory where the filtered maps may be written.
         diagnosticsDir (:obj:`str`, optional): Path to the `diagnostics` directory, where the filters may be
             written to disk.
         selFnDir (:obj:`str`, optional): Path to the `selFn` directory, where area masks may be written.
         verbose (:obj:`bool`, optional): If True, write information about progress to the terminal.
         undoPixelWindow (:obj:`bool`, optional): If True, undo the pixel window effect on the output filtered
             maps.
-        useCachedMaps (:obj:`bool`, optional): If True, and previously made maps are found, these will be
-            read from disk, rather than re-calculating and re-applying the filter.
+        useCachedFilter (:obj:`bool`, optional): If True, and a previously made filter is found, it will be
+            read from disk, rather than re-calculated (used by source injection simulations).
         returnFilter (:obj:`bool`, optional): If True, the filter object is returned, as well as a dictionary
             containing the filtered map.
     
     Returns:
         A dictionary containing the filtered map in signal units, a signal-to-noise-map, area mask, WCS, and
         a label (for housekeeping).
     
     """
         
     f=filterParams
     label=f['label']+"#"+tileName
-    filteredMapFileName=filteredMapsDir+os.path.sep+"%s_filteredMap.fits"  % (label)
-    SNMapFileName=filteredMapsDir+os.path.sep+"%s_SNMap.fits" % (label)
-    if os.path.exists(filteredMapFileName) == False or useCachedMaps == False:
-        
-        print("... making filtered map %s ..." % (label))
-        filterClass=eval('%s' % (f['class']))
-        filterObj=filterClass(f['label'], unfilteredMapsDictList, f['params'], tileName = tileName, 
-                              diagnosticsDir = diagnosticsDir, selFnDir = selFnDir)
-        filteredMapDict=filterObj.buildAndApply()
-            
-        # Keywords we need for photometry later
-        filteredMapDict['wcs'].header['BUNIT']=filteredMapDict['mapUnits']
-        if 'beamSolidAngle_nsr' in filteredMapDict.keys() and filteredMapDict['beamSolidAngle_nsr'] > 0:
-            filteredMapDict['wcs'].header['BEAMNSR']=filteredMapDict['beamSolidAngle_nsr']
-            filteredMapDict['wcs'].header['FREQGHZ']=filteredMapDict['obsFreqGHz']
-        filteredMapDict['wcs'].updateFromHeader()
-                                    
-        # Undo pixel window function using Sigurd's FFT method (takes into account variable pixel scale etc.)
-        # We only need to do this for maps of signal (cancels in S/N map)
-        # We do this once because it does take some time... 
-        # ... and then we can forget about if e.g. stacking or doing forced photometry later
-        if undoPixelWindow == True:
-            mask=np.equal(filteredMapDict['data'], 0)
-            filteredMapDict['data']=enmap.apply_window(filteredMapDict['data'], pow=-1.0)
-            filteredMapDict['data'][mask]=0 # just in case we rely elsewhere on zero == no data
-
-        if 'saveFilteredMaps' in filterObj.params and filterObj.params['saveFilteredMaps'] == True:
-            maps.saveFITS(filteredMapFileName, filteredMapDict['data'], filteredMapDict['wcs'])
-            maps.saveFITS(SNMapFileName, filteredMapDict['SNMap'], filteredMapDict['wcs'])            
-        # Uncomment for quicker testing/re-runs...
-        #astImages.saveFITS(filteredMapFileName, filteredMapDict['data'], filteredMapDict['wcs'])
-        #astImages.saveFITS(SNMapFileName, filteredMapDict['SNMap'], filteredMapDict['wcs'])   
-
-    else:
-        print("... loading cached map %s ..." % (filteredMapFileName))
-        filteredMapDict={}
-        with pyfits.open(filteredMapFileName) as img:
-            filteredMapDict['data']=img[0].data
-            filteredMapDict['wcs']=astWCS.WCS(img[0].header, mode = 'pyfits')
-            filteredMapDict['mapUnits']=filteredMapDict['wcs'].header['BUNIT']
-            if 'BEAMNSR' in filteredMapDict['wcs'].header.keys():
-                filteredMapDict['beamSolidAngle_nsr']=filteredMapDict['wcs'].header['BEAMNSR']
-                filteredMapDict['obsFreqGHz']=filteredMapDict['wcs'].header['FREQGHZ']
-        with pyfits.open(SNMapFileName) as img:
-            filteredMapDict['SNMap']=img[0].data
-        filteredMapDict['surveyMask'], wcs=completeness.loadAreaMask(tileName, selFnDir)
-        filteredMapDict['label']=f['label']
-        filteredMapDict['tileName']=tileName
-    
+        
+    print("... making filtered map %s" % (label))
+    filterClass=eval('%s' % (f['class']))
+    filterObj=filterClass(f['label'], unfilteredMapsDictList, f['params'], tileName = tileName,
+                            diagnosticsDir = diagnosticsDir, selFnDir = selFnDir)
+    filteredMapDict=filterObj.buildAndApply(useCachedFilter = useCachedFilter)
+
+    # Keywords we need for photometry later
+    filteredMapDict['wcs'].header['BUNIT']=filteredMapDict['mapUnits']
+    if 'beamSolidAngle_nsr' in filteredMapDict.keys() and filteredMapDict['beamSolidAngle_nsr'] > 0:
+        filteredMapDict['wcs'].header['BEAMNSR']=filteredMapDict['beamSolidAngle_nsr']
+        filteredMapDict['wcs'].header['FREQGHZ']=filteredMapDict['obsFreqGHz']
+    filteredMapDict['wcs'].updateFromHeader()
+
+    # Undo pixel window function using Sigurd's FFT method (takes into account variable pixel scale etc.)
+    # We only need to do this for maps of signal (cancels in S/N map)
+    # We do this once because it does take some time...
+    # ... and then we can forget about if e.g. stacking or doing forced photometry later
+    if undoPixelWindow == True:
+        mask=np.equal(filteredMapDict['data'], 0)
+        filteredMapDict['data']=enmap.apply_window(filteredMapDict['data'], pow=-1.0)
+        filteredMapDict['data'][mask]=0 # just in case we rely elsewhere on zero == no data
+
     if returnFilter == True:
         return filteredMapDict, filterObj
     
     return filteredMapDict
     
 #------------------------------------------------------------------------------------------------------------
 class MapFilter(object):
@@ -173,25 +144,33 @@
         
         self.label=label
         self.params=paramsDict
         
         self.diagnosticsDir=diagnosticsDir
         self.selFnDir=selFnDir
         self.tileName=tileName
-        self.filterFileName=self.diagnosticsDir+os.path.sep+"filter_%s#%s.fits" % (self.label, self.tileName)
+        self.filterFileName=self.diagnosticsDir+os.path.sep+self.tileName+os.path.sep+"filter_%s#%s.fits" % (self.label, self.tileName)
         
         # Prepare all the unfilteredMaps (in terms of cutting sections, masks etc.)
-        # NOTE: we're now copying the input unfilteredMapsDictList, for supporting multi-ext tileDir files
+        # NOTE: This is a copy to deal with repeated runs (yes, it's necessary)
         self.unfilteredMapsDictList=[]
-        for mapDict in unfilteredMapsDictList:           
-            mapDict=maps.preprocessMapDict(mapDict.copy(), tileName = tileName, diagnosticsDir = diagnosticsDir)
-            self.unfilteredMapsDictList.append(mapDict)
-        self.wcs=mapDict['wcs']
-        self.shape=mapDict['data'].shape
-                                
+        for mapDict in unfilteredMapsDictList:
+            if 'mapToUse' in self.params.keys() and mapDict['label'] != self.params['mapToUse']:
+                continue
+            newMapDict=mapDict.copy()
+            newMapDict.preprocess(tileName = tileName, diagnosticsDir = diagnosticsDir)
+            self.unfilteredMapsDictList.append(newMapDict)
+        self.wcs=self.unfilteredMapsDictList[0]['wcs']
+        self.shape=self.unfilteredMapsDictList[0]['data'].shape
+
+        # Combine flag masks (yes, we may need to think about this more...)
+        self.flagMask=np.zeros(self.shape, dtype = int)
+        for mapDict, i in zip(self.unfilteredMapsDictList, range(len(self.unfilteredMapsDictList))):
+            self.flagMask=self.flagMask+(mapDict['flagMask']*(i+1))
+
         # Get beam solid angle info (units: nanosteradians)... we'll need for fluxes in Jy later
         self.beamSolidAnglesDict={}
         for mapDict in self.unfilteredMapsDictList:    
             if 'solidAngle_nsr' in mapDict.keys():
                 solidAngle_nsr=mapDict['solidAngle_nsr']
             else:
                 beamFileName=mapDict['beamFileName']
@@ -211,15 +190,15 @@
         
         # For pixell / enmap
         self.enwcs=self.wcs.AWCS
 
         # We could make this adjustable... added after switch to pixell
         self.apodPix=20
         
-        # Sanity check that all maps are the same dimensions
+        # Check that all maps are the same dimensions
         shape=self.unfilteredMapsDictList[0]['data'].shape
         for mapDict in self.unfilteredMapsDictList:
             if mapDict['data'].shape != shape:
                 raise Exception("Maps at different frequencies have different dimensions!")
         
         # This is used by routines that make signal templates
         self.makeRadiansMap()
@@ -421,19 +400,25 @@
                                 chunkRMS=np.std(chunkValues[mask])
                     else:
                         chunkRMS=0.
                 if chunkRMS > 0:
                     RMSMap[weightMask]=chunkRMS
 
         # The grid method now recognises numNoiseBins in cells
-        else:  
-            gridSize=int(round((self.params['noiseParams']['noiseGridArcmin']/60.)/self.wcs.getPixelSizeDeg()))
-            overlapPix=int(gridSize/2)
-            numXChunks=mapData.shape[1]/gridSize
-            numYChunks=mapData.shape[0]/gridSize
+        else:
+            # We may want to just bin and not grid
+            if 'noiseGridArcmin' not in self.params['noiseParams'].keys() or self.params['noiseParams']['noiseGridArcmin'] is None:
+                overlapPix=0
+                numXChunks=1
+                numYChunks=1
+            else: # The usual gridding
+                gridSize=int(round((self.params['noiseParams']['noiseGridArcmin']/60.)/self.wcs.getPixelSizeDeg()))
+                overlapPix=int(gridSize/2)
+                numXChunks=mapData.shape[1]/gridSize
+                numYChunks=mapData.shape[0]/gridSize
             yChunks=np.linspace(0, mapData.shape[0], int(numYChunks+1), dtype = int)
             xChunks=np.linspace(0, mapData.shape[1], int(numXChunks+1), dtype = int)
             apodMask=np.not_equal(mapData, 0)
             RMSMap=np.zeros(mapData.shape)
             # For this mode, interpreted as number of noise bins per cell
             if 'numNoiseBins' in self.params['noiseParams'].keys():
                 numBins=self.params['noiseParams']['numNoiseBins']
@@ -529,57 +514,52 @@
         
 #------------------------------------------------------------------------------------------------------------
 class MatchedFilter(MapFilter):
     """A multi-frequency matched filter, implemented in Fourier space. Derived from :class:`MapFilter`.
     
     """
 
-    def buildAndApply(self):
+    def buildAndApply(self, useCachedFilter = False):
         
         fMapsToFilter=[]
         for mapDict in self.unfilteredMapsDictList:
             fMapsToFilter.append(enmap.fft(enmap.apod(mapDict['data'], self.apodPix)))
         fMapsToFilter=np.array(fMapsToFilter)
         
         # NOTE: We've tidied up the config file, so we don't have to feed in surveyMask and psMask like this
         # (see startUp.parseConfig)
         surveyMask=self.unfilteredMapsDictList[0]['surveyMask']
-        psMask=self.unfilteredMapsDictList[0]['psMask']
-            
-        if os.path.exists(self.filterFileName) == False:
-                        
+        psMask=self.unfilteredMapsDictList[0]['pointSourceMask']
+
+        if os.path.exists(self.filterFileName) == False and useCachedFilter == False:
+
             fMapsForNoise=[]
             for i in range(len(self.unfilteredMapsDictList)):
                 mapDict=self.unfilteredMapsDictList[i]
                 d=mapDict['data']
                 if self.params['noiseParams']['method'] == 'dataMap':
-                    if 'noiseMaskCatalog' in mapDict.keys() and mapDict['noiseMaskCatalog'] is not None:
-                        modelPath=self.diagnosticsDir+os.path.sep+"noiseMaskModel_%.1f.fits" % (mapDict['obsFreqGHz'])
-                        if os.path.exists(modelPath) == True:
-                            with pyfits.open(modelPath) as img:
-                                model=img[0].data
-                        else:
-                            model=maps.makeModelImage(d.shape, self.wcs, mapDict['noiseMaskCatalog'],
+                    if 'noiseModelCatalog' in self.params.keys() and self.params['noiseModelCatalog'] is not None:
+                        assert(type(self.params['noiseModelCatalog']) == list)
+                        for noiseModelCatalog in self.params['noiseModelCatalog']:
+                            model=maps.makeModelImage(d.shape, self.wcs, noiseModelCatalog,
                                                       mapDict['beamFileName'],
-                                                      obsFreqGHz = mapDict['obsFreqGHz'],
-                                                      minSNR = 5.0)
-                            maps.saveFITS(modelPath, model, self.wcs)
-                        if model is not None:
-                            d=d-model
+                                                      obsFreqGHz = mapDict['obsFreqGHz'])
+                            if model is not None:
+                                d=d-model
                     fMapsForNoise.append(enmap.fft(enmap.apod(d, self.apodPix)))
                 elif self.params['noiseParams']['method'] == 'model':
                     # Assuming weights are actually inv var white noise level per pix
                     # (which they are for Sigurd's maps)
                     valid=np.nonzero(mapDict['weights'])
                     RMS=np.mean(1/np.sqrt(mapDict['weights'][valid]))
                     if RMS < 10.0:  # Minimum level to stop this blowing up
                         RMS=10.0
                     # Seeds fixed so that outputs are the same on repeated runs
-                    cmb=maps.simCMBMap(self.shape, self.wcs, beamFileName = mapDict['beamFileName'], 
-                                       seed = 3141592654+i, noiseLevel = RMS, fixNoiseSeed = True)
+                    cmb=maps.simCMBMap(self.shape, self.wcs, beam = mapDict['beamFileName'],
+                                       seed = 3141592654+i, noiseLevel = RMS)
                     fMapsForNoise.append(enmap.fft(enmap.apod(cmb, self.apodPix)))
                 else:
                     raise Exception("'%s' is not a valid filter noise method name - fix the .yml config file" % (self.params['noiseParams']['method']))
             fMapsForNoise=np.array(fMapsForNoise)
         
             # Smoothing noise here is essential
             kernelSize=(3,3)
@@ -664,26 +644,32 @@
                     signalMap=enmap.apply_window(signalMap, pow=1.0) # Needed for clusters, 1.5% effect
                     signalMaps.append(signalMap)
                     fSignal=enmap.fft(signalMap)
                     fSignalMaps.append(fSignal)
                 signalMaps=np.array(signalMaps)
                 fSignalMaps=np.array(fSignalMaps)        
                 filteredSignal=self.applyFilter(fSignalMaps)
-                self.signalNorm=y0/filteredSignal.max()
-
+                # This is a 0.6% difference to the previous version
+                cRADeg, cDecDeg=self.wcs.getCentreWCSCoords()
+                cx, cy=self.wcs.wcs2pix(cRADeg, cDecDeg)
+                mapInterpolator=interpolate.RectBivariateSpline(np.arange(filteredSignal.shape[0]),
+                                                                np.arange(filteredSignal.shape[1]),
+                                                                filteredSignal, kx = 3, ky = 3)
+                peakFilteredSignal=mapInterpolator(cy, cx)[0][0]
+                #peakFilteredSignal=filteredSignal.max() # Previous version
+                self.signalNorm=y0/peakFilteredSignal
                 # For relativistic corrections (see signals module)
                 totalSignal=filteredSignal.flatten()[np.argmax(filteredSignal)]
                 filteredSignalCube=np.real(enmap.ifft(fSignalMaps*self.filt, normalize = False))
                 self.fRelWeights={}
                 for filteredSignalPlane, mapDict in zip(filteredSignalCube, self.unfilteredMapsDictList):
                     freqGHz=mapDict['obsFreqGHz']
                     fRelWeight=filteredSignalPlane.flatten()[np.argmax(filteredSignal)]/totalSignal
                     self.fRelWeights[freqGHz]=fRelWeight
                 del fSignalMaps
-                self.signalNorm=y0/filteredSignal.max()
             elif self.params['outputUnits'] == 'uK':
                 #if len(self.unfilteredMapsDictList) > 1:
                     #raise Exception("multi-frequency filtering not currently supported for outputUnits 'uK' (point source finding)")
                 combinedObsFreqGHz=float(list(self.beamSolidAnglesDict.keys())[0])  # Make less clunky...
                 signalMaps=[]
                 fSignalMaps=[]
                 for mapDict in self.unfilteredMapsDictList:
@@ -696,16 +682,19 @@
                 fSignalMaps=np.array(fSignalMaps)        
                 filteredSignal=self.applyFilter(fSignalMaps)
                 self.signalNorm=1.0/filteredSignal.max()
                 del fSignalMaps
             else:
                 raise Exception('need to specify "outputUnits" ("yc" or "uK") in filter params')
         else:
-            print("... loading cached filter ...")
+            print("... loading cached filter")
             self.loadFilter()
+            self.params['saveRMSMap']=False
+            self.params['saveFilter']=False
+            self.params['savePlots']=False
         
         # Apply filter
         filteredMap=self.applyFilter(fMapsToFilter)
         del fMapsToFilter
                 
         # Units etc.
         if self.params['outputUnits'] == 'yc':
@@ -728,47 +717,50 @@
         RMSMap=self.makeNoiseMap(filteredMap)
         validMask=np.greater(RMSMap, 0)
         SNMap=np.zeros(filteredMap.shape)+filteredMap
         SNMap[validMask]=SNMap[validMask]/RMSMap[validMask]
                 
         # Use rank filter to zap edges where RMS will be artificially low - we use a bit of a buffer here
         # NOTE: Now point source mask is applied above, we fill the holes back in here when finding edges
+        # NOTE: This all works on maps which have a zero border. If they don't, edgeTrimArcmin has no effect
         if 'edgeTrimArcmin' in self.params.keys() and self.params['edgeTrimArcmin'] > 0:
             trimSizePix=int(round((self.params['edgeTrimArcmin']/60.)/self.wcs.getPixelSizeDeg()))
-        elif 'noiseGridArcmin' in self.params['noiseParams'] and self.params['noiseParams']['noiseGridArcmin'] != "smart":
+        elif 'noiseGridArcmin' in self.params['noiseParams'] and self.params['noiseParams']['noiseGridArcmin'] != "smart"\
+                and self.params['noiseParams']['noiseGridArcmin'] is not None:
             gridSize=int(round((self.params['noiseParams']['noiseGridArcmin']/60.)/self.wcs.getPixelSizeDeg()))
             trimSizePix=int(round(gridSize*3.0))
         else:
             trimSizePix=0.0
         if trimSizePix  > 0:
             edgeCheck=ndimage.rank_filter(abs(filteredMap+(1-psMask)), 0, size = (trimSizePix, trimSizePix))
             edgeCheck=np.array(np.greater(edgeCheck, 0), dtype = float)
         else:
             edgeCheck=np.ones(filteredMap.shape)
         filteredMap=filteredMap*edgeCheck
-        apodMask=np.not_equal(filteredMap, 0)
         surveyMask=edgeCheck*surveyMask*psMask
         filteredMap=filteredMap*surveyMask # NOTE: Needed for 2-pass (I think)
         del edgeCheck
 
+        # Just in case... we always want to trim the apodized region from the region searched
+        # This has no effect if we're using a survey mask already
+        # Doing this makes life easier when running tests that use small survey masks or go right to edge of tile otherwise
+        apodMask=np.equal(enmap.apod(np.ones(filteredMap.shape), self.apodPix), 1)
+        surveyMask=surveyMask*apodMask
+
         # Apply final survey mask to signal-to-noise map and RMS map
         # NOTE: need to avoid NaNs in here, otherwise map interpolation for e.g. S/N will fail later on
         # NOTE: we now save the mask after detecting objects, as we can detect rings around extremely
         # bright sources and add those to the mask there (see pipelines module)
         SNMap=SNMap*surveyMask
         SNMap[np.isnan(SNMap)]=0.
         RMSMap=RMSMap*surveyMask
-        #maskFileName=self.selFnDir+os.path.sep+"areaMask#%s.fits" % (self.tileName)
-        #surveyMask=np.array(surveyMask, dtype = int)
-        #if os.path.exists(maskFileName) == False:
-            #maps.saveFITS(maskFileName, surveyMask, self.wcs, compressed = True)
                 
         if 'saveRMSMap' in self.params and self.params['saveRMSMap'] == True:
-            RMSFileName=self.selFnDir+os.path.sep+"RMSMap_%s#%s.fits" % (self.label, self.tileName)
-            maps.saveFITS(RMSFileName, RMSMap, self.wcs, compressed = True)
+            RMSFileName=self.selFnDir+os.path.sep+self.tileName+os.path.sep+"RMSMap_%s#%s.fits" % (self.label, self.tileName)
+            maps.saveFITS(RMSFileName, RMSMap, self.wcs, compressionType = "RICE_1")
 
         if 'savePlots' in self.params and self.params['savePlots'] == True:
             self.saveRealSpaceFilterProfile()
                 
         if 'saveFilter' in self.params and self.params['saveFilter'] == True:
             img=pyfits.PrimaryHDU()                                                                                                                                                              
             img.header['SIGNORM']=self.signalNorm
@@ -777,17 +769,17 @@
                 count=count+1
                 img.header['RW%d_GHZ' % (count)]=key
                 img.header['RW%d' % (count)]=self.fRelWeights[key]
             img.data=self.filt                                                                                                                                                                      
             img.writeto(self.filterFileName, overwrite = True) 
             
         # NOTE: What to do about frequency here? Generalise for non-SZ
-        return {'data': filteredMap, 'wcs': self.wcs, 'obsFreqGHz': combinedObsFreqGHz, 'SNMap': SNMap, 
-                'surveyMask': surveyMask, 'mapUnits': mapUnits, 'beamSolidAngle_nsr': beamSolidAngle_nsr,
-                'label': self.label, 'tileName': self.tileName}
+        return {'data': filteredMap, 'wcs': self.wcs, 'obsFreqGHz': combinedObsFreqGHz, 'SNMap': SNMap,
+                'surveyMask': surveyMask, 'flagMask': self.flagMask, 'mapUnits': mapUnits,
+                'beamSolidAngle_nsr': beamSolidAngle_nsr, 'label': self.label, 'tileName': self.tileName}
 
 
     def loadFilter(self):
         """Loads in a previously saved filter.
         
         Returns:
             None
@@ -843,28 +835,28 @@
         """
         
         # NOTE: need to check appropriate signalNorm after reshaping
         if mapDataToFilter.shape == self.filt.shape:
             filt=self.filt
         else:
             filt=self.reshapeFilter(mapDataToFilter.shape)
-        
+
         if 'complex' in mapDataToFilter.dtype.name:
             fMapsToFilter=mapDataToFilter
         else:
             fMapsToFilter=enmap.fft(enmap.apod(mapDataToFilter, self.apodPix))
 
         filteredMap=np.real(enmap.ifft(fMapsToFilter*filt, normalize = False)).sum(axis = 0)
 
         # Optional additional high-pass filter
         if 'bckSub' in self.params.keys() and 'bckSubScaleArcmin' in self.params.keys() and self.params['bckSub'] == True:
             filteredMap=maps.subtractBackground(filteredMap, self.wcs, smoothScaleDeg = self.params['bckSubScaleArcmin']/60.)
         
         filteredMap=filteredMap*self.signalNorm
-        
+
         return filteredMap
         
 #------------------------------------------------------------------------------------------------------------
 class RealSpaceMatchedFilter(MapFilter):
     """Makes a matched-filter kernel using the noise properties of a specified region of the map (e.g.,
     the deepest part) in Fourier space, which is converted into real space and truncated such that the 
     kernel is small enough in footprint to be applied by direct convolution with the map in a (relatively)
@@ -919,36 +911,36 @@
         wcs=self.wcs
         
         # Build the matched-filter kernel in a small section of the map
         # Apply the same difference of Gaussians high pass filter here
         # NOTE: we could merge 'bckSubScaleArcmin' and 'maxArcmin' keys here!
         #mapDict['bckSubScaleArcmin']=maxArcmin
         keysWanted=['mapFileName', 'weightsFileName', 'obsFreqGHz', 'units', 'beamFileName', 'addNoise', 
-                    'pointSourceRemoval', 'weightsType']
+                    'pointSourceRemoval', 'weightsType', 'tileName']
         kernelUnfilteredMapsDictList=[]
         for mapDict in self.unfilteredMapsDictList:
-            kernelUnfilteredMapsDict={}
-            for k in keysWanted:
-                if k in list(mapDict.keys()):
-                    kernelUnfilteredMapsDict[k]=mapDict[k]
+            for key in list(mapDict.keys()):
+                if key not in keysWanted:
+                    del mapDict[key]
+            kernelUnfilteredMapsDict=maps.MapDict(mapDict, tileCoordsDict = mapDict.tileCoordsDict)
             kernelUnfilteredMapsDict['RADecSection']=RADecSection
             kernelUnfilteredMapsDictList.append(kernelUnfilteredMapsDict)
         kernelLabel="realSpaceKernel_%s" % (self.label)
         matchedFilterDir=self.diagnosticsDir+os.path.sep+kernelLabel+"#"+self.tileName
         diagnosticsDir=matchedFilterDir+os.path.sep+'diagnostics'
         selFnDir=matchedFilterDir+os.path.sep+'selFn'
         for d in [matchedFilterDir, diagnosticsDir, selFnDir]:
             if os.path.exists(d) == False:
                 os.makedirs(d, exist_ok = True)
         matchedFilterClass=eval(self.params['noiseParams']['matchedFilterClass'])
-        matchedFilter=matchedFilterClass(kernelLabel, kernelUnfilteredMapsDictList, self.params, 
+        matchedFilter=matchedFilterClass(kernelLabel, kernelUnfilteredMapsDictList, self.params,
                                          tileName = mapDict['tileName'],
                                          diagnosticsDir = matchedFilterDir+os.path.sep+'diagnostics',
                                          selFnDir = matchedFilterDir+os.path.sep+'selFn')
-        filteredMapDict=matchedFilter.buildAndApply()   
+        filteredMapDict=matchedFilter.buildAndApply()
         
         # Turn the matched filter into a smaller real space convolution kernel
         # This means we have to roll off the kernel to 0 at some radius
         # This is set by maxArcmin in the config file
         kernelMaxArcmin=self.params['noiseParams']['kernelMaxArcmin']
         prof, arcminRange=matchedFilter.makeRealSpaceFilterProfile()
         rIndex=np.where(arcminRange > kernelMaxArcmin)[0][0]
@@ -1076,23 +1068,23 @@
         plt.savefig(self.diagnosticsDir+os.path.sep+"filterPlot1D_%s#%s.pdf" % (self.label, self.tileName))
         plt.close()
 
             
     def buildAndApply(self):
 
         surveyMask=self.unfilteredMapsDictList[0]['surveyMask']
-        psMask=self.unfilteredMapsDictList[0]['psMask']
-            
+        psMask=self.unfilteredMapsDictList[0]['pointSourceMask']
+
         if os.path.exists(self.filterFileName) == False:
-            
+
             # Noise region to use
             RAMin, RAMax, decMin, decMax=self.wcs.getImageMinMaxWCSCoords()
             if self.params['noiseParams']['RADecSection'] == 'tileNoiseRegions':
                 RADecSection=[self.wcs.header['NRAMIN'], self.wcs.header['NRAMAX'], 
-                            self.wcs.header['NDEMIN'], self.wcs.header['NDEMAX']]
+                              self.wcs.header['NDEMIN'], self.wcs.header['NDEMAX']]
             elif self.params['noiseParams']['RADecSection'] == 'auto':
                 cRA, cDec=self.wcs.getCentreWCSCoords()
                 halfSizeDeg=2.0
                 nRAMin=cRA-halfSizeDeg/np.cos(np.radians(cDec))
                 nRAMax=cRA+halfSizeDeg/np.cos(np.radians(cDec))
                 nDecMin=cDec-halfSizeDeg
                 nDecMax=cDec+halfSizeDeg
@@ -1103,18 +1095,18 @@
             self.applyRACentre=(RAMax+RAMin)/2.
             
             # Build kernel   
             self.buildKernel(RADecSection, RADeg = self.applyRACentre, decDeg = self.applyDecCentre)
         else:
             self.loadFilter()
 
-        # Apply kernel        
+        # Apply kernel
         mapDataToFilter=[]
         for mapDict in self.unfilteredMapsDictList:
-            mapDataToFilter.append(mapDict['data'])
+            mapDataToFilter.append(mapDict.loadTile('mapFileName', tileName = self.tileName))
         mapDataToFilter=np.array(mapDataToFilter)
         filteredMap=self.applyFilter(mapDataToFilter)
                                                 
         # Apply the point source mask here (before noise estimates etc.)
         filteredMap=filteredMap*psMask
         
         # Make noise and S/N maps
@@ -1146,36 +1138,36 @@
             trimSizePix=int(round(gridSize*3.0))
         if trimSizePix > 0:
             edgeCheck=ndimage.rank_filter(abs(filteredMap+(1-psMask)), 0, size = (trimSizePix, trimSizePix))
         else:
             edgeCheck=np.ones(filteredMap.shape)
         edgeCheck=np.array(np.greater(edgeCheck, 0), dtype = float)
         filteredMap=filteredMap*edgeCheck
-        apodMask=np.not_equal(filteredMap, 0)
         surveyMask=edgeCheck*surveyMask*psMask
         del edgeCheck
 
+        # Just in case... we always want to trim the apodized region from the region searched
+        # This has no effect if we're using a survey mask already
+        # Doing this makes life easier when running tests that use small survey masks or go right to edge of tile otherwise
+        apodMask=np.equal(enmap.apod(np.ones(filteredMap.shape), self.apodPix), 1)
+        surveyMask=surveyMask*apodMask
+
         # Apply final survey mask to signal-to-noise map and RMS map
         # NOTE: need to avoid NaNs in here, otherwise map interpolation for e.g. S/N will fail later on
         SNMap=SNMap*surveyMask
         SNMap[np.isnan(SNMap)]=0.
         RMSMap=RMSMap*surveyMask
 
-        maskFileName=self.selFnDir+os.path.sep+"areaMask#%s.fits" % (self.tileName)
-        surveyMask=np.array(surveyMask, dtype = int)
-        if os.path.exists(maskFileName) == False:
-            maps.saveFITS(maskFileName, surveyMask, self.wcs, compressed = True, compressionType = 'PLIO_1')
-        
         if 'saveRMSMap' in self.params and self.params['saveRMSMap'] == True:
             RMSFileName=self.selFnDir+os.path.sep+"RMSMap_%s#%s.fits" % (self.label, self.tileName)
-            maps.saveFITS(RMSFileName, RMSMap, self.wcs, compressed = True)
+            maps.saveFITS(RMSFileName, RMSMap, self.wcs, compressionType = 'RICE_1')
 
         return {'data': filteredMap, 'wcs': self.wcs, 'obsFreqGHz': combinedObsFreqGHz, 'SNMap': SNMap, 
-                'surveyMask': surveyMask, 'mapUnits': mapUnits, 'beamSolidAngle_nsr': beamSolidAngle_nsr,
-                'label': self.label, 'tileName': self.tileName}
+                'surveyMask': surveyMask, 'flagMask': self.flagMask, 'mapUnits': mapUnits,
+                'beamSolidAngle_nsr': beamSolidAngle_nsr, 'label': self.label, 'tileName': self.tileName}
 
     
     def applyFilter(self, mapDataToFilter, calcFRelWeights = False):
         """Apply the filter to the given map data (must be 3d array, i.e., a cube, with each plane
         corresponding to a different frequency).
 
         Args:
@@ -1241,21 +1233,23 @@
 class ArnaudModelFilter(MapFilter):
     """Base class for filters using the GNFW profile as described in 
     `Arnaud et al. (2010) <https://ui.adsabs.harvard.edu/abs/2010A%26A...517A..92A/abstract>`_.
     Derived from :class:`MapFilter`.
     
     """
     
-    def makeSignalTemplateMap(self, beamFileName, amplitude = None):        
-        signalMap=signals.makeArnaudModelSignalMap(self.params['z'], self.params['M500MSun'], 
-                                                   np.degrees(self.radiansMap),
-                                                   self.wcs, beamFileName, 
+    def makeSignalTemplateMap(self, beamFileName, amplitude = None):
+        RADeg, decDeg=self.wcs.getCentreWCSCoords()
+        signalMap=signals.makeArnaudModelSignalMap(self.params['z'], self.params['M500MSun'],
+                                                   self.shape, self.wcs, beam = beamFileName,
+                                                   RADeg = RADeg, decDeg = decDeg,
                                                    GNFWParams = self.params['GNFWParams'],
-                                                   amplitude = amplitude)
-        
+                                                   amplitude = amplitude,
+                                                   convolveWithBeam = True)
+
         return signalMap
 
 #------------------------------------------------------------------------------------------------------------
 class BattagliaModelFilter(MapFilter):
     """Base class for filters using the GNFW profile as described in
     `Battaglia et al. (2012) <https://ui.adsabs.harvard.edu/abs/2012ApJ...758...75B/abstract>`_.
     Derived from :class:`MapFilter`.
@@ -1264,20 +1258,22 @@
         This is the same as :class:`ArnaudModelFilter` (it is still a GNFW profile), but has non-self-similar
         evolution with redshift, which is accounted for here. The convention for how the GNFW parameters are
         defined follows `Arnaud et al. (2010) <https://ui.adsabs.harvard.edu/abs/2010A%26A...517A..92A/abstract>`_,
         rather than `Battaglia et al. (2012) <https://ui.adsabs.harvard.edu/abs/2012ApJ...758...75B/abstract>`_.
 
     """
     
-    def makeSignalTemplateMap(self, beamFileName, amplitude = None):        
-        signalMap=signals.makeBattagliaModelSignalMap(self.params['z'], self.params['M500MSun'], 
-                                                   np.degrees(self.radiansMap),
-                                                   self.wcs, beamFileName, 
+    def makeSignalTemplateMap(self, beamFileName, amplitude = None):
+        RADeg, decDeg=self.wcs.getCentreWCSCoords()
+        signalMap=signals.makeBattagliaModelSignalMap(self.params['z'], self.params['M500MSun'],
+                                                   self.shape, self.wcs, beam = beamFileName,
+                                                   RADeg = RADeg, decDeg = decDeg,
                                                    GNFWParams = self.params['GNFWParams'],
-                                                   amplitude = amplitude)
+                                                   amplitude = amplitude,
+                                                   convolveWithBeam = True)
         
         return signalMap
     
 #------------------------------------------------------------------------------------------------------------
 # Definitions of actual filters that can be used
 
 class ArnaudModelMatchedFilter(MatchedFilter, ArnaudModelFilter):
```

### Comparing `nemo-sz-0.5.0/nemo/gnfw.py` & `nemo-sz-0.6.0/nemo/gnfw.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/nemo/maps.py` & `nemo-sz-0.6.0/nemo/maps.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,31 +16,639 @@
 import colorcet
 import numpy as np
 import pylab as plt
 import glob
 import os
 import sys
 import math
-import pyximport; pyximport.install()
-import nemoCython
 import time
 import shutil
 import copy
 import yaml
 import pickle
-from pixell import enmap
+from pixell import enmap, curvedsky, utils, powspec
+import sharp
 import nemo
+try:
+    import reproject
+except:
+    pass
 from . import catalogs
 from . import signals
 from . import photometry
 from . import plotSettings
 from . import pipelines
 from . import completeness
 np.random.seed()
-              
+
+#------------------------------------------------------------------------------------------------------------
+class MapDict(dict):
+    """A dictionary for managing a sky map (a 2d array with an associated WCS) within Nemo. Keys within the
+    dictionary can be set to values that control preprocessing of the map (usually done before filtering).
+    Many of the keys in the dictionary map to entries in the .yml config file used by Nemo.
+
+    Args:
+        inputDict (:obj:`dict`): Input dictionary (usually this mirrors the contents of `unfilteredMaps` in
+            Nemo .yml config files).
+        tileCoordsDict (:obj:`dict`, optional): A dictionary that describes the tiling of a large map, as
+            produced by :meth:`startUp.NemoConfig.getTileCoordsDict`.
+
+    Attributes:
+        tileCoordsDict (:obj:`dict`): A dictionary that describes the tiling of a large map, as
+            produced by :meth:`startUp.NemoConfig.getTileCoordsDict`.
+        validMapKeys (:obj:`list`): A list of keys that may contain a path to a map in FITS image format.
+            These are: ['mapFileName', 'weightsFileName', 'pointSourceMask', 'surveyMask', 'flagMask'].
+
+    """
+
+    def __init__(self, inputDict, tileCoordsDict = None):
+        super(MapDict, self).__init__(inputDict)
+        self.tileCoordsDict=tileCoordsDict
+        self._maskKeys=['pointSourceMask', 'surveyMask', 'flagMask', 'extendedMask']
+        self.validMapKeys=['mapFileName', 'weightsFileName']+self._maskKeys
+
+
+    def copy(self):
+        """Make a copy of this :class:`MapDict` object.
+
+        Returns:
+            A deep copy of the :class:`MapDict` object.
+
+        """
+        return MapDict(self, tileCoordsDict = self.tileCoordsDict)
+
+
+    def loadTile(self, mapKey, tileName, returnWCS = False):
+        """Given a key in the map dictionary that contains the path to a FITS image, return the map
+        as a 2d array and (optionally) the WCS.
+
+        Args:
+            mapKey (:obj:`str`): Name of a key in a map dictionary that contains the path to map FITS image.
+                See self.`validMapKeys` for a list.
+            tileName (:obj:`str`): The name of the tile to load.
+
+        Returns:
+            Map data as a 2d array (and optionally a WCS)
+
+        Note:
+            Tiles can be re-projected from CAR to TAN on the fly if the 'reprojectToTan' is set in the
+            Nemo config.
+
+        """
+
+        if mapKey not in self.validMapKeys:
+            raise Exception("mapKey must be one of %s - given mapKey = '%s'." % (self.validMapKeys, mapKey))
+
+        pathToTileImages=self.get(mapKey)
+        if os.path.isdir(pathToTileImages) == True:
+            # Directory full of tile images (used by, e.g., on-the-fly extended source masking)
+            with pyfits.open(pathToTileImages+os.path.sep+tileName+".fits") as img:
+                extName=0
+                tileData=img[extName].data
+                if tileData is None:
+                    for extName in img:
+                        tileData=img[extName].data
+                        if tileData is not None:
+                            break
+                assert tileData is not None
+                if returnWCS == True or self['reprojectToTan'] == True:
+                    # Zapping keywords in old ACT maps that confuse astropy.wcs
+                    wcs=astWCS.WCS(img[extName].header, mode = 'pyfits', zapKeywords = ['PC1_1', 'PC1_2', 'PC2_1', 'PC2_2'])
+                data=tileData
+        elif type(pathToTileImages) == np.ndarray:
+            # We no longer want to support this kind of thing... clean this up later
+            raise Exception("Expected a path but got an array instead (image already loaded).")
+        else:
+            # On-the-fly tile clipping
+            with pyfits.open(pathToTileImages) as img:
+                for ext in img:
+                    if img[ext].data is not None:
+                        break
+                if returnWCS == True or self['reprojectToTan'] == True:
+                    wcs=astWCS.WCS(self.tileCoordsDict[tileName]['header'], mode = 'pyfits')
+                minX, maxX, minY, maxY=self.tileCoordsDict[tileName]['clippedSection']
+                if img[ext].data.ndim == 3:
+                    data=img[ext].data[0, minY:maxY, minX:maxX]
+                elif img[ext].data.ndim == 2:
+                    data=img[ext].data[minY:maxY, minX:maxX]
+                else:
+                    raise Exception("Map data has %d dimensions - only ndim = 2 or ndim = 3 are currently handled." % (img[ext].data.ndim))
+
+        # Convert any mask to 8-bit unsigned ints to save memory
+        if mapKey in self._maskKeys:
+            if data.dtype != np.uint8:
+                data=np.array(data, dtype = np.uint8)
+
+        # Survey masks are special: we need to zap the border overlap area or area calculations will be wrong
+        if mapKey == 'surveyMask':
+            minX, maxX, minY, maxY=self.tileCoordsDict[tileName]['areaMaskInClipSection']
+            data[:minY, :]=0
+            data[maxY:, :]=0
+            data[:, :minX]=0
+            data[:, maxX:]=0
+
+        # Optional TAN reprojection - may help avoid biases due to distortion at high dec in CAR
+        # WARNING: Probably introduces a new pixel window if we're not careful
+        if self['reprojectToTan'] == True:
+            if mapKey in self._maskKeys:
+                order=0
+            else:
+                order='bicubic'
+            tanWCS=_makeTanWCS(wcs)
+            ySizePix, xSizePix=tanWCS.header['NAXIS2'], tanWCS.header['NAXIS1']
+            tanData, footprint=reproject.reproject_interp((data, wcs.AWCS), tanWCS.AWCS, shape_out = [ySizePix, xSizePix],
+                                                          order = order, return_footprint = True)
+            tanData[footprint == 0]=0 # get rid of nans which will be in borders anyway
+            # checkData=reproject.reproject_interp((tanData, tanWCS.AWCS), wcs.AWCS, shape_out = data.shape, order = 'bicubic',
+                                                 # return_footprint = False)
+            wcs=tanWCS
+            data=tanData
+
+        if returnWCS == True:
+            return data, wcs
+        else:
+            return data
+
+
+    def preprocess(self, tileName = 'PRIMARY', diagnosticsDir = None):
+        """Applies a number of pre-processing steps to the map described by this :class:`MapDict` object,
+        typically used before filtering.
+
+        The first step is to load the map itself and the associated weights. Some other operations that may be
+        applied are controlled by keys added to the MapDict. Some of these may be specified in the .yml
+        configuration file, while others are applied by particular filter objects or by routines that generate
+        simulated data. The following keys are understood:
+
+        surveyMask (:obj:`str`)
+            Path to a mask (.fits image; 1 = valid, 0 = masked) that defines the valid object search area.
+
+        pointSourceMask (:obj:`str`)
+            Path to a mask (.fits image; 1 = valid, 0 = masked) that contains holes at the locations of point
+            sources, defining regions that are excluded from the object search area.
+
+        RADecSection (:obj:`list`)
+            Defines a region to extract from the map. Use the format [RAMin, RAMax, decMin, decMax] (units:
+            decimal degrees).
+
+        CMBSimSeed (:obj:`int`)
+            If present, replace the map with a source-free simulated CMB realisation, generated using the given
+            seed number. Used by :meth:`estimateContaminationFromSkySim`.
+
+        applyBeamConvolution (:obj:`bool`)
+            If True, the map is convolved with the beam given in the beamFileName key. This should only be
+            needed when using preliminary y-maps made by tILe-C.
+
+        Args:
+            tileName (:obj:`str`): Name of the map tile (extension name) to operate on.
+            diagnosticsDir (:obj:`str`): Path to a directory where miscellaneous diagnostic data may be written.
+
+        Returns:
+            None - values in the map dictionary are updated in-place, and additional keys may be added.
+
+        """
+
+        data, wcs=self.loadTile('mapFileName', tileName, returnWCS = True)
+
+        # Optional calibration factor
+        if 'calibFactor' in self.keys():
+            data=data*self['calibFactor']
+
+        if self['units'] == 'Jy/sr':
+            if self['obsFreqGHz'] == 148:
+                data=(data/1.072480e+09)*2.726*1e6
+            elif self['obsFreqGHz'] == 219:
+                data=(data/1.318837e+09)*2.726*1e6
+            else:
+                raise Exception("no code added to support conversion to uK from Jy/sr for freq = %.0f GHz" \
+                        % (self['obsFreqGHz']))
+
+        # Load weight map if given
+        if 'weightsFileName' in list(self.keys()) and self['weightsFileName'] is not None:
+            weights=self.loadTile('weightsFileName', tileName)
+            # For Enki maps... take only I (temperature) for now, add options for this later
+            if weights.ndim == 3:       # I, Q, U
+                weights=weights[0, :]
+            elif weights.ndim == 4:     # I, Q, U and also a covariance matrix
+                weights=weights[0, 0, :]
+        else:
+            weights=np.ones(data.shape)
+
+        # We rely on pixels with zero weight having zero value in actual maps later (automated edge trimming)
+        # This might not be the case if the map has been filtered slightly before being fed into nemo
+        data[weights == 0]=0
+
+        # Load survey and point source masks, if given
+        if 'surveyMask' in list(self.keys()) and self['surveyMask'] is not None:
+            surveyMask=self.loadTile('surveyMask', tileName)
+        else:
+            surveyMask=np.ones(data.shape, dtype = np.uint8)
+            surveyMask[weights == 0]=0
+
+        # Some apodisation of the data outside the survey mask
+        # NOTE: should add adjustable parameter for this somewhere later
+        if 'apodizeUsingSurveyMask' in list(self.keys()) and self['apodizeUsingSurveyMask'] == True:
+            # We need to remain unapodized to at least noiseGridArcmin beyond the edge of the survey mask
+            # We'll need to make these adjustable parameters
+            apodMask=np.array(surveyMask, dtype = bool)
+            for i in range(120):
+                apodMask=mahotas.dilate(apodMask)
+            apodMask=ndimage.gaussian_filter(np.array(apodMask, dtype = float), 20)
+            data=data*apodMask
+            del apodMask
+
+        if 'pointSourceMask' in list(self.keys()) and self['pointSourceMask'] is not None:
+            psMask=self.loadTile('pointSourceMask', tileName)
+        else:
+            psMask=np.ones(data.shape, dtype = np.uint8)
+
+        # Use for tracking regions where subtraction/in-painting took place to make flags in catalog
+        # We can also supply a flag mask at the start, e.g., for marking dusty regions without zapping them
+        # NOTE: flag masks for each frequency map get combined within filter objects
+        if 'flagMask' in list(self.keys()) and self['flagMask'] is not None:
+            flagMask=self.loadTile('flagMask', tileName)*surveyMask
+        else:
+            flagMask=np.zeros(data.shape, dtype = np.uint8)
+
+        # Optional map clipping
+        if 'RADecSection' in list(self.keys()) and self['RADecSection'] is not None:
+            RAMin, RAMax, decMin, decMax=self['RADecSection']
+            clip=astImages.clipUsingRADecCoords(data, wcs, RAMin, RAMax, decMin, decMax)
+            data=clip['data']
+            whtClip=astImages.clipUsingRADecCoords(weights, wcs, RAMin, RAMax, decMin, decMax)
+            weights=whtClip['data']
+            psClip=astImages.clipUsingRADecCoords(psMask, wcs, RAMin, RAMax, decMin, decMax)
+            psMask=psClip['data']
+            surveyClip=astImages.clipUsingRADecCoords(surveyMask, wcs, RAMin, RAMax, decMin, decMax)
+            surveyMask=surveyClip['data']
+            flagClip=astImages.clipUsingRADecCoords(flagMask, wcs, RAMin, RAMax, decMin, decMax)
+            flagMask=flagClip['data']
+            wcs=clip['wcs']
+            if len(clip['data']) == 0:
+                raise Exception("Clipping using RADecSection returned empty array - check RADecSection in config .yml file is in map")
+
+        # For source-free simulations (contamination tests)
+        if 'CMBSimSeed' in list(self.keys()):
+            randMap=simCMBMap(data.shape, wcs, noiseLevel = 0, beam = self['beamFileName'],
+                              seed = self['CMBSimSeed'])
+            randMap[np.equal(weights, 0)]=0
+            # Add white noise that varies according to inv var map...
+            # Noise needed is the extra noise we need to add to match the real data, scaled by inv var map
+            # This initial estimate is too high, so we use a grid search to get a better estimate
+            mask=np.nonzero(data)
+            dataSigma=data[mask].std()
+            whiteNoiseLevel=np.zeros(weights.shape)
+            whiteNoiseLevel[mask]=1/np.sqrt(weights[mask])
+            noiseNeeded=np.sqrt(data[mask].var()-randMap[mask].var()-np.median(whiteNoiseLevel[mask])**2)
+            noiseBoostFactor=noiseNeeded/np.median(whiteNoiseLevel[mask])
+            # NOTE: disabled finding boost factor below for now...
+            bestBoostFactor=1.
+            # --- disabled
+            #bestDiff=1e6
+            #bestBoostFactor=noiseBoostFactor
+            #simNoiseValues=simNoise[mask]
+            #for boostFactor in np.linspace(noiseBoostFactor*0.5, noiseBoostFactor, 10):
+                #diff=abs(dataSigma-(simNoiseValues+generatedNoise*boostFactor).std())
+                #if diff < bestDiff:
+                    #bestBoostFactor=boostFactor
+                    #bestDiff=diff
+            # ---
+            data[mask]=np.random.normal(randMap[mask], bestBoostFactor*whiteNoiseLevel[mask],
+                                        whiteNoiseLevel[mask].shape)
+            outFileName=diagnosticsDir+os.path.sep+"CMBSim_%d#%s.fits" % (self['obsFreqGHz'], tileName)
+            saveFITS(outFileName, data, wcs)
+
+        # For position recovery tests, completeness calculations
+        if 'injectSources' in list(self.keys()):
+            # NOTE: Need to add varying GNFWParams here
+            if 'GNFWParams' in self['injectSources'].keys():
+                GNFWParams=self['injectSources']['GNFWParams']
+                obsFreqGHz=self['obsFreqGHz']
+            else:
+                GNFWParams=None
+                obsFreqGHz=None
+            # Unsure if we actually want/need the below...
+            # source injection sim tiles are processed independently (so shouldn't be double counting in overlaps anyway)
+            validAreaSection=self.tileCoordsDict[tileName]['areaMaskInClipSection']
+            modelMap=makeModelImage(data.shape, wcs, self['injectSources']['catalog'],
+                                    self['beamFileName'], obsFreqGHz = obsFreqGHz,
+                                    GNFWParams = GNFWParams, profile = self['injectSources']['profile'],
+                                    validAreaSection = validAreaSection,
+                                    override = self['injectSources']['override'])
+            if modelMap is not None:
+                modelMap[weights == 0]=0
+                data=data+modelMap
+
+        # Should only be needed for handling preliminary tILe-C maps
+        if 'applyBeamConvolution' in self.keys() and self['applyBeamConvolution'] == True:
+            data=convolveMapWithBeam(data, wcs, self['beamFileName'], maxDistDegrees = 1.0)
+            if diagnosticsDir is not None:
+                saveFITS(diagnosticsDir+os.path.sep+"beamConvolved#%s.fits" % (tileName), data, wcs)
+
+        # Smoothing with some kernel (used, e.g., in PSF-matching between maps in nemoSpec)
+        if 'smoothKernel' in self.keys():
+            if 'smoothAttenuationFactor' in self.keys():
+                data=data*self['smoothAttenuationFactor']
+            data=convolveMapWithBeam(data, wcs, self['smoothKernel'], maxDistDegrees = 1.0)
+
+        # Check if we're going to need to fill holes - if so, set-up smooth background only once
+        # NOTE: If this needs changing, needs parametrizing as used in e.g. ACT DR5 results
+        holeFillingKeys=['maskPointSourcesFromCatalog', 'maskAndFillFromCatalog', 'extendedMask']
+        holeFilling=False
+        for h in holeFillingKeys:
+            if h in list(self.keys()):
+                holeFilling=True
+                break
+        if holeFilling == True:
+            pixRad=(10.0/60.0)/wcs.getPixelSizeDeg()
+            bckData=ndimage.median_filter(data, int(pixRad))
+
+        if 'extendedMask' in list(self.keys()):
+            # Filling with white noise + smooth large scale image
+            # WARNING: Assumes weights are ivar maps [true for Sigurd's maps]
+            extendedMask=self.loadTile('extendedMask', tileName = tileName)
+            mask=np.nonzero(weights)
+            whiteNoiseLevel=np.zeros(weights.shape)
+            whiteNoiseLevel[mask]=1/np.sqrt(weights[mask])
+            data[extendedMask == 1]=bckData[extendedMask == 1]+np.random.normal(0, whiteNoiseLevel[extendedMask == 1])
+            surveyMask=surveyMask*(1-extendedMask)
+            #flagMask=flagMask+extendedMask
+
+        # Optional masking of point sources from external catalog
+        # Especially needed if using Fourier-space matched filter (and maps not already point source subtracted)
+        if 'maskPointSourcesFromCatalog' in list(self.keys()) and self['maskPointSourcesFromCatalog'] is not None:
+            # This is fast enough if using small tiles and running in parallel...
+            # If our masking/filling is effective enough, we may not need to mask so much here...
+            if type(self['maskPointSourcesFromCatalog']) is not list:
+                self['maskPointSourcesFromCatalog']=[self['maskPointSourcesFromCatalog']]
+            psMask=np.ones(data.shape, dtype = np.uint8)
+            #pixRad=(10.0/60.0)/wcs.getPixelSizeDeg()
+            #bckData=ndimage.median_filter(data, int(pixRad))
+            rDegMap=np.ones(data.shape, dtype = float)*1e6
+            for catalogInfo in self['maskPointSourcesFromCatalog']:
+                if type(catalogInfo) == str:
+                    catalogPath=catalogInfo
+                    fluxCutJy=0.0
+                elif type(catalogInfo) == dict:
+                    catalogPath=catalogInfo['path']
+                    fluxCutJy=catalogInfo['fluxCutJy']
+                else:
+                    raise Exception("Didn't understand contents of 'maskPointSourcesFromCatalog' - should be a path, or a dict with 'path' key.")
+                tab=atpy.Table().read(catalogPath)
+                if 'fluxJy' in tab.keys():
+                    tab=tab[tab['fluxJy'] > fluxCutJy]
+                tab=catalogs.getCatalogWithinImage(tab, data.shape, wcs)
+                # If we're given a catalog that already has rArcmin in it, we use that to set hole size
+                # Otherwise, if we have shape measurements (ellipse_A at least), we can use that
+                for row in tab:
+                    # Extended sources - identify by measured size > masking radius
+                    # These will mess up noise term in filter, so add to psMask also and fill + smooth
+                    # We won't fiddle with PA here, we'll just maximise based on x-pixel scale (because CAR)
+                    if 'rArcmin' in tab.keys():
+                        maskRadiusArcmin=row['rArcmin']
+                    elif 'ellipse_A' in tab.keys():
+                        xPixSizeArcmin=(wcs.getXPixelSizeDeg()/np.cos(np.radians(row['decDeg'])))*60
+                        ASizeArcmin=row['ellipse_A']/xPixSizeArcmin
+                        maskRadiusArcmin=ASizeArcmin/2
+                    else:
+                        raise Exception("To mask sources in a catalog, need either 'rArcmin' or 'ellipse_A' column to be present.")
+                    rDegMap, xBounds, yBounds=makeDegreesDistanceMap(rDegMap, wcs,
+                                                                     row['RADeg'], row['decDeg'],
+                                                                     maskRadiusArcmin/60)
+                    surveyMask[rDegMap < maskRadiusArcmin/60.0]=0
+                    psMask[rDegMap < maskRadiusArcmin/60.0]=0
+                    data[rDegMap < maskRadiusArcmin/60.0]=bckData[rDegMap < maskRadiusArcmin/60.0]
+
+        if 'subtractModelFromCatalog' in list(self.keys()) and self['subtractModelFromCatalog'] is not None:
+            if type(self['subtractModelFromCatalog']) is not list:
+                self['subtractModelFromCatalog']=[self['subtractModelFromCatalog']]
+            for tab in self['subtractModelFromCatalog']:
+                if type(tab) != atpy.Table:
+                    tab=atpy.Table().read(catalogPath)
+                tab=catalogs.getCatalogWithinImage(tab, data.shape, wcs)
+                model=makeModelImage(data.shape, wcs, tab, self['beamFileName'], obsFreqGHz = self['obsFreqGHz'])
+                if model is not None:
+                    data=data-model
+                    # Threshold of > 1 uK here should be made adjustable in config
+                    flagMask=flagMask+np.greater(model, 1)
+
+        if 'maskAndFillFromCatalog' in list(self.keys()) and self['maskAndFillFromCatalog'] is not None:
+            if type(self['maskAndFillFromCatalog']) is not list:
+                self['maskAndFillFromCatalog']=[self['maskAndFillFromCatalog']]
+            for tab in self['maskAndFillFromCatalog']:
+                if type(tab) != atpy.Table:
+                    tab=atpy.Table().read(catalogPath)
+                tab=catalogs.getCatalogWithinImage(tab, data.shape, wcs)
+                if len(tab) > 0 and 'ellipse_A' not in tab.keys():
+                    raise Exception("Need to set measureShapes: True to use maskAndFillFromCatalog")
+                for row in tab:
+                    x, y=wcs.wcs2pix(row['RADeg'], row['decDeg'])
+                    rArcminMap=np.ones(data.shape, dtype = float)*1e6
+                    if 'ellipse_A' and 'ellipse_B' in tab.keys():
+                        xPixSizeArcmin=(wcs.getXPixelSizeDeg()/np.cos(np.radians(row['decDeg'])))*60
+                        maskRadiusArcmin=(row['ellipse_A']/xPixSizeArcmin)/2
+                    if 'maskHoleDilationFactor' in self.keys() and self['maskHoleDilationFactor'] is not None:
+                        maskRadiusArcmin=maskRadiusArcmin*self['maskHoleDilationFactor']
+                    rArcminMap, xBounds, yBounds=makeDegreesDistanceMap(rArcminMap, wcs,
+                                                                        row['RADeg'], row['decDeg'],
+                                                                        maskRadiusArcmin/60)
+                    rArcminMap=rArcminMap*60
+                    surveyMask[rArcminMap < maskRadiusArcmin]=0
+                    psMask[rArcminMap < maskRadiusArcmin]=0
+                    data[rArcminMap < maskRadiusArcmin]=bckData[rArcminMap < maskRadiusArcmin]
+
+        # Add the map data to the dict
+        self['data']=data
+        self['weights']=weights
+        self['wcs']=wcs
+        self['surveyMask']=surveyMask
+        self['pointSourceMask']=psMask
+        self['flagMask']=flagMask
+        self['tileName']=tileName
+
+        # No point continuing if masks are different shape to map (easier to tell user here)
+        if self['data'].shape != self['pointSourceMask'].shape:
+            raise Exception("Map and point source mask dimensions are not the same (they should also have same WCS)")
+        if self['data'].shape != self['surveyMask'].shape:
+            raise Exception("Map and survey mask dimensions are not the same (they should also have same WCS)")
+
+
+#------------------------------------------------------------------------------------------------------------
+class MapDictList(object):
+    """Blah. We want this to iterate over the mapDictList and be indexable.
+
+    """
+
+    def __init__(self, mapDictList, tileCoordsDict = None):
+        """Blah.
+
+        """
+
+        self.mapDictList=[]
+        for mapDict in mapDictList:
+            self.mapDictList.append(MapDict(mapDict, tileCoordsDict))
+
+
+    def __iter__(self):
+        yield from self.mapDictList
+
+
+    def __getitem__(self, item):
+        return self.mapDictList[item]
+
+
+#------------------------------------------------------------------------------------------------------------
+class TileDict(dict):
+    """A dictionary for collecting tile images, for later saving as multi-extension FITS or outputting as a
+    single monolithic FITS image. Keys within the dictionary map to tile names. Handles on-the-fly
+    reprojection between TAN and CAR if specified in the Nemo config.
+
+    Args:
+        inputDict (:obj:`dict`): Input dictionary (keys map to tile names).
+        tileCoordsDict (:obj:`dict`, optional): A dictionary that describes the tiling of a large map, as
+            produced by :meth:`startUp.NemoConfig.getTileCoordsDict`.
+
+    Attributes:
+        tileCoordsDict (:obj:`dict`): A dictionary that describes the tiling of a large map, as
+            produced by :meth:`startUp.NemoConfig.getTileCoordsDict`.
+
+    """
+
+    def __init__(self, inputDict, tileCoordsDict = None):
+        super(TileDict, self).__init__(inputDict)
+        self.tileCoordsDict=tileCoordsDict
+
+
+    def copy(self):
+        """Make a copy of this :class:`TileDict` object.
+
+        Returns:
+            A deep copy of the :class:`TileDict` object.
+
+        """
+        return TileDict(self, tileCoordsDict = self.tileCoordsDict)
+
+
+    def saveMEF(self, outFileName, compressionType = None):
+        """Save the tile images as a multi-extension FITS file.
+
+        Args:
+            outFileName (:obj:`str`): Path where the MEF file will be written.
+            compressionType (:obj:`str`): If given, the data will be compressed using the given
+                method (as understood by :mod:`astropy.io.fits`). Use `PLIO_1` for masks,
+                and `RICE_1` for other image data that can stand lossy compression. If None,
+                the image data is not compressed.
+
+        Returns:
+            None
+
+        """
+        newImg=pyfits.HDUList()
+        for tileName in self.keys():
+            if self.tileCoordsDict[tileName]['reprojectToTan'] == True:
+                wcs=astWCS.WCS(self.tileCoordsDict[tileName]['header'], mode = 'pyfits')
+                tanWCS=_makeTanWCS(wcs)
+                header=tanWCS.header
+            else:
+                header=self.tileCoordsDict[tileName]['header']
+            if compressionType is not None:
+                if compressionType == 'PLIO_1':
+                    dtype=np.uint8
+                else:
+                    dtype=np.float32
+                hdu=pyfits.CompImageHDU(np.array(self[tileName], dtype = dtype),
+                                        header, name = tileName,
+                                        compression_type = compressionType)
+            else:
+                hdu=pyfits.ImageHDU(self[tileName], header, name = tileName)
+            newImg.append(hdu)
+        newImg.writeto(outFileName, overwrite = True)
+
+
+    def saveStitchedFITS(self, outFileName, stitchedWCS, compressionType = None):
+        """Stitch together the tiles into a monolithic image and save in a FITS file.
+
+        Args:
+            outFileName (:obj:`str`): Path where the stitched image FITS file will be written.
+            stitchedWCS (:obj:`astWCS.WCS`): WCS object corresponding to the stitched map
+                that will be produced.
+            compressionType (:obj:`str`): If given, the data will be compressed using the given
+                method (as understood by :mod:`astropy.io.fits`). Use `PLIO_1` for masks,
+                and `RICE_1` for other image data that can stand lossy compression. If None,
+                the image data is not compressed.
+
+        Returns:
+            None
+
+        """
+
+        wcs=stitchedWCS
+        d=np.zeros([stitchedWCS.header['NAXIS2'], stitchedWCS.header['NAXIS1']])
+        for tileName in self.keys():
+            if self.tileCoordsDict[tileName]['reprojectToTan'] == True:
+                carWCS=astWCS.WCS(self.tileCoordsDict[tileName]['header'], mode = 'pyfits')
+                tanWCS=_makeTanWCS(carWCS)
+                shape=[self.tileCoordsDict[tileName]['header']['NAXIS2'],
+                       self.tileCoordsDict[tileName]['header']['NAXIS1']]
+                if compressionType == 'PLIO_1':
+                    order=0
+                else:
+                    order='bicubic'
+                carData, footprint=reproject.reproject_interp((self[tileName], tanWCS.AWCS), carWCS.AWCS, shape_out = shape, order = order,
+                                                              return_footprint = True)
+                carData[footprint == 0]=0 # get rid of nans which will be in borders anyway
+            else:
+                carData=self[tileName]
+            minX, maxX, minY, maxY=self.tileCoordsDict[tileName]['clippedSection']
+            d[minY:maxY, minX:maxX]=d[minY:maxY, minX:maxX]+carData
+        saveFITS(outFileName, d, wcs, compressionType = compressionType)
+
+#-------------------------------------------------------------------------------------------------------------
+def _makeTanWCS(wcs, pixScale = 0.5/60.0):
+    """Generate a TAN WCS.
+
+    Returns:
+        TAN WCS
+
+    """
+
+    RADeg, decDeg=wcs.getCentreWCSCoords()
+    CRVAL1, CRVAL2=RADeg, decDeg
+    xSizeDeg, ySizeDeg=wcs.getFullSizeSkyDeg()
+    xSizePix, ySizePix=int(xSizeDeg/pixScale), int(ySizeDeg/pixScale)
+    xRefPix=xSizePix/2.0
+    yRefPix=ySizePix/2.0
+    xOutPixScale=xSizeDeg/xSizePix
+    yOutPixScale=ySizeDeg/ySizePix
+    newHead=pyfits.Header()
+    newHead['NAXIS']=2
+    newHead['NAXIS1']=xSizePix
+    newHead['NAXIS2']=ySizePix
+    newHead['CTYPE1']='RA---TAN'
+    newHead['CTYPE2']='DEC--TAN'
+    newHead['CRVAL1']=CRVAL1
+    newHead['CRVAL2']=CRVAL2
+    newHead['CRPIX1']=xRefPix+1
+    newHead['CRPIX2']=yRefPix+1
+    newHead['CDELT1']=-xOutPixScale
+    newHead['CDELT2']=xOutPixScale    # Makes more sense to use same pix scale
+    newHead['CUNIT1']='DEG'
+    newHead['CUNIT2']='DEG'
+    tanWCS=astWCS.WCS(newHead, mode='pyfits')
+
+    return tanWCS
+
+    import reproject
+    tanData, footprint=reproject.reproject_interp((data, wcs.AWCS), tanWCS.AWCS, shape_out = [ySizePix, xSizePix],
+                                                    order = 'bicubic', return_footprint = True)
+    tanData[footprint == 0]=0 # get rid of nans which will be in borders anyway
+    # checkData=reproject.reproject_interp((tanData, tanWCS.AWCS), wcs.AWCS, shape_out = data.shape, order = 'bicubic',
+                                            # return_footprint = False)
+    wcs=tanWCS
+    data=tanData
+
 #-------------------------------------------------------------------------------------------------------------
 def convertToY(mapData, obsFrequencyGHz = 148):
     """Converts an array (e.g., a map) in ΔTemperature (μK) with respect to the CMB to Compton y parameter
     values at the given frequency.
     
     Args:
         mapData (:obj:`np.ndarray`): An array containing delta T (micro Kelvin, with respect to CMB) values.
@@ -91,89 +699,95 @@
         targetTileHeight (float): Desired tile height, in degrees (dec direction for CAR).
     
     Returns:
         Dictionary list defining tiles in same format as config file.
     
     Note:
         While this routine will try to match the target file sizes, it may not match exactly. Also,
-        makeTileDir will expand tiles by a user-specified amount such that they overlap.
+        :meth:`startUp.NemoConfig.getTileCoordsDict` will expand tiles by a user-specified amount such that
+        they overlap.
     
     """
     
     # This deals with identifying boss vs. full AdvACT footprint maps 
     mapCentreRA, mapCentreDec=wcs.getCentreWCSCoords()    
     skyWidth, skyHeight=wcs.getFullSizeSkyDeg()
     if mapCentreRA < 0.1 and skyWidth < 0.1 or skyWidth > 359.9:
         handle180Wrap=True
     else:
         handle180Wrap=False
     
     segMap=surveyMask
-    segMap, numObjects=ndimage.label(np.greater(segMap, 0))
-    fieldIDs=np.arange(1, numObjects+1)
-        
+    try:
+        numObjects=ndimage.label(segMap, output = segMap)
+    except:
+        raise Exception("surveyMask given for autotiler is probably too complicated (breaks into > 256 regions) - check your mask and/or config file.")
+
+    # More memory efficient than previous version
+    fieldIDs=np.arange(1, numObjects+1, dtype = segMap.dtype)
+    maskSections=ndimage.find_objects(segMap)
     tileList=[]
-    for f in fieldIDs:
-        ys, xs=np.where(segMap == f)
-        if len(ys) < 1000:  # In case of stray individual pixels (e.g., combined with extended sources mask)
+    for maskSection, f in zip(maskSections, fieldIDs):
+        yMin=maskSection[0].start
+        yMax=maskSection[0].stop-1
+        if yMax-yMin < 1000:  # In case of stray individual pixels (e.g., combined with extended sources mask)
             continue
-        yMin=ys.min()
-        yMax=ys.max()
-        xc=int((xs.min()+xs.max())/2)
-        
+        xc=int((maskSection[1].start+(maskSection[1].stop-1))/2)
+
         # Some people want to run on full sky CAR ... so we have to avoid that blowing up at the poles
         decMin, decMax=np.nan, np.nan
         deltaY=0
         while np.isnan(decMin) and np.isnan(decMax):
             RAc, decMin=wcs.pix2wcs(xc, yMin+deltaY)
             RAc, decMax=wcs.pix2wcs(xc, yMax-deltaY)
             deltaY=deltaY+0.01
-        
+
         numRows=int((decMax-decMin)/targetTileHeight)
         if numRows == 0:
             raise Exception("targetTileHeight is larger than the height of the map - edit your config file accordingly.")
         tileHeight=np.ceil(((decMax-decMin)/numRows)*100)/100
 
         for i in range(numRows):
             decBottom=decMin+i*tileHeight
             decTop=decMin+(i+1)*tileHeight
             xc, yBottom=wcs.wcs2pix(RAc, decBottom)
             xc, yTop=wcs.wcs2pix(RAc, decTop)
             yBottom=int(yBottom)
             yTop=int(yTop)
             yc=int((yTop+yBottom)/2)
-            
+
             strip=segMap[yBottom:yTop]
             ys, xs=np.where(strip == f)
             xMin=xs.min()
             xMax=xs.max()
+            del ys, xs, strip
             stripWidthDeg=(xMax-xMin)*wcs.getXPixelSizeDeg()
             RAMax, decc=wcs.pix2wcs(xMin, yc)
             RAMin, decc=wcs.pix2wcs(xMax, yc)
             numCols=int(stripWidthDeg/targetTileWidth)
             tileWidth=np.ceil((stripWidthDeg/numCols)*100)/100
             #assert(tileWidth < targetTileWidth*1.1)
-        
-            stretchFactor=1/np.cos(np.radians(decTop)) 
+
+            stretchFactor=1/np.cos(np.radians(decTop))
             numCols=int(stripWidthDeg/(targetTileWidth*stretchFactor))
             for j in range(numCols):
                 tileWidth=np.ceil((stripWidthDeg/numCols)*100)/100
                 RALeft=RAMax-j*tileWidth
                 RARight=RAMax-(j+1)*tileWidth
                 if RALeft < 0:
                     RALeft=RALeft+360
                 if RARight < 0:
                     RARight=RARight+360
                 # HACK: Edge-of-map handling
                 if handle180Wrap == True:
                     if RARight < 180.01 and RALeft < 180+tileWidth and RALeft > 180.01:
                         RARight=180.01
                 # NOTE: floats here to make tileDefinitions.yml readable
-                tileList.append({'tileName': '%d_%d_%d' % (f, i, j), 
-                                 'RADecSection': [float(RARight), float(RALeft), float(decBottom), float(decTop)]})   
+                tileList.append({'tileName': '%d_%d_%d' % (f, i, j),
+                                 'RADecSection': [float(RARight), float(RALeft), float(decBottom), float(decTop)]})
 
     return tileList
 
 #------------------------------------------------------------------------------------------------------------
 def saveTilesDS9RegionsFile(parDict, DS9RegionFileName):
     """Writes a DS9 .reg file containing the locations of tiles defined in parDict.
     
@@ -194,345 +808,14 @@
         tileNames.append(tileDict['tileName'])   
     with open(DS9RegionFileName, "w") as outFile:
         outFile.write("# Region file format: DS9 version 4.1\n")
         outFile.write('global color=blue dashlist=8 3 width=1 font="helvetica 10 normal roman" select=1 highlite=1 dash=0 fixed=0 edit=1 move=1 delete=1 include=1 source=1\n')
         outFile.write("fk5\n")
         for c, name in zip(coordsList, tileNames):
             outFile.write('polygon(%.6f, %.6f, %.6f, %.6f, %.6f, %.6f, %.6f, %.6f) # text="%s"\n' % (c[0], c[2], c[0], c[3], c[1], c[3], c[1], c[2], name))  
-                
-#------------------------------------------------------------------------------------------------------------
-def addAutoTileDefinitions(parDict, DS9RegionFileName = None, cacheFileName = None):
-    """Runs autotiler to add automatic tile definitions into the parameters dictionary in-place.
-    
-    Args:
-        parDict (:obj:`dict`): Dictionary containing the contents of the Nemo config file.
-        DS9RegionFileName (str, optional): Path to DS9 regions file to be written.
-        cacheFileName (str, optional): Path to output a cached .yml file which will can be read instead on 
-            repeated runs (for speed).
-
-    """
-    
-    if cacheFileName is not None and os.path.exists(cacheFileName):
-        with open(cacheFileName, "r") as stream:
-            parDict['tileDefinitions']=yaml.safe_load(stream)
-        return None
-
-    if 'tileDefinitions' in parDict.keys() and type(parDict['tileDefinitions']) == dict:
-        # If we're not given a survey mask, we'll make one up from the map image itself
-        if 'mask' in parDict['tileDefinitions'].keys() and parDict['tileDefinitions']['mask'] is not None:
-            surveyMaskPath=parDict['tileDefinitions']['mask']
-        else:
-            surveyMaskPath=parDict['unfilteredMaps'][0]['mapFileName']
-        with pyfits.open(surveyMaskPath) as img:    
-            # Just in case RICE-compressed or similar
-            if img[0].data is None:
-                surveyMask=img['COMPRESSED_IMAGE'].data
-                wcs=astWCS.WCS(img['COMPRESSED_IMAGE'].header, mode = 'pyfits')
-            else:
-                surveyMask=img[0].data
-                wcs=astWCS.WCS(img[0].header, mode = 'pyfits')
-            # One day we will write a routine to deal with the multi-plane thing sensibly...
-            # But today is not that day
-            if surveyMask.ndim == 3:
-                surveyMask=surveyMask[0, :]
-            assert(surveyMask.ndim == 2)   
-            surveyMask[surveyMask != 0]=1
-        parDict['tileDefinitions']=autotiler(surveyMask, wcs, 
-                                             parDict['tileDefinitions']['targetTileWidthDeg'],
-                                             parDict['tileDefinitions']['targetTileHeightDeg'])
-        print("... breaking map into %d tiles ..." % (len(parDict['tileDefinitions'])))
-        if DS9RegionFileName is not None:
-            saveTilesDS9RegionsFile(parDict, DS9RegionFileName)
-    
-        if cacheFileName is not None:
-            stream=yaml.dump(parDict['tileDefinitions'])
-            with open(cacheFileName, "w") as outFile: 
-                outFile.write(stream) 
-
-#-------------------------------------------------------------------------------------------------------------
-def loadTile(pathToTileImages, tileName, returnWCS = False):
-    """Given a path to a directory full of tiles, or a .fits file, return the map array and (optionally)
-    the WCS.
-    
-    Args:
-        pathToTileImages(str): Path to either a .fits file, or a directory full of .fits files named by tileName.
-        tileName(str): The name of the tile to load.
-        
-    Returns:
-        Map data (and optionally wcs)
-    
-    """
-
-    if os.path.isdir(pathToTileImages) == True:
-        with pyfits.open(pathToTileImages+os.path.sep+tileName+".fits") as img:
-            extName=0
-            tileData=img[extName].data
-            if tileData is None:
-                for extName in img:
-                    tileData=img[extName].data
-                    if tileData is not None:
-                        break
-            assert tileData is not None
-            if returnWCS == True:
-                # Zapping keywords in old ACT maps that confuse astropy.wcs
-                wcs=astWCS.WCS(img[extName].header, mode = 'pyfits', zapKeywords = ['PC1_1', 'PC1_2', 'PC2_1', 'PC2_2'])
-            data=tileData
-    else:
-        with pyfits.open(pathToTileImages) as img:
-            # Handle compressed full-size masks
-            if tileName == 'PRIMARY':
-                for ext in img:
-                    if img[ext].data is not None:
-                        break
-            else:
-                ext=tileName
-            if returnWCS == True:
-                wcs=astWCS.WCS(img[ext].header, mode = 'pyfits', zapKeywords = ['PC1_1', 'PC1_2', 'PC2_1', 'PC2_2'])
-            data=img[ext].data
-        
-    if returnWCS == True:
-        return data, wcs
-    else:
-        return data
-
-#-------------------------------------------------------------------------------------------------------------
-def makeTileDir(parDict, writeToDisk = True):
-    """Update this later. Revised version. Instead of making a MEF, makes a directory for each map and puts
-    individual tile images there. We'll only need to edit preprocessMapDict to handle the difference. Why
-    are we doing this? Just in case reading from the same file is gumming up MPI runs on hippo when using lots
-    of nodes.
-    
-    Makes a tileDir (directory containing .fits images, one per tile) file, if the needed parameters are 
-    given in parDict. Adjusts unfilteredMapsDictList accordingly and returns it.
-    
-    If the options for making a tileDir image aren't given in parDict, then we pass through a standard
-    single extension file (or rather the path to it, as originally given)
-    
-    NOTE: If the map given in unfilteredMaps is 3d (enki gives I, Q, U as a datacube), then this will extract
-    only the I (temperature) part and save that in the tileDir file. This will need changing if hunting for
-    polarized sources...
-    
-    Returns unfilteredMapsDictList [input for filterMaps], list of extension names, dictionary of clip coords
-    
-    NOTE: Under MPI, this should only be called by the rank = 0 process
-    
-    """
-    
-    if 'makeTileDir' not in list(parDict.keys()):
-        parDict['makeTileDir']=False
-    
-    # Some of this is rather clunky...
-    unfilteredMapsDictList=[]
-    clipCoordsDict={}
-    if parDict['makeTileDir'] == False:
-        tileNames=[]        
-        for mapDict in parDict['unfilteredMaps']:
-            unfilteredMapsDictList.append(mapDict.copy())
-            with pyfits.open(mapDict['mapFileName']) as img:
-                if tileNames == []:
-                    for ext in img:
-                        if img[ext].data is not None:
-                            tileNames.append(ext.name)
-                            clipCoordsDict[ext.name]={'clippedSection': [0, ext.header['NAXIS1'], 0, ext.header['NAXIS2']],
-                                                      'header': ext.header,
-                                                      'areaMaskInClipSection': [0, ext.header['NAXIS1'], 0, ext.header['NAXIS2']]}
-                else:
-                    for ext in img:
-                        if ext.name not in tileNames:
-                            raise Exception("extension names do not match between all maps in unfilteredMapsDictList")
-    else:
-        tileNames=[]
-        wcs=None
-        for mapDict in parDict['unfilteredMaps']:
-            if 'tileDefLabel' in list(parDict.keys()):
-                tileDefLabel=parDict['tileDefLabel']
-            else:
-                tileDefLabel='userDefined'
-            tileDirFileNameLabel="%s_%.1f" % (tileDefLabel, parDict['tileOverlapDeg'])
-            
-            # Figure out what the input / output files will be called
-            # NOTE: we always need to make a survey mask if none exists, as used to zap over regions, so that gets special treatment
-            fileNameKeys=['mapFileName', 'weightsFileName', 'pointSourceMask', 'surveyMask']
-            inFileNames=[]
-            outFileNames=[]
-            mapTypeList=[]
-            for f in fileNameKeys:
-                if f in list(mapDict.keys()) and mapDict[f] is not None:
-                    inFileNames.append(mapDict[f])
-                    mapDir, mapFileName=os.path.split(mapDict[f])
-                    if mapDir != '':
-                        mapDirStr=mapDir+os.path.sep
-                    else:
-                        mapDirStr=''
-                    outFileNames.append(mapDirStr+"tileDir_%s_" % (tileDirFileNameLabel)+mapFileName)
-                    mapTypeList.append(f)
-            if 'surveyMask' not in mapTypeList:
-                inFileNames.append(None)
-                mapTypeList.append('surveyMask')
-                outFileNames.append('tileDir_%s_surveyMask' % (tileDirFileNameLabel))
-
-            if wcs is None:
-                wcsPath=parDict['unfilteredMaps'][0]['mapFileName']
-                # Allows compressed format (yes, we should tidy this up properly...)
-                with pyfits.open(wcsPath) as img:
-                    for extName in img:
-                        if img[extName].data is not None:
-                            break
-                    wcs=astWCS.WCS(img[extName].header, mode = 'pyfits')
-                
-            # Extract tile definitions (may have been inserted by autotiler before calling here)
-            tileNames=[]
-            coordsList=[]
-            for tileDict in parDict['tileDefinitions']:
-                ra0, ra1, dec0, dec1=tileDict['RADecSection']
-                x0, y0=wcs.wcs2pix(ra0, dec0)
-                x1, y1=wcs.wcs2pix(ra1, dec1)
-                xMin=min([x0, x1])
-                xMax=max([x0, x1])
-                yMin=min([y0, y1])
-                yMax=max([y0, y1])
-                coordsList.append([xMin, xMax, yMin, yMax])
-                tileNames.append(tileDict['tileName'])   
-            
-            # Make tiles
-            # NOTE: we accommodate having user-defined regions for calculating noise power in filters here
-            # Since we would only use such an option with tileDir files, this should be okay
-            # Although since we do this by modifying headers, would need to remake tileDir files each time adjusted in .par file
-            # NOTE: now treating surveyMask as special, and zapping overlap regions there (simplify selection function stuff later)
-            tileOverlapDeg=parDict['tileOverlapDeg']
-            for mapType, inMapFileName, outMapFileName in zip(mapTypeList, inFileNames, outFileNames):
-                mapData=None    # only load the map if we have to
-                if writeToDisk == True:
-                    os.makedirs(outMapFileName, exist_ok = True)
-                for c, name, tileDict in zip(coordsList, tileNames, parDict['tileDefinitions']):
-                    tileFileName=outMapFileName+os.path.sep+name+".fits"
-                    
-                    # If config or map was modified more recently than tile was written, re-write tile
-                    # (this is a fairly blunt instrument, but should be a little more user friendly)
-                    writeNewTileFile=False
-                    if os.path.exists(tileFileName) == True:
-                        if '_file_last_modified_ctime' in parDict.keys():
-                            if parDict['_file_last_modified_ctime'] > os.path.getctime(tileFileName):
-                                writeNewTileFile=True
-                            if inMapFileName is not None and parDict['_file_last_modified_ctime'] > os.path.getctime(inMapFileName):
-                                writeNewTileFile=True
-                            
-                    if mapData is None:
-                        # Special handling for case where surveyMask not supplied
-                        if mapType == 'surveyMask' and inMapFileName is None:
-                            with pyfits.open(inFileNames[0]) as img:
-                                for extName in img:
-                                    mapData=img[extName].data
-                                    if mapData is not None:
-                                        break
-                                mapData=np.ones(img[extName].data.shape, dtype = int)
-                        else:
-                            # Allows compressed format masks
-                            with pyfits.open(inMapFileName) as img:
-                                for extName in img:
-                                    mapData=img[extName].data
-                                    if mapData is not None:
-                                        break
-                                mapData=img[extName].data
-                        # Deal with Sigurd's maps which have T, Q, U as one 3d array
-                        # If anyone wants to find polarized sources, this will need changing...
-                        if mapData.ndim == 3:
-                            mapData=mapData[0, :]
-                    # Defining clip region
-                    y0=c[2]
-                    y1=c[3]
-                    x0=c[0]
-                    x1=c[1]
-                    ra0, dec0=wcs.pix2wcs(x0, y0)
-                    ra1, dec1=wcs.pix2wcs(x1, y1)
-                    # Be careful with signs here... and we're assuming approx pixel size is ok
-                    if x0-tileOverlapDeg/wcs.getPixelSizeDeg() > 0:
-                        ra0=ra0+tileOverlapDeg
-                    if x1+tileOverlapDeg/wcs.getPixelSizeDeg() < mapData.shape[1]:
-                        ra1=ra1-tileOverlapDeg
-                    if y0-tileOverlapDeg/wcs.getPixelSizeDeg() > 0:
-                        dec0=dec0-tileOverlapDeg
-                    if y1+tileOverlapDeg/wcs.getPixelSizeDeg() < mapData.shape[0]:
-                        dec1=dec1+tileOverlapDeg
-                    if ra1 > ra0:
-                        ra1=-(360-ra1)
-                    clip=astImages.clipUsingRADecCoords(mapData, wcs, ra1, ra0, dec0, dec1)
-                    
-                    # This bit is necessary to avoid Q -> 0.2 ish problem with Fourier filter
-                    # (which happens if image dimensions are both odd)
-                    # I _think_ this is related to the interpolation done in signals.fitQ
-                    if (clip['data'].shape[0] % 2 != 0 and clip['data'].shape[1] % 2 != 0) == True:
-                        newArr=np.zeros([clip['data'].shape[0]+1, clip['data'].shape[1]])
-                        newArr[:clip['data'].shape[0], :]=clip['data']
-                        newWCS=clip['wcs'].copy()
-                        newWCS.header['NAXIS1']=newWCS.header['NAXIS1']+1
-                        newWCS.updateFromHeader()
-                        testClip=astImages.clipUsingRADecCoords(newArr, newWCS, ra1, ra0, dec0, dec1)
-                        # Check if we see the same sky, if not and we trip this, we need to think about this more
-                        assert((testClip['data']-clip['data']).sum() == 0)
-                        clip['data']=newArr
-                        clip['wcs']=newWCS
-                    
-                    # Storing clip coords etc. so can stitch together later
-                    # areaMaskSection here is used to define the region that would be kept (takes out overlap)
-                    ra0, dec0=wcs.pix2wcs(x0, y0)
-                    ra1, dec1=wcs.pix2wcs(x1, y1)
-                    clip_x0, clip_y0=clip['wcs'].wcs2pix(ra0, dec0)
-                    clip_x1, clip_y1=clip['wcs'].wcs2pix(ra1, dec1)
-                    clip_x0=int(round(clip_x0))
-                    clip_x1=int(round(clip_x1))
-                    clip_y0=int(round(clip_y0))
-                    clip_y1=int(round(clip_y1))
-                    if name not in clipCoordsDict:
-                        clipCoordsDict[name]={'clippedSection': clip['clippedSection'], 'header': clip['wcs'].header,
-                                              'areaMaskInClipSection': [clip_x0, clip_x1, clip_y0, clip_y1]}
-                    else:
-                        assert(clipCoordsDict[name]['clippedSection'] == clip['clippedSection'])
-                    print("... adding %s [%d, %d, %d, %d ; %d, %d] ..." % (name, ra1, ra0, dec0, dec1, ra0-ra1, dec1-dec0))
-                    header=clip['wcs'].header#.copy()
-                    if 'tileNoiseRegions' in list(parDict.keys()):
-                        if name in list(parDict['tileNoiseRegions'].keys()):
-                            noiseRAMin, noiseRAMax, noiseDecMin, noiseDecMax=parDict['tileNoiseRegions'][name]
-                        else:
-                            if 'autoBorderDeg' in parDict['tileNoiseRegions']:
-                                autoBorderDeg=parDict['tileNoiseRegions']['autoBorderDeg']
-                                for tileDef in parDict['tileDefinitions']:
-                                    if tileDef['tileName'] == name:
-                                        break
-                                noiseRAMin, noiseRAMax, noiseDecMin, noiseDecMax=tileDef['RADecSection']
-                                noiseRAMin=noiseRAMin+autoBorderDeg
-                                noiseRAMax=noiseRAMax-autoBorderDeg
-                                noiseDecMin=noiseDecMin+autoBorderDeg
-                                noiseDecMax=noiseDecMax-autoBorderDeg
-                            else:
-                                raise Exception("No entry in tileNoiseRegions in config file for tileName '%s' - either add one, or add 'autoBorderDeg': 0.5 (or similar) to tileNoiseRegions" % (name))
-                        print("... adding noise region [%.3f, %.3f, %.3f, %.3f] to header %s ..." % (noiseRAMin, noiseRAMax, noiseDecMin, noiseDecMax, name))
-                        header['NRAMIN']=noiseRAMin
-                        header['NRAMAX']=noiseRAMax
-                        header['NDEMIN']=noiseDecMin
-                        header['NDEMAX']=noiseDecMax
-                    # Survey mask is special: zap overlap regions outside of tile definitions
-                    if mapType == 'surveyMask':
-                        clip_x0, clip_x1, clip_y0, clip_y1=clipCoordsDict[name]['areaMaskInClipSection']
-                        zapMask=np.zeros(clip['data'].shape)
-                        zapMask[clip_y0:clip_y1, clip_x0:clip_x1]=1.
-                        clip['data']=clip['data']*zapMask
-                    if (os.path.exists(tileFileName) == False or writeNewTileFile == True)  and writeToDisk == True:
-                        if mapType == 'surveyMask' or mapType == 'pointSourceMask':
-                            saveFITS(tileFileName, clip['data'], clip['wcs'], compressed = True,
-                                     compressionType = 'PLIO_1')
-                        else:
-                            saveFITS(tileFileName, clip['data'], clip['wcs'])
-                                
-            # Replace entries in unfilteredMapsDictList in place
-            for key, outFileName in zip(mapTypeList, outFileNames):
-                mapDict[key]=outFileName
-            unfilteredMapsDictList.append(mapDict.copy())
-        
-    return unfilteredMapsDictList, tileNames, clipCoordsDict
 
 #-------------------------------------------------------------------------------------------------------------
 def shrinkWCS(origShape, origWCS, scaleFactor):
     """Given an astWCS object and corresponding image shape, scale the WCS by scaleFactor. Used for making 
     downsampled quicklook images (using stitchMaps).
     
     Args:
@@ -580,60 +863,125 @@
     scaledWCS.header['CD1_2']=scaledCDMatrix[0][1]
     scaledWCS.header['CD2_2']=scaledCDMatrix[1][1]
     scaledWCS.updateFromHeader()
     
     return scaledShape, scaledWCS
 
 #-------------------------------------------------------------------------------------------------------------
-def checkMask(fileName):
+def chunkLoadMask(fileName, numChunks = 8, dtype = np.uint8, returnWCS = True):
+    """Load a FITS-format mask file (with default 8-bit integer values) in chunks, for memory efficiency,
+    at the expense of some speed. Masks in compressed format (see :meth:`saveFITS`) are supported.
+
+    Args:
+        fileName (:obj:`str`): Path to the FITS-format mask file.
+        numChunks (:obj:`int`): Number of chunks in which to load the file. Largers numbers use less memory,
+            but it takes a little longer for the mask to load.
+        returnWCS (:obj:`bool`, optional): If given, return the WCS of the mask.
+
+    Returns:
+        Mask image (2d array of 8-bit unsigned integers), and optionally a WCS object.
+
+    Note:
+        This can also be used to load large compressed maps in a memory-efficient way by setting
+        ``dtype = np.float32``.
+
+    """
+
+    shape=None
+    with pyfits.open(fileName) as img:
+        for hdu in img:
+            if hdu.data is not None:
+                shape=hdu.data.shape
+                if returnWCS == True:
+                    wcs=astWCS.WCS(hdu.header, mode = 'pyfits')
+                break
+    del img
+
+    height=shape[0]
+    chunkSize=int(height/numChunks)
+    maskArr=np.zeros(shape, dtype = dtype)
+    for i in range(numChunks):
+        with pyfits.open(fileName) as img:
+            for hdu in img:
+                if hdu.data is not None:
+                    start=i*chunkSize
+                    end=(i+1)*chunkSize
+                    if end >= height:
+                        end=height-1
+                    chunk=hdu.data[start:end]
+                    maskArr[start:end]=chunk
+                    del chunk
+            del hdu.data
+        del img
+
+    if returnWCS == True:
+        return maskArr, wcs
+    else:
+        return maskArr
+
+#-------------------------------------------------------------------------------------------------------------
+def checkMask(fileName, numChunks = 8):
     """Checks whether a mask contains negative values (invalid) and throws an exception if this is the case.
     
     Args:
-        fileName (str): Name of the .fits format mask file to check
+        fileName (str): Name of the FITS format mask file to check.
         
     """
-    
+
+    # This is now more horrid looking to save memory, at the expense of speed
+    height=None
     with pyfits.open(fileName) as img:
         for hdu in img:
             if hdu.data is not None:
-                if np.less(hdu.data, 0).sum() > 0:
-                    raise Exception("Mask file '%s' contains negative values - please fix your mask." % (fileName))
+                height=hdu.data.shape[0]
+    del img
+
+    chunkSize=int(height/numChunks)
+    for i in range(numChunks):
+        with pyfits.open(fileName) as img:
+            for hdu in img:
+                if hdu.data is not None:
+                    start=i*chunkSize
+                    end=(i+1)*chunkSize
+                    if end >= height:
+                        end=height-1
+                    chunk=hdu.data[start:end].flatten()
+                    if np.any(chunk < 0) == True:
+                        raise Exception("Mask file '%s' contains negative values - please fix your mask." % (fileName))
+                    del chunk
+            del hdu.data
+        del img
 
 #-------------------------------------------------------------------------------------------------------------
 def stitchTiles(config):
     """Stitches together full size filtered maps, SN maps, area maps, and noise maps that have been previously
     been saved as tiles.
     
     """
     
     # Defining the maps to stitch together and where they will go
     stitchDictList=[{'pattern': config.filteredMapsDir+os.path.sep+"$TILENAME"+os.path.sep+"$FILTLABEL#$TILENAME_filteredMap.fits",
                      'outFileName': config.filteredMapsDir+os.path.sep+"stitched_$FILTLABEL_filteredMap.fits",
-                     'compressed': False,
                      'compressionType': None},
                     {'pattern': config.filteredMapsDir+os.path.sep+"$TILENAME"+os.path.sep+"$FILTLABEL#$TILENAME_SNMap.fits",
                      'outFileName': config.filteredMapsDir+os.path.sep+"stitched_$FILTLABEL_SNMap.fits",
-                     'compressed': False,
                      'compressionType': None},
-                    {'pattern': config.selFnDir+os.path.sep+"areaMask#$TILENAME.fits",
-                     'outFileName': config.selFnDir+os.path.sep+"stitched_areaMask.fits",
-                     'compressed': True,
-                     'compressionType': 'PLIO_1'},
-                    {'pattern': config.selFnDir+os.path.sep+"RMSMap_$FILTLABEL#$TILENAME.fits",
+                    {'pattern': config.selFnDir+os.path.sep+"$TILENAME"+os.path.sep+"RMSMap_$FILTLABEL#$TILENAME.fits",
                      'outFileName': config.selFnDir+os.path.sep+"stitched_RMSMap_$FILTLABEL.fits",
-                     'compressed': True,
                      'compressionType': 'RICE_1'}]
 
     tileCoordsDict=config.tileCoordsDict
     for filterDict in config.parDict['mapFilters']:
         if 'saveFilteredMaps' in filterDict['params'].keys() and filterDict['params']['saveFilteredMaps'] == True:
             for stitchDict in stitchDictList:
                 pattern=stitchDict['pattern']
                 outFileName=stitchDict['outFileName'].replace("$FILTLABEL", filterDict['label'])
-                compressed=stitchDict['compressed']
+                if os.path.exists(outFileName) == True:
+                    print("... stitched map %s already exists - skipping" % (outFileName))
+                    continue
                 compressionType=stitchDict['compressionType']
                 d=np.zeros([config.origWCS.header['NAXIS2'], config.origWCS.header['NAXIS1']])
                 wcs=config.origWCS
                 for tileName in tileCoordsDict.keys():
                     f=pattern.replace("$TILENAME", tileName).replace("$FILTLABEL", filterDict['label'])
                     if os.path.exists(f) == True:
                         # Handle compressed or otherwise
@@ -645,18 +993,36 @@
                                     if tileData is not None:
                                         break
                             assert tileData is not None
                     else:
                         continue
                     areaMask, areaWCS=completeness.loadAreaMask(tileName, config.selFnDir)
                     minX, maxX, minY, maxY=config.tileCoordsDict[tileName]['clippedSection']
-                    # Accounting for tiles that may have been extended by 1 pix for FFT purposes (Q-related)
+                    # Accounting for tiles that may have been extended by 1 pix for FFT purposes (Q-related, may no longer be relevant)
                     height=maxY-minY; width=maxX-minX
+                    # Check if we reprojected to TAN and if so, go back to CAR
+                    if tileCoordsDict[tileName]['reprojectToTan'] == True:
+                        carWCS=astWCS.WCS(config.tileCoordsDict[tileName]['header'], mode = 'pyfits')
+                        tanWCS=_makeTanWCS(carWCS) # this should match areaWCS actually
+                        shape=[config.tileCoordsDict[tileName]['header']['NAXIS2'],
+                               config.tileCoordsDict[tileName]['header']['NAXIS1']]
+                        if compressionType == 'PLIO_1':
+                            order=0
+                        else:
+                            order='bicubic'
+                        carData, footprint=reproject.reproject_interp((tileData, tanWCS.AWCS), carWCS.AWCS,
+                                                                      shape_out = shape, order = order,
+                                                                      return_footprint = True)
+                        carData[footprint == 0]=0 # get rid of nans which will be in borders anyway
+                        tileData=carData
+                        areaMask=reproject.reproject_interp((areaMask, tanWCS.AWCS), carWCS.AWCS,
+                                                             shape_out = shape, order = 0, return_footprint = False)
+                        areaMask[footprint == 0]=0
                     d[minY:maxY, minX:maxX]=d[minY:maxY, minX:maxX]+areaMask[:height, :width]*tileData[:height, :width]
-                saveFITS(outFileName, d, wcs, compressed = compressed, compressionType = compressionType)
+                saveFITS(outFileName, d, wcs, compressionType = compressionType)
 
 #-------------------------------------------------------------------------------------------------------------
 def stitchTilesQuickLook(filePattern, outFileName, outWCS, outShape, fluxRescale = 1.0):
     """Fast routine for stitching map tiles back together. Since this uses interpolation, you probably don't 
     want to do analysis on the output - this is just for checking / making plots etc.. This routine sums 
     images as it pastes them into the larger map grid. So, if the zeroed (overlap) borders are not handled,
     correctly, this will be obvious in the output.
@@ -704,15 +1070,15 @@
         xOut=np.array(RAToX(inRA), dtype = int)
         yOut=np.array(DecToY(inDec), dtype = int)
         for i in range(len(yOut)):
             try:
                 outData[yOut[i]][xOut]=outData[yOut[i]][xOut]+d[yIn[i], xIn]
             except:
                 raise Exception("Output pixel coords invalid - if you see this, probably outWCS.header has keywords that confuse astropy.wcs (PC1_1 etc. - in old ACT maps)")
-    saveFITS(outFileName, outData*fluxRescale, outWCS, compressed = True)
+    saveFITS(outFileName, outData*fluxRescale, outWCS, compressionType = 'RICE_1')
 
 #-------------------------------------------------------------------------------------------------------------
 def maskOutSources(mapData, wcs, catalog, radiusArcmin = 7.0, mask = 0.0, growMaskedArea = 1.0):
     """Given a mapData array and a catalog of source positions, replace the values at the object positions 
     in the map within radiusArcmin with replacement values. If mask == 'whiteNoise', this will be white
     noise with mean and sigma set by the pixel values in an annulus of 1 < r < 2 * radiusArcmin.
     
@@ -731,17 +1097,17 @@
     mapInterpolator=interpolate.RectBivariateSpline(np.arange(mapData.shape[0]), 
                                                 np.arange(mapData.shape[1]), 
                                                 bckSubbed, kx = 1, ky = 1)
 
     for obj in catalog:
         if wcs.coordsAreInImage(obj['RADeg'], obj['decDeg']) == True:
             degreesMap=np.ones(mapData.shape, dtype = float)*1e6
-            rRange, xBounds, yBounds=nemoCython.makeDegreesDistanceMap(degreesMap, wcs, 
-                                                                       obj['RADeg'], obj['decDeg'], 
-                                                                       20.0/60.0)         
+            rRange, xBounds, yBounds=makeDegreesDistanceMap(degreesMap, wcs,
+                                                            obj['RADeg'], obj['decDeg'],
+                                                            20.0/60.0)
             circleMask=np.less(rRange, radiusArcmin/60.0)
             grownCircleMask=np.less(rRange, (radiusArcmin*growMaskedArea)/60.0)
             maskMap[grownCircleMask]=1.0
             if type(mask) == float or type(mask) == int:
                 maskedMapData[circleMask]=mask
 
             elif mask == 'shuffle':
@@ -819,17 +1185,17 @@
             print("Add code to subtract point sources")
             ipshell()
             sys.exit()
         elif mask == "whiteNoise":
             RADeg, decDeg=mapWCS.pix2wcs(pos[1], pos[0])
             if np.isnan(RADeg) == False and np.isnan(decDeg) == False:
                 degreesMap=np.ones(mapData.shape, dtype = float)*1e6
-                rRange, xBounds, yBounds=nemoCython.makeDegreesDistanceMap(degreesMap, mapWCS, 
-                                                                           RADeg, decDeg, 
-                                                                           (radiusArcmin*4)/60.0)        
+                rRange, xBounds, yBounds=makeDegreesDistanceMap(degreesMap, mapWCS,
+                                                                RADeg, decDeg,
+                                                                (radiusArcmin*4)/60.0)
                 # Get pedestal level and white noise level from average between radiusArcmin and  2*radiusArcmin
                 annulusMask=np.logical_and(np.greater(rRange, radiusArcmin/60.0), \
                                               np.less(rRange, 2*radiusArcmin/60.0))
                 # Below just does a quick sanity check - we don't bother masking if std == 0, because we're
                 # most likely applying this in the middle of a fake source sim with map set to zero for testing
                 sigma=mapData[annulusMask].std()
                 if sigma > 0:
@@ -845,349 +1211,147 @@
     
     """
     
     noise=np.random.normal(0, noisePerPix, mapData.shape)
     mapData=mapData+noise
     
     return mapData
-    
-#-------------------------------------------------------------------------------------------------------------
-def preprocessMapDict(mapDict, tileName = 'PRIMARY', diagnosticsDir = None):
-    """Applies a number of pre-processing steps to the map described by `mapDict`, prior to filtering.
-    
-    The first step is to load the map itself and the associated weights. Some other operations that may be 
-    applied are controlled by keys added to `mapDict`. Some of these may be specified in the .yml configuration
-    file, while others are applied by particular filter objects or by routines that generate simulated data. 
-    The following keys are understood:
-    
-    surveyMask (:obj:`str`)
-        Path to a mask (.fits image; 1 = valid, 0 = masked) that defines the valid object search area.
-    
-    pointSourceMask (:obj:`str`) 
-        Path to a mask (.fits image; 1 = valid, 0 = masked) that contains holes at the locations of point
-        sources, defining regions that are excluded from the object search area.
-        
-    RADecSection (:obj:`list`)
-        Defines a region to extract from the map. Use the format [RAMin, RAMax, decMin, decMax] (units: 
-        decimal degrees).
-        
-    CMBSimSeed (:obj:`int`)
-        If present, replace the map with a source-free simulated CMB realisation, generated using the given
-        seed number. Used by :meth:`estimateContaminationFromSkySim`.
-    
-    applyBeamConvolution (:obj: `str`)
-        If True, the map is convolved with the beam given in the beamFileName key. This should only be 
-        needed when using preliminary y-maps made by tILe-C.
-            
-    Args:
-        mapDict (:obj:`dict`): A dictionary with the same keys as given in the unfilteredMaps list in the 
-            .yml configuration file (i.e., it must contain at least the keys 'mapFileName', 'units', and
-            'weightsFileName', and may contain some of the optional keys listed above).
-        tileName (:obj:`str`): Name of the map tile (extension name) to operate on.
-        diagnosticsDir (:obj:`str`): Path to a directory where miscellaneous diagnostic data are written.
-    
-    Returns:
-        A dictionary with keys that point to the map itself ('data'), weights ('weights'), masks 
-        ('surveyMask', 'pointSourceMask'), and WCS object ('wcs').
-    
-    """
-    
-    data, wcs=loadTile(mapDict['mapFileName'], tileName, returnWCS = True)
-        
-    # Optional calibration factor
-    if 'calibFactor' in mapDict.keys():
-        data=data*mapDict['calibFactor']
-    
-    # For Enki maps... take only I (temperature) for now, add options for this later
-    if data.ndim == 3:
-        data=data[0, :]
-    if mapDict['units'] == 'Jy/sr':
-        if mapDict['obsFreqGHz'] == 148:
-            data=(data/1.072480e+09)*2.726*1e6
-        elif mapDict['obsFreqGHz'] == 219:
-            data=(data/1.318837e+09)*2.726*1e6
-        else:
-            raise Exception("no code added to support conversion to uK from Jy/sr for freq = %.0f GHz" \
-                    % (mapDict['obsFreqGHz']))
-
-    # Load weight map if given
-    if 'weightsFileName' in list(mapDict.keys()) and mapDict['weightsFileName'] is not None:
-        weights=loadTile(mapDict['weightsFileName'], tileName)
-        # For Enki maps... take only I (temperature) for now, add options for this later
-        if weights.ndim == 3:       # I, Q, U
-            weights=weights[0, :]
-        elif weights.ndim == 4:     # I, Q, U and also a covariance matrix
-            weights=weights[0, 0, :]
-    else:
-        weights=np.ones(data.shape)
-
-    # We rely on pixels with zero weight having zero value in actual maps later (automated edge trimming)
-    # This might not be the case if the map has been filtered slightly before being fed into nemo
-    data[weights == 0]=0
-
-    # Load survey and point source masks, if given
-    if 'surveyMask' in list(mapDict.keys()) and mapDict['surveyMask'] is not None:
-        surveyMask=loadTile(mapDict['surveyMask'], tileName)
-    else:
-        surveyMask=np.ones(data.shape)
-        surveyMask[weights == 0]=0
-    
-    # Some apodisation of the data outside the survey mask
-    # NOTE: should add adjustable parameter for this somewhere later
-    if 'apodizeUsingSurveyMask' in list(mapDict.keys()) and mapDict['apodizeUsingSurveyMask'] == True:
-        # We need to remain unapodized to at least noiseGridArcmin beyond the edge of the survey mask
-        # We'll need to make these adjustable parameters
-        apodMask=np.array(surveyMask, dtype = bool)
-        for i in range(120):
-            apodMask=mahotas.dilate(apodMask)
-        apodMask=ndimage.gaussian_filter(np.array(apodMask, dtype = float), 20)
-        data=data*apodMask
-        del apodMask
-
-    if 'pointSourceMask' in list(mapDict.keys()) and mapDict['pointSourceMask'] is not None:
-        psMask=loadTile(mapDict['pointSourceMask'], tileName)
-    else:
-        psMask=np.ones(data.shape)
-                
-    # Optional map clipping
-    if 'RADecSection' in list(mapDict.keys()) and mapDict['RADecSection'] is not None:
-        RAMin, RAMax, decMin, decMax=mapDict['RADecSection']
-        clip=astImages.clipUsingRADecCoords(data, wcs, RAMin, RAMax, decMin, decMax)
-        data=clip['data']
-        whtClip=astImages.clipUsingRADecCoords(weights, wcs, RAMin, RAMax, decMin, decMax)
-        weights=whtClip['data']
-        psClip=astImages.clipUsingRADecCoords(psMask, wcs, RAMin, RAMax, decMin, decMax)
-        psMask=psClip['data']
-        surveyClip=astImages.clipUsingRADecCoords(surveyMask, wcs, RAMin, RAMax, decMin, decMax)
-        surveyMask=surveyClip['data']
-        wcs=clip['wcs']
-        if len(clip['data']) == 0:
-            raise Exception("Clipping using RADecSection returned empty array - check RADecSection in config .yml file is in map")
-        #astImages.saveFITS(diagnosticsDir+os.path.sep+'%d' % (mapDict['obsFreqGHz'])+"_weights.fits", weights, wcs)
-    
-    # For source-free simulations (contamination tests)
-    if 'CMBSimSeed' in list(mapDict.keys()):
-        randMap=simCMBMap(data.shape, wcs, noiseLevel = 0, beamFileName = mapDict['beamFileName'], 
-                          seed = mapDict['CMBSimSeed'])
-        randMap[np.equal(weights, 0)]=0
-        # Add white noise that varies according to inv var map...
-        # Noise needed is the extra noise we need to add to match the real data, scaled by inv var map
-        # This initial estimate is too high, so we use a grid search to get a better estimate
-        mask=np.nonzero(data)
-        dataSigma=data[mask].std()
-        whiteNoiseLevel=np.zeros(weights.shape)
-        whiteNoiseLevel[mask]=1/np.sqrt(weights[mask])
-        noiseNeeded=np.sqrt(data[mask].var()-randMap[mask].var()-np.median(whiteNoiseLevel[mask])**2)
-        noiseBoostFactor=noiseNeeded/np.median(whiteNoiseLevel[mask])
-        # NOTE: disabled finding boost factor below for now...
-        bestBoostFactor=1.
-        # --- disabled
-        #bestDiff=1e6
-        #bestBoostFactor=noiseBoostFactor
-        #simNoiseValues=simNoise[mask]
-        #for boostFactor in np.linspace(noiseBoostFactor*0.5, noiseBoostFactor, 10):
-            #diff=abs(dataSigma-(simNoiseValues+generatedNoise*boostFactor).std())
-            #if diff < bestDiff:
-                #bestBoostFactor=boostFactor
-                #bestDiff=diff
-        # ---
-        data[mask]=np.random.normal(randMap[mask], bestBoostFactor*whiteNoiseLevel[mask], 
-                                    whiteNoiseLevel[mask].shape)
-        outFileName=diagnosticsDir+os.path.sep+"CMBSim_%d#%s.fits" % (mapDict['obsFreqGHz'], tileName) 
-        saveFITS(outFileName, data, wcs)
-    
-    # For position recovery tests
-    if 'injectSources' in list(mapDict.keys()):
-        # NOTE: Need to add varying GNFWParams here
-        if 'GNFWParams' in mapDict['injectSources'].keys():
-            GNFWParams=mapDict['injectSources']['GNFWParams']
-            obsFreqGHz=mapDict['obsFreqGHz']
-        else:
-            GNFWParams=None
-            obsFreqGHz=None
-        modelMap=makeModelImage(data.shape, wcs, mapDict['injectSources']['catalog'], 
-                                mapDict['beamFileName'], obsFreqGHz = obsFreqGHz, 
-                                GNFWParams = GNFWParams,
-                                override = mapDict['injectSources']['override'])
-        modelMap[weights == 0]=0
-        data=data+modelMap
-
-    # Should only be needed for handling preliminary tILe-C maps
-    if 'applyBeamConvolution' in mapDict.keys() and mapDict['applyBeamConvolution'] == True:
-        data=convolveMapWithBeam(data, wcs, mapDict['beamFileName'], maxDistDegrees = 1.0)
-        if diagnosticsDir is not None:
-            saveFITS(diagnosticsDir+os.path.sep+"beamConvolved#%s.fits" % (tileName), data, wcs)
-            
-    # Optional smoothing with a Gaussian kernel (for approximate PSF-matching)
-    # NOTE: Turns out this is not good enough for real ACT beams - use full convolution kernel instead (see below)
-    #if 'smoothScaleDeg' in mapDict.keys():
-        #if 'smoothAttenuationFactor' in mapDict.keys():
-            #data=data*mapDict['smoothAttenuationFactor']
-        #data=smoothMap(data, wcs, RADeg = 'centre', decDeg = 'centre', smoothScaleDeg = mapDict['smoothScaleDeg'])
-    if 'smoothKernel' in mapDict.keys():
-        if 'smoothAttenuationFactor' in mapDict.keys():
-            data=data*mapDict['smoothAttenuationFactor']
-        data=convolveMapWithBeam(data, wcs, mapDict['smoothKernel'], maxDistDegrees = 1.0)
-                
-    # Optional masking of point sources from external catalog
-    # Especially needed if using Fourier-space matched filter (and maps not already point source subtracted)
-    if 'maskPointSourcesFromCatalog' in list(mapDict.keys()) and mapDict['maskPointSourcesFromCatalog'] is not None:  
-        # This is fast enough if using small tiles and running in parallel...
-        # If our masking/filling is effective enough, we may not need to mask so much here...
-        if type(mapDict['maskPointSourcesFromCatalog']) is not list:
-            mapDict['maskPointSourcesFromCatalog']=[mapDict['maskPointSourcesFromCatalog']]
-        psMask=np.ones(data.shape)
-        pixRad=(10.0/60.0)/wcs.getPixelSizeDeg()
-        bckData=ndimage.median_filter(data, int(pixRad))
-        rArcminMap=np.ones(data.shape, dtype = float)*1e6
-        for catalogInfo in mapDict['maskPointSourcesFromCatalog']:
-            if type(catalogInfo) == str:
-                catalogPath=catalogInfo
-                fluxCutJy=0.0
-            elif type(catalogInfo) == dict:
-                catalogPath=catalogInfo['path']
-                fluxCutJy=catalogInfo['fluxCutJy']
-            else:
-                raise Exception("Didn't understand contents of 'maskPointSourcesFromCatalog' - should be a path, or a dict with 'path' key.")
-            tab=atpy.Table().read(catalogPath)
-            if 'fluxJy' in tab.keys():
-                tab=tab[tab['fluxJy'] > fluxCutJy]
-            tab=catalogs.getCatalogWithinImage(tab, data.shape, wcs)
-            # If we're given a catalog that already has rArcmin in it, we use that to set hole size
-            # Otherwise, if we have shape measurements (ellipse_A at least), we can use that
-            for row in tab:
-                # Extended sources - identify by measured size > masking radius
-                # These will mess up noise term in filter, so add to psMask also and fill + smooth
-                # We won't fiddle with PA here, we'll just maximise based on x-pixel scale (because CAR)
-                if 'rArcmin' in tab.keys():
-                    maskRadiusArcmin=row['rArcmin']
-                elif 'ellipse_A' in tab.keys():
-                    xPixSizeArcmin=(wcs.getXPixelSizeDeg()/np.cos(np.radians(row['decDeg'])))*60
-                    ASizeArcmin=row['ellipse_A']/xPixSizeArcmin
-                    maskRadiusArcmin=ASizeArcmin/2
-                else:
-                    raise Exception("To mask sources in a catalog, need either 'rArcmin' or 'ellipse_A' column to be present.")
-                rArcminMap, xBounds, yBounds=nemoCython.makeDegreesDistanceMap(rArcminMap, wcs, 
-                                                                                row['RADeg'], row['decDeg'],
-                                                                                maskRadiusArcmin/60)
-                rArcminMap=rArcminMap*60
-                surveyMask[rArcminMap < maskRadiusArcmin]=0
-                psMask[rArcminMap < maskRadiusArcmin]=0
-                data[rArcminMap < maskRadiusArcmin]=bckData[rArcminMap < maskRadiusArcmin]
-
-    # Optional subtraction of point sources based on a catalog
-    # We'll also (optionally) add a small mask at these locations to the survey mask
-    if 'subtractPointSourcesFromCatalog' in list(mapDict.keys()) and mapDict['subtractPointSourcesFromCatalog'] is not None:
-        if type(mapDict['subtractPointSourcesFromCatalog']) is not list:
-            mapDict['subtractPointSourcesFromCatalog']=[mapDict['subtractPointSourcesFromCatalog']]
-        for tab in mapDict['subtractPointSourcesFromCatalog']:
-            if type(tab) != atpy.Table:
-                tab=atpy.Table().read(catalogPath)
-            tab=catalogs.getCatalogWithinImage(tab, data.shape, wcs) 
-            model=makeModelImage(data.shape, wcs, tab, mapDict['beamFileName'], obsFreqGHz = None)
-            if model is not None:
-                data=data-model
-            # Optionally blank small exclusion zone around these sources in survey mask
-            # (this is needed for SZ searches, to avoid any issue with possible oversubtraction)
-            # NOTE: Also masking and filling extended sources (no other way to deal with right now) - these are rare
-            if 'maskSubtractedPointSources' in list(mapDict.keys()) and mapDict['maskSubtractedPointSources'] == True:
-                # For hole filling extended sources
-                pixRad=(10.0/60.0)/wcs.getPixelSizeDeg()
-                bckData=ndimage.median_filter(data, int(pixRad))
-                for row in tab:
-                    x, y=wcs.wcs2pix(row['RADeg'], row['decDeg'])
-                    if surveyMask[int(y), int(x)] != 0:
-                        rArcminMap=np.ones(data.shape, dtype = float)*1e6
-                        if row['SNR'] > 1000:
-                            maskRadiusArcmin=10.0
-                        else:
-                            maskRadiusArcmin=4.0
-                        # Extended sources - identify by measured size > masking radius
-                        # These will mess up noise term in filter, so add to psMask also and fill + smooth
-                        # We won't fiddle with PA here, we'll just maximise based on x-pixel scale (because CAR)
-                        extendedSource=False
-                        if 'ellipse_A' and 'ellipse_B' in tab.keys():
-                            xPixSizeArcmin=(wcs.getXPixelSizeDeg()/np.cos(np.radians(row['decDeg'])))*60
-                            ASizeArcmin=(row['ellipse_A']/xPixSizeArcmin)/2
-                            if ASizeArcmin > maskRadiusArcmin:
-                                extendedSource=True
-                                maskRadiusArcmin=ASizeArcmin
-                        if 'maskHoleDilationFactor' in mapDict.keys() and mapDict['maskHoleDilationFactor'] is not None:
-                            maskRadiusArcmin=maskRadiusArcmin*mapDict['maskHoleDilationFactor']
-                        rArcminMap, xBounds, yBounds=nemoCython.makeDegreesDistanceMap(rArcminMap, wcs, 
-                                                                                       row['RADeg'], row['decDeg'],
-                                                                                       maskRadiusArcmin/60)
-                        rArcminMap=rArcminMap*60
-                        surveyMask[rArcminMap < maskRadiusArcmin]=0
-                        if extendedSource == True:
-                            psMask[rArcminMap < maskRadiusArcmin]=0
-                            data[rArcminMap < maskRadiusArcmin]=bckData[rArcminMap < maskRadiusArcmin]
-    
-    # Add the map data to the dict
-    mapDict['data']=data
-    mapDict['weights']=weights
-    mapDict['wcs']=wcs
-    mapDict['surveyMask']=surveyMask
-    mapDict['psMask']=psMask
-    mapDict['tileName']=tileName
-    
-    # No point continuing if masks are different shape to map (easier to tell user here)
-    if mapDict['data'].shape != mapDict['psMask'].shape:
-        raise Exception("Map and point source mask dimensions are not the same (they should also have same WCS)")
-    if mapDict['data'].shape != mapDict['surveyMask'].shape:
-        raise Exception("Map and survey mask dimensions are not the same (they should also have same WCS)")
-    
-    return mapDict
 
 #------------------------------------------------------------------------------------------------------------
-def simCMBMap(shape, wcs, noiseLevel = 0.0, beamFileName = None, seed = None, fixNoiseSeed = False):
+def simCMBMap(shape, wcs, noiseLevel = None, beam = None, seed = None):
     """Generate a simulated CMB map, optionally convolved with the beam and with (white) noise added.
     
     Args:
         shape (:obj:`tuple`): A tuple describing the map (numpy array) shape in pixels (height, width).
         wcs (:obj:`astWCS.WCS`): An astWCS object.
         noiseLevel (:obj:`numpy.ndarray` or float): If a single number, this is taken as sigma (in map units,
             usually uK) for generating white noise that is added across the whole map. Alternatively, an array
             with the same dimensions as shape may be used, specifying sigma (in map units) per corresponding 
             pixel. Noise will only be added where non-zero values appear in noiseLevel.
-        beamFileName (:obj:`str`): The file name of the text file that describes the beam with which the map will be
-            convolved. If None, no beam convolution is applied.
+        beam (:obj:`str` or :obj:`signals.BeamProfile`): Either the file name of the text file that describes
+            the beam with which the map will be convolved, or a :obj:`signals.BeamProfile` object. If None,
+            no beam convolution is applied.
         seed (:obj:`int`): The seed used for the random CMB realisation.
-        fixNoiseSeed (:obj:`bool`): If True, forces white noise to be generated with given seed.
             
     Returns:
         A map (:obj:`numpy.ndarray`)
     
     """
+
+    # Power spectrum array ps here is indexed by ell, starting from 0
+    # i.e., each element corresponds to the power at ell = 0, 1, 2 ... etc.
+    ps=powspec.read_spectrum(nemo.__path__[0]+os.path.sep+"data"+os.path.sep+"planck_lensedCls.dat",
+                             scale = True, expand = None)
+    ps=ps[0]
+    lps=np.arange(0, len(ps))
+
+    if beam is not None:
+        if type(beam) == str:
+            beam=signals.BeamProfile(beamFileName = beam)
+        assert(type(beam) == signals.BeamProfile)
+        lbeam=np.interp(lps, beam.ell, beam.Bell)
+        ps*=lbeam
+
+    randMap=curvedsky.rand_map(shape, wcs.AWCS, ps = ps, spin = [0,2], seed = seed)
+
+    if noiseLevel is not None:
+        randMap=randMap+simNoiseMap(shape, noiseLevel)
+
+    np.random.seed()
     
-    from pixell import curvedsky, utils, powspec
-    
-    ps=powspec.read_spectrum(nemo.__path__[0]+os.path.sep+"data"+os.path.sep+"planck_lensedCls.dat", 
-                             scale = True)
-    randMap=curvedsky.rand_map(shape, wcs.AWCS, ps=ps, spin=[0,2], seed = seed)
-    if fixNoiseSeed == False:
-        np.random.seed()
-    
-    if beamFileName is not None:
-        randMap=convolveMapWithBeam(randMap, wcs, beamFileName)
+    return randMap
+
+#-------------------------------------------------------------------------------------------------------------
+def simNoiseMap(shape, noiseLevel, wcs = None, lKnee = None, alpha = -3, noiseMode = 'perPixel'):
+    """Generate a simulated noise map. This may contain just white noise, or optionally a 1/f noise component
+    can be generated.
+
+    Args:
+        shape (:obj:`tuple`): A tuple describing the map (numpy array) shape in pixels (height, width).
+        noiseLevel (:obj:`numpy.ndarray` or float): If a single number, this is taken as sigma (in map units,
+            usually uK) for generating white noise that is added across the whole map. Alternatively, an array
+            with the same dimensions as shape may be used, specifying sigma (in map units) per corresponding
+            pixel. Noise will only be added where non-zero values appear in noiseLevel.
+        lKnee (:obj:`float`): If given, 1/f noise will be generated using the power spectrum
+            N_l = (1 + l/lknee)^-alpha) - see Appendix A of MacCrann et al. 2023.
+        alpha (:obj:`float`): Power-law exponent in the power spectrum used for generating 1/f noise. Has
+            no effect unless lKnee is also given.
+        noiseMode(:obj:`str`): Either 'perPixel', or 'perSquareArcmin' - if the latter, constant noise in terms
+            of surface brightness will be added (accounts for varying pixel scale, if present).
+
+    Returns:
+        A map (:obj:`numpy.ndarray`)
+
+    """
+
+    np.random.seed()
 
-    if type(noiseLevel) == np.ndarray:
-        mask=np.nonzero(noiseLevel)
+    assert(noiseMode in ['perPixel', 'perSquareArcmin'])
+    if noiseMode == 'perSquareArcmin' and lKnee is not None:
+        raise Exception("Adding 1/f noise when noiseMode != 'perPixel' is not supported yet")
+    if noiseMode == 'perSquareArcmin' and type(noiseLevel) == np.ndarray:
+        raise Exception("noiseLevel is a map - this is only currently supported if noiseMode = 'perPixel' (noiseMode = 'perSquareArcmin' given)")
+
+    if lKnee is None:
+        # White noise only
+        randMap=np.zeros(shape)
         generatedNoise=np.zeros(randMap.shape)
-        generatedNoise[mask]=np.random.normal(0, noiseLevel[mask], noiseLevel[mask].shape)
+        if type(noiseLevel) == np.ndarray:
+            mask=np.nonzero(noiseLevel)
+            generatedNoise[mask]=np.random.normal(0, noiseLevel[mask], noiseLevel[mask].shape)
+        else:
+            if noiseLevel > 0:
+                if noiseMode == 'perPixel':
+                    generatedNoise=np.random.normal(0, noiseLevel, randMap.shape)
+                else:
+                    arcmin2Map=getPixelAreaArcmin2Map(shape, wcs)
+                    generatedNoise=np.random.normal(0, noiseLevel/arcmin2Map, randMap.shape)
         randMap=randMap+generatedNoise
+
     else:
-        if noiseLevel > 0:
-            generatedNoise=np.random.normal(0, noiseLevel, randMap.shape)
-            randMap=randMap+generatedNoise
-    
-    np.random.seed()
-    
+        # 1/f noise + white noise, using Niall's routines
+        mlmax=6000 # following config in Niall's code, could be made a parameter
+        if wcs is None:
+            raise Exception("wcs is None - need to supply a wcs to generate a noise map with 1/f noise included.")
+        if type(noiseLevel) == np.ndarray:
+            mask=noiseLevel > 1e-07
+            ivarMap=np.zeros(shape)
+            ivarMap[mask]=1/noiseLevel[mask]**2
+            ivarMap=enmap.enmap(ivarMap, wcs.AWCS)
+        else:
+            ivarMap=enmap.enmap(np.ones(shape)*(1/noiseLevel**2), wcs.AWCS)
+
+        def _mod_noise_map(ivar, Nl):
+            map1 = enmap.rand_gauss(ivar.shape, ivar.wcs)
+            lmax = len(Nl)-1
+            ainfo = sharp.alm_info(lmax)
+            alm = curvedsky.map2alm(map1, ainfo=ainfo)
+            map2 = curvedsky.alm2map(alm, np.zeros_like(map1))
+            map1 -= map2
+            ainfo.lmul(alm, Nl**0.5, alm)
+            map2 = curvedsky.alm2map(alm, np.zeros_like(map1))
+            map1 += map2
+            map1 *= ivar**-0.5
+            ivar_nonzero = ivar>0.
+            ivar_median = np.median(ivar[ivar_nonzero])
+            valid_ivar = ivar_nonzero*(ivar>ivar_median/1.e6)
+            map1[~(valid_ivar)] = 0.
+            return map1
+
+        assert np.all(np.isfinite(ivarMap))
+        shape, wcs=ivarMap.shape, ivarMap.wcs
+        ells = np.arange(mlmax+1)
+        Nl_atm = (lKnee/ells)**-alpha + 1
+        Nl_atm[~np.isfinite(Nl_atm)] = 0.
+        assert np.all(np.isfinite(Nl_atm))
+        randMap = _mod_noise_map(ivarMap, Nl_atm)
+        assert np.all(np.isfinite(randMap))
+
     return randMap
-        
+
 #-------------------------------------------------------------------------------------------------------------
 def subtractBackground(data, wcs, RADeg = 'centre', decDeg = 'centre', smoothScaleDeg = 30.0/60.0):
     """Smoothes map with Gaussian of given scale and subtracts it, to get rid of large scale power.
     
     If RADeg, decDeg = 'centre', then the pixel scales used to set the kernel shape will be set from that at the
     centre of the WCS. Otherwise, they will be taken at the given coords.
     
@@ -1232,16 +1396,16 @@
         yPad=0
     if data.shape[1] % 2 == 0:
         xPad=1
     else:
         xPad=0
     degreesMap=np.ones([data.shape[0]+yPad, data.shape[1]+xPad], dtype = float)*1e6
     RADeg, decDeg=wcs.pix2wcs(int(degreesMap.shape[1]/2)+1, int(degreesMap.shape[0]/2)+1)
-    degreesMap, xBounds, yBounds=nemoCython.makeDegreesDistanceMap(degreesMap, wcs, RADeg, decDeg, 
-                                                                   maxDistDegrees)
+    degreesMap, xBounds, yBounds=makeDegreesDistanceMap(degreesMap, wcs, RADeg, decDeg,
+                                                        maxDistDegrees)
     beamMap=signals.makeBeamModelSignalMap(degreesMap, wcs, beam)
     if (yBounds[1]-yBounds[0]) > beamMap.shape[1] and (yBounds[1]-yBounds[0]) % 2 == 0:
         yBounds[0]=yBounds[0]-1
     if (xBounds[1]-xBounds[0]) > beamMap.shape[0] and (xBounds[1]-xBounds[0]) % 2 == 0:
         xBounds[0]=xBounds[0]-1    
     beamMap=beamMap[yBounds[0]:yBounds[1], xBounds[0]:xBounds[1]]
     beamMap=beamMap/np.sum(beamMap)
@@ -1375,15 +1539,15 @@
         for tileName in simConfig.tileNames:
             mapFileNames=glob.glob(simRootOutDir+os.path.sep+"filteredMaps"+os.path.sep+"*#%s_*.fits" % (tileName))
             for m in mapFileNames:
                 os.remove(m)
                 
         simImageDict=pipelines.filterMapsAndMakeCatalogs(simConfig, 
                                                          rootOutDir = simRootOutDir,
-                                                         copyFilters = True)
+                                                         useCachedFilters = True)
         
         # Write out the last sim map catalog for debugging
         # NOTE: tileName here makes no sense - this should be happening in the pipeline call above
         #optimalCatalogFileName=simRootOutDir+os.path.sep+"CMBSim_optimalCatalog#%s.csv" % (tileName)    
         #optimalCatalog=simImageDict['optimalCatalog']
         #if len(optimalCatalog) > 0:
             #catalogs.writeCatalog(optimalCatalog, optimalCatalogFileName.replace(".csv", ".fits"), constraintsList = ["SNR > 0.0"])
@@ -1560,17 +1724,17 @@
             contaminTab.add_column(atpy.Column(contaminDict[key], key))
         
         contaminTabDict['%s_%s' % (label, SNRKey)]=contaminTab
         
     return contaminTabDict
 
 #------------------------------------------------------------------------------------------------------------
-def makeModelImage(shape, wcs, catalog, beamFileName, obsFreqGHz = None, GNFWParams = 'default', 
-                   profile = 'A10', cosmoModel = None, applyPixelWindow = True, override = None,
-                   validAreaSection = None, minSNR = 0.0, TCMBAlpha = 0):
+def makeModelImage(shape, wcs, catalog, beamFileName, obsFreqGHz = None, GNFWParams = 'default',\
+                   profile = 'A10', cosmoModel = None, applyPixelWindow = True, override = None,\
+                   validAreaSection = None, minSNR = -99, TCMBAlpha = 0):
     """Make a map with the given dimensions (shape) and WCS, containing model clusters or point sources, 
     with properties as listed in the catalog. This can be used to either inject or subtract sources
     from real maps.
     
     Args:
         shape (tuple): The dimensions of the output map (height, width) that will contain the model sources.
         wcs (:obj:`astWCS.WCS`): A WCS object that defines the coordinate system of the map. 
@@ -1620,370 +1784,416 @@
         SNRKey='SNR'
     elif 'fixed_SNR' in catalog.keys():
         SNRKey='fixed_SNR'
     else:
         SNRKey=None
     if SNRKey is not None:
         catalog=catalog[catalog[SNRKey] > minSNR]
-        
+
+    # If we want to restrict painting to just area mask within in a tile
+    # (avoids double painting of objects in overlap areas)
+    if validAreaSection is not None and len(catalog) > 0:
+        x0, x1, y0, y1=validAreaSection
+        coords=wcs.wcs2pix(catalog['RADeg'], catalog['decDeg'])
+        x=np.array(coords)[:, 0]
+        y=np.array(coords)[:, 1]
+        xMask=np.logical_and(x >= x0, x < x1)
+        yMask=np.logical_and(y >= y0, y < y1)
+        cMask=np.logical_and(xMask, yMask)
+        catalog=catalog[cMask]
+
     if len(catalog) == 0:
         return None
 
     if cosmoModel is None:
         cosmoModel=signals.fiducialCosmoModel
-    
-    # We could use this to replace how GNFWParams are fed in also (easier for nemoModel script)
-    if profile == 'A10':
-        makeClusterSignalMap=signals.makeArnaudModelSignalMap
-    elif profile == 'B12':
-        makeClusterSignalMap=signals.makeBattagliaModelSignalMap
-    else:
-        raise Exception("Didn't understand profile - should be A10 or B12. This would be an excellent place\
-                        to accept a string of GNFW parameters, but that is not implemented yet.")
-    
+
     # Set initial max size in degrees from beam file (used for sources; clusters adjusted for each object)
     numFWHM=5.0
     beam=signals.BeamProfile(beamFileName = beamFileName)
     maxSizeDeg=(beam.FWHMArcmin*numFWHM)/60
     
     # Map of distance(s) from objects - this will get updated in place (fast)
     degreesMap=np.ones(modelMap.shape, dtype = float)*1e6
     
-    if 'fixed_y_c' in catalog.keys() or 'true_fixed_y_c' in catalog.keys():
-        # Clusters: for speed - assume all objects are the same shape
+    if 'y_c' in catalog.keys() or 'true_y_c' in catalog.keys():
+        # Clusters - insert one at a time (with different scales etc.)
+        # We could use this to replace how GNFWParams are fed in also (easier for nemoModel script)
+        if profile == 'A10':
+            makeClusterSignalMap=signals.makeArnaudModelSignalMap
+        elif profile == 'B12':
+            makeClusterSignalMap=signals.makeBattagliaModelSignalMap
+        else:
+            raise Exception("Didn't understand profile - should be A10 or B12. This would be an excellent place\
+                            to accept a string of GNFW parameters, but that is not implemented yet.")
+        count=0
+        # First bit here (override) is for doing injection sims faster
         if override is not None:
-            fluxScaleMap=np.zeros(modelMap.shape)
-            for row in catalog:
-                degreesMap, xBounds, yBounds=nemoCython.makeDegreesDistanceMap(degreesMap, wcs, 
-                                                                            row['RADeg'], row['decDeg'], 
-                                                                            maxSizeDeg)
-                fluxScaleMap[yBounds[0]:yBounds[1], xBounds[0]:xBounds[1]]=row['fixed_y_c']*1e-4
-            theta500Arcmin=signals.calcTheta500Arcmin(override['redshift'], override['M500'], cosmoModel)
+            z=override['redshift']
+            M500=override['M500']
+            y0ToInsert=catalog['y_c'].data*1e-4
+            RAs=catalog['RADeg'].data
+            decs=catalog['decDeg'].data
+            theta500Arcmin=signals.calcTheta500Arcmin(z, M500, cosmoModel)
             maxSizeDeg=5*(theta500Arcmin/60)
-            modelMap=makeClusterSignalMap(override['redshift'], override['M500'], degreesMap, 
-                                          wcs, beam, GNFWParams = GNFWParams,
-                                          maxSizeDeg = maxSizeDeg, convolveWithBeam = False)
-            modelMap=modelMap*fluxScaleMap
-            modelMap=convolveMapWithBeam(modelMap, wcs, beam, maxDistDegrees = 1.0)
-
-        # Clusters - insert one at a time (with different scales etc.) - currently taking ~1.6 sec per object
+            modelMap=makeClusterSignalMap(z, M500, modelMap.shape, wcs, RADeg = RAs,
+                                          decDeg = decs, beam = beam,
+                                          GNFWParams = GNFWParams, amplitude = y0ToInsert,
+                                          maxSizeDeg = maxSizeDeg, convolveWithBeam = True,
+                                          cosmoModel = cosmoModel)
+            if obsFreqGHz is not None:
+                modelMap=convertToDeltaT(modelMap, obsFrequencyGHz = obsFreqGHz,
+                                         TCMBAlpha = TCMBAlpha, z = z)
         else:
-            count=0
             for row in catalog:
-                # This should avoid overlaps if tiled - we only add cluster if inside areaMask region
-                # NOTE: Should move this out of this switch so applied to all catalog types
-                if validAreaSection is not None:
-                    x0, x1, y0, y1=validAreaSection
-                    x, y=wcs.wcs2pix(row['RADeg'], row['decDeg'])
-                    if (x >= x0 and x < x1 and y >= y0 and y < y1) == False:
-                        continue
                 count=count+1
                 if 'true_M500c' in catalog.keys():
                     # This case is for when we're running from nemoMock output
                     # Since the idea of this is to create noise-free model images, we must use true values here
                     # (to avoid any extra scatter/selection effects after adding model clusters to noise maps).
                     M500=row['true_M500c']*1e14
                     z=row['redshift']
-                    y0ToInsert=row['true_fixed_y_c']*1e-4
-                    y0ToInsert=y0ToInsert/row['true_Q']
+                    y0ToInsert=row['true_y_c']*1e-4
                 else:
                     # NOTE: This case is for running from nemo output
                     # We need to adapt this for when the template names are not in this format
                     if 'template' not in catalog.keys():
                         raise Exception("No M500, z, or template column found in catalog.")
                     bits=row['template'].split("#")[0].split("_")
                     M500=float(bits[1][1:].replace("p", "."))
                     z=float(bits[2][1:].replace("p", "."))
                     y0ToInsert=row['y_c']*1e-4  # or fixed_y_c...
                 theta500Arcmin=signals.calcTheta500Arcmin(z, M500, cosmoModel)
                 maxSizeDeg=5*(theta500Arcmin/60)
-                degreesMap=np.ones(modelMap.shape, dtype = float)*1e6 # NOTE: never move this
-                degreesMap, xBounds, yBounds=nemoCython.makeDegreesDistanceMap(degreesMap, wcs, 
-                                                                            row['RADeg'], row['decDeg'], 
-                                                                            maxSizeDeg)
-                signalMap=makeClusterSignalMap(z, M500, degreesMap, wcs, beam, 
-                                               GNFWParams = GNFWParams, amplitude = y0ToInsert,
-                                               maxSizeDeg = maxSizeDeg, convolveWithBeam = False)
+                signalMap=makeClusterSignalMap(z, M500, modelMap.shape, wcs, RADeg = row['RADeg'],
+                                                decDeg = row['decDeg'], beam = beam,
+                                                GNFWParams = GNFWParams, amplitude = y0ToInsert,
+                                                maxSizeDeg = maxSizeDeg, convolveWithBeam = True,
+                                                cosmoModel = cosmoModel)
                 if obsFreqGHz is not None:
                     signalMap=convertToDeltaT(signalMap, obsFrequencyGHz = obsFreqGHz,
-                                              TCMBAlpha = TCMBAlpha, z = z)
+                                                TCMBAlpha = TCMBAlpha, z = z)
                 modelMap=modelMap+signalMap
-            modelMap=convolveMapWithBeam(modelMap, wcs, beam, maxDistDegrees = 1.0)
-
     else:
         # Sources - slower but more accurate way
         for row in catalog:
             if validAreaSection is not None:
                 x0, x1, y0, y1=validAreaSection
                 x, y=wcs.wcs2pix(row['RADeg'], row['decDeg'])
                 if (x >= x0 and x < x1 and y >= y0 and y < y1) == False:
                     continue
             degreesMap=np.ones(modelMap.shape, dtype = float)*1e6 # NOTE: never move this
-            degreesMap, xBounds, yBounds=nemoCython.makeDegreesDistanceMap(degreesMap, wcs, 
-                                                                        row['RADeg'], row['decDeg'], 
-                                                                        maxSizeDeg)
+            degreesMap, xBounds, yBounds=makeDegreesDistanceMap(degreesMap, wcs,
+                                                                row['RADeg'], row['decDeg'],
+                                                                maxSizeDeg)
             signalMap=signals.makeBeamModelSignalMap(degreesMap, wcs, beam)*row['deltaT_c']
             modelMap=modelMap+signalMap
-        # Sources - note this is extremely fast, but goes wrong for closely packed sources
-        # So we should just get rid of it
-        #fluxScaleMap=np.zeros(modelMap.shape)
-        #for row in catalog:
-            #degreesMap, xBounds, yBounds=nemoCython.makeDegreesDistanceMap(degreesMap, wcs, 
-                                                                        #row['RADeg'], row['decDeg'], 
-                                                                        #maxSizeDeg)
-            #fluxScaleMap[yBounds[0]:yBounds[1], xBounds[0]:xBounds[1]]=row['deltaT_c']
-        #modelMap=signals.makeBeamModelSignalMap(degreesMap, wcs, beam)
-        #modelMap=modelMap*fluxScaleMap
-        
+
     # Optional: apply pixel window function - generally this should be True
     # (because the source-insertion routines in signals.py interpolate onto the grid rather than average)
     if applyPixelWindow == True:
         modelMap=enmap.apply_window(modelMap, pow = 1.0)
         
     return modelMap
         
 #------------------------------------------------------------------------------------------------------------
-def sourceInjectionTest(config, writeRankTable = True):
+def sourceInjectionTest(config):
     """Insert sources with known positions and properties into the map, apply the filter, and record their
     offset with respect to the true location as a function of S/N (for the fixed reference scale only).
     If the inserted sources are clusters, the Q function will be applied to the output fluxes, to account 
     for any mismatch between the reference filter scale and the inserted clusters.
     
     Writes output to the diagnostics/ directory.
     
     Args:
         config (:obj:`nemo.startUp.NemoConfig`): Nemo configuration object.
-        writeRankTable (bool, optional): If True, saves a table as output for this MPI rank under the 
-            diagnostics/ directory. Useful for MPI debugging only.
-    
+
     Returns:
         An astropy Table containing recovered position offsets and fluxes versus fixed_SNR for inserted
         sources.
+
+    Note:
+        Injection tests for clusters use the reference filter only (set with the `photFilter` keyword
+        in the config). Input amplitudes for clusters are in `y_c`, while output is in `fixed_y_c`
+        (because the reference filter is used). Similarly, output SNR is `fixed_SNR`, although the
+        output column is labelled as `SNR`.
     
     """
-    
-    simRootOutDir=config.diagnosticsDir+os.path.sep+"sourceInjection_rank%d" % (config.rank)
-    SNRKeys=['fixed_SNR']
-    
-    # We don't copy this, because it's complicated due to containing MPI-related things (comm)
-    # So... we modify the config parameters in-place, and restore them before exiting this method
-    simConfig=config
-    simConfig.parDict['twoPass']=False      # We re-use filters we already made, so no need to do full two pass
-    
+
+    # WARNING: For multi-pass mode, this has the desired behaviour IF this is called after a nemo run
+    # (i.e., the config is already set to the last filterSet)
+    # But, can we guarantee that? Probably not. But we could put a warning in the docs for now?
+
+    # This should perhaps be a config parameter
+    realExclusionRadiusArcmin=5.0
+
     # This should make it quicker to generate test catalogs (especially when using tiles)
     selFn=completeness.SelFn(config.selFnDir, 4.0, configFileName = config.configFileName,
                              enableCompletenessCalc = False, setUpAreaMask = True,
-                             tileNames = config.tileNames)
+                             tileNames = config.allTileNames)
     
     print(">>> Position recovery test [rank = %d] ..." % (config.rank))
 
     if 'sourceInjectionIterations' not in config.parDict.keys():
         numIterations=1
     else:
         numIterations=config.parDict['sourceInjectionIterations']
-    
-    # For clusters, we may want to run multiple scales
-    # We're using theta500Arcmin as the label here
-    filtDict=simConfig.parDict['mapFilters'][0]
-    if filtDict['class'].find("ArnaudModel") != -1:
+
+    # Change to previous behavior - if config doesn't specify models to use, assume it's point sources
+    if 'sourceInjectionModels' in config.parDict.keys():
         clusterMode=True
-        if 'sourceInjectionModels' not in config.parDict.keys():
-            sourceInjectionModelList=[{'redshift': 0.4, 'M500': 2e14}]
-        else:
-            sourceInjectionModelList=config.parDict['sourceInjectionModels']
+        sourceInjectionModelList=config.parDict['sourceInjectionModels']
+        SNRCol='SNR'
+        fluxCol='y_c'
+        noiseLevelCol='err_y_c'
         for sourceInjectionModel in sourceInjectionModelList:
-            label='%.2f' % (signals.calcTheta500Arcmin(sourceInjectionModel['redshift'], 
-                                                       sourceInjectionModel['M500'], signals.fiducialCosmoModel))
+            theta500Arcmin=signals.calcTheta500Arcmin(sourceInjectionModel['redshift'],
+                                                      sourceInjectionModel['M500'],
+                                                      signals.fiducialCosmoModel)
+            label='%.2f' % (theta500Arcmin)
             sourceInjectionModel['label']=label
-        # We need Q for flux recovery stuff...
-        QFit=signals.QFit(config.selFnDir+os.path.sep+"QFit.fits", tileNames = config.tileNames)
+            sourceInjectionModel['theta500Arcmin']=theta500Arcmin
     else:
         # Sources
         clusterMode=False
         sourceInjectionModelList=[{'label': 'pointSource'}]
+        SNRCol='SNR'
+        fluxCol='deltaT_c'
+        noiseLevelCol='err_deltaT_c'
+
     # This isn't really important as avoidance radius will stop us putting in too many sources
     if 'sourcesPerTile' not in config.parDict.keys():
         numSourcesPerTile=300
     else:
         numSourcesPerTile=config.parDict['sourcesPerTile']
     
     # We need the actual catalog to throw out spurious 'recoveries'
     # i.e., we only want to cross-match with objects we injected
     catFileName=config.rootOutDir+os.path.sep+"%s_optimalCatalog.fits" % (os.path.split(config.rootOutDir)[-1])
     if os.path.exists(catFileName) == False:
         raise Exception("Catalog file '%s' not found - needed to do source injection test." % (catFileName))
     realCatalog=atpy.Table().read(catFileName)
     
     # Run each scale / model and then collect everything into one table afterwards
-    # NOTE: raw flux error in catalogs is from RMS map, but e.g. outFlux will have Q applied here if cluster
+    # NOTE: These dictionaries contain recovered measurements from running the finder
+    RADegDict={}
+    decDegDict={}
     SNRDict={}
     rArcminDict={}
     inFluxDict={}
     outFluxDict={}
     noiseLevelDict={}
     tileNamesDict={}
+    # NOTE: This list collects all the input catalogs
+    allInputCatalogs=[]
+    modelCount=0
     for sourceInjectionModel in sourceInjectionModelList:
+        modelCount=modelCount+1
+        print(">>> Source injection model: %d/%d" % (modelCount, len(sourceInjectionModelList)))
+        RADegDict[sourceInjectionModel['label']]=[]
+        decDegDict[sourceInjectionModel['label']]=[]
         SNRDict[sourceInjectionModel['label']]=[]
         rArcminDict[sourceInjectionModel['label']]=[]
         inFluxDict[sourceInjectionModel['label']]=[]
         outFluxDict[sourceInjectionModel['label']]=[]
         noiseLevelDict[sourceInjectionModel['label']]=[]
         tileNamesDict[sourceInjectionModel['label']]=[]
         for i in range(numIterations):        
-            print(">>> Source injection and recovery test %d/%d [rank = %d] ..." % (i+1, numIterations, config.rank))
-                        
+            print(">>> Source injection and recovery test %d/%d [rank = %d]" % (i+1, numIterations, config.rank))
+
             # NOTE: This block below should be handled when parsing the config file - fix/remove
             # Optional override of default GNFW parameters (used by Arnaud model), if used in filters given
-            if 'GNFWParams' not in list(simConfig.parDict.keys()):
-                simConfig.parDict['GNFWParams']='default'
-            for filtDict in simConfig.parDict['mapFilters']:
-                filtDict['params']['GNFWParams']=simConfig.parDict['GNFWParams']
+            if 'GNFWParams' not in list(config.parDict.keys()):
+                config.parDict['GNFWParams']='default'
+            for filtDict in config.parDict['mapFilters']:
+                filtDict['params']['GNFWParams']=config.parDict['GNFWParams']
             
             # We don't want to save/cache position recovery test maps
-            for filtDict in simConfig.parDict['mapFilters']:
+            for filtDict in config.parDict['mapFilters']:
                 keysToFalsify=['saveFilteredMaps', 'savePlots']
                 for key in keysToFalsify:
                     filtDict['params'][key]=False
             
             # Delete all non-reference scale filters (otherwise we'd want to cache all filters for speed)
             # NOTE: As it stands, point-source only runs may not define photFilter - we need to handle that
             # That should be obvious, as mapFilters will only have one entry
-            for filtDict in simConfig.parDict['mapFilters']:
-                if filtDict['label'] == simConfig.parDict['photFilter']:
+            for filtDict in config.parDict['mapFilters']:
+                if filtDict['label'] == config.parDict['photFilter']:
                     break
-            simConfig.parDict['mapFilters']=[filtDict] 
+            config.parDict['mapFilters']=[filtDict]
                 
             # Filling maps with injected sources will be done when maps.preprocessMapDict is called by the filter object
             # So, we only generate the catalog here
-            print("... generating mock catalog ...")
-            if filtDict['class'].find("ArnaudModel") != -1:
-                fluxCol='fixed_y_c'
-                noiseLevelCol='fixed_err_y_c'
-                SNRCol='fixed_SNR'
-                # Quick test catalog - takes < 1 sec to generate
-                mockCatalog=catalogs.generateTestCatalog(config, numSourcesPerTile, 
-                                                         amplitudeColumnName = 'fixed_y_c', 
-                                                         amplitudeRange = [0.001, 1], 
-                                                         amplitudeDistribution = 'linear',
-                                                         selFn = selFn, maskDilationPix = 20)
-                # Or... proper mock, but this takes ~24 sec for E-D56
-                #mockCatalog=pipelines.makeMockClusterCatalog(config, writeCatalogs = False, verbose = False)[0]                
-                injectSources={'catalog': mockCatalog, 'GNFWParams': config.parDict['GNFWParams'], 
-                               'override': sourceInjectionModel}
-            elif filtDict['class'].find("Beam") != -1:
-                fluxCol='deltaT_c'
-                noiseLevelCol='err_deltaT_c'
-                SNRCol='SNR'
-                mockCatalog=catalogs.generateTestCatalog(config, numSourcesPerTile, 
-                                                         amplitudeColumnName = fluxCol, 
-                                                         amplitudeRange = [1, 1000], 
-                                                         amplitudeDistribution = 'log', 
-                                                         selFn = selFn, maskDilationPix = 20)
-                injectSources={'catalog': mockCatalog, 'override': sourceInjectionModel}
+            print("... generating mock catalog")
+            if config.rank == 0:
+                if filtDict['class'].find("ArnaudModel") != -1:
+                    if 'sourceInjectionAmplitudeRange' not in config.parDict.keys():
+                        amplitudeRange=[0.001, 10]
+                    else:
+                        amplitudeRange=config.parDict['sourceInjectionAmplitudeRange']
+                        if amplitudeRange == 'auto':
+                            amplitudeRange=[realCatalog['fixed_y_c'].min()*0.5, realCatalog['fixed_y_c'].max()]
+                    if 'sourceInjectionDistribution' not in config.parDict.keys():
+                        distribution='linear'
+                    else:
+                        distribution=config.parDict['sourceInjectionDistribution']
+                    # Quick test catalog - takes < 1 sec to generate
+                    mockCatalog=catalogs.generateTestCatalog(config, numSourcesPerTile,
+                                                            amplitudeColumnName = fluxCol,
+                                                            amplitudeRange = amplitudeRange,
+                                                            amplitudeDistribution = distribution,
+                                                            selFn = selFn, maskDilationPix = 20)
+                    # Or... proper mock, but this takes ~24 sec for E-D56
+                    #mockCatalog=pipelines.makeMockClusterCatalog(config, writeCatalogs = False, verbose = False)[0]
+                    injectSources={'catalog': mockCatalog, 'GNFWParams': config.parDict['GNFWParams'],
+                                   'override': sourceInjectionModel, 'profile': 'A10'}
+                elif filtDict['class'].find("Beam") != -1:
+                    if 'sourceInjectionAmplitudeRange' not in config.parDict.keys():
+                        amplitudeRange=[1, 1000]
+                    else:
+                        amplitudeRange=config.parDict['sourceInjectionAmplitudeRange']
+                    if 'sourceInjectionDistribution' not in config.parDict.keys():
+                        distribution='log'
+                    else:
+                        distribution=config.parDict['sourceInjectionDistribution']
+                    mockCatalog=catalogs.generateTestCatalog(config, numSourcesPerTile,
+                                                            amplitudeColumnName = fluxCol,
+                                                            amplitudeRange = amplitudeRange,
+                                                            amplitudeDistribution = distribution,
+                                                            selFn = selFn, maskDilationPix = 20)
+                    injectSources={'catalog': mockCatalog, 'override': sourceInjectionModel, 'profile': None}
+                else:
+                    raise Exception("Don't know how to generate injected source catalogs for filterClass '%s'" % (filtDict['class']))
+                if 'theta500Arcmin' in sourceInjectionModel.keys():
+                    mockCatalog['theta500Arcmin']=sourceInjectionModel['theta500Arcmin']
+                allInputCatalogs.append(mockCatalog)
             else:
-                raise Exception("Don't know how to generate injected source catalogs for filterClass '%s'" % (filtDict['class']))
-            for mapDict in simConfig.unfilteredMapsDictList:
+                injectSources=None
+                mockCatalog=None
+
+            if config.MPIEnabled == True:
+                bcastInjectSources=config.comm.bcast(injectSources, root = 0)
+                config.comm.barrier()
+                if config.rank > 0:
+                    injectSources=bcastInjectSources
+                    mockCatalog=bcastInjectSources['catalog']
+
+            for mapDict in config.unfilteredMapsDictList:
                 mapDict['injectSources']=injectSources
             
-            # NOTE: we need to zap ONLY specific maps for when we are running in parallel
-            for tileName in simConfig.tileNames:
-                mapFileNames=glob.glob(simRootOutDir+os.path.sep+"filteredMaps"+os.path.sep+"*#%s_*.fits" % (tileName))
-                for m in mapFileNames:
-                    os.remove(m)
-
             # Ideally we shouldn't have blank tiles... but if we do, skip
             if len(mockCatalog) > 0:
-                recCatalog=pipelines.filterMapsAndMakeCatalogs(simConfig, rootOutDir = simRootOutDir,
-                                                               copyFilters = True, useCachedMaps = False)
+
+                # Uncomment line below if want to save filtered maps for quick and dirty debugging
+                # Overwrites the original filtered map, but can compare to 'stitched' map
+                # config.parDict['mapFilters'][0]['params']['saveFilteredMaps']=True
+
+                recCatalog=pipelines.filterMapsAndMakeCatalogs(config, useCachedFilters = True,
+                                                               useCachedRMSMap = True, writeAreaMask = False,
+                                                               writeFlagMask = False)
+
+                # NOTE: Below here only rank 0 really needed (could then broadcast result)
+
                 # We should be conservative in removing potential matches with real objects
                 # Because we have a huge sky area and there's no reason to risk contamination of this kind
                 # Effectively this is the same as using 5' circular holes in the survey mask on real objects
                 # (but actually adding the avoidance radius parameter to the test catalogs really solved this)
                 if len(recCatalog) > 0:
-                    recCatalog=catalogs.removeCrossMatched(recCatalog, realCatalog, radiusArcmin = 5.0)
+                    recCatalog=catalogs.removeCrossMatched(recCatalog, realCatalog,
+                                                           radiusArcmin = realExclusionRadiusArcmin)
                 if len(recCatalog) > 0:
                     try:
-                        x_mockCatalog, x_recCatalog, rDeg=catalogs.crossMatch(mockCatalog, recCatalog, radiusArcmin = 5.0)
+                        x_mockCatalog, x_recCatalog, rDeg=catalogs.crossMatch(mockCatalog, recCatalog,
+                                                                              radiusArcmin = realExclusionRadiusArcmin)
                     except:
-                        raise Exception("Position recovery test: cross match failed on tileNames = %s; mockCatalog length = %d; recCatalog length = %d" % (str(simConfig.tileNames), len(mockCatalog), len(recCatalog)))
-                    # If we're using clusters, we need to put in the Q correction
-                    # NOTE: This assumes the model name gives theta500c in arcmin!
-                    if clusterMode == True:
-                        for tileName in np.unique(x_recCatalog['tileName']):
-                            theta500Arcmin=float(sourceInjectionModel['label'])
-                            Q=QFit.getQ(theta500Arcmin, tileName = tileName)
-                            mask=(x_recCatalog['tileName'] == tileName)
-                            x_recCatalog[fluxCol][mask]=x_recCatalog[fluxCol][mask]/Q
+                        raise Exception("Source injection test: cross match failed on tileNames = %s; mockCatalog length = %d; recCatalog length = %d" % (str(config.tileNames), len(mockCatalog), len(recCatalog)))
+
                     # Catching any crazy mismatches, writing output for debugging
                     if clusterMode == False and np.logical_and(rDeg > 1.5/60, x_recCatalog['SNR'] > 10).sum() > 0:
                         mask=np.logical_and(rDeg > 1.5/60, x_recCatalog['SNR'] > 10)
-                        simConfig.parDict['mapFilters'][0]['params']['saveFilteredMaps']=True
-                        recCatalog2=pipelines.filterMapsAndMakeCatalogs(simConfig, rootOutDir = simRootOutDir,
-                                                                       copyFilters = True, useCachedMaps = False)
-                        recCatalog2=catalogs.removeCrossMatched(recCatalog2, realCatalog, radiusArcmin = 5.0)
+                        config.parDict['mapFilters'][0]['params']['saveFilteredMaps']=True
+                        recCatalog2=pipelines.filterMapsAndMakeCatalogs(config, useCachedFilters = True,
+                                                                        writeAreaMask = False, writeFlagMask = False)
+                        recCatalog2=catalogs.removeCrossMatched(recCatalog2, realCatalog,
+                                                                radiusArcmin = realExclusionRadiusArcmin)
                         catalogs.catalog2DS9(x_recCatalog[mask],
                                              simRootOutDir+os.path.sep+"filteredMaps"+os.path.sep+tileName+os.path.sep+"mismatch-rec.reg")
                         catalogs.catalog2DS9(x_mockCatalog[mask],
                                              simRootOutDir+os.path.sep+"filteredMaps"+os.path.sep+tileName+os.path.sep+"mismatch-input.reg",
                                              color = 'red')
                         msg="Caught recovered source at large offset - check output under %s" % (simRootOutDir+os.path.sep+"filteredMaps"+os.path.sep+tileName)
-                        if simConfig.parDict['haltOnPositionRecoveryProblem'] == True:
+                        if config.parDict['haltOnPositionRecoveryProblem'] == True:
                             raise Exception(msg)
                         else:
                             print("... Warning: %s ..." % (msg))
 
                     # Store everything - analyse later
+                    RADegDict[sourceInjectionModel['label']]=RADegDict[sourceInjectionModel['label']]+x_recCatalog['RADeg'].tolist()
+                    decDegDict[sourceInjectionModel['label']]=decDegDict[sourceInjectionModel['label']]+x_recCatalog['decDeg'].tolist()
                     SNRDict[sourceInjectionModel['label']]=SNRDict[sourceInjectionModel['label']]+x_recCatalog[SNRCol].tolist()
                     rArcminDict[sourceInjectionModel['label']]=rArcminDict[sourceInjectionModel['label']]+(rDeg*60).tolist()
                     inFluxDict[sourceInjectionModel['label']]=inFluxDict[sourceInjectionModel['label']]+x_mockCatalog[fluxCol].tolist()
                     outFluxDict[sourceInjectionModel['label']]=outFluxDict[sourceInjectionModel['label']]+x_recCatalog[fluxCol].tolist()
                     noiseLevelDict[sourceInjectionModel['label']]=noiseLevelDict[sourceInjectionModel['label']]+x_recCatalog[noiseLevelCol].tolist()
                     tileNamesDict[sourceInjectionModel['label']]=tileNamesDict[sourceInjectionModel['label']]+x_recCatalog['tileName'].tolist()
 
+        RADegDict[sourceInjectionModel['label']]=np.array(RADegDict[sourceInjectionModel['label']])
+        decDegDict[sourceInjectionModel['label']]=np.array(decDegDict[sourceInjectionModel['label']])
         SNRDict[sourceInjectionModel['label']]=np.array(SNRDict[sourceInjectionModel['label']])
         rArcminDict[sourceInjectionModel['label']]=np.array(rArcminDict[sourceInjectionModel['label']])
         inFluxDict[sourceInjectionModel['label']]=np.array(inFluxDict[sourceInjectionModel['label']])
         outFluxDict[sourceInjectionModel['label']]=np.array(outFluxDict[sourceInjectionModel['label']])
         noiseLevelDict[sourceInjectionModel['label']]=np.array(noiseLevelDict[sourceInjectionModel['label']])
         tileNamesDict[sourceInjectionModel['label']]=np.array(tileNamesDict[sourceInjectionModel['label']])
         
-    # Just collect results as long tables (model, SNR, rArcmin, inFlux, outFlux) that we can later stack and average etc.
-    # (see positionRecoveryAnalysis below)
+    # Collecting all results into one giant table
     models=[]
+    theta500s=[]
+    RAs=[]
+    decs=[]
     SNRs=[]
     rArcmin=[]
     inFlux=[]
     outFlux=[]
     noiseLevel=[]
     tileNames=[]
     for sourceInjectionModel in sourceInjectionModelList:
         label=sourceInjectionModel['label']
+        if 'theta500Arcmin' in sourceInjectionModel.keys():
+            theta500s=theta500s+[sourceInjectionModel['theta500Arcmin']]*len(SNRDict[label])
         models=models+[label]*len(SNRDict[label])
+        RAs=RAs+RADegDict[label].tolist()
+        decs=decs+decDegDict[label].tolist()
         SNRs=SNRs+SNRDict[label].tolist()
         rArcmin=rArcmin+rArcminDict[label].tolist()
         inFlux=inFlux+inFluxDict[label].tolist()
         outFlux=outFlux+outFluxDict[label].tolist()
         noiseLevel=noiseLevel+noiseLevelDict[label].tolist()
         tileNames=tileNames+tileNamesDict[label].tolist()
     resultsTable=atpy.Table()
+    resultsTable.add_column(atpy.Column(RAs, 'RADeg'))
+    resultsTable.add_column(atpy.Column(decs, 'decDeg'))
     resultsTable.add_column(atpy.Column(models, 'sourceInjectionModel'))
+    if len(theta500s) == len(resultsTable):
+        resultsTable.add_column(atpy.Column(theta500s, 'theta500Arcmin'))
     resultsTable.add_column(atpy.Column(SNRs, SNRCol))
     resultsTable.add_column(atpy.Column(rArcmin, 'rArcmin'))
     resultsTable.add_column(atpy.Column(inFlux, 'inFlux'))
     resultsTable.add_column(atpy.Column(outFlux, 'outFlux'))
     resultsTable.add_column(atpy.Column(noiseLevel, 'noiseLevel'))
     resultsTable.add_column(atpy.Column(tileNames, 'tileName'))
 
-    # Shouldn't be necessary BUT seems we have trouble gathering very large runs
-    # So it's actually more reliable to write/read from disk
-    if writeRankTable == True:
-        fitsOutFileName=config.diagnosticsDir+os.path.sep+"sourceInjection_rank%d.fits" % (config.rank)
-        resultsTable.meta['NEMOVER']=nemo.__version__
-        resultsTable.write(fitsOutFileName, overwrite = True)
-    
+    # Store the giant combined input catalog as well, for completeness calculations
+    # NOTE: Not all objects in this may have been injected (masking, avoiding overlap etc.)
+    if config.rank == 0:
+        allInputTab=atpy.vstack(allInputCatalogs)
+        allInputTab.rename_column(fluxCol, "inFlux")
+        allInputTab=catalogs.removeCrossMatched(allInputTab, realCatalog, radiusArcmin = realExclusionRadiusArcmin)
+        allInputTab.write(config.selFnDir+os.path.sep+"sourceInjectionInputCatalog.fits", overwrite = True)
+
     # Restore the original config parameters (which we overrode here)
     config.restoreConfig()
 
     return resultsTable
 
 #------------------------------------------------------------------------------------------------------------
 def positionRecoveryAnalysis(posRecTable, plotFileName, percentiles = [50, 95, 99.7],
@@ -2007,25 +2217,27 @@
         selFnDir (string, optional): If given, model fit parameters will be written to a file named
             posRecModelParameters.txt under the given selFn directory path.
             
     """
 
     # Sources or clusters table?
     tab=posRecTable
+    if len(tab) == 0:
+        return None
     if np.unique(tab['sourceInjectionModel'])[0] == 'pointSource':
         SNRCol='SNR'
         plotSNRLabel="SNR"
         rArcminThreshold=np.linspace(0, 5, 201)
         plotUnits="arcsec"
         plotUnitsMultiplier=60
         plotUnitsLabel="$^{\prime\prime}$"
     else:
-        # Clusters
-        SNRCol='fixed_SNR'
-        plotSNRLabel="SNR$_{2.4}$"
+        # Clusters - SNR is really fixed_SNR here, because injection sims use only ref filter
+        SNRCol='SNR'
+        plotSNRLabel="fixed_SNR"
         rArcminThreshold=np.linspace(0, 10, 101)
         plotUnits="arcmin"
         plotUnitsMultiplier=1
         plotUnitsLabel="$^\prime$"
     
     # Optional cut on injected signal model
     if sourceInjectionModel is not None:
@@ -2149,49 +2361,171 @@
             
     """
 
     print("Work in progress - skipped")
     return None
         
 #---------------------------------------------------------------------------------------------------
-def saveFITS(outputFileName, mapData, wcs, compressed = False, compressionType = 'RICE_1'):
-    """Writes a map (2d image array) to a new .fits file.
+def saveFITS(outputFileName, mapData, wcs, compressionType = None):
+    """Writes a map (2d image array) to a new FITS file.
     
     Args:
         outputFileName (str): Filename of output FITS image.
         mapData (:obj:`np.ndarray`): Map data array.
         wcs (:obj:`astWCS.WCS`): Map WCS object.
-        compressed (bool, optional): If True, writes a compressed image.
-        compressionType (str, optional): The type of compression to use ('PLIO_1' for masks and
-            'RICE_1' for images are recommended).
+        compressionType (str, optional): If given, the data will be compressed using the given
+            method (as understood by :mod:`astropy.io.fits`). Use `PLIO_1` for masks,
+            and `RICE_1` for other image data that can stand lossy compression. If None,
+            the image data is not compressed.
     
     """
     
     wcs.header['NEMOVER']=nemo.__version__
     
     if os.path.exists(outputFileName):
         os.remove(outputFileName)
     
-    if compressed == False:
+    if compressionType is None:
         if wcs is not None:
             hdu=pyfits.PrimaryHDU(mapData, wcs.header)
         else:
             hdu=pyfits.PrimaryHDU(mapData, None)
     
-    if compressed == True:
+    if compressionType is not None:
         if wcs is not None:
             if compressionType == 'PLIO_1':
-                #wcs.header['BITPIX']=8
-                #wcs.updateFromHeader()
-                dtype=np.int32
+                dtype=np.uint8
             else:
-                dtype=np.float
+                dtype=np.float32
             hdu=pyfits.CompImageHDU(np.array(mapData, dtype = dtype), wcs.header, 
                                     compression_type = compressionType)
         else:
             hdu=pyfits.CompImageHDU(np.array(mapData, dtype = dtype), None,
                                     compression_type = compressionType)
             
     newImg=pyfits.HDUList()
     newImg.append(hdu)
     newImg.writeto(outputFileName)
     newImg.close()
+
+#---------------------------------------------------------------------------------------------------
+def makeDegreesDistanceMap(degreesMap, wcs, RADeg, decDeg, maxDistDegrees):
+    """Fills (in place) the 2d array degreesMap with distance in degrees from the given position,
+    out to some user-specified maximum distance.
+
+    Args:
+        degreesMap (:obj:`np.ndarray`): Map (2d array) that will be filled with angular distance
+            from the given coordinates. Probably you should feed in an array set to some extreme
+            initial value (e.g., 1e6 everywhere) to make it easy to filter for pixels near the
+            object coords afterwards.
+        wcs (:obj:`astWCS.WCS`): WCS corresponding to degreesMap.
+        RADeg (float): RA in decimal degrees of position of interest (e.g., object location).
+        decDeg (float): Declination in decimal degrees of position of interest (e.g., object
+            location).
+        maxDistDegrees: The maximum radius out to which distance will be calculated.
+
+    Returns:
+        A map (2d array) of distance in degrees from the given position,
+        (min x, max x) pixel coords corresponding to maxDistDegrees box,
+        (min y, max y) pixel coords corresponding to maxDistDegrees box
+
+    Note:
+        This routine measures the pixel scale local to the given position, then assumes that it
+        does not change. So, this routine may only be accurate close to the given position,
+        depending upon the WCS projection used.
+
+    """
+
+    x0, y0=wcs.wcs2pix(RADeg, decDeg)
+    ra0, dec0=RADeg, decDeg
+    ra1, dec1=wcs.pix2wcs(x0+1, y0+1)
+    xPixScale=astCoords.calcAngSepDeg(ra0, dec0, ra1, dec0)
+    yPixScale=astCoords.calcAngSepDeg(ra0, dec0, ra0, dec1)
+
+    xDistPix=int(round((maxDistDegrees)/xPixScale))
+    yDistPix=int(round((maxDistDegrees)/yPixScale))
+
+    Y=degreesMap.shape[0]
+    X=degreesMap.shape[1]
+
+    minX=int(round(x0))-xDistPix
+    maxX=int(round(x0))+xDistPix
+    minY=int(round(y0))-yDistPix
+    maxY=int(round(y0))+yDistPix
+    if minX < 0:
+        minX=0
+    if maxX > X:
+        maxX=X
+    if minY < 0:
+        minY=0
+    if maxY > Y:
+        maxY=Y
+
+    xDeg=(np.arange(degreesMap.shape[1])-x0)*xPixScale
+    yDeg=(np.arange(degreesMap.shape[0])-y0)*yPixScale
+    for i in range(minY, maxY):
+        degreesMap[i][minX:maxX]=np.sqrt(yDeg[i]**2+xDeg[minX:maxX]**2)
+
+    return degreesMap, [minX, maxX], [minY, maxY]
+
+#---------------------------------------------------------------------------------------------------
+def makeExtendedSourceMask(config, tileName):
+    """Find extended sources in all maps, adding an extended mask to the Nemo config. Each frequency
+    map will then have extended mask holes filled when preprocess is called.
+
+    """
+
+    settings=config.parDict['findAndMaskExtended']
+
+    maskCube=[]
+    for mapDict in config.unfilteredMapsDictList:
+        data, wcs=mapDict.loadTile('mapFileName', tileName, returnWCS = True)
+        weights=mapDict.loadTile('weightsFileName', tileName)
+        validMask=np.nonzero(weights)
+        whiteNoiseLevel=np.zeros(weights.shape)
+        whiteNoiseLevel[validMask]=1/np.sqrt(weights[validMask]) # Assumed inverse variance
+        # Isolate a scale that's extended
+        s1=subtractBackground(data, wcs, smoothScaleDeg = settings['bigScaleDeg'])
+        s2=subtractBackground(data, wcs, smoothScaleDeg = settings['smallScaleDeg'])
+        s=s1-s2
+        del s1, s2
+        # Make a simple global 3-sigma clipped noise estimate from the filtered map
+        # Then scale that according to the white noise level map from the map maker
+        # Assume that median white noise level there should correspond with our global clipped noise estimate
+        # (we were using mean but that blows up in edge tiles)
+        mean=0
+        sigma=1e6
+        vals=s.flatten()
+        for i in range(10):
+            mask=np.less(abs(vals-mean), 3*sigma)
+            mean=np.mean(vals[mask])
+            sigma=np.std(vals[mask])
+        scaleFactor=sigma/np.median(whiteNoiseLevel[validMask])
+        whiteNoiseLevel[validMask]=whiteNoiseLevel[validMask]*scaleFactor
+        snr=np.zeros(s.shape)
+        snr[validMask]=s[validMask]/whiteNoiseLevel[validMask]
+        # Mask set such that 1 = masked, 0 = not masked
+        extendedMask=np.array(np.greater(snr, settings['thresholdSigma']), dtype = np.uint8)
+        if 'dilationPix' in settings.keys() and settings['dilationPix'] > 0:
+            for i in range(settings['dilationPix']):
+                extendedMask=mahotas.dilate(extendedMask)
+        extendedMask[extendedMask > 0]=1
+        maskCube.append(extendedMask)
+    maskCube=np.array(maskCube, dtype = np.uint8)
+    extendedMask=maskCube.sum(axis = 0)
+    extendedMask[extendedMask > 0]=1
+
+    # Optionally cut any small objects
+    if 'minSizeArcmin2' in settings.keys() and settings['minSizeArcmin2'] > 0:
+        arcmin2Map=getPixelAreaArcmin2Map(extendedMask.shape, wcs)
+        segMap, numObjects=ndimage.label(extendedMask)
+        for i in range(1, numObjects+1):
+            if arcmin2Map[segMap == i].sum() < settings['minSizeArcmin2']:
+                extendedMask[segMap == i]=0
+
+    os.makedirs(config.diagnosticsDir+os.path.sep+"extendedMask", exist_ok = True)
+    outFileName=config.diagnosticsDir+os.path.sep+"extendedMask"+os.path.sep+tileName+".fits"
+    saveFITS(outFileName, extendedMask, wcs, compressionType = 'PLIO_1')
+
+    for mapDict in config.unfilteredMapsDictList:
+        mapDict['extendedMask']=config.diagnosticsDir+os.path.sep+"extendedMask"
+
```

### Comparing `nemo-sz-0.5.0/nemo/photometry.py` & `nemo-sz-0.6.0/nemo/photometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
            
     if rejectBorder is None:
         rejectBorder=0
 
     data=filteredMapDict['SNMap']
     areaMask=filteredMapDict['surveyMask']
     wcs=filteredMapDict['wcs']
+    flagMask=filteredMapDict['flagMask']
     
     # This is for checking contamination
     if invertMap == True:
         data=data*-1
         
     # Thresholding to identify significant pixels
     # NOTE: We're now going to detection S/N=3 to find any rings
@@ -63,15 +64,15 @@
         for i in range(len(ringIDs)):
             if type(ringNumPix) != float and ringNumPix[i] > minRingPix:
                 y, x=ringPositions[i]
                 if ringSegMap[int(y), int(x)] != ringIDs[i]:
                     ringSegMap[np.equal(ringSegMap, ringIDs[i])]=-1*ringSegMap[np.equal(ringSegMap, ringIDs[i])]
         ringSegMap=np.array(np.less(ringSegMap, 0), dtype = int)
         ringMask=ringSegMap
-        filteredMapDict['surveyMask']=filteredMapDict['surveyMask']-ringMask
+        #filteredMapDict['flagMask']=filteredMapDict['flagMask']-ringMask
     else:
         ringMask=None
 
     # In the past this had problems - Simone using happily in his fork though, so now optional
     if useInterpolator == True:
         mapInterpolator=interpolate.RectBivariateSpline(np.arange(data.shape[0]), 
                                                         np.arange(data.shape[1]), 
@@ -117,14 +118,15 @@
             objDict['numSigPix']=objNumPix[i]
             objDict['template']=filteredMapDict['label']
             objDict['tileName']=filteredMapDict['tileName']
             if useInterpolator == True:
                 objDict['SNR']=mapInterpolator(objDict['y'], objDict['x'])[0][0]
             else:
                 objDict['SNR']=data[int(round(objDict['y'])), int(round(objDict['x']))]
+            objDict['flags']=flagMask[int(round(objDict['y'])), int(round(objDict['x']))]
             # Optional SExtractor style shape measurements                
             if measureShapes == True:
                 doubleCheck=False
                 if objDict['numSigPix'] > 9:
                     mask=np.equal(segMap, objIDs[i])
                     ys, xs=np.where(segMap == objIDs[i])
                     yMin=ys.min()
```

### Comparing `nemo-sz-0.5.0/nemo/pipelines.py` & `nemo-sz-0.6.0/nemo/pipelines.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """
 
 import os
 import sys
 import glob
 import shutil
 import time
+import astropy
 import astropy.io.fits as pyfits
 import astropy.table as atpy
 from astLib import astWCS
 import numpy as np
 from scipy import ndimage, interpolate
 import copy
 from pixell import enmap
@@ -22,134 +23,101 @@
 from . import filters
 from . import photometry
 from . import catalogs
 from . import maps
 from . import signals
 from . import completeness
 from . import MockSurvey
-import nemoCython
 
 #------------------------------------------------------------------------------------------------------------
-def filterMapsAndMakeCatalogs(config, rootOutDir = None, copyFilters = False, measureFluxes = True, 
-                              invertMap = False, verbose = True, useCachedMaps = True):
+def filterMapsAndMakeCatalogs(config, rootOutDir = None, useCachedFilters = False, useCachedRMSMap = False,\
+                              measureFluxes = True, invertMap = False, verbose = True, writeAreaMask = False,\
+                              writeFlagMask = False):
     """Runs the map filtering and catalog construction steps according to the given configuration.
     
     Args:
         config (:obj: 'startup.NemoConfig'): Nemo configuration object.
         rootOutDir (str): If None, use the default given by config. Otherwise, use this to override where the
             output filtered maps and catalogs are written.
-        copyFilters (bool, optional): If True, and rootOutDir is given (not None), then filters will be
-            copied from the default output location (from a pre-existing nemo run) to the appropriate
-            directory under rootOutDir. This is used by, e.g., contamination tests based on sky sims, where
-            the same kernels as used on the real data are applied to simulated maps. If rootOutDir = None,
-            setting copyKernels = True has no effect.
+        useCachedFilters (:obj:`bool`, optional): If True, and previously made filters are found, they will be
+            read from disk, rather than re-calculated (used by source injection simulations).
+        useCachedRMSMap (:obj:`bool`, optional): If True, use the previously estimated noise map, which has
+            been saved to disk. This is only useful for source injection simulations.
         measureFluxes (bool, optional): If True, measure fluxes. If False, just extract S/N values for 
             detected objects.
         invertMap (bool, optional): If True, multiply all maps by -1; needed by 
             :meth:maps.estimateContaminationFromInvertedMaps).
     
     Returns:
         Optimal catalog (keeps the highest S/N detection when filtering at multiple scales).
     
     Note:
         See bin/nemo for how this pipeline is applied to real data, and maps.sourceInjectionTest
         for how this is applied to source-free sims that are generated on the fly.
         
     """
     
-    if config.parDict['twoPass'] == False:
-        catalog=_filterMapsAndMakeCatalogs(config, rootOutDir = rootOutDir, copyFilters = copyFilters, 
-                                           measureFluxes = measureFluxes, invertMap = invertMap, 
-                                           verbose = verbose, useCachedMaps = useCachedMaps)
-    
+    # Multi-pass pipeline, enabled with use of filterSets parameter in config file
+    if config.filterSets != [] and useCachedFilters == False:
+        # If we wanted to save results from each step, could set-up filterSet specific diagnostics dir here
+        if rootOutDir is None:
+            rootOutDir=config.rootOutDir
+        for setNum in config.filterSets:
+            print(">>> Filter set: %d" % (setNum))
+            config.setFilterSet(setNum)
+            if setNum == config.filterSets[-1]:
+                writeAreaMask=True
+                writeFlagMask=True
+            config.filterSetOptions[setNum]['catalog']=_filterMapsAndMakeCatalogs(config, verbose = True,
+                                                                                  useCachedFilters = False,
+                                                                                  writeAreaMask = writeAreaMask,
+                                                                                  writeFlagMask = writeFlagMask)
+
+            if config.filterSetOptions[setNum]['addSiphonedFromSets'] is not None:
+                toStack=[config.filterSetOptions[setNum]['catalog']]
+                for siphonSetNum in config.filterSetOptions[setNum]['addSiphonedFromSets']:
+                    toStack.append(config.filterSetOptions[siphonSetNum]['catalog'])
+                config.filterSetOptions[setNum]['catalog']=atpy.vstack(toStack)
+
+            if config.rank == 0:
+                if config.filterSetOptions[setNum]['saveCatalog'] == True:
+                    if 'label' not in config.filterSetOptions[setNum].keys():
+                        label="filterSet%d" % (setNum)
+                    else:
+                        label=config.filterSetOptions[setNum]['label']
+                    outFileName=rootOutDir+os.path.sep+label+"_catalog.fits"
+                    catalogs.writeCatalog(config.filterSetOptions[setNum]['catalog'], outFileName)
+                    catalogs.catalog2DS9(config.filterSetOptions[setNum]['catalog'], outFileName.replace(".fits", ".reg"))
+
+        catalog=config.filterSetOptions[config.filterSets[-1]]['catalog']
+
     else:
-        
-        # Two pass pipeline
-        # On 1st pass, find sources (and maybe clusters) with canned settings, masking nothing.
-        # On 2nd pass, the 1st pass catalog will be used to mask or subtract sources from maps used for 
-        # noise estimation only.
-        
-        # No point doing this if we're not using the map itself for the noise term in the filter
-        for f in config.parDict['mapFilters']:
-            for key in f.keys():
-                if key == 'noiseParams' and f['noiseParams']['method'] != 'dataMap':
-                    raise Exception("There is no point running if filter noise method != 'dataMap'.")
-
-        # Pass 1 - find point sources, save nothing
-        # NOTE: We need to do this for each map in the list, if we have a multi-frequency filter
-        pass1PtSrcSettings={'label': "Beam",
-                            'class': "BeamMatchedFilter",
-                            'params': {'noiseParams': {'method': "model",
-                                                       'noiseGridArcmin': 40.0,
-                                                       'numNoiseBins': 2},
-                            'saveFilteredMaps': False,
-                            'outputUnits': 'uK',
-                            'edgeTrimArcmin': 0.0}}
-        config.parDict['mapFilters']=[pass1PtSrcSettings]
-        config.parDict['photFilter']=None
-        config.parDict['maskPointSourcesFromCatalog']=[]    # This is only applied on the 2nd pass
-        config.parDict['measureShapes']=True    # Double-lobed extended source at f090 causes havoc in one tile
-        orig_unfilteredMapsDictList=list(config.unfilteredMapsDictList)
-        config.parDict['forcedPhotometryCatalog']=None # If in this mode, only wanted on 2nd pass
-        pass1CatalogsList=[]
-        surveyMasksList=[] # ok, these should all be the same, otherwise we have problems...
-        for mapDict in orig_unfilteredMapsDictList:
-            # We use whole tile area (i.e., don't trim overlaps) so that we get everything if under MPI
-            # Otherwise, powerful sources in overlap regions mess things up under MPI
-            # Serial mode doesn't have this issue as it can see the whole catalog over all tiles
-            # But since we now use full area, we may double subtract ovelap sources when in serial mode
-            # So the removeDuplicates call fixes that, and doesn't impact anything else here
-            surveyMasksList.append(mapDict['surveyMask'])
-            mapDict['surveyMask']=None
-            config.unfilteredMapsDictList=[mapDict]
-            catalog=_filterMapsAndMakeCatalogs(config, verbose = False, writeAreaMasks = False)
-            if len(catalog) > 0 :
-                catalog, numDuplicatesFound, names=catalogs.removeDuplicates(catalog)
-            pass1CatalogsList.append(catalog)
-
-        # Pass 2 - subtract point sources in the maps used for noise term in filter only
-        # To avoid ringing in the pass 2, we siphon off the super bright things found in pass 1
-        # We subtract those from the maps used in pass 2 - we then need to add them back at the end
-        config.restoreConfig()
-        config.parDict['measureShapes']=True    # We'll keep this for pass 2 as well
-        siphonSNR=50
-        for mapDict, catalog, surveyMask in zip(orig_unfilteredMapsDictList, pass1CatalogsList, surveyMasksList):
-            #catalogs.catalog2DS9(catalog[catalog['SNR'] > siphonSNR], config.diagnosticsDir+os.path.sep+"pass1_highSNR_siphoned.reg")
-            mapDict['noiseMaskCatalog']=catalog[catalog['SNR'] < siphonSNR]
-            mapDict['subtractPointSourcesFromCatalog']=[catalog[catalog['SNR'] > siphonSNR]]
-            mapDict['maskSubtractedPointSources']=True
-            mapDict['surveyMask']=surveyMask
-        config.unfilteredMapsDictList=orig_unfilteredMapsDictList
-        catalog=_filterMapsAndMakeCatalogs(config, verbose = False)
-        
-        # Merge back in the bright sources that were subtracted in pass 1
-        # (but we don't do that in forced photometry mode)
-        mergeList=[catalog]
-        if config.parDict['forcedPhotometryCatalog'] is None:
-            for pass1Catalog in pass1CatalogsList:
-                mergeList.append(pass1Catalog[pass1Catalog['SNR'] > siphonSNR])
-        catalog=atpy.vstack(mergeList)
-    
+        # Default single pass behaviour (also used by source injection tests)
+        catalog=_filterMapsAndMakeCatalogs(config, rootOutDir = rootOutDir, useCachedFilters = useCachedFilters,
+                                           useCachedRMSMap = useCachedRMSMap, measureFluxes = measureFluxes,
+                                           invertMap = invertMap, verbose = verbose,
+                                           writeAreaMask = writeAreaMask, writeFlagMask = writeFlagMask)
+
+    if verbose == True and config.rank == 0:
+        print("... after map filtering and making catalogs: time since start = %.3f sec" % (time.time()-config._timeStarted))
+
     return catalog
-    
+
 #------------------------------------------------------------------------------------------------------------
-def _filterMapsAndMakeCatalogs(config, rootOutDir = None, copyFilters = False, measureFluxes = True, 
-                               invertMap = False, verbose = True, useCachedMaps = True,
-                               writeAreaMasks = True):
+def _filterMapsAndMakeCatalogs(config, rootOutDir = None, useCachedFilters = False, useCachedRMSMap = False,\
+                               measureFluxes = True, invertMap = False, verbose = True, writeAreaMask = False,\
+                               writeFlagMask = False):
     """Runs the map filtering and catalog construction steps according to the given configuration.
     
     Args:
         config (:obj: 'startup.NemoConfig'): Nemo configuration object.
         rootOutDir (str): If None, use the default given by config. Otherwise, use this to override where the
             output filtered maps and catalogs are written.
-        copyFilters (bool, optional): If True, and rootOutDir is given (not None), then filters will be
-            copied from the default output location (from a pre-existing nemo run) to the appropriate
-            directory under rootOutDir. This is used by, e.g., contamination tests based on sky sims, where
-            the same kernels as used on the real data are applied to simulated maps. If rootOutDir = None,
-            setting copyKernels = True has no effect.
+        useCachedFilters (:obj:`bool`, optional): If True, and previously made filters are found, they will be
+            read from disk, rather than re-calculated (used by source injection simulations).
         measureFluxes (bool, optional): If True, measure fluxes. If False, just extract S/N values for 
             detected objects.
         invertMap (bool, optional): If True, multiply all maps by -1; needed by 
             :meth:maps.estimateContaminationFromInvertedMaps).
     
     Returns:
         Optimal catalog (keeps the highest S/N detection when filtering at multiple scales).
@@ -165,26 +133,14 @@
     # will then be loaded automatically when filterMaps is called. Yes, this is a bit clunky...
     if rootOutDir is not None:
         filteredMapsDir=rootOutDir+os.path.sep+"filteredMaps"
         diagnosticsDir=rootOutDir+os.path.sep+"diagnostics"
         dirList=[rootOutDir, filteredMapsDir, diagnosticsDir]
         for d in dirList:
             os.makedirs(d, exist_ok = True)
-        if copyFilters == True:
-            for tileName in config.tileNames:
-                fileNames=glob.glob(config.diagnosticsDir+os.path.sep+tileName+os.path.sep+"filter*#%s*.fits" % (tileName))
-                if len(fileNames) == 0:
-                    raise Exception("Could not find pre-computed filters to copy - you need to add 'saveFilter: True' to the filter params in the config file (this is essential for doing source injection sims quickly).")
-                kernelCopyDestDir=diagnosticsDir+os.path.sep+tileName
-                os.makedirs(kernelCopyDestDir, exist_ok = True)
-                for f in fileNames:
-                    dest=kernelCopyDestDir+os.path.sep+os.path.split(f)[-1]
-                    if os.path.exists(dest) == False:
-                        shutil.copyfile(f, dest) 
-                        print("... copied filter %s to %s ..." % (f, dest))
     else:
         rootOutDir=config.rootOutDir
         filteredMapsDir=config.filteredMapsDir
         diagnosticsDir=config.diagnosticsDir
     
     # We re-sort the filters list here - in case we have photFilter defined
     photFilter=config.parDict['photFilter']
@@ -194,44 +150,70 @@
             if f['label'] == photFilter:
                 filtersList.append(f)
     for f in config.parDict['mapFilters']:
         if photFilter is not None:
             if f['label'] == photFilter:
                 continue
         filtersList.append(f)
-    if photFilter is not None:
+    if photFilter is not None and len(config.parDict['mapFilters']) > 1:
         assert(filtersList[0]['label'] == photFilter)
     photFilteredMapDict=None
-    
+
+    # For source injection stuff (yes, this is messy - see below for why we do this)
+    undoPixelWindow=True
+    if useCachedRMSMap == True:
+        undoPixelWindow=False
+
     # Make filtered maps for each filter and tile
     catalogDict={}
+    areaMaskDict=maps.TileDict({}, tileCoordsDict = config.tileCoordsDict)
+    flagMaskDict=maps.TileDict({}, tileCoordsDict = config.tileCoordsDict)
     for tileName in config.tileNames:
-        # Now have per-tile directories (friendlier for Lustre)
-        tileFilteredMapsDir=filteredMapsDir+os.path.sep+tileName
-        tileDiagnosticsDir=diagnosticsDir+os.path.sep+tileName
-        for d in [tileFilteredMapsDir, tileDiagnosticsDir]:
-            os.makedirs(d, exist_ok = True)
-        if verbose == True: print(">>> Making filtered maps - tileName = %s ..." % (tileName))
-        # We could load the unfiltered map only once here?
-        # We could also cache 'dataMap' noise as it will always be the same
+        if verbose == True: print(">>> [rank = %d] Making filtered maps - tileName = %s " % (config.rank, tileName))
+        # Operations that only need to be done once go here
+        if 'findAndMaskExtended' in config.parDict.keys():
+            maps.makeExtendedSourceMask(config, tileName)
         for f in filtersList:
 
             label=f['label']+"#"+tileName            
             catalogDict[label]={}
             if 'saveDS9Regions' in f['params'] and f['params']['saveDS9Regions'] == True:
                 DS9RegionsPath=config.filteredMapsDir+os.path.sep+tileName+os.path.sep+"%s_filteredMap.reg"  % (label)
             else:
                 DS9RegionsPath=None
-                
+
             filteredMapDict=filters.filterMaps(config.unfilteredMapsDictList, f, tileName, 
-                                               filteredMapsDir = tileFilteredMapsDir,
-                                               diagnosticsDir = tileDiagnosticsDir, selFnDir = config.selFnDir, 
-                                               verbose = True, undoPixelWindow = True,
-                                               useCachedMaps = useCachedMaps)
-            
+                                               diagnosticsDir = config.diagnosticsDir, selFnDir = config.selFnDir,
+                                               verbose = True, undoPixelWindow = undoPixelWindow,
+                                               useCachedFilter = useCachedFilters)
+
+            if useCachedRMSMap == True and photFilter is not None: # i.e., only an option for cluster insertion sims
+                # This is messy:
+                # 1. the saved RMS map doesn't have pixel window correction undone
+                # 2. we make the S/N map before doing the pixel window correction (it would cancel)
+                # 3. but if we're running a source injection sim using the cached RMS map, we'd make a new SN map
+                #    here that has the pixel window correction undone for S, but not for N
+                # 4. so, if we're doing source injection sims, we DON'T want to undo pixel window in call to filterMaps
+                #    above
+                # 5. but then we DO want to undo the pixel window after we've made our new S/N map here
+                RMSMap, wcs=completeness.loadRMSMap(tileName, config.selFnDir, photFilter)
+                validMask=np.greater(RMSMap, 0)
+                SNMap=np.zeros(filteredMapDict['data'].shape)+filteredMapDict['data']
+                SNMap[validMask]=SNMap[validMask]/RMSMap[validMask]
+                filteredMapDict['SNMap']=SNMap
+                mask=np.equal(filteredMapDict['data'], 0)
+                filteredMapDict['data']=enmap.apply_window(filteredMapDict['data'], pow=-1.0)
+                filteredMapDict['data'][mask]=0 # just in case we rely elsewhere on zero == no data
+
+            if 'saveFilteredMaps' in f['params'] and f['params']['saveFilteredMaps'] == True:
+                filteredMapFileName=filteredMapsDir+os.path.sep+tileName+os.path.sep+"%s_filteredMap.fits"  % (label)
+                SNMapFileName=filteredMapsDir+os.path.sep+tileName+os.path.sep+"%s_SNMap.fits" % (label)
+                maps.saveFITS(filteredMapFileName, filteredMapDict['data'], filteredMapDict['wcs'])
+                maps.saveFITS(SNMapFileName, filteredMapDict['SNMap'], filteredMapDict['wcs'])
+
             if f['label'] == photFilter:
                 photFilteredMapDict={}
                 photFilteredMapDict['SNMap']=filteredMapDict['SNMap']
                 photFilteredMapDict['data']=filteredMapDict['data']
 
             # Forced photometry on user-supplied list of objects, or detect sources
             if 'forcedPhotometryCatalog' in config.parDict.keys() and config.parDict['forcedPhotometryCatalog'] is not None:
@@ -239,136 +221,217 @@
                                                                config.parDict['forcedPhotometryCatalog'],
                                                                useInterpolator = config.parDict['useInterpolator'],
                                                                DS9RegionsPath = DS9RegionsPath)
             else:
                 # Normal mode
                 catalog=photometry.findObjects(filteredMapDict, threshold = config.parDict['thresholdSigma'], 
                                                minObjPix = config.parDict['minObjPix'], 
-                                               findCenterOfMass = config.parDict['findCenterOfMass'], 
+                                               findCenterOfMass = config.parDict['findCenterOfMass'],
                                                removeRings = config.parDict['removeRings'],
                                                ringThresholdSigma = config.parDict['ringThresholdSigma'],
                                                rejectBorder = config.parDict['rejectBorder'], 
-                                               objIdent = config.parDict['objIdent'], 
+                                               objIdent = config.parDict['objIdent'],
                                                longNames = config.parDict['longNames'],
                                                useInterpolator = config.parDict['useInterpolator'], 
                                                measureShapes = config.parDict['measureShapes'],
                                                invertMap = invertMap,
                                                DS9RegionsPath = DS9RegionsPath)
             
-            # We write area mask here, because it gets modified by findObjects if removing rings
-            # NOTE: condition added to stop writing tile maps again when running nemoMass in forced photometry mode
-            maskFileName=config.selFnDir+os.path.sep+"areaMask#%s.fits" % (tileName)
-            surveyMask=np.array(filteredMapDict['surveyMask'], dtype = int)
-            if writeAreaMasks == True:
-                if os.path.exists(maskFileName) == False and os.path.exists(config.selFnDir+os.path.sep+"areaMask.fits") == False:
-                    maps.saveFITS(maskFileName, surveyMask, filteredMapDict['wcs'], compressed = True,
-                                  compressionType = 'PLIO_1')
+            # We collect the area mask here, because it gets modified by findObjects if removing rings
+            # NOTE: area mask should always be the same across all filters, could add a consistency check here
+            if writeAreaMask == True and tileName not in areaMaskDict.keys():
+                areaMaskDict[tileName]=np.array(filteredMapDict['surveyMask'], dtype = np.uint8)
+
+            if writeFlagMask == True and tileName not in flagMaskDict.keys():
+                flagMaskDict[tileName]=filteredMapDict['flagMask']
             
             if measureFluxes == True:
                 photometry.measureFluxes(catalog, filteredMapDict, config.diagnosticsDir,
                                          photFilteredMapDict = photFilteredMapDict,
                                          useInterpolator = config.parDict['useInterpolator'])
 
             else:
                 # Get S/N only - if the reference (fixed) filter scale has been given
                 # This is (probably) only used by maps.estimateContaminationFromInvertedMaps
                 if photFilter is not None:
                     photometry.getSNRValues(catalog, photFilteredMapDict['SNMap'], 
                                             filteredMapDict['wcs'], prefix = 'fixed_', 
                                             useInterpolator = config.parDict['useInterpolator'],
                                             invertMap = invertMap)
-            
+            del filteredMapDict
             catalogDict[label]['catalog']=catalog
 
     # Merged/optimal catalogs
     optimalCatalog=catalogs.makeOptimalCatalog(catalogDict, constraintsList = config.parDict['catalogCuts'])
     
+    if config.MPIEnabled == True:
+        # area mask
+        if writeAreaMask == True:
+            #config.comm.barrier()
+            if config.rank > 0:
+                config.comm.send(areaMaskDict, dest = 0)
+            elif config.rank == 0:
+                gathered_tileDicts=[]
+                gathered_tileDicts.append(areaMaskDict)
+                for source in range(1, config.size):
+                    gathered_tileDicts.append(config.comm.recv(source = source))
+                print("... gathered area mask")
+                for tileDict in gathered_tileDicts:
+                    for tileName in tileDict.keys():
+                        areaMaskDict[tileName]=tileDict[tileName]
+        # flag mask
+        if writeFlagMask == True:
+            #config.comm.barrier()
+            if config.rank > 0:
+                config.comm.send(flagMaskDict, dest = 0)
+            elif config.rank == 0:
+                gathered_tileDicts=[]
+                gathered_tileDicts.append(flagMaskDict)
+                for source in range(1, config.size):
+                    gathered_tileDicts.append(config.comm.recv(source = source))
+                print("... gathered flag mask")
+                for tileDict in gathered_tileDicts:
+                    for tileName in tileDict.keys():
+                        flagMaskDict[tileName]=tileDict[tileName]
+
+        # catalogs - every node now gets the whole catalog, for running in multipass mode
+        optimalCatalogList=config.comm.allgather(optimalCatalog)
+        if config.rank == 0: print("... gathered catalogs")
+        toStack=[]  # We sometimes return [] if no objects found - we can't vstack those
+        for collectedTab in optimalCatalogList:
+            if type(collectedTab) == astropy.table.table.Table and len(collectedTab) > 0:
+                toStack.append(collectedTab)
+        optimalCatalog=atpy.vstack(toStack)
+        # Strip out duplicates (this is necessary when run in tileDir mode under MPI)
+        if len(optimalCatalog) > 0:
+            optimalCatalog, numDuplicatesFound, names=catalogs.removeDuplicates(optimalCatalog)
+
+    # Write masks - MEFs [barrier here because needed for next step]
+    if config.rank == 0:
+        if writeAreaMask == True:
+            areaMaskDict.saveMEF(config.selFnDir+os.path.sep+"areaMask.fits", compressionType = 'PLIO_1')
+        if writeFlagMask == True:
+            flagMaskDict.saveMEF(config.selFnDir+os.path.sep+"flagMask.fits", compressionType = 'PLIO_1')
+    if config.MPIEnabled == True:
+        config.comm.barrier()
+
+    # Write masks - stitched [done by rank 0 while processesothers move on]
+    if config.rank == 0:
+        if writeAreaMask == True and config.parDict['stitchTiles'] == True:
+            areaMaskDict.saveStitchedFITS(config.selFnDir+os.path.sep+"stitched_areaMask.fits",
+                                          config.origWCS, compressionType = 'PLIO_1')
+
+        if writeFlagMask == True and config.parDict['stitchTiles'] == True:
+            flagMaskDict.saveStitchedFITS(config.selFnDir+os.path.sep+"stitched_flagMask.fits",
+                                          config.origWCS, compressionType = 'PLIO_1')
+
+    del areaMaskDict, flagMaskDict, catalogDict
+
     return optimalCatalog
 
 #------------------------------------------------------------------------------------------------------------
-def makeSelFnCollection(config, mockSurvey):
+def makeRMSTables(config):
     """Makes a collection of selection function dictionaries (one per footprint specified in selFnFootprints
-    in the config file, plus the full survey mask), that contain information on noise levels, area covered, 
-    and completeness. 
-    
-    Returns a dictionary (keys: 'full' - corresponding to whole survey, plus other keys named by footprint).
-    
+    in the config file, plus the full survey mask), that contain information on noise levels and area covered,
+    and completeness. Adds footprint columns to object catalog.
+
     """
-    
-    # Q varies across tiles
-    Q=signals.QFit(config)
-        
+
     # We only care about the filter used for fixed_ columns
+    if config.parDict['photFilter'] is None:
+        return None
     photFilterLabel=config.parDict['photFilter']
     for filterDict in config.parDict['mapFilters']:
         if filterDict['label'] == photFilterLabel:
             break
-
-    # We'll only calculate completeness for this given selection
-    SNRCut=config.parDict['selFnOptions']['fixedSNRCut']
-
-    # Handle any missing options for calcCompleteness (these aren't used by the default fast method anyway)
-    if 'numDraws' not in config.parDict['selFnOptions'].keys():
-        config.parDict['selFnOptions']['numDraws']=2000000
-    if 'numIterations' not in config.parDict['selFnOptions'].keys():
-        config.parDict['selFnOptions']['numIterations']=100
     
     # We can calculate stats in different extra areas (e.g., inside optical survey footprints)
     footprintsList=[]
     if 'selFnFootprints' in config.parDict.keys():
         footprintsList=footprintsList+config.parDict['selFnFootprints']
         
     # Run the selection function calculation on each tile in turn
     selFnCollection={'full': []}
     for footprintDict in footprintsList:
         if footprintDict['label'] not in selFnCollection.keys():
             selFnCollection[footprintDict['label']]=[]
-            
+
     for tileName in config.tileNames:
         RMSTab=completeness.getRMSTab(tileName, photFilterLabel, config.selFnDir)
-        compMz=completeness.calcCompleteness(RMSTab, SNRCut, tileName, mockSurvey, config.parDict['massOptions'], Q, 
-                                           numDraws = config.parDict['selFnOptions']['numDraws'],
-                                           numIterations = config.parDict['selFnOptions']['numIterations'],
-                                           method = config.parDict['selFnOptions']['method'])
         selFnDict={'tileName': tileName,
                    'RMSTab': RMSTab,
-                   'tileAreaDeg2': RMSTab['areaDeg2'].sum(),
-                   'compMz': compMz}
+                   'tileAreaDeg2': RMSTab['areaDeg2'].sum()}
         selFnCollection['full'].append(selFnDict)
-        
+
         # Generate footprint intersection masks (e.g., with HSC) and RMS tables, which are cached
         # May as well do this bit here (in parallel) and assemble output later
         for footprintDict in footprintsList:
             completeness.makeIntersectionMask(tileName, config.selFnDir, footprintDict['label'], masksList = footprintDict['maskList'])
             tileAreaDeg2=completeness.getTileTotalAreaDeg2(tileName, config.selFnDir, footprintLabel = footprintDict['label'])
             if tileAreaDeg2 > 0:
                 RMSTab=completeness.getRMSTab(tileName, photFilterLabel, config.selFnDir,
                                               footprintLabel = footprintDict['label'])
-                compMz=completeness.calcCompleteness(RMSTab, SNRCut, tileName, mockSurvey, config.parDict['massOptions'], Q,
-                                                   numDraws = config.parDict['selFnOptions']['numDraws'],
-                                                   numIterations = config.parDict['selFnOptions']['numIterations'],
-                                                   method = config.parDict['selFnOptions']['method'])
                 selFnDict={'tileName': tileName,
                            'RMSTab': RMSTab,
-                           'tileAreaDeg2': RMSTab['areaDeg2'].sum(),
-                           'compMz': compMz}
+                           'tileAreaDeg2': RMSTab['areaDeg2'].sum()}
                 selFnCollection[footprintDict['label']].append(selFnDict)
-            
-        # Optional mass-limit maps
-        if 'massLimitMaps' in list(config.parDict['selFnOptions'].keys()):
-            for massLimitDict in config.parDict['selFnOptions']['massLimitMaps']:
-                completeness.makeMassLimitMap(SNRCut, massLimitDict['z'], tileName, photFilterLabel, mockSurvey, 
-                                            config.parDict['massOptions'], Q, config.diagnosticsDir,
-                                            config.selFnDir) 
-    
-    return selFnCollection
-                
+
+    if config.MPIEnabled == True:
+        #config.comm.barrier()
+        gathered_selFnCollections=config.comm.gather(selFnCollection, root = 0)
+        if config.rank == 0:
+            print("... gathered RMS tables")
+            all_selFnCollection={'full': []}
+            for key in selFnCollection.keys():
+                if key not in all_selFnCollection.keys():
+                    all_selFnCollection[key]=[]
+            for selFnCollection in gathered_selFnCollections:
+                for key in all_selFnCollection.keys():
+                    all_selFnCollection[key]=all_selFnCollection[key]+selFnCollection[key]
+            selFnCollection=all_selFnCollection
+
+    # Combine RMSTab files (we can downsample further later if needed)
+    # We add a column for the tileName just in case want to select on this later
+    if config.rank == 0:
+        strLen=0
+        for tileName in config.allTileNames:
+            if len(tileName) > strLen:
+                strLen=len(tileName)
+        for footprint in selFnCollection.keys():
+            if footprint == "full":
+                label=""
+            else:
+                label="_"+footprint
+            outFileName=config.selFnDir+os.path.sep+"RMSTab"+label+".fits"
+            tabList=[]
+            for selFnDict in selFnCollection[footprint]:
+                tileName=selFnDict['tileName']
+                tileTab=selFnDict['RMSTab']
+                tileTab['tileName']=atpy.Column(np.array([tileName]*len(tileTab),
+                                                dtype = '<U%d' % (strLen)), "tileName")
+                tabList.append(tileTab)
+            if len(tabList) > 0:
+                tab=atpy.vstack(tabList)
+                tab.sort('y0RMS')
+                tab.meta['NEMOVER']=nemo.__version__
+                tab.write(outFileName, overwrite = True)
+
+        # Add footprint columns to object catalog
+        catFileName=config.rootOutDir+os.path.sep+"%s_optimalCatalog.fits" % (os.path.split(config.rootOutDir)[-1])
+        tab=atpy.Table().read(catFileName)
+        for footprintDict in footprintsList:
+            for maskPath in footprintDict['maskList']:
+                m, wcs=maps.chunkLoadMask(maskPath)
+                tab=catalogs.addFootprintColumnToCatalog(tab, footprintDict['label'], m, wcs)
+        catalogs.writeCatalog(tab, catFileName)
+        catalogs.writeCatalog(tab, catFileName.replace(".fits", ".csv"))
+
 #------------------------------------------------------------------------------------------------------------
-def makeMockClusterCatalog(config, numMocksToMake = 1, combineMocks = False, writeCatalogs = True, 
-                           writeInfo = True, verbose = True):
+def makeMockClusterCatalog(config, numMocksToMake = 1, combineMocks = False, writeCatalogs = True,\
+                           writeInfo = True, verbose = True, QSource = 'fit'):
     """Generate a mock cluster catalog using the given nemo config.
     
     Returns:
         List of catalogs (each is an astropy Table object)
     
     """
     
@@ -387,17 +450,16 @@
         applyIntrinsicScatter=True
     if 'applyNoiseScatter' in config.parDict.keys():
         applyNoiseScatter=config.parDict['applyNoiseScatter']
     else:
         applyNoiseScatter=True
     if verbose: print(">>> Mock noise sources (Poisson, intrinsic, measurement noise) = (%s, %s, %s) ..." % (applyPoissonScatter, applyIntrinsicScatter, applyNoiseScatter))
     
-    # Q varies across tiles
-    Q=signals.QFit(config)
-    
+    Q=signals.QFit(QSource = QSource, selFnDir = config.selFnDir, tileNames = config.allTileNames)
+
     # We only care about the filter used for fixed_ columns
     photFilterLabel=config.parDict['photFilter']
     for filterDict in config.parDict['mapFilters']:
         if filterDict['label'] == photFilterLabel:
             break
         
     # The same as was used for detecting objects
@@ -480,14 +542,15 @@
     sigma8=massOptions['sigma8']
     ns=massOptions['ns']
     delta=massOptions['delta']
     rhoType=massOptions['rhoType']
     mockSurvey=MockSurvey.MockSurvey(minMass, totalAreaDeg2, zMin, zMax, H0, Om0, Ob0, sigma8, ns, 
                                      delta = delta, rhoType = rhoType, enableDrawSample = True)
     print("... mock survey parameters:")
+    print("    QSource = %s" % (QSource))
     for key in defCosmo.keys():
         print("    %s = %s" % (key, str(massOptions[key])))
     for key in ['tenToA0', 'B0', 'Mpivot', 'sigma_int']:
         print("    %s = %s" % (key, str(scalingRelationDict[key])))
     print("    total area = %.1f square degrees" % (totalAreaDeg2))
     print("    random seed = %s" % (str(seed)))
     
@@ -516,14 +579,15 @@
         if verbose: print("... making mock catalog %d took %.3f sec ..." % (i+1, t1-t0))
         
         # Write catalog and .reg file
         if writeCatalogs == True:
             #colNames=['name', 'RADeg', 'decDeg', 'template', 'redshift', 'redshiftErr', 'true_M500', 'true_fixed_y_c', 'fixed_SNR', 'fixed_y_c', 'fixed_err_y_c']
             #colFmts =['%s',   '%.6f',  '%.6f',   '%s',       '%.3f',     '%.3f',        '%.3f',      '%.3f',           '%.1f',      '%.3f',      '%.3f']
             mockCatalogFileName=config.mocksDir+os.path.sep+"mockCatalog_%d.csv" % (i+1)
+            tab.meta['QSOURCE']=QSource
             catalogs.writeCatalog(tab, mockCatalogFileName)
             catalogs.writeCatalog(tab, mockCatalogFileName.replace(".csv", ".fits"))
 
             addInfo=[{'key': 'fixed_SNR', 'fmt': '%.1f'}]
             catalogs.catalog2DS9(tab, mockCatalogFileName.replace(".csv", ".reg"), constraintsList = [], 
                                     addInfo = addInfo, color = "cyan") 
             
@@ -534,14 +598,15 @@
             stackTab=atpy.Table().read(mockCatalogFileName)
             if tab == None:
                 tab=stackTab
             else:
                 tab=atpy.vstack([tab, stackTab])
         outFileName=config.mocksDir+os.path.sep+"mockCatalog_combined.fits"
         tab.meta['NEMOVER']=nemo.__version__
+        tab.meta['QSOURCE']=QSource
         tab.write(outFileName, overwrite = True)
     
     # Write a small text file with the parameters used to generate the mocks into the mocks dir (easier than using headers)
     if writeInfo == True:
         mockKeys=['massOptions', 'makeMockCatalogs', 'applyPoissonScatter', 'applyIntrinsicScatter', 'applyNoiseScatter']
         with open(config.mocksDir+os.path.sep+"mockParameters.txt", "w") as outFile:
             for m in mockKeys:
@@ -699,15 +764,15 @@
             wcs.header['CDELT2']=np.diff(refBeam.rDeg)[0]
             wcs.header['NAXIS1']=int(np.ceil(2*refBeam.rDeg.max()/wcs.header['CDELT1'])) 
             wcs.header['NAXIS2']=int(np.ceil(2*refBeam.rDeg.max()/wcs.header['CDELT2']))
             wcs.updateFromHeader()
             shape=(wcs.header['NAXIS2'], wcs.header['NAXIS1'])
             degreesMap=np.ones([shape[0], shape[1]], dtype = float)*1e6
             RADeg, decDeg=wcs.pix2wcs(int(degreesMap.shape[1]/2), int(degreesMap.shape[0]/2))
-            degreesMap, xBounds, yBounds=nemoCython.makeDegreesDistanceMap(degreesMap, wcs, RADeg, decDeg, 1.0)
+            degreesMap, xBounds, yBounds=maps.makeDegreesDistanceMap(degreesMap, wcs, RADeg, decDeg, 1.0)
             beamMap=signals.makeBeamModelSignalMap(degreesMap, wcs, beam, amplitude = None)
             refBeamMap=signals.makeBeamModelSignalMap(degreesMap, wcs, refBeam, amplitude = None)
             matchedBeamMap=maps.convolveMapWithBeam(beamMap*attenuationFactor, wcs, convKernel, maxDistDegrees = 1.0)
             
             # Find and apply radial fudge factor
             yRow=np.where(refBeamMap == refBeamMap.max())[0][0]
             rowValid=np.logical_and(degreesMap[yRow] < refBeam.rDeg.max(), matchedBeamMap[yRow] != 0)
@@ -912,17 +977,17 @@
         tileTab=catalogs.getCatalogWithinImage(tab, shape, wcs)
         for label in freqLabels:
             tileTab['diskT_uKArcmin2_%s' % (label)]=np.zeros(len(tileTab))
             tileTab['err_diskT_uKArcmin2_%s' % (label)]=np.zeros(len(tileTab))
             tileTab['diskSNR_%s' % (label)]=np.zeros(len(tileTab))
         for row in tileTab:
             degreesMap=np.ones(shape, dtype = float)*1e6 # NOTE: never move this
-            degreesMap, xBounds, yBounds=nemoCython.makeDegreesDistanceMap(degreesMap, wcs, 
-                                                                           row['RADeg'], row['decDeg'],
-                                                                           maxSizeDeg)
+            degreesMap, xBounds, yBounds=maps.makeDegreesDistanceMap(degreesMap, wcs,
+                                                                     row['RADeg'], row['decDeg'],
+                                                                     maxSizeDeg)
             innerMask=degreesMap < innerRadiusArcmin/60
             outerMask=np.logical_and(degreesMap >= innerRadiusArcmin/60, degreesMap < outerRadiusArcmin/60)
             for mapDict, label in zip(mapDictList, freqLabels):
                 d=mapDict['data'] 
                 diskFlux=(d[innerMask]*pixAreaMap[innerMask]).sum()-(d[outerMask]*pixAreaMap[outerMask]).sum()
                 row['diskT_uKArcmin2_%s' % (label)]=diskFlux
             
@@ -931,17 +996,17 @@
         # We can later add something that scales / fits using the weight map?
         if estimateErrors == True:
             randTab=catalogs.generateRandomSourcesCatalog(mapDict['surveyMask'], wcs, 1000)
             for label in freqLabels:
                 randTab['diskT_uKArcmin2_%s' % (label)]=np.zeros(len(randTab))
             for row in randTab:
                 degreesMap=np.ones(shape, dtype = float)*1e6 # NOTE: never move this
-                degreesMap, xBounds, yBounds=nemoCython.makeDegreesDistanceMap(degreesMap, wcs, 
-                                                                                row['RADeg'], row['decDeg'], 
-                                                                                maxSizeDeg)
+                degreesMap, xBounds, yBounds=maps.makeDegreesDistanceMap(degreesMap, wcs,
+                                                                         row['RADeg'], row['decDeg'],
+                                                                         maxSizeDeg)
                 innerMask=degreesMap < innerRadiusArcmin/60
                 outerMask=np.logical_and(degreesMap >= innerRadiusArcmin/60, degreesMap < outerRadiusArcmin/60)
                 for mapDict, label in zip(mapDictList, freqLabels):
                     d=mapDict['data'] 
                     diskFlux=(d[innerMask]*pixAreaMap[innerMask]).sum()-(d[outerMask]*pixAreaMap[outerMask]).sum()
                     row['diskT_uKArcmin2_%s' % (label)]=diskFlux
             noiseLevels={}
```

### Comparing `nemo-sz-0.5.0/nemo/plotSettings.py` & `nemo-sz-0.6.0/nemo/plotSettings.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,9 +38,9 @@
     # defined
     for key in dict:
         plt.rcParams[key] = dict[key]
 
     # From https://github.com/mhasself/rg_friendly
     plt.rcParams['axes.prop_cycle']=cycler(color=['#2424f0','#df6f0e','#3cc03c','#d62728','#b467bd','#ac866b','#e397d9','#9f9f9f','#ecdd72','#77becf'])
 
-
-
+# Let's just do this whenever it's imported
+update_rcParams()
```

### Comparing `nemo-sz-0.5.0/nemo/signals.py` & `nemo-sz-0.6.0/nemo/signals.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This module contains routines for modeling cluster and source signals.
 
 """
 
 import os
 import sys
-from pixell import enmap
+from pixell import enmap, curvedsky, utils, pointsrcs
 import astropy
 import astropy.wcs as enwcs
 import astropy.io.fits as pyfits
 import astropy.constants as constants
 #from astropy.cosmology import FlatLambdaCDM
 from astLib import *
 from scipy import ndimage
@@ -20,23 +20,22 @@
 import astropy.table as atpy
 import nemo
 from . import maps
 from . import catalogs
 from . import photometry
 from . import filters
 from . import gnfw
+from . import completeness
 from . import plotSettings
 import numpy as np
 import numpy.fft as fft
 import math
 import pylab as plt
 import pickle
 import operator
-import pyximport; pyximport.install()
-import nemoCython
 import nemo
 import glob
 import shutil
 import yaml
 import warnings
 #import IPython
 np.random.seed()
@@ -73,158 +72,200 @@
     M200cDef=None
     M500cDef=None
 
 #------------------------------------------------------------------------------------------------------------
 class BeamProfile(object):
     """Describes the beam profile (i.e., the point spread function for some instrument in real space). This
     can be either read from a white-space delimited text file (with the angle in degrees in the first column
-    and the response in the second column), or can be set directly using arrays.
+    and the response in the second column; or as a beam transform file with *l* in the first column, and
+    *B*\ :sub:`l` in the second column), or can be set directly using arrays.
     
     Args:
-        beamFileName(:obj:`str`, optional): Path to text file containing a beam profile in the ACT format.
+        beamFileName(:obj:`str`, optional): Path to text file containing a beam profile (or transform) in
+            the ACT format.
         profile1d (:obj:`np.ndarray`, optional): One dimensional beam profile, with index 0 at the centre.
         rDeg (:obj:`np.ndarray`, optional): Corresponding angular distance in degrees from the centre for
             the beam profile.
-        
+
     Attributes:
         profile1d (:obj:`np.ndarray`): One dimensional beam profile, with index 0 at the centre.
         rDeg (:obj:`np.ndarray`): Corresponding angular distance in degrees from the centre for the 
             beam profile.
         tck (:obj:`tuple`): Spline knots for interpolating the beam onto different angular binning 
             (in degrees), for use with :meth:`scipy.interpolate.splev`.
         FWHMArcmin (float): Estimate of the beam FWHM in arcmin.
 
     """
     
     def __init__(self, beamFileName = None, profile1d = None, rDeg = None):
         
         if beamFileName is not None:
             beamData=np.loadtxt(beamFileName).transpose()
-            self.profile1d=beamData[1]
-            self.rDeg=beamData[0]
+            # Identify if beam file is a profile or a transform
+            if beamData[0][1]-beamData[0][0] >= 1:
+                ell=beamData[0]
+                Bell=beamData[1]
+                if len(np.unique(np.diff(ell))) != 1:
+                    raise Exception("If using a beam transform file, need delta ell = 1 between all ell values.")
+                rDeg=np.linspace(0.0, 0.5, 1800) # This may need adjusting
+                prof=curvedsky.harm2profile(Bell, np.radians(rDeg))
+                prof=prof/prof[0]
+                self.profile1d=prof
+                self.rDeg=rDeg
+                self.Bell=Bell
+                self.ell=ell
+            else:
+                self.profile1d=beamData[1]
+                self.rDeg=beamData[0]
+                self.Bell=curvedsky.profile2harm(self.profile1d, np.radians(self.rDeg))
+                self.Bell=self.Bell/self.Bell[0]
+                self.ell=np.arange(len(self.Bell))
+                #prof=curvedsky.harm2profile(Bell, np.radians(self.rDeg))
         else:
             self.profile1d=profile1d
             self.rDeg=rDeg
-        
+
         if self.profile1d is not None and self.rDeg is not None:
             self.tck=interpolate.splrep(self.rDeg, self.profile1d)
         
         # This is really just for sorting a list of beams by resolution
         self.FWHMArcmin=self.rDeg[np.argmin(abs(self.profile1d-0.5))]*60*2
 
 #------------------------------------------------------------------------------------------------------------
 class QFit(object):
     """A class for managing the filter mismatch function, referred to as `Q` in the ACT papers from
     `Hasselfield et al. (2013) <http://adsabs.harvard.edu/abs/2013JCAP...07..008H>`_ onwards.
     
     Args:
-        QFitFileName (:obj:`str`): Path to a FITS-table format file as made by :meth:`fitQ`.
-        tileNames (:obj:`list`): If given, the Q-function will be defined only for these tiles (their names
-            must appear in the file specified by `QFitFileName`).
+        QSource (:obj:`str`, optional): The source to use for Q (the filter mismatch function) - either
+            'fit' (to use results from the original Q-fitting routine), 'injection' (to use Q derived
+            from source injection simulations), or 'hybrid' (to use 'fit' at scales less than the
+            reference filter scale, and 'injection' at scales greater than the reference filter scale).
+            For the 'injection' and 'hybrid' methods, `selFnDir` must be supplied.
+        selFnDir (:obj:`str`, optional): Path to a ``selFn/`` directory, as produced by the :ref:`nemoCommand`
+            command. This directory contains information such as the survey noise maps, area masks,
+            and information needed to construct the filter mismatch function, `Q`, used in mass
+            modeling.
+        QFitFileName (`str`, optional): Path to a FITStable containing Q fits for all tiles - this is
+            normally ``selFn/QFit.fits``). This is only used if QSource is set to ``fit``.
+        tileNames (:obj:`list`): If given, the Q-function will be defined only for these tiles.
     
     Attributes:
         fitDict (:obj:`dict`): Dictionary of interpolation objects, indexed by `tileName`. You should not
             need to access this directly - use :meth:`getQ` instead.
     
     """
         
-    def __init__(self, QFitFileName = None, tileNames = None):
+    def __init__(self, QSource = 'fit', selFnDir = None, QFitFileName = None, tileNames = None):
         self._zGrid=np.array([0.05, 0.1, 0.2, 0.3, 0.4, 0.6, 0.8, 1.0, 1.2, 1.6, 2.0])
         self._theta500ArcminGrid=np.logspace(np.log10(0.1), np.log10(55), 10)
         self.zMin=(self._zGrid).min()
         self.zMax=(self._zGrid).max()
         self.zDependent=None
         self.zDepThetaMax=None
+        self.selFnDir=selFnDir
+
+        self.fitDict={}
+
+        self.QSource=QSource
+        if self.QSource not in ['fit', 'injection', 'hybrid']:
+            raise Exception("QSource must be either 'fit', 'injection', or 'hybrid'")
+
+        if self.QSource == 'fit' or self.QSource == 'hybrid':
+            if self.selFnDir is not None and QFitFileName is None:
+                self.loadQ(self.selFnDir+os.path.sep+"QFit.fits", tileNames = tileNames)
+            if QFitFileName is not None:
+                self.loadQ(QFitFileName, tileNames = tileNames)
+
+        elif self.QSource == 'injection':
+            theta500s, thetaQ=self._loadInjectionData()
+            self.fitDict[None]=interpolate.InterpolatedUnivariateSpline(theta500s, thetaQ, ext = 1)
+
+
+    def _loadInjectionData(self):
+        # Stuff from the source injection sims (now required for completeness calculation)
+        if self.selFnDir is None:
+            raise Exception("selFnDir must be supplied when using 'injection' or 'hybrid' QSource")
+        injDataPath=self.selFnDir+os.path.sep+"sourceInjectionData.fits"
+        inputDataPath=self.selFnDir+os.path.sep+"sourceInjectionInputCatalog.fits"
+        injTab=atpy.Table().read(injDataPath)
+        inputTab=atpy.Table().read(inputDataPath)
+        SNRCut=5.0
+        theta500s, binCentres, compThetaGrid, thetaQ=completeness._parseSourceInjectionData(injTab, inputTab, SNRCut)
+
+        return theta500s, thetaQ
 
-        self.fitDict={}                
-        if QFitFileName is not None:
-            self.loadQ(QFitFileName, tileNames = tileNames)
-        
         
-    def loadQ(self, source, tileNames = None):
+    def loadQ(self, QFitFileName, tileNames = None):
         """Load the filter mismatch function Q (see `Hasselfield et al. 2013 
         <https://ui.adsabs.harvard.edu/abs/2013JCAP...07..008H/abstract>`_) as a dictionary of spline fits.
         
         Args:
-            source (:obj:`nemo.startUp.NemoConfig` or str): Either the path to a .fits table (containing Q fits
-                for all tiles - this is normally ``selFn/QFit.fits``), or a :obj:`nemo.startUp.NemoConfig` object 
-                (from which the path and tiles to use will be inferred).
+            QFitFileName(:obj:`str`): The path to a .fits table (containing Q fits for all tiles - this is
+                normally ``selFn/QFit.fits``).
             tileNames (optional, list): A list of tiles for which the Q function spline fit coefficients 
                 will be extracted. If source is a :obj:`nemo.startUp.NemoConfig` object, this should be set to 
                 ``None``.
-        
+
         Returns:
-            A dictionary (with tilNames as keys), containing spline knots for the Q function for each tile.
-            Q values can then be obtained by using these with :func:`scipy.interpolate.splev`.
-            
+            None
+
         """
 
-        # Bit messy, but two modes here: 
-        # - combined Q fit file for all tiles
-        # - single Q fit for a single tile (interim stage, when under nemo MPI run)
-        if type(source) == nemo.startUp.NemoConfig:
-            tileNames=source.tileNames
-            combinedQTabFileName=source.selFnDir+os.path.sep+"QFit.fits"
-            loadMode=None
-            if os.path.exists(combinedQTabFileName) == True:
-                tileNamesInFile=[]
-                with pyfits.open(combinedQTabFileName) as QTabFile:
-                    for ext in QTabFile:
-                        if type(ext) == astropy.io.fits.hdu.table.BinTableHDU:
-                            tileNamesInFile.append(ext.name)
-                tileNamesInFile.sort()
-                if tileNames is None:
-                    tileNames=tileNamesInFile
-                loadMode="combined"
-            else:
-                globStr=source.selFnDir+os.path.sep+"QFit#*.fits"
-                QTabFileNames=glob.glob(globStr)
-                loadMode="single"
-                if len(QTabFileNames) == 0:
-                    raise Exception("could not find either '%s' or '%s' - needed to make QFit object" % (combinedQTabFileName, globStr))
-            zMin=self._zGrid.max()
-            zMax=self._zGrid.min()
-            for tileName in tileNames:
-                if loadMode == "combined":
-                    QTab=atpy.Table().read(combinedQTabFileName, hdu = tileName)
-                elif loadMode == "single":
-                    QTab=atpy.Table().read(source.selFnDir+os.path.sep+"QFit#%s.fits" % (tileName))
-                else:
-                    raise Exception("loadMode is not defined")
-                if QTab['z'].min() < zMin:
-                    self.zMin=QTab['z'].min()
-                if QTab['z'].max() > zMax:
-                    self.zMax=QTab['z'].max()
-                self.fitDict[tileName]=self._makeInterpolator(QTab)
-
-        elif os.path.exists(source) == True:
-            # Inspect file and get tile names if MEF
-            if tileNames is None:
-                tileNames=[]
-                with pyfits.open(source) as QTab:
-                    for ext in QTab:
-                        if type(ext) == astropy.io.fits.hdu.table.BinTableHDU:
-                            tileNames.append(ext.name)
-            zMin=self._zGrid.max()
-            zMax=self._zGrid.min()
-            for tileName in tileNames:
-                if tileName == '': # Individual, interim file name
-                    assert(source.find("QFit#") > 0)
-                    tileName=os.path.split(source)[-1].split("QFit#")[-1].split(".fits")[0]
-                    QTab=atpy.Table().read(source)
-                else:
-                    QTab=atpy.Table().read(source, hdu = tileName)
-                if QTab['z'].min() < zMin:
-                    self.zMin=QTab['z'].min()
-                if QTab['z'].max() > zMax:
-                    self.zMax=QTab['z'].max()
-                self.fitDict[tileName]=self._makeInterpolator(QTab)
-    
+        if self.QSource == 'hybrid':
+            injThetas, injQs=self._loadInjectionData()
+            refTheta=None
+
+        # Inspect file and get tile names if MEF
+        if tileNames is None:
+            tileNames=[]
+            with pyfits.open(QFitFileName) as QTab:
+                for ext in QTab:
+                    if type(ext) == astropy.io.fits.hdu.table.BinTableHDU:
+                        tileNames.append(ext.name)
+        zMin=self._zGrid.max()
+        zMax=self._zGrid.min()
+        QStack=[]
+        thetaStack=[]
+        for tileName in tileNames:
+            QTab=atpy.Table().read(QFitFileName, hdu = tileName)
+            if QTab['z'].min() < zMin:
+                self.zMin=QTab['z'].min()
+            if QTab['z'].max() > zMax:
+                self.zMax=QTab['z'].max()
+            if self.QSource == 'hybrid':
+                # Splice on the injection Q estimate at scales larger than reference scale
+                # NOTE: Doing things this way to ensure using same thetas across all tiles
+                # (so we can average easily below)
+                if refTheta is None:
+                    refTheta=QTab['theta500Arcmin'][QTab['Q'] > 1].min()
+                fitQs=QTab['Q'][QTab['theta500Arcmin'] <= refTheta]
+                fitThetas=QTab['theta500Arcmin'][QTab['theta500Arcmin'] <= refTheta]
+                hybQTab=atpy.Table()
+                hybQTab['theta500Arcmin']=list(fitThetas)+list(injThetas[injThetas > refTheta])
+                hybQTab['Q']=list(fitQs)+list(injQs[injThetas > refTheta])
+                hybQTab.meta=QTab.meta
+                QTab=hybQTab
+            QStack.append(QTab['Q'].data)
+            thetaStack.append(QTab['theta500Arcmin'].data)
+            self.fitDict[tileName]=self._makeInterpolatorFromQTab(QTab)
+
+        # Average Q across all tiles
+        medQ=np.median(np.array(QStack), axis = 0)
+        medTheta=np.median(np.array(thetaStack), axis = 0)
+        medQTab=atpy.Table()
+        medQTab['Q']=medQ
+        medQTab['theta500Arcmin']=QTab['theta500Arcmin']
+        if 'z' in QTab.keys():
+            medQTab['z']=QTab['z']
+        medQTab.meta=QTab.meta
+        self.fitDict[None]=self._makeInterpolatorFromQTab(medQTab)
+
 
-    def _makeInterpolator(self, QTab):
+    def _makeInterpolatorFromQTab(self, QTab):
         """Inspects QTab, and makes an interpolator object - 2d if there is z-dependence, 1d if not.
         
         """
         
         if QTab.meta['ZDEPQ'] == 0:
             QTab.sort('theta500Arcmin')
             spline=interpolate.InterpolatedUnivariateSpline(QTab['theta500Arcmin'], QTab['Q'], ext = 1)
@@ -257,24 +298,29 @@
         Args:
             theta500Arcmin (:obj:`float` or :obj:`np.ndarray`): The angular scale at which *Q* will
                 be calculated. This can be an array or a single value.
             z (:obj:`float`, optional): Redshift, only used if *Q* is a function of
                 redshift, otherwise it is ignored. This must be a single value only, 
                 i.e., not an array.
             tileName (:obj:`str`, optional): The name of the tile to use for the *Q* function.
+                If None, or if the given tileName is not found, then an average over all tiles
+                is used.
             
         Returns:
             The value of *Q* (an array or a single float, depending on the input).
             
         Note:
             In the case where *Q* is a function of redshift, values outside of the range for which
             *Q* has been calculated will be filled with zeros (i.e., there is no extrapolation in
             redshift).
                     
         """
+
+        if tileName not in self.fitDict.keys():
+            tileName=None
         
         if z is not None:
             if type(z) == np.ndarray and z.shape == (1,):
                 z=float(z)
             if type(z) is not float and type(z) is not np.float64:
                 raise Exception("z must be a float, and not, e.g., an array")
         
@@ -283,14 +329,18 @@
             thetaMask=theta500Arcmin > self.zDepThetaMax(z)
             Qs[thetaMask]=0.0
             if z < self.zMin or z > self.zMax:
                 Qs=0
         else:
             # Univariate case handles own valid bounds checking
             Qs=self.fitDict[tileName](theta500Arcmin)
+
+        if (Qs < 0).sum() > 0:
+            #print("WARNING: negative Q value in tileName = %s" % (tileName))
+            Qs[Qs < 0]=0
         
         return Qs
 
 #------------------------------------------------------------------------------------------------------------
 def fSZ(obsFrequencyGHz, TCMBAlpha = 0.0, z = None):
     """Returns the frequency dependence of the (non-relativistic) Sunyaev-Zel'dovich effect.
     
@@ -338,19 +388,17 @@
     if type(MDelta) == str:
         raise Exception("MDelta is a string - use, e.g., 1.0e+14 (not 1e14 or 1e+14)")
 
     Ez=ccl.h_over_h0(cosmoModel, 1/(1+z))
     if wrt == 'critical':
         wrtDensity=ccl.physical_constants.RHO_CRITICAL*(Ez*cosmoModel['h'])**2
     elif wrt == 'mean':
-        wrtDensity=ccl.omega_x(cosmoModel, 1/(1+z), 'matter')
-        #wrtDensity=cosmoModel.Om(z)*cosmoModel.critical_density(z).value
+        wrtDensity=ccl.omega_x(cosmoModel, 1/(1+z), 'matter')*ccl.physical_constants.RHO_CRITICAL*(Ez*cosmoModel['h'])**2
     else:
         raise Exception("wrt should be either 'critical' or 'mean'")
-    #wrtDensity=(wrtDensity*np.power(Mpc_in_cm, 3))/MSun_in_g # NOTE: not needed for CCL units (MSun, Mpc etc.)
     RDeltaMpc=np.power((3*MDelta)/(4*np.pi*delta*wrtDensity), 1.0/3.0)
         
     return RDeltaMpc
 
 #------------------------------------------------------------------------------------------------------------
 def calcR500Mpc(z, M500c, cosmoModel):
     """Calculate R500 (in Mpc), with respect to critical density.
@@ -387,15 +435,15 @@
     R500Mpc=calcR500Mpc(z, M500, cosmoModel)
     #theta500Arcmin=np.degrees(np.arctan(R500Mpc/cosmoModel.angular_diameter_distance(z).value))*60.0
     theta500Arcmin=np.degrees(np.arctan(R500Mpc/ccl.angular_diameter_distance(cosmoModel, 1/(1+z))))*60.0
     
     return theta500Arcmin
     
 #------------------------------------------------------------------------------------------------------------
-def makeArnaudModelProfile(z, M500, GNFWParams = 'default', cosmoModel = None):
+def makeArnaudModelProfile(z, M500, GNFWParams = 'default', cosmoModel = None, binning = 'log'):
     """Given z, M500 (in MSun), returns dictionary containing Arnaud model profile (well, knots from spline 
     fit, 'tckP' - assumes you want to interpolate onto an array with units of degrees) and parameters 
     (particularly 'y0', 'theta500Arcmin').
     
     Use GNFWParams to specify a different shape. If GNFWParams = 'default', then the default parameters as listed
     in gnfw.py are used, i.e., 
     
@@ -414,15 +462,20 @@
     if cosmoModel is None:
         cosmoModel=fiducialCosmoModel
 
     if GNFWParams == 'default':
         GNFWParams=gnfw._default_params
     
     # Adjust tol for speed vs. range of b covered
-    bRange=np.linspace(0, 30, 1000)
+    if binning == 'linear': # Old
+        bRange=np.linspace(0, 30, 1000)
+    elif binning == 'log':
+        bRange=np.logspace(np.log10(1e-6), np.log10(100), 300)
+    else:
+        raise Exception("'binning' must be 'linear' or 'log' (given '%s')." % (binning))
     cylPProfile=[]
     tol=1e-6
     for i in range(len(bRange)):
         b=bRange[i]
         cylPProfile.append(gnfw.integrated(b, params = GNFWParams))
         if i > 0 and abs(cylPProfile[i] - cylPProfile[i-1]) < tol:
             break
@@ -494,15 +547,16 @@
     GNFWParams['P0']=P0z
     GNFWParams['beta']=betaz+0.3
     GNFWParams['c500']=1/xcz
     GNFWParams['gamma']=0.3
     GNFWParams['alpha']=1.0    
     
     # Adjust tol for speed vs. range of b covered
-    bRange=np.linspace(0, 30, 1000)
+    # bRange=np.linspace(0, 30, 1000) # old
+    bRange=np.logspace(np.log10(1e-6), np.log10(100), 300)
     cylPProfile=[]
     tol=1e-6
     for i in range(len(bRange)):
         b=bRange[i]
         cylPProfile.append(gnfw.integrated(b, params = GNFWParams))
         if i > 0 and abs(cylPProfile[i] - cylPProfile[i-1]) < tol:
             break
@@ -547,127 +601,211 @@
     
     if amplitude is None:
         amplitude=1.0
     
     if type(beam) == str:
         beam=BeamProfile(beamFileName = beam)        
     profile1d=amplitude*beam.profile1d
-    
+
     # Turn 1d profile into 2d
     r2p=interpolate.interp1d(beam.rDeg, profile1d, bounds_error=False, fill_value=0.0)
     signalMap=r2p(degreesMap)
     
     return signalMap
-    
+
+#------------------------------------------------------------------------------------------------------------
+def _paintSignalMap(shape, wcs, tckP, beam = None, RADeg = None, decDeg = None, amplitude = None,
+                    maxSizeDeg = 10.0, convolveWithBeam = True, vmin = 1e-12):
+    """Use Sigurd's fast object painter to paint given signal into map.
+
+    Notes:
+        Setting vmin arbitrarily small seems the best way to avoid unwanted behavior (e.g., cutting off
+        clusters before they are painted in properly).
+
+    """
+
+    # Now allowing arrays of sky coords and amplitudes (but one profile shape)
+    if RADeg is None and decDeg is None:
+        RADeg, decDeg=wcs.getCentreWCSCoords()
+    dtype=np.float32 # only float32 supported by fast srcsim
+    amp=1.0
+    if convolveWithBeam == True:
+        if beam is None:
+            raise Exception("No beam supplied.")
+        if type(beam) == str:
+            beam=BeamProfile(beamFileName = beam)
+        rht=utils.RadialFourierTransform()
+        rprof=interpolate.splev(np.degrees(rht.r), tckP, ext = 1)
+        lbeam=np.interp(rht.l, beam.ell, beam.Bell)
+        lprof=rht.real2harm(rprof)
+        lprof*=lbeam
+        rprof=rht.harm2real(lprof)
+        r, rprof=rht.unpad(rht.r, rprof)
+    else:
+        rDeg=np.logspace(np.log10(1e-6), np.log10(maxSizeDeg), 5000)
+        rprof=interpolate.splev(rDeg, tckP, ext = 1)
+        r=np.radians(rDeg)
+    if amplitude is not None:
+        amp=rprof[0]*amplitude
+        rprof=rprof/rprof[0]
+
+    if type(RADeg) == np.ndarray and type(decDeg) == np.ndarray:
+        poss=np.array([np.radians(decDeg), np.radians(RADeg)]).astype(dtype)
+    else:
+        poss=np.array([[np.radians(decDeg)], [np.radians(RADeg)]]).astype(dtype)
+    if type(amp) == np.ndarray:
+        amps=np.array(amp, dtype = dtype)
+    else:
+        amps=np.array([amp], dtype = dtype)
+
+    signalMap=pointsrcs.sim_objects(shape, wcs.AWCS, poss, amps, (r, abs(rprof)), vmin = vmin,
+                                    rmax = np.radians(maxSizeDeg), prof_equi = False)
+
+    if rprof[0] < 0:
+        signalMap=signalMap*-1
+
+    return np.array(signalMap)
+
 #------------------------------------------------------------------------------------------------------------
-def makeArnaudModelSignalMap(z, M500, degreesMap, wcs, beam, GNFWParams = 'default', amplitude = None, 
-                             maxSizeDeg = 15.0, convolveWithBeam = True):
-    """Makes a 2d signal only map containing an Arnaud model cluster. 
+def makeArnaudModelSignalMap(z, M500, shape, wcs, beam = None, RADeg = None, decDeg = None,\
+                             GNFWParams = 'default', amplitude = None, maxSizeDeg = 15.0,\
+                             convolveWithBeam = True, cosmoModel = None, painter = 'pixell'):
+    """Makes a 2d signal only map containing an Arnaud model cluster.
     
     Args:
         z (float): Redshift; used for setting angular size.
         M500 (float): Mass within R500, defined with respect to critical density; units are solar masses.
-        degreesMap (:obj:`numpy.ndarray`): A 2d array containing radial distance measured in degrees from 
-            the centre of the model to be inserted. The output map will have the same dimensions and pixel
-            scale (see nemoCython.makeDegreesDistanceMap).
+        shape (:obj:`tuple`): A tuple describing the map (numpy array) shape in pixels (height, width).
+        wcs (:obj:`astWCS.WCS`): An astWCS object.
+        beam (:obj:`str` or :obj:`signals.BeamProfile`): Either the file name of the text file that describes
+            the beam with which the map will be convolved, or a :obj:`signals.BeamProfile` object. If None,
+            no beam convolution is applied.
+        RADeg (float, or array, optional): If None, the signal will be inserted at the center of the generated map.
+        decDeg (float, or array, optional): If None, the signal will be inserted at the center of the generated map.
         GNFWParams (dict, optional): Used to specify a different profile shape to the default (which follows 
             Arnaud et al. 2010). If GNFWParams = 'default', then the default parameters as listed in 
             gnfw.py are used, i.e., GNFWParams = {'gamma': 0.3081, 'alpha': 1.0510, 'beta': 5.4905, 
             'tol': 1e-7, 'npts': 100}. Otherwise, give a dictionary that specifies the wanted values. This 
             would usually be specified using the GNFWParams key in the .yml config used when running nemo
             (see the examples/ directory).
-        amplitude (float, optional): Amplitude of the cluster, i.e., the central decrement (in map units, 
+        amplitude (float, or array, optional): Amplitude of the cluster, i.e., the central decrement (in map units,
             e.g., uK), or the central Comptonization parameter (dimensionless), before beam convolution. 
             Not needed for generating filter kernels.
         maxSizeDeg (float, optional): Use to limit the region over which the beam convolution is done, 
             for optimization purposes.
-        convolveWithBeam (bool, optional): If False, no beam convolution is done (it can be quicker to apply
-            beam convolution over a whole source-injected map rather than per object).
+        convolveWithBeam (bool, optional): If False, no beam convolution is done.
     
     Returns:
         signalMap (:obj:`np.ndarray`).
 
     Note:
         The pixel window function is not applied here; use pixell.enmap.apply_window to do that (see 
         nemo.filters.filterMaps).    
+
+    Note:
+        If arrays of sky coordinates and amplitudes are given, multiple clusters (with the same profile) will
+        be painted in the map. This is useful for running cluster injection simulations for estimating
+        completeness, but only works with the 'pixell' object painter.
         
     """
 
+    if RADeg is None or decDeg is None:
+        RADeg, decDeg=wcs.getCentreWCSCoords()
+
     # Making the 1d profile itself is the slowest part (~1 sec)
-    signalDict=makeArnaudModelProfile(z, M500, GNFWParams = GNFWParams)
+    signalDict=makeArnaudModelProfile(z, M500, GNFWParams = GNFWParams, cosmoModel = cosmoModel)
     tckP=signalDict['tckP']
-    
-    # Make cluster map (unit-normalised profile)
-    rDeg=np.linspace(0.0, maxSizeDeg, 5000)
-    profile1d=interpolate.splev(rDeg, tckP, ext = 1)
-    if amplitude is not None:
-        profile1d=profile1d*amplitude
-    r2p=interpolate.interp1d(rDeg, profile1d, bounds_error=False, fill_value=0.0)
-    signalMap=r2p(degreesMap)
-    
-    if convolveWithBeam == True:        
-        signalMap=maps.convolveMapWithBeam(signalMap, wcs, beam, maxDistDegrees = maxSizeDeg)
-    
+
+    if painter == 'legacy': # Old method
+        degreesMap=np.ones(shape, dtype = np.float64)*1e6
+        degreesMap, xBounds, yBounds=maps.makeDegreesDistanceMap(degreesMap, wcs, RADeg, decDeg,
+                                                                 maxSizeDeg)
+        rDeg=np.linspace(0.0, maxSizeDeg, 5000)
+        profile1d=interpolate.splev(rDeg, tckP, ext = 1)
+        if amplitude is not None:
+            profile1d=profile1d*amplitude
+        r2p=interpolate.interp1d(rDeg, profile1d, bounds_error=False, fill_value=0.0)
+        signalMap=r2p(degreesMap)
+        if convolveWithBeam == True:
+            signalMap=maps.convolveMapWithBeam(signalMap, wcs, beam, maxDistDegrees = maxSizeDeg)
+    elif painter == 'pixell': # New method - using Sigurd's object painter
+        signalMap=_paintSignalMap(shape, wcs, tckP, beam = beam, RADeg = RADeg, decDeg = decDeg,
+                                  amplitude = amplitude, maxSizeDeg = maxSizeDeg,
+                                  convolveWithBeam = convolveWithBeam)
+    else:
+        raise Exception("'painter' must be 'legacy' or 'pixell' (given '%s')." % (painter))
+
     return signalMap
 
 #------------------------------------------------------------------------------------------------------------
-def makeBattagliaModelSignalMap(z, M500, degreesMap, wcs, beam, GNFWParams = 'default', amplitude = None, 
-                                 maxSizeDeg = 15.0, convolveWithBeam = True):
+def makeBattagliaModelSignalMap(z, M500, shape, wcs, beam = None, RADeg = None, decDeg = None,\
+                                GNFWParams = 'default', amplitude = None, maxSizeDeg = 15.0,\
+                                convolveWithBeam = True, cosmoModel = None):
     """Makes a 2d signal only map containing a Battaglia+2012 model cluster (taking into account the redshift
     evolution described in Table 1 and equation 11 there).
-    
+
     Args:
         z (float): Redshift; used for setting angular size.
         M500 (float): Mass within R500, defined with respect to critical density; units are solar masses.
-        degreesMap (:obj:`numpy.ndarray`): A 2d array containing radial distance measured in degrees from 
-            the centre of the model to be inserted. The output map will have the same dimensions and pixel
-            scale (see nemoCython.makeDegreesDistanceMap).
-        GNFWParams (dict, optional): Used to specify a different profile shape to the default (which follows 
-            Battaglia et al. 2012). If GNFWParams = 'default', then the default parameters as listed in 
-            Battaglia et al. 2012 are used, i.e., GNFWParams = {'gamma': 0.3, 'alpha': 1.0, 'beta': 4.49,
-            'c500': 1.408, 'tol': 1e-7, 'npts': 100}. Note that the definitions/sign convention is slightly
-            different in Battaglia+2012 compared to Arnaud+2010 (we follow the latter). 
-            Otherwise, give a dictionary that specifies the wanted values. This 
+        shape (:obj:`tuple`): A tuple describing the map (numpy array) shape in pixels (height, width).
+        wcs (:obj:`astWCS.WCS`): An astWCS object.
+        beam (:obj:`str` or :obj:`signals.BeamProfile`): Either the file name of the text file that describes
+            the beam with which the map will be convolved, or a :obj:`signals.BeamProfile` object. If None,
+            no beam convolution is applied.
+        RADeg: If None, the signal will be inserted at the center of the generated map.
+        decDeg: If None, the signal will be inserted at the center of the generated map.
+        GNFWParams (dict, optional): Used to specify a different profile shape to the default (which follows
+            Arnaud et al. 2010). If GNFWParams = 'default', then the default parameters as listed in
+            gnfw.py are used, i.e., GNFWParams = {'gamma': 0.3081, 'alpha': 1.0510, 'beta': 5.4905,
+            'tol': 1e-7, 'npts': 100}. Otherwise, give a dictionary that specifies the wanted values. This
             would usually be specified using the GNFWParams key in the .yml config used when running nemo
             (see the examples/ directory).
-        amplitude (float, optional): Amplitude of the cluster, i.e., the central decrement (in map units, 
-            e.g., uK), or the central Comptonization parameter (dimensionless), before beam convolution. 
+        amplitude (float, optional): Amplitude of the cluster, i.e., the central decrement (in map units,
+            e.g., uK), or the central Comptonization parameter (dimensionless), before beam convolution.
             Not needed for generating filter kernels.
-        maxSizeDeg (float, optional): Use to limit the region over which the beam convolution is done, 
+        maxSizeDeg (float, optional): Use to limit the region over which the beam convolution is done,
             for optimization purposes.
-        convolveWithBeam (bool, optional): If False, no beam convolution is done (it can be quicker to apply
-            beam convolution over a whole source-injected map rather than per object).
-    
+        convolveWithBeam (bool, optional): If False, no beam convolution is done.
+
     Returns:
         signalMap (:obj:`np.ndarray`).
 
     Note:
-        The pixel window function is not applied here; use pixell.enmap.apply_window to do that (see 
-        nemo.filters.filterMaps).    
-        
+        The pixel window function is not applied here; use pixell.enmap.apply_window to do that (see
+        nemo.filters.filterMaps).
+
     """
-    
+
     if GNFWParams == 'default':
         # NOTE: These are Table 1 values from Battaglia+2012 for M500c
         GNFWParams={'P0': 7.49, 'gamma': 0.3, 'alpha': 1.0, 'beta': 4.49, 'c500': 1.408, 'tol': 1e-7, 'npts': 100}
 
-    # Making the 1d profile itself is the slowest part (~1 sec)
-    signalDict=makeBattagliaModelProfile(z, M500, GNFWParams = GNFWParams)
-    tckP=signalDict['tckP']
-    
-    # Make cluster map (unit-normalised profile)
-    rDeg=np.linspace(0.0, maxSizeDeg, 5000)
-    profile1d=interpolate.splev(rDeg, tckP, ext = 1)
-    if amplitude is not None:
-        profile1d=profile1d*amplitude
-    r2p=interpolate.interp1d(rDeg, profile1d, bounds_error=False, fill_value=0.0)
-    signalMap=r2p(degreesMap)
+    #----
+    # Old
+    ## Making the 1d profile itself is the slowest part (~1 sec)
+    #signalDict=makeBattagliaModelProfile(z, M500, GNFWParams = GNFWParams)
+    #tckP=signalDict['tckP']
+    
+    ## Make cluster map (unit-normalised profile)
+    #rDeg=np.linspace(0.0, maxSizeDeg, 5000)
+    #profile1d=interpolate.splev(rDeg, tckP, ext = 1)
+    #if amplitude is not None:
+        #profile1d=profile1d*amplitude
+    #r2p=interpolate.interp1d(rDeg, profile1d, bounds_error=False, fill_value=0.0)
+    #signalMap=r2p(degreesMap)
     
-    if convolveWithBeam == True:        
-        signalMap=maps.convolveMapWithBeam(signalMap, wcs, beam, maxDistDegrees = maxSizeDeg)
+    #if convolveWithBeam == True:
+        #signalMap=maps.convolveMapWithBeam(signalMap, wcs, beam, maxDistDegrees = maxSizeDeg)
+
+    # New - using Sigurd object painter
+    signalDict=makeBattagliaModelProfile(z, M500, GNFWParams = GNFWParams, cosmoModel = cosmoModel)
+    tckP=signalDict['tckP']
+    return _paintSignalMap(shape, wcs, tckP, beam = beam, RADeg = RADeg, decDeg = decDeg,
+                           amplitude = amplitude, maxSizeDeg = maxSizeDeg,
+                           convolveWithBeam = convolveWithBeam)
     
     return signalMap
 
 #------------------------------------------------------------------------------------------------------------
 def getFRelWeights(config):
     """Returns a dictionary of frequency weights used in relativistic corrections for each tile. This is 
     cached in the selFn/ dir after the first time this routine is called.
@@ -715,28 +853,26 @@
                 fRelWeightsDict[row['tileName']][float(key)]=row[key]
     
     return fRelWeightsDict
 
 #------------------------------------------------------------------------------------------------------------
 def fitQ(config):
     """Calculates the filter mismatch function *Q* on a grid of scale sizes for each tile in the map. The
-    results are initially cached (with a separate .fits table for each tile) under the `selFn` directory,
-    before being combined into a single file at the end of a :ref:`nemoCommand` run. 
+    results are combined into a single file written under the `selFn` directory.
     
     The `GNFWParams` key in the `config` dictionary can be used to specify a different cluster profile shape.
     
     Args:
         config (:obj:`startUp.NemoConfig`): A NemoConfig object.
     
     Note:
-        See :class:`QFit` for how to read in and use the output of this function.
+        See :class:`QFit` for how to read in and use the file produced by this function.
         
     """
     
-    t0=time.time()
     cosmoModel=fiducialCosmoModel
         
     # Spin through the filter kernels
     photFilterLabel=config.parDict['photFilter']
     filterList=config.parDict['mapFilters']
     for f in filterList:
         if f['label'] == photFilterLabel:
@@ -757,35 +893,52 @@
     
     # M, z -> theta ranges for Q calc - what's most efficient depends on whether there is z-dependence, or not
     # NOTE: ref filter that sets scale we compare to must ALWAYS come first
     if zDepQ == 0:
         # To safely (numerically, at least) apply Q at z ~ 0.01, we need to go to theta500 ~ 500 arcmin (< 10 deg)
         MRange=[ref['params']['M500MSun']]
         zRange=[ref['params']['z']]
-        minTheta500Arcmin=0.1
-        maxTheta500Arcmin=500.0
-        numPoints=50
-        theta500Arcmin_wanted=np.logspace(np.log10(minTheta500Arcmin), np.log10(maxTheta500Arcmin), numPoints)
-        zRange_wanted=np.zeros(numPoints)
-        zRange_wanted[np.less(theta500Arcmin_wanted, 3.0)]=2.0
-        zRange_wanted[np.logical_and(np.greater(theta500Arcmin_wanted, 3.0), np.less(theta500Arcmin_wanted, 6.0))]=1.0
-        zRange_wanted[np.logical_and(np.greater(theta500Arcmin_wanted, 6.0), np.less(theta500Arcmin_wanted, 10.0))]=0.5
-        zRange_wanted[np.logical_and(np.greater(theta500Arcmin_wanted, 10.0), np.less(theta500Arcmin_wanted, 20.0))]=0.1
-        zRange_wanted[np.logical_and(np.greater(theta500Arcmin_wanted, 20.0), np.less(theta500Arcmin_wanted, 30.0))]=0.05
-        zRange_wanted[np.greater(theta500Arcmin_wanted, 30.0)]=0.01
+        # Old - to 30 arcmin
+        # theta500Arcmin_wanted=np.logspace(np.log10(0.1), np.log10(30), 50)
+        # zRange_wanted=[2.0]*10 + [1.0]*10 + [0.6]*10 + [0.3]*10 + [0.1]*10
+        # New - same spacing over same range, with some extra scales
+        theta500Arcmin_wanted=np.power(10, np.arange(np.log10(0.1), np.log10(50), 0.05055349))
+        zRange_wanted=[2.0]*10 + [1.0]*10 + [0.6]*10 + [0.3]*10 + [0.1]*10 + [0.07]*4
         MRange_wanted=[]
         for theta500Arcmin, z in zip(theta500Arcmin_wanted, zRange_wanted):
             Ez=ccl.h_over_h0(cosmoModel, 1/(1+z))
             criticalDensity=ccl.physical_constants.RHO_CRITICAL*(Ez*cosmoModel['h'])**2
             R500Mpc=np.tan(np.radians(theta500Arcmin/60.0))*ccl.angular_diameter_distance(cosmoModel, 1/(1+z))
             M500=(4/3.0)*np.pi*np.power(R500Mpc, 3)*500*criticalDensity
-            MRange_wanted.append(M500)         
+            MRange_wanted.append(M500)
         MRange=MRange+MRange_wanted
-        zRange=zRange+zRange_wanted.tolist()
-        signalMapSizeDeg=10.0
+        zRange=zRange+zRange_wanted
+        signalMapSizeDeg=15.0
+        # Old
+        # minTheta500Arcmin=0.1
+        # maxTheta500Arcmin=500
+        # numPoints=50
+        # theta500Arcmin_wanted=np.logspace(np.log10(minTheta500Arcmin), np.log10(maxTheta500Arcmin), numPoints)
+        # zRange_wanted=np.zeros(numPoints)
+        # zRange_wanted[np.less(theta500Arcmin_wanted, 3.0)]=2.0
+        # zRange_wanted[np.logical_and(np.greater(theta500Arcmin_wanted, 3.0), np.less(theta500Arcmin_wanted, 6.0))]=1.0
+        # zRange_wanted[np.logical_and(np.greater(theta500Arcmin_wanted, 6.0), np.less(theta500Arcmin_wanted, 10.0))]=0.5
+        # zRange_wanted[np.logical_and(np.greater(theta500Arcmin_wanted, 10.0), np.less(theta500Arcmin_wanted, 20.0))]=0.1
+        # zRange_wanted[np.logical_and(np.greater(theta500Arcmin_wanted, 20.0), np.less(theta500Arcmin_wanted, 30.0))]=0.05
+        # zRange_wanted[np.greater(theta500Arcmin_wanted, 30.0)]=0.01
+        # MRange_wanted=[]
+        # for theta500Arcmin, z in zip(theta500Arcmin_wanted, zRange_wanted):
+        #     Ez=ccl.h_over_h0(cosmoModel, 1/(1+z))
+        #     criticalDensity=ccl.physical_constants.RHO_CRITICAL*(Ez*cosmoModel['h'])**2
+        #     R500Mpc=np.tan(np.radians(theta500Arcmin/60.0))*ccl.angular_diameter_distance(cosmoModel, 1/(1+z))
+        #     M500=(4/3.0)*np.pi*np.power(R500Mpc, 3)*500*criticalDensity
+        #     MRange_wanted.append(M500)
+        # MRange=MRange+MRange_wanted
+        # zRange=zRange+zRange_wanted.tolist()
+        # signalMapSizeDeg=15.0
     elif zDepQ == 1:
         # On a z grid for evolving profile models (e.g., Battaglia et al. 2012)
         MRange=[ref['params']['M500MSun']]
         zRange=[ref['params']['z']]
         zGrid=[0.05, 0.1, 0.2, 0.3, 0.4, 0.6, 0.8, 1.0, 1.2, 1.6, 2.0]
         minTheta500Arcmin=0.1
         maxTheta500Arcmin=100.0  # 55' corresponds to M500c = 1e16 MSun at z = 0.05
@@ -797,191 +950,181 @@
                 Ez=ccl.h_over_h0(cosmoModel, 1/(1+z))
                 criticalDensity=ccl.physical_constants.RHO_CRITICAL*(Ez*cosmoModel['h'])**2
                 R500Mpc=np.tan(np.radians(theta500Arcmin/60.0))*ccl.angular_diameter_distance(cosmoModel, 1/(1+z))
                 M500=(4/3.0)*np.pi*np.power(R500Mpc, 3)*500*criticalDensity
                 MRange_wanted.append(M500)
             MRange=MRange+MRange_wanted
             zRange=zRange+([z]*len(MRange_wanted))
-        signalMapSizeDeg=5.0
+        signalMapSizeDeg=15.0
     else:
         raise Exception("valid values for zDepQ are 0 or 1")
             
     # Here we save the fit for each tile separately... 
-    # completeness.tidyUp will put them into one file at the end of a nemo run
+    QTabDict={}
     for tileName in config.tileNames:
-        tileQTabFileName=config.selFnDir+os.path.sep+"QFit#%s.fits" % (tileName)
-        if os.path.exists(tileQTabFileName) == True:
-            print("... already done Q fit for tile %s ..." % (tileName))
-            continue
-        print("... fitting Q in tile %s ..." % (tileName))
+        t0=time.time()
+        print("... fitting Q in tile %s" % (tileName))
 
         # Load reference scale filter
         foundFilt=False
         for filt in config.parDict['mapFilters']:
             if filt['label'] == config.parDict['photFilter']:
                 foundFilt=True
                 break
         if foundFilt == False:
             raise Exception("couldn't find filter that matches photFilter")
         filterClass=eval('filters.%s' % (filt['class']))
         filterObj=filterClass(filt['label'], config.unfilteredMapsDictList, filt['params'], \
                               tileName = tileName, 
-                              diagnosticsDir = config.diagnosticsDir+os.path.sep+tileName)
+                              diagnosticsDir = config.diagnosticsDir)
         filterObj.loadFilter()
         
         # Real space kernel or Fourier space filter?
         if issubclass(filterObj.__class__, filters.RealSpaceMatchedFilter) == True:
             realSpace=True
         else:
             realSpace=False
         
         # Set-up the beams
         beamsDict={}
         for mapDict in config.parDict['unfilteredMaps']:
             obsFreqGHz=mapDict['obsFreqGHz']
             beamsDict[obsFreqGHz]=mapDict['beamFileName']
-        
-        # A bit clunky but gets map pixel scale and shrinks map size we'll use for inserting signals
-        # signalMapSizeDeg set according to lowest z model (see above), using smaller for z dependent to save RAM
-        # (but then have a higher low-z cut where Q will be valid)
+
+        # Uncomment if debugging large scale Q business
+        #MRange=[MRange[-3]]
+        #zRange=[zRange[-3]]
+
+        # Actually measuring Q...
         extMap=np.zeros(filterObj.shape)
         wcs=filterObj.wcs
-        RADeg, decDeg=wcs.getCentreWCSCoords()                
-        clipDict=astImages.clipImageSectionWCS(extMap, wcs, RADeg, decDeg, signalMapSizeDeg)
-        wcs=clipDict['wcs']
-        extMap=clipDict['data']
-        
+        nativeNPix=extMap.shape[0]*extMap.shape[1]
+        # Uncomment to pad signal maps [but then need to adjust normalization]
+        #extMap=enmap.enmap(extMap, wcs = wcs.AWCS)
+        #yZoom=signalMapSizeDeg/wcs.getFullSizeSkyDeg()[1]
+        #xZoom=signalMapSizeDeg/wcs.getFullSizeSkyDeg()[0]
+        #yPad=int(extMap.shape[0]*yZoom-extMap.shape[0])
+        #xPad=int(extMap.shape[1]*xZoom-extMap.shape[1])
+        #extMap=enmap.pad(extMap, (yPad, xPad))
+        #h=extMap.wcs.to_header()
+        #h.insert(0, ('NAXIS2', extMap.shape[0]))
+        #h.insert('NAXIS2', ('NAXIS1', extMap.shape[1]))
+        #wcs=astWCS.WCS(h, mode = 'pyfits')
+        #paddedNPix=extMap.shape[0]*extMap.shape[1]
+        # Set centre coords
+        shape=extMap.shape
+        RADeg, decDeg=wcs.getCentreWCSCoords()
+        x, y=wcs.wcs2pix(RADeg, decDeg)
+
+        # For testing effects of adding CMB + noise
+        #simCMBDict={}
+        #seed=1234
+        #noiseLevel=120.0
+        #for obsFreqGHz in list(beamsDict.keys()):
+            #simCMBDict[obsFreqGHz]=maps.simCMBMap(shape, wcs, noiseLevel = noiseLevel, beam = beamsDict[obsFreqGHz], seed = seed)
+        #print("... adding CMB and noise = %.3f in Q models" % (noiseLevel))
+
         # Input signal maps to which we will apply filter(s)
         # We do this once and store in a dictionary for speed
         theta500ArcminDict={}
-        signalMapDict={}
-        signalMap=np.zeros(extMap.shape)
-        degreesMap=np.ones(signalMap.shape, dtype = float)*1e6
-        degreesMap, xBounds, yBounds=nemoCython.makeDegreesDistanceMap(degreesMap, wcs, RADeg, decDeg, signalMapSizeDeg)
+        signalMap=np.zeros(shape)
+        Q=[]
+        QTheta500Arcmin=[]
+        Qz=[]
+        cubeStore={} # For debugging object painting
+        for obsFreqGHz in list(beamsDict.keys()):
+            cubeStore[obsFreqGHz]=[]
         for z, M500MSun in zip(zRange, MRange):
             key='%.2f_%.2f' % (z, np.log10(M500MSun))
             signalMaps=[]
             fSignalMaps=[]
-            y0=2e-4
+            y0=2e-04
             for obsFreqGHz in list(beamsDict.keys()):
                 if mapDict['obsFreqGHz'] is not None:   # Normal case
                     amplitude=maps.convertToDeltaT(y0, obsFreqGHz)
                 else:                                   # TILe-C case
                     amplitude=y0
                 # NOTE: Q is to adjust for mismatched filter shape
                 # Yes, this should have the beam in it (certainly for TILe-C)
                 # NOTE: CCL can blow up for some of the extreme masses we try to feed in here
                 # (so we just skip those if it happens)
-                try:
-                    signalMap=makeSignalModelMap(z, M500MSun, degreesMap, wcs, beamsDict[obsFreqGHz], 
-                                                 amplitude = amplitude, convolveWithBeam = True, 
-                                                 GNFWParams = config.parDict['GNFWParams'])
-                except:
-                    continue
+                # try:
+                signalMap=makeSignalModelMap(z, M500MSun, shape, wcs, beam = beamsDict[obsFreqGHz],
+                                             amplitude = amplitude, convolveWithBeam = True,
+                                             GNFWParams = config.parDict['GNFWParams'])
+                signalMap=enmap.apply_window(signalMap, pow = 1.0)
+                # except:
+                #     continue
+                #signalMap=signalMap+simCMBDict[obsFreqGHz]
+                #signalMap=signalMap+np.random.normal(0, noiseLevel, signalMap.shape)
+                #cubeStore[obsFreqGHz].append(signalMap)
                 if realSpace == True:
                     signalMaps.append(signalMap)
                 else:
                     signalMaps.append(enmap.fft(signalMap))
             signalMaps=np.array(signalMaps)
-            # Skip any failed ones (see above - CCL blowing up for extreme masses)
+            # Filter maps with ref kernel
             if len(signalMaps) == len(list(beamsDict.keys())):
-                signalMapDict[key]=signalMaps
-                theta500ArcminDict[key]=calcTheta500Arcmin(z, M500MSun, fiducialCosmoModel)
-        
-        # Filter maps with the ref kernel
-        # NOTE: keep only unique values of Q, theta500Arcmin (or interpolation routines will fail)
-        Q=[]
-        QTheta500Arcmin=[]
-        Qz=[]
-        for z, M500MSun in zip(zRange, MRange):
-            key='%.2f_%.2f' % (z, np.log10(M500MSun))
-            if key in signalMapDict.keys():
-                filteredSignal=filterObj.applyFilter(signalMapDict[key]) 
-                peakFilteredSignal=filteredSignal.max()
+                filteredSignal=filterObj.applyFilter(signalMaps)
+                mapInterpolator=interpolate.RectBivariateSpline(np.arange(filteredSignal.shape[0]),
+                                                                np.arange(filteredSignal.shape[1]),
+                                                                filteredSignal, kx = 3, ky = 3)
+                peakFilteredSignal=mapInterpolator(y, x)[0][0]
+                # Below is if we wanted to simulate object-finding here
+                #peakFilteredSignal=filteredSignal[int(y)-10:int(y)+10, int(x)-10:int(x)+10].max() # Avoids mess at edges
                 if peakFilteredSignal not in Q:
-                    Q.append(peakFilteredSignal)      
-                    QTheta500Arcmin.append(theta500ArcminDict[key])
+                    Q.append(peakFilteredSignal)
+                    QTheta500Arcmin.append(calcTheta500Arcmin(z, M500MSun, fiducialCosmoModel))
                     Qz.append(z)
         Q=np.array(Q)
-        Q=Q/Q[0]
-            
-        # Sort and save as FITS table (interim - all tile files gets combined at end of nemo run)
+        if abs(1-Q[0]/y0) > 1e-6:
+            raise Exception("Q[0]/y0 outside tolerance")
+        Q=Q/y0
+
+        # Sort and make FITS table
         QTab=atpy.Table()
         QTab.add_column(atpy.Column(Q, 'Q'))
         QTab.add_column(atpy.Column(QTheta500Arcmin, 'theta500Arcmin'))
         QTab.add_column(atpy.Column(Qz, 'z'))
         QTab.sort('theta500Arcmin')
         QTab.meta['NEMOVER']=nemo.__version__
         QTab.meta['ZDEPQ']=zDepQ
-        QTab.write(tileQTabFileName, overwrite = True)
-        
-        # Test plot
-        Q=QFit(tileQTabFileName)
-        plotSettings.update_rcParams()
-        plt.figure(figsize=(9,6.5))
-        ax=plt.axes([0.12, 0.11, 0.86, 0.88])
-        for z in [0.05, 0.1, 0.4, 1.0, 2.0]:
-            mask=(QTab['z'] == z)
-            if mask.sum() > 0:
-                plt.plot(QTab['theta500Arcmin'][mask], QTab['Q'][mask], '.', label = "z = %.2f" % (z))
-                thetaArr=np.logspace(np.log10(QTab['theta500Arcmin'][mask].min()), 
-                                 np.log10(QTab['theta500Arcmin'][mask].max()), numPoints)
-                plt.plot(thetaArr, Q.getQ(thetaArr, z, tileName = tileName), 'k-')
-        plt.legend()
-        plt.semilogx()
-        plt.xlabel("$\\theta_{\\rm 500c}$ (arcmin)")
-        plt.ylabel("$Q$ ($\\theta_{\\rm 500c}$, $z$)")
-        plt.savefig(config.diagnosticsDir+os.path.sep+tileName+os.path.sep+"QFit_%s.pdf" % (tileName))
-        plt.savefig(config.diagnosticsDir+os.path.sep+tileName+os.path.sep+"QFit_%s.png" % (tileName))
-        plt.close()
-        
-        t1=time.time()
-        print("... Q fit finished [tileName = %s, rank = %d, time taken = %.3f] ..." % (tileName, config.rank, t1-t0))
-        
-
-#------------------------------------------------------------------------------------------------------------
-def makeCombinedQTable(config):
-    """Writes dictionary of tables (containing individual tile Q fits) as a single .fits table.
-    
-    Returns combined Q astropy table object
-    
-    """
-
-    outFileName=config.selFnDir+os.path.sep+"QFit.fits"    
-    if os.path.exists(outFileName) == True:
-        return atpy.Table().read(outFileName)
-        
-    QTabDict={}
-    for tileName in config.allTileNames:
-        QTabDict[tileName]=atpy.Table().read(config.selFnDir+os.path.sep+"QFit#%s.fits" % (tileName))
-    
-    #----
-    # New - MEF
-    QTabMEF=pyfits.HDUList()
-    for tileName in config.allTileNames:
-        with pyfits.open(config.selFnDir+os.path.sep+"QFit#%s.fits" % (tileName)) as QTab:
-            QTab[1].name=tileName
-            QTabMEF.append(QTab[1].copy())
-    QTabMEF.writeto(outFileName, overwrite = True)
-    combinedQTab=QTabMEF
-    
-    #----
-    # Old
-    #combinedQTab=atpy.Table()
-    #for tabKey in list(QTabDict.keys()):
-        #for colKey in QTabDict[tabKey].keys():
-            #if colKey == 'theta500Arcmin':
-                #if colKey not in combinedQTab.keys():
-                    #combinedQTab.add_column(QTabDict[tabKey]['theta500Arcmin'], index = 0)
-            #else:
-                #combinedQTab.add_column(atpy.Column(QTabDict[tabKey][colKey].data, tabKey))
-    #combinedQTab.meta['NEMOVER']=nemo.__version__
-    #combinedQTab.write(outFileName, overwrite = True)
-    
-    return combinedQTab
+        QTab.meta['TILENAME']=tileName
+        QTabDict[tileName]=QTab
+        del Q, filterObj #, clipDict
+
+    if config.MPIEnabled == True:
+        #config.comm.barrier()
+        QTabDictList=config.comm.gather(QTabDict, root = 0)
+        if config.rank == 0:
+            print("... gathered Q fits")
+            combQTabDict={}
+            for QTabDict in QTabDictList:
+                for key in QTabDict:
+                    if key not in combQTabDict:
+                        combQTabDict[key]=QTabDict[key]
+            QTabDict=combQTabDict
+
+    # Write output as MEF
+    if config.rank == 0:
+        outFileName=config.selFnDir+os.path.sep+"QFit.fits"
+        QTabMEF=pyfits.HDUList()
+        for tileName in config.allTileNames:
+            if tileName in QTabDict.keys():
+                QTabHDU=pyfits.table_to_hdu(QTabDict[tileName])
+                QTabHDU.name=tileName
+                QTabMEF.append(QTabHDU)
+        QTabMEF.writeto(outFileName, overwrite = True)
+
+    if config.rank == 0:
+        print("... after Q fits completed: time since start = %.3f sec" % (time.time()-config._timeStarted))
+
+    ## Make sure we all leave here together
+    #if config.MPIEnabled == True:
+        #config.comm.barrier()
 
 #------------------------------------------------------------------------------------------------------------
 def calcWeightedFRel(z, M500, Ez, fRelWeightsDict):
     """Return fRel for the given (z, M500), weighted by frequency according to fRelWeightsDict
     
     """
     
@@ -1169,31 +1312,32 @@
     """
     
     if y0 < 0:
         raise Exception('y0 cannot be negative')
     if y0 > 1e-2:
         raise Exception('y0 is suspiciously large - probably you need to multiply by 1e-4')
             
-    P=calcPMass(y0, y0Err, z, zErr, QFit, mockSurvey, tenToA0 = tenToA0, B0 = B0, Mpivot = Mpivot, 
-                sigma_int = sigma_int, Ez_gamma = Ez_gamma, onePlusRedshift_power = onePlusRedshift_power, 
-                applyMFDebiasCorrection = applyMFDebiasCorrection,
-                applyRelativisticCorrection = applyRelativisticCorrection, fRelWeightsDict = fRelWeightsDict,
-                tileName = tileName)
+    P, bestQ=calcPMass(y0, y0Err, z, zErr, QFit, mockSurvey, tenToA0 = tenToA0, B0 = B0, Mpivot = Mpivot,
+                       sigma_int = sigma_int, Ez_gamma = Ez_gamma, onePlusRedshift_power = onePlusRedshift_power,
+                       applyMFDebiasCorrection = applyMFDebiasCorrection,
+                       applyRelativisticCorrection = applyRelativisticCorrection, fRelWeightsDict = fRelWeightsDict,
+                       tileName = tileName, returnQ = True)
     
     M500, errM500Minus, errM500Plus=getM500FromP(P, mockSurvey.log10M, calcErrors = calcErrors)
     
     label=mockSurvey.mdefLabel
     
-    return {'%s' % (label): M500, '%s_errPlus' % (label): errM500Plus, '%s_errMinus' % (label): errM500Minus}
+    return {'%s' % (label): M500, '%s_errPlus' % (label): errM500Plus, '%s_errMinus' % (label): errM500Minus,
+            'Q': bestQ}
 
 #------------------------------------------------------------------------------------------------------------
 def calcPMass(y0, y0Err, z, zErr, QFit, mockSurvey, tenToA0 = 4.95e-5, B0 = 0.08, Mpivot = 3e14, 
               sigma_int = 0.2, Ez_gamma = 2, onePlusRedshift_power = 0.0, applyMFDebiasCorrection = True, 
               applyRelativisticCorrection = True, fRelWeightsDict = {148.0: 1.0}, return2D = False,
-              tileName = None):
+              returnQ = False, tileName = None):
     """Calculates P(M500) assuming a y0 - M relation (default values assume UPP scaling relation from Arnaud 
     et al. 2010), taking into account the steepness of the mass function. The approach followed is described 
     in H13, Section 3.2. The binning for P(M500) is set according to the given mockSurvey, as are the assumed
     cosmological parameters.
     
     This routine is used by calcMass.
     
@@ -1275,28 +1419,35 @@
     # 2D PArr is what we would want to project onto (M, z) grid
     PArr=np.array(PArr)
         
     # Marginalised over z uncertainty
     P=np.sum(PArr, axis = 0)
     P=P/np.trapz(P, log10Ms)
     
+    # If we want Q corresponding to mass (need more work to add errors if we really want them)
+    PQ=P/np.trapz(P, Qs)
+    fittedQ=Qs[np.argmax(PQ)]
+
     # Reshape to (M, z) grid - use this if use different log10M range to mockSurvey
     #tck=interpolate.splrep(log10Ms, P)
     #P=interpolate.splev(mockSurvey.log10M, tck, ext = 1)
         
     if return2D == True:
         P2D=np.zeros(mockSurvey.clusterCount.shape)
         if zErr == 0:
             P2D[np.argmin(abs(mockSurvey.z-z))]=PArr
         else:
             P2D[zMask]=PArr
         P=P2D/P2D.sum()
         #astImages.saveFITS("test.fits", P.transpose(), None)
-        
-    return P
+
+    if returnQ == True:
+        return P, fittedQ
+    else:
+        return P
 
 #------------------------------------------------------------------------------------------------------------
 # Mass conversion routines
 
 # For getting x(f) - see Hu & Kravtsov
 x=np.linspace(1e-3, 10, 1000)
 fx=(x**3)*(np.log(1+1./x)-np.power(1+x, -1))
@@ -1346,40 +1497,54 @@
     """
     
     rho_mean=astCalc.OmegaMz(z)*criticalDensity(z)
     
     return rho_mean  
 
 #------------------------------------------------------------------------------------------------------------
-def M500cToMdef(M500c, z, massDef, cosmoModel):
-    """Convert M500c to some other mass definition.
-    
-    massDef (`obj`:ccl.halos.MassDef): CCL halo mass definition
-    
-    """
+def MDef1ToMDef2(mass, z, MDef1, MDef2, cosmoModel):
+    """Convert some mass at some z defined using MDef1 into a mass defined according to MDef2.
 
-    M500cDef=ccl.halos.MassDef(500, "critical")
+    Args:
+        mass (float): Halo mass in MSun.
+        z (float): Redshift of the halo.
+        MDef1 (`obj`:ccl.halos.MassDef): CCL halo mass definition you want to convert from.
+        MDef2 (`obj`:ccl.halos.MassDef): CCL halo mass definition you want to convert to.
+
+    """
 
     tolerance=1e-5
     scaleFactor=3.0
     ratio=1e6
     count=0
-    while abs(1.0-ratio) > tolerance:
-        testM500c=massDef.translate_mass(cosmoModel, scaleFactor*M500c, 1/(1+z), M500cDef)
-        ratio=M500c/testM500c
-        scaleFactor=scaleFactor*ratio
-        count=count+1
-        if count > 10:
-            raise Exception("M500c -> massDef conversion didn't converge quickly enough")
-        
-    massX=scaleFactor*M500c
-    
+    try:
+        massX=MDef1.translate_mass(cosmoModel, mass, 1/(1+z), MDef2)
+    except:
+        while abs(1.0-ratio) > tolerance:
+            testMass=MDef2.translate_mass(cosmoModel, scaleFactor*mass, 1/(1+z), MDef1)
+            ratio=mass/testMass
+            scaleFactor=scaleFactor*ratio
+            count=count+1
+            if count > 10:
+                raise Exception("MDef1 -> MDef2 mass conversion didn't converge quickly enough")
+        massX=scaleFactor*mass
+
     return massX
 
 #------------------------------------------------------------------------------------------------------------
+def M500cToMdef(M500c, z, massDef, cosmoModel):
+    """Convert M500c to some other mass definition.
+    
+    massDef (`obj`:ccl.halos.MassDef): CCL halo mass definition
+    
+    """
+
+    return MDef1ToMDef2(M500c, z, ccl.halos.MassDef(500, "critical"), massDef, cosmoModel)
+
+#------------------------------------------------------------------------------------------------------------
 def convertM200mToM500c(M200m, z):
     """Returns M500c (MSun), R500c (Mpc) for given M200m and redshift. Uses the Bhattacharya et al. c-M
     relation: http://adsabs.harvard.edu/abs/2013ApJ...766...32B
 
     See also Hu & Kravtsov: http://iopscience.iop.org/article/10.1086/345846/pdf
     
     """
```

### Comparing `nemo-sz-0.5.0/nemo_sz.egg-info/PKG-INFO` & `nemo-sz-0.6.0/nemo_sz.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: nemo-sz
-Version: 0.5.0
+Version: 0.6.0
 Summary: Millimeter-wave galaxy cluster and source detection package.
 Home-page: https://nemo-sz.readthedocs.io
 Author: Matt Hilton + Nemo Contributors
 Author-email: hiltonm@ukzn.ac.za
-License: UNKNOWN
-Description: Millimeter-wave map filtering and Sunyaev-Zel'dovich galaxy cluster/source detection package. Originally developed for the Atacama Cosmology Telescope project.
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Astronomy
+License-File: LICENSE
+
+Millimeter-wave map filtering and Sunyaev-Zel'dovich galaxy cluster/source detection package. Originally developed for the Atacama Cosmology Telescope project.
```

### Comparing `nemo-sz-0.5.0/nemo_sz.egg-info/SOURCES.txt` & `nemo-sz-0.6.0/nemo_sz.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 INSTALL.rst
+LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 versioneer.py
 bin/nemo
 bin/nemoCatalogCheck
-bin/nemoCosmo
 bin/nemoMass
 bin/nemoMock
 bin/nemoModel
-bin/nemoSelFn
 bin/nemoSpec
 docs/Makefile
 docs/advanced.rst
 docs/commands.rst
 docs/conf.py
 docs/config.rst
 docs/development.rst
@@ -24,15 +23,14 @@
 docs/index.rst
 docs/install.rst
 docs/outputs.rst
 docs/quickstart.rst
 docs/reference.rst
 docs/sosims_tutorial.rst
 docs/testing.rst
-docs/tilec_tutorial.rst
 docs/tutorials.rst
 examples/ACT-DR3-clusters/ACTPol_clusters.fits
 examples/ACT-DR3-clusters/ACTPol_redshifts.fits
 examples/ACT-DR3-clusters/E-D56Clusters.fits
 examples/ACT-DR3-clusters/README.rst
 examples/ACT-DR3-clusters/equD56.yml
 examples/ACT-DR3-clusters/equD56_quick.yml
@@ -100,15 +98,14 @@
 nemo/__init__.py
 nemo/_version.py
 nemo/catalogs.py
 nemo/completeness.py
 nemo/filters.py
 nemo/gnfw.py
 nemo/maps.py
-nemo/nemoCython.pyx
 nemo/photometry.py
 nemo/pipelines.py
 nemo/plotSettings.py
 nemo/signals.py
 nemo/startUp.py
 nemo/data/planck_lensedCls.dat
 nemo_sz.egg-info/PKG-INFO
@@ -123,14 +120,16 @@
 tests/quick.robot
 tests/configs/MPITestSurveyMaskHeader.txt
 tests/configs/PSTest_E-D56.yml
 tests/configs/PSTest_south2008.yml
 tests/configs/PSTest_south2008_fourier.yml
 tests/configs/README.rst
 tests/configs/equD56_quick_fourier.yml
+tests/configs/quickstart-multipass.yml
 tests/configs/sim_cl_A10_MFMF_tiles.yml
+tests/configs/sim_cl_A10_MFMF_tiles_multipass.yml
 tests/configs/sim_cl_B12_MFMF_tiles.yml
 tests/configs/sim_cl_MFMF.yml
 tests/configs/sim_cl_MFMF_pass2.yml
 tests/configs/sim_ptsrc_f090.yml
 tests/configs/smallTestSurveyMaskHeader.txt
 tests/lib/NemoTests.py
```

### Comparing `nemo-sz-0.5.0/setup.py` & `nemo-sz-0.6.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 #
 # nemo install script
 
 import os
 import glob
 from setuptools import setup
 from setuptools import Extension
-from Cython.Distutils import build_ext
+#from Cython.Distutils import build_ext
 import numpy
 import versioneer
 
 cmdclass=versioneer.get_cmdclass()
-cmdclass['build_ext']=build_ext
+#cmdclass['build_ext']=build_ext
 
 setup(name='nemo-sz',
       version=versioneer.get_version(),
       cmdclass=cmdclass,
       url="https://nemo-sz.readthedocs.io",
       author='Matt Hilton + Nemo Contributors',
       author_email='hiltonm@ukzn.ac.za',
@@ -27,23 +27,23 @@
                    'Operating System :: POSIX',
                    'Programming Language :: Python',
                    'Topic :: Scientific/Engineering :: Astronomy'],
       description='Millimeter-wave galaxy cluster and source detection package.',
       long_description="""Millimeter-wave map filtering and Sunyaev-Zel'dovich galaxy cluster/source detection package. Originally developed for the Atacama Cosmology Telescope project.""",
       packages=['nemo'],
       package_data={'nemo': ['data/*']},
-      scripts=['bin/nemo', 'bin/nemoMass', 'bin/nemoSelFn', 'bin/nemoMock', 'bin/nemoCatalogCheck', 'bin/nemoCosmo', 'bin/nemoModel', 'bin/nemoSpec'],
-      ext_modules=[Extension("nemoCython", ["nemo/nemoCython.pyx"], include_dirs=[numpy.get_include()])],
+      scripts=['bin/nemo', 'bin/nemoMass', 'bin/nemoMock', 'bin/nemoCatalogCheck', 'bin/nemoModel', 'bin/nemoSpec'],
+      #ext_modules=[Extension("nemoCython", ["nemo/nemoCython.pyx"], include_dirs=[numpy.get_include()])],
       install_requires=["astropy >= 4.0",
                         "numpy >= 1.19",
                         "matplotlib >= 2.0",
-                        "astLib >= 0.11.6",
-                        "pixell >= 0.5",
+                        "astLib >= 0.11.8",
+                        "pixell >= 0.17",
                         "scipy >= 1.0",
                         "pillow",
-                        "cython",
+                        #"cython",
                         "PyYAML",
                         #"pyccl >= 2.1",
                         #"mpi4py",
                         "colorcet >= 1.0",
                         "mahotas >= 1.4"]
 )
```

### Comparing `nemo-sz-0.5.0/tests/README.rst` & `nemo-sz-0.6.0/tests/README.rst`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/tests/clusters.robot` & `nemo-sz-0.6.0/tests/clusters.robot`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/tests/configs/MPITestSurveyMaskHeader.txt` & `nemo-sz-0.6.0/tests/configs/MPITestSurveyMaskHeader.txt`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/tests/configs/PSTest_E-D56.yml` & `nemo-sz-0.6.0/tests/configs/PSTest_E-D56.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/tests/configs/PSTest_south2008.yml` & `nemo-sz-0.6.0/tests/configs/PSTest_south2008.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/tests/configs/PSTest_south2008_fourier.yml` & `nemo-sz-0.6.0/tests/configs/PSTest_south2008_fourier.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/tests/configs/equD56_quick_fourier.yml` & `nemo-sz-0.6.0/tests/configs/equD56_quick_fourier.yml`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/tests/configs/sim_cl_A10_MFMF_tiles.yml` & `nemo-sz-0.6.0/tests/configs/sim_cl_A10_MFMF_tiles.yml`

 * *Files 1% similar despite different names*

```diff
@@ -54,25 +54,25 @@
               redshiftCatalog: "S18Clusters/AdvACT_confirmed.fits"}
 
 # Selection function options - this calculation can also be enabled with the nemo -S switch
 # NOTE: could eventually add 'completenessFraction' to 'massLimitMaps', which is why that's a dictionary list
 # Use selFnFootprints to calculate average completeness in given sky areas - e.g., overlap with optical surveys
 calcSelFn: False
 selFnOptions: {fixedSNRCut: 5.0,
-               method: 'montecarlo',
+               method: 'injection',
                numIterations: 1000, 
                massLimitMaps: [{z: 0.5}]}
                
-selFnFootprints: 
-    - {label: "HSC",
-       maskList: ["HSCCheckAndSelFn/s19a_fdfc_CAR_contarea_ziy-gt-5.fits"]}
-    - {label: "KiDS",
-       maskList: ["KiDSSelFn/mask_KiDSN.fits", "KiDSSelFn/mask_KiDSS.fits"]}
-    - {label: "DES",
-       maskList: ["DESY3/AdvACT_y3a2_footprint_griz_1exp_v2.0.fits"]}
+#selFnFootprints:
+    #- {label: "HSC",
+       #maskList: ["HSCCheckAndSelFn/s19a_fdfc_CAR_contarea_ziy-gt-5.fits"]}
+    #- {label: "KiDS",
+       #maskList: ["KiDSSelFn/mask_KiDSN.fits", "KiDSSelFn/mask_KiDSS.fits"]}
+    #- {label: "DES",
+       #maskList: ["DESY3/AdvACT_y3a2_footprint_griz_1exp_v2.0.fits"]}
 
 # Filter definitions:
 # allFilters is a dictionary of parameters that will be copied into all mapFilters
 # (these can be overridden by keys with the same name in mapFilters)
 allFilters: {class: "ArnaudModelMatchedFilter",
              params: {noiseParams: {method: "dataMap",
                                     noiseGridArcmin: 40.},
```

### Comparing `nemo-sz-0.5.0/tests/configs/sim_cl_B12_MFMF_tiles.yml` & `nemo-sz-0.6.0/tests/configs/sim_cl_B12_MFMF_tiles.yml`

 * *Files 2% similar despite different names*

```diff
@@ -50,25 +50,25 @@
               redshiftCatalog: "S18Clusters/AdvACT_confirmed.fits"}
 
 # Selection function options - this calculation can also be enabled with the nemo -S switch
 # NOTE: could eventually add 'completenessFraction' to 'massLimitMaps', which is why that's a dictionary list
 # Use selFnFootprints to calculate average completeness in given sky areas - e.g., overlap with optical surveys
 calcSelFn: False
 selFnOptions: {fixedSNRCut: 5.0,
-               method: 'montecarlo',
+               method: 'injection',
                numIterations: 1000, 
                massLimitMaps: [{z: 0.5}]}
                
-selFnFootprints: 
-    - {label: "HSC",
-       maskList: ["HSCCheckAndSelFn/s19a_fdfc_CAR_contarea_ziy-gt-5.fits"]}
-    - {label: "KiDS",
-       maskList: ["KiDSSelFn/mask_KiDSN.fits", "KiDSSelFn/mask_KiDSS.fits"]}
-    - {label: "DES",
-       maskList: ["DESY3/AdvACT_y3a2_footprint_griz_1exp_v2.0.fits"]}
+#selFnFootprints:
+    #- {label: "HSC",
+       #maskList: ["HSCCheckAndSelFn/s19a_fdfc_CAR_contarea_ziy-gt-5.fits"]}
+    #- {label: "KiDS",
+       #maskList: ["KiDSSelFn/mask_KiDSN.fits", "KiDSSelFn/mask_KiDSS.fits"]}
+    #- {label: "DES",
+       #maskList: ["DESY3/AdvACT_y3a2_footprint_griz_1exp_v2.0.fits"]}
 
 # Filter definitions:
 # allFilters is a dictionary of parameters that will be copied into all mapFilters
 # (these can be overridden by keys with the same name in mapFilters)
 allFilters: {class: "BattagliaModelMatchedFilter",
              params: {noiseParams: {method: "dataMap",
                                     noiseGridArcmin: 40.},
```

### Comparing `nemo-sz-0.5.0/tests/configs/sim_cl_MFMF.yml` & `nemo-sz-0.6.0/tests/configs/sim_cl_A10_MFMF_tiles_multipass.yml`

 * *Files 1% similar despite different names*

```diff
@@ -54,25 +54,25 @@
               redshiftCatalog: "S18Clusters/AdvACT_confirmed.fits"}
 
 # Selection function options - this calculation can also be enabled with the nemo -S switch
 # NOTE: could eventually add 'completenessFraction' to 'massLimitMaps', which is why that's a dictionary list
 # Use selFnFootprints to calculate average completeness in given sky areas - e.g., overlap with optical surveys
 calcSelFn: False
 selFnOptions: {fixedSNRCut: 5.0,
-               method: 'montecarlo',
+               method: 'injection',
                numIterations: 1000, 
                massLimitMaps: [{z: 0.5}]}
                
-selFnFootprints: 
-    - {label: "HSC",
-       maskList: ["HSCCheckAndSelFn/s19a_fdfc_CAR_contarea_ziy-gt-5.fits"]}
-    - {label: "KiDS",
-       maskList: ["KiDSSelFn/mask_KiDSN.fits", "KiDSSelFn/mask_KiDSS.fits"]}
-    - {label: "DES",
-       maskList: ["DESY3/AdvACT_y3a2_footprint_griz_1exp_v2.0.fits"]}
+#selFnFootprints:
+    #- {label: "HSC",
+       #maskList: ["HSCCheckAndSelFn/s19a_fdfc_CAR_contarea_ziy-gt-5.fits"]}
+    #- {label: "KiDS",
+       #maskList: ["KiDSSelFn/mask_KiDSN.fits", "KiDSSelFn/mask_KiDSS.fits"]}
+    #- {label: "DES",
+       #maskList: ["DESY3/AdvACT_y3a2_footprint_griz_1exp_v2.0.fits"]}
 
 # Filter definitions:
 # allFilters is a dictionary of parameters that will be copied into all mapFilters
 # (these can be overridden by keys with the same name in mapFilters)
 allFilters: {class: "ArnaudModelMatchedFilter",
              params: {noiseParams: {method: "dataMap",
                                     noiseGridArcmin: 40.},
@@ -129,20 +129,18 @@
 sourceInjectionModels:
     - {redshift: 0.8, M500: 2.0e+14}
     - {redshift: 0.4, M500: 2.0e+14}
     - {redshift: 0.2, M500: 2.0e+14}
     - {redshift: 0.1, M500: 2.0e+14}
 
 # tileDir options - cut-up each map into smaller sections
-#makeTileDir: True
-#makeQuickLookMaps: True
-#stitchTiles: True
-#tileOverlapDeg: 1.0
-#tileDefLabel: 'auto'
-#tileDefinitions: {mask: 'maps/Jun2020/AdvACTSurveyMask_v7_S18.fits',
-                  #targetTileWidthDeg: 10.0, 
-                  #targetTileHeightDeg: 5.0}
+makeTileDir: True
+stitchTiles: True
+tileOverlapDeg: 1.0
+tileDefLabel: 'auto'
+tileDefinitions: {targetTileWidthDeg: 10.0, 
+                  targetTileHeightDeg: 5.0}
 
 # If this is given, only the named tiles will be processed (useful for testing)
 #tileNameList:
     #- '1_10_7'
     #- '1_10_8'      # contains J2327 (next to a source)
```

### Comparing `nemo-sz-0.5.0/tests/configs/sim_cl_MFMF_pass2.yml` & `nemo-sz-0.6.0/tests/configs/sim_cl_MFMF_pass2.yml`

 * *Files 1% similar despite different names*

```diff
@@ -56,25 +56,25 @@
               redshiftCatalog: "S18Clusters/AdvACT_confirmed.fits"}
 
 # Selection function options - this calculation can also be enabled with the nemo -S switch
 # NOTE: could eventually add 'completenessFraction' to 'massLimitMaps', which is why that's a dictionary list
 # Use selFnFootprints to calculate average completeness in given sky areas - e.g., overlap with optical surveys
 calcSelFn: False
 selFnOptions: {fixedSNRCut: 5.0,
-               method: 'montecarlo',
+               method: 'injection',
                numIterations: 1000, 
                massLimitMaps: [{z: 0.5}]}
                
-selFnFootprints: 
-    - {label: "HSC",
-       maskList: ["HSCCheckAndSelFn/s19a_fdfc_CAR_contarea_ziy-gt-5.fits"]}
-    - {label: "KiDS",
-       maskList: ["KiDSSelFn/mask_KiDSN.fits", "KiDSSelFn/mask_KiDSS.fits"]}
-    - {label: "DES",
-       maskList: ["DESY3/AdvACT_y3a2_footprint_griz_1exp_v2.0.fits"]}
+#selFnFootprints:
+    #- {label: "HSC",
+       #maskList: ["HSCCheckAndSelFn/s19a_fdfc_CAR_contarea_ziy-gt-5.fits"]}
+    #- {label: "KiDS",
+       #maskList: ["KiDSSelFn/mask_KiDSN.fits", "KiDSSelFn/mask_KiDSS.fits"]}
+    #- {label: "DES",
+       #maskList: ["DESY3/AdvACT_y3a2_footprint_griz_1exp_v2.0.fits"]}
 
 # Filter definitions:
 # allFilters is a dictionary of parameters that will be copied into all mapFilters
 # (these can be overridden by keys with the same name in mapFilters)
 allFilters: {class: "ArnaudModelMatchedFilter",
              params: {noiseParams: {method: "dataMap",
                                     noiseGridArcmin: 40.},
```

### Comparing `nemo-sz-0.5.0/tests/configs/sim_ptsrc_f090.yml` & `nemo-sz-0.6.0/tests/configs/sim_ptsrc_f090.yml`

 * *Files 22% similar despite different names*

```diff
@@ -19,17 +19,22 @@
 useInterpolator: True
 rejectBorder: 0
 objIdent: 'MOCK-S'
 longNames: False
 
 # mapFilters is a list of all the different filters to apply
 # (keys in mapFilters with the same name as those in allFilters take priority)
-twoPass: False
 mapFilters:
-        - {label: "Beam090",
-           class: "BeamMatchedFilter",
-           params: {noiseParams: {method: "dataMap",
-                                  noiseGridArcmin: 40.0,
-                                  numNoiseBins: 8},
-                    saveFilteredMaps: True,
-                    outputUnits: 'uK',
-                    edgeTrimArcmin: 0.0}}
+    - {label: "Beam090",
+        class: "BeamMatchedFilter",
+        params: {noiseParams: {method: "dataMap",
+                                noiseGridArcmin: 40.0,
+                                numNoiseBins: 8},
+                saveFilteredMaps: True,
+                saveFilter: True,
+                outputUnits: 'uK',
+                edgeTrimArcmin: 0.0}}
+
+# Source injection test settings
+haltOnPositionRecoveryProblem: True
+sourceInjectionIterations: 3
+sourcesPerTile: 300
```

### Comparing `nemo-sz-0.5.0/tests/configs/smallTestSurveyMaskHeader.txt` & `nemo-sz-0.6.0/tests/configs/smallTestSurveyMaskHeader.txt`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/tests/debug.py` & `nemo-sz-0.6.0/tests/debug.py`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/tests/lib/NemoTests.py` & `nemo-sz-0.6.0/tests/lib/NemoTests.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import numpy as np
 from nemo import catalogs, maps, plotSettings
 from astLib import *
 import astropy.io.fits as pyfits
 import astropy.table as atpy
 from astropy.coordinates import SkyCoord, match_coordinates_sky
 import pylab as plt
-import IPython
 
 plotSettings.update_rcParams()
 plotTitleSize=14
 
 #------------------------------------------------------------------------------------------------------------
 class NemoTests(object):
 
@@ -136,16 +135,15 @@
         # Generate mask file(s) for simming
         headerFileNames=["configs/smallTestSurveyMaskHeader.txt", "configs/MPITestSurveyMaskHeader.txt"]
         maskFileNames=["smallTestSurveyMask.fits", "MPITestSurveyMask.fits"]
         for headerFileName, maskFileName in zip(headerFileNames, maskFileNames):
             header=pyfits.Header().fromtextfile(headerFileName)
             wcs=astWCS.WCS(header, mode = 'pyfits')
             d=np.ones([wcs.header['NAXIS2'], wcs.header['NAXIS1']], dtype = int)
-            maps.saveFITS(self.cacheDir+os.path.sep+maskFileName, d, wcs,
-                          compressed = True, compressionType = 'PLIO_1')
+            maps.saveFITS(self.cacheDir+os.path.sep+maskFileName, d, wcs, compressionType = 'PLIO_1')
         
         # Map/frequency-related defaults
         self.bandsDict={'f150': {'beam': "maps/s16_pa2_f150_nohwp_night_beam_profile_jitter.txt",
                                  'freq': str(149.6)},
                         'f090': {'beam': "maps/s16_pa3_f090_nohwp_night_beam_profile_jitter.txt",
                                  'freq': str(97.8)}
                        }
@@ -165,16 +163,20 @@
         self.mocksDir=configFileName.replace(".yml", "")+os.path.sep+"mocks"
         
         
     def run_nemo(self):
         self._run_command(["nemo", self.configFileName])
 
 
+    def run_nemo_injection_test(self):
+        self._run_command(["nemo", self.configFileName, "-I"])
+
+
     def run_parallel_nemo(self):
-        self._run_command(["mpiexec", "nemo", self.configFileName, "-M"])
+        self._run_command(["mpiexec", "-np", "4", "nemo", self.configFileName, "-M"])
 
 
     def run_nemo_mass(self, catalogFileName = None):
         args=['nemoMass', self.configFileName]
         if catalogFileName != None:
             args=args+['-c', catalogFileName]
         self._run_command(args)
@@ -184,15 +186,15 @@
         args=['nemoModel', catalogFileName, self.sizesDict[size]['mask'], self.bandsDict[band]['beam'], 
               "sim_%s.fits" % (band), '-f', self.bandsDict[band]['freq'], 
               '-C', '-N', noiseLevel, '-S', seed]
         self._run_command(args)
 
 
     def make_parallel_sim(self, catalogFileName = None, noiseLevel = None, seed = None, band = None, size = None, profile = None):
-        args=['mpiexec', 'nemoModel', catalogFileName, self.sizesDict[size]['mask'], self.bandsDict[band]['beam'], 
+        args=['mpiexec', '-np', '4', 'nemoModel', catalogFileName, self.sizesDict[size]['mask'], self.bandsDict[band]['beam'],
               "sim_%s.fits" % (band), '-f', self.bandsDict[band]['freq'],
               '-C', '-N', noiseLevel, '-S', seed, '-M']
         if profile is not None:
             args=args+['-p', profile]
         self._run_command(args)
 
 
@@ -206,15 +208,15 @@
     def make_signal_only_sim(self, catalogFileName = None, band = None, size = None):
         args=['nemoModel', catalogFileName, self.sizesDict[size]['mask'], self.bandsDict[band]['beam'], 
               "signal_model_only_%s.fits" % (band), '-f', self.bandsDict[band]['freq']]
         self._run_command(args)
         
         
     def make_parallel_signal_only_sim(self, catalogFileName = None, band = None, size = None, profile = None):
-        args=['mpiexec', 'nemoModel', catalogFileName, self.sizesDict[size]['mask'], self.bandsDict[band]['beam'], 
+        args=['mpiexec', '-np', '4', 'nemoModel', catalogFileName, self.sizesDict[size]['mask'], self.bandsDict[band]['beam'],
               "signal_model_only_%s.fits" % (band), '-f', self.bandsDict[band]['freq'], '-M']
         if profile is not None:
             args=args+['-p', profile]
         self._run_command(args)
     
 
     def run_nemo_selfn(self, configFileName = None):
@@ -272,15 +274,15 @@
                 break
         if RAKey == None or decKey == None:
             raise Exception("couldn't identify RA, dec columns in the supplied table")
         
         return RAKey, decKey
         
         
-    def check_recovered_ratio(self, inKey, outKey, toleranceSigma = 1.0, SNRCut = 4,
+    def check_recovered_ratio(self, inKey, outKey, toleranceSigma = 1.0, expectedRatio = 1.0, SNRCut = 4,
                               SNRKey = 'fixed_SNR', errInKey = None, errOutKey = None,
                               plotLabel = None, plotsDir = "plots"):
         """Catalogs must have been cross matched before this can be run.
         Calculate the ratio of the columns pointed to by inKey, outKey. If tolerance (defined as
         1 - average ratio) is exceeded, the test is failed. SNRCut is applied to SNRKey in the output catalog.
         
         """
@@ -318,15 +320,15 @@
             plt.plot(plotRange, plotRange, 'k--')
             plt.xlim(plotMin, plotMax)
             plt.ylim(plotMin, plotMax)
             plt.loglog()
             plt.title(label, fontdict = {'size': plotTitleSize})
             plt.savefig(plotsDir+os.path.sep+plotLabel+"_XvY.png")
             plt.close()
-        if abs((1.0-meanRatio)/meanRatioErr) > toleranceSigma:
+        if abs((expectedRatio-meanRatio)/meanRatioErr) > toleranceSigma:
             self._status="FAILED"
         else:
             self._status="SUCCESS"
             
             
     def check_recovered_positions(self, toleranceArcsec = 12.0, SNRKey = 'SNR', SNRMax = 10.0, 
                                   plotLabel = None, plotsDir = "plots"):
```

### Comparing `nemo-sz-0.5.0/tests/point_sources.robot` & `nemo-sz-0.6.0/tests/point_sources.robot`

 * *Files identical despite different names*

### Comparing `nemo-sz-0.5.0/tests/quick.robot` & `nemo-sz-0.6.0/tests/quick.robot`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 *** Test Cases ***
 
 Quickstart clusters tutorial runs
     Run quickstart clusters
     Cross match             testsCache/quickstart-clusters/quickstart-clusters_optimalCatalog.fits      testsCache/DR5_cluster-catalog_v1.1.fits
-    Check recovered ratio   fixed_y_c    fixed_y_c    toleranceSigma=3.0    errInKey=fixed_err_y_c  errOutKey=fixed_err_y_c  SNRKey=fixed_SNR  SNRCut=5.0  plotLabel=quickstart-clusters
+    Check recovered ratio   fixed_y_c    fixed_y_c    toleranceSigma=3.0    expectedRatio=0.94  errInKey=fixed_err_y_c  errOutKey=fixed_err_y_c  SNRKey=fixed_SNR  SNRCut=5.0  plotLabel=quickstart-clusters
     Status should be        SUCCESS
 
 Quickstart sources tutorial runs
     Run quickstart sources
 
+Source injection test runs
+    Generate simulated source maps
+    Set config      configs/sim_ptsrc_f090.yml
+    Run nemo injection test
+
+Quickstart multipass config runs
+    Run quickstart multipass
+    Cross match             testsCache/quickstart-multipass/quickstart-multipass_optimalCatalog.fits      testsCache/DR5_cluster-catalog_v1.1.fits
+    Check recovered ratio   fixed_y_c    fixed_y_c    toleranceSigma=3.0    expectedRatio=0.92  errInKey=fixed_err_y_c  errOutKey=fixed_err_y_c  SNRKey=fixed_SNR  SNRCut=5.0  plotLabel=quickstart-multipass
+    Status should be        SUCCESS
+
 Cluster sim with nemoModel runs
     Generate simulated cluster maps
 
 Source sim with nemoModel runs
     Generate simulated source maps
     
 Recovered sim source amplitudes are unbiased
     Generate simulated source maps
     Set config      configs/sim_ptsrc_f090.yml
     Run nemo
     Cross match     testsCache/sim_f090_inputCatalog.fits     testsCache/sim_ptsrc_f090/sim_ptsrc_f090_optimalCatalog.fits
-    Check recovered ratio   deltaT_c    deltaT_c    toleranceSigma=3.0  SNRKey=SNR  SNRCut=5.0  plotLabel=sim_ptsrc_amplitudes
+    Check recovered ratio   deltaT_c    deltaT_c    toleranceSigma=3.0  SNRKey=SNR  SNRCut=7.0  plotLabel=sim_ptsrc_amplitudes
     Status should be        SUCCESS
     
 End-to-end source recovery and subtraction
     Generate simulated source maps
     Set config      configs/sim_ptsrc_f090.yml
     Run nemo
     Make signal only sim    sim_ptsrc_f090/sim_ptsrc_f090_optimalCatalog.fits   f090    small
@@ -46,14 +57,18 @@
     Set config              ../examples/quickstart/quickstart-clusters.yml
     Run nemo
 
 Run quickstart sources
     Set config              ../examples/quickstart/quickstart-sources.yml
     Run nemo
 
+Run quickstart multipass
+    Set config              configs/quickstart-multipass.yml
+    Run nemo
+
 Generate simulated cluster maps
     Setup quickstart
     Make sim    DR5_cluster-catalog_v1.1.fits   50.0    1234    f150    large
     Make sim    DR5_cluster-catalog_v1.1.fits   50.0    1234    f090    large
 
 Generate simulated cluster maps in parallel
     [Arguments]   ${profile}
@@ -89,26 +104,21 @@
     Check map sigma     testsCache/signal_free-cl_${profile}_f090_diff.fits    50
     Status should be        SUCCESS
     [Teardown]  Clean up cluster sim    ${profile}
 
 Clean up cluster sim
     [Arguments]   ${profile}
     Remove directory        testsCache/sim_cl_${profile}_MFMF_tiles     True
-    Remove directory        testsCache/tileDir_auto_1.0_sim_f090.fits   True
-    Remove directory        testsCache/tileDir_auto_1.0_sim_f150.fits   True
 
 Clean up
-    Remove directory        testsCache/sim_cl_MFMF  True
-    Remove directory        testsCache/tileDir_auto_1.0_surveyMask  True
-    Remove directory        testsCache/tileDir_auto_1.0_sim_f090.fits   True
-    Remove directory        testsCache/tileDir_auto_1.0_sim_f150.fits   True
-    #Remove directory        testsCache/sim_cl_MFMF_pass2  True
-    Remove directory        testsCache/sim_ptsrc_f090  True
-    Remove directory        testsCache/quickstart-clusters  True
-    Remove directory        testsCache/quickstart-sources   True
+    Remove directory        testsCache/sim_cl_MFMF                      True
+    Remove directory        testsCache/sim_ptsrc_f090                   True
+    Remove directory        testsCache/quickstart-clusters              True
+    Remove directory        testsCache/quickstart-sources               True
+    Remove directory        testsCache/quickstart-multipass             True
 
 
 *** Settings ***
 #Documentation              To be added here
 Library                     OperatingSystem
 Library                     lib/NemoTests.py
 Suite Setup                 Setup quickstart
```

### Comparing `nemo-sz-0.5.0/versioneer.py` & `nemo-sz-0.6.0/versioneer.py`

 * *Files identical despite different names*

