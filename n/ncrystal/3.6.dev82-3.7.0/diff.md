# Comparing `tmp/ncrystal-3.6.dev82.tar.gz` & `tmp/ncrystal-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncrystal-3.6.dev82.tar", last modified: Fri Jul 14 18:10:46 2023, max compression
+gzip compressed data, was "ncrystal-3.7.0.tar", last modified: Fri Jul 14 17:26:21 2023, max compression
```

## Comparing `ncrystal-3.6.dev82.tar` & `ncrystal-3.7.0.tar`

### file list

```diff
@@ -1,433 +1,434 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.492546 ncrystal-3.6.dev82/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.436545 ncrystal-3.6.dev82/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.440544 ncrystal-3.6.dev82/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/.github/ISSUE_TEMPLATE/request-for-new-material.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.440544 ncrystal-3.6.dev82/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/.github/workflows/cmake.yml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    76764 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)    35344 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/FILES
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/INSTALL
--rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.444545 ncrystal-3.6.dev82/NCrystal/
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40112 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/_chooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/_coreimpl.py
--rw-r--r--   0 runner    (1001) docker     (123)    16356 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/_miscimpl.py
--rw-r--r--   0 runner    (1001) docker     (123)    85698 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/_ncmatimpl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    25999 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/_testimpl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/atomdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/cfgstr.py
--rw-r--r--   0 runner    (1001) docker     (123)    74600 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/cifutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    74942 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/datasrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/mcstasutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11032 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    38896 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/ncmat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/obsolete.py
--rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    45843 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/vdos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-14 18:10:46.492546 ncrystal-3.6.dev82/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/README
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.444545 ncrystal-3.6.dev82/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/cmake/NCrystalConfig.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.444545 ncrystal-3.6.dev82/cmake/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/cmake/modules/ncrystal_legacyoptions.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/cmake/modules/ncrystal_options.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/cmake/modules/ncrystal_utils.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/cmake/ncrystal-config.in
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/cmake/template_setup.py.in
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/cmake/template_setup.sh.in
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/cmake/template_unsetup.sh.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.464545 ncrystal-3.6.dev82/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/AcrylicGlass_C5O2H8.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/AgBr_sg225_SilverBromide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ag_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Al2O3_sg167_Corundum.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Al4C3_sg166_AluminiumCarbide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/AlN_sg186_AluminumNitride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Al_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ar_Gas_STP.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Au_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/BaF2_sg225_BariumFluoride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/BaO_sg225_BariumOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ba_sg229.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Be3N2_sg206_BerylliumNitride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/BeF2_sg152_Beryllium_Fluoride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/BeO_sg186.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Be_sg194.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Bi_sg166.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/C_sg194_pyrolytic_graphite.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/C_sg227_Diamond.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/CaCO3_sg62_Aragonite.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/CaF2_sg225_CalciumFlouride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/CaH2_sg62_CalciumHydride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/CaO2H2_sg164_CalciumHydroxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/CaO_sg225_CalciumOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/CaSiO3_sg2_Wollastonite.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ca_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ca_sg229_Calcium-gamma.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/CeO2_sg225_CeriumOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Cr_sg229.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Cu2O_sg224_Cuprite.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Cu_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Dy2O3_sg206_DysprosiumOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Epoxy_Araldite506_C18H20O3.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Fe_sg225_Iron-gamma.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Fe_sg229_Iron-alpha.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/GaN_sg186_GalliumNitride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/GaSe_sg194_GalliumSelenide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ge3Bi4O12_sg220_BismuthGermanate.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ge_sg227.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/He_Gas_STP.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/HfO2_sg14_HafniumOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ho2O3_sg206_HolmiumOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/KBr_sg225_PotassiumBromide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/KF_sg225_PotassiumFlouride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/KOH_sg4_PotassiumHydroxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/K_sg229.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Kapton_C22H10N2O5.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Kr_Gas_STP.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/LaBr3_sg176_LanthanumBromide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Li2O_sg225_LithiumOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Li3N_sg191_LithiumNitride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/LiF_sg225_LithiumFlouride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/LiH_sg225_LithiumHydride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)  1560968 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/LiquidHeavyWaterD2O_T293.6K.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)   528493 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/LiquidWaterH2O_T293.6K.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Lu2O3_sg206_LutetiumOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Lu2SiO5_sg15.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Mg2SiO4_sg62_MagnesiumSilicate.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/MgAl2O4_sg227_MAS.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/MgCO3_sg167_MagnesiumCarbonate.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/MgD2_sg136_MagnesiumDeuteride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/MgF2_sg136_MagnesiumFlouride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/MgH2_sg136_MagnesiumHydride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/MgO2H2_sg164_MagnesiumHydroxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/MgO_sg225_Periclase.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Mg_sg194.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Mo_sg229.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Na4Si3Al3O12Cl_sg218_Sodalite.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/NaBr_sg225_SodiumBromide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/NaCl_sg225_SodiumChloride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/NaF_sg225_SodiumFlouride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/NaI_sg225_SodiumIodide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Na_sg229.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Nb_sg229.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ne_Gas_STP.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ni_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Nylon11_C11H21NO.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Nylon12_C12H23NO.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Nylon610_C16H30N2O2.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Nylon66or6_C12H22N2O2.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/PEEK_C19H12O3.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/PVC_C2H3Cl.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/PbF2-beta_sg225_BetaLeadFlouride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/PbO-alpha_sg129_Litharge.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/PbO-beta_sg57_Massicot.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/PbS_sg225_LeadSulfide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Pb_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Pd_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Polycarbonate_C16O3H14.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Polyester_C10H8O4.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Polyethylene_CH2.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Polylactide_C3H4O2.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Polypropylene_C3H6.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Polystyrene_C8H8.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Pt_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Rb_sg229.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Rubber_C5H8.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Sc_sg194.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/SiC-beta_sg216_BetaSiliconCarbide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/SiO2-alpha_sg154_AlphaQuartz.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/SiO2-beta_sg180_BetaQuartz.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Si_sg227.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Sn_sg141.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/SrF2_sg225_StrontiumFluoride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/SrH2_sg62_StrontiumHydride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Sr_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Th3N4_sg166_ThoriumNitride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/ThO2_sg225_ThoriumDioxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Th_sg225.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/TiO2_sg136_Rutile.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/TiO2_sg141_Anatase.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ti_sg194.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/TlBr_sg221_ThaliumBromide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Tm2O3_sg206_ThuliumOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/UF6_sg62_UraniumHexaflouride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/UO2_sg225_UraniumDioxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/V_sg229.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/W_sg229.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Xe_Gas_STP.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Y2O3_sg206_Yttrium_Oxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Y2SiO5_sg15_YSO.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Y3Al5O12_sg230_YAG.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Y_sg194.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/ZnF2_sg136_ZincFlouride.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/ZnO_sg186_ZincOxide.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/ZnS_sg216_Sphalerite.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Zn_sg194.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/ZrF4-beta_sg84.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/ZrO2_sg137_Zirconia.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/ZrO2_sg14_Zirconia.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Zr_sg194.ncmat
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/void.ncmat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.464545 ncrystal-3.6.dev82/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    39216 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/docs/ncmat_doc.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.468545 ncrystal-3.6.dev82/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/examples/NCrystal_example_mcstas.instr
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/examples/ncrystal_example_c.c
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/examples/ncrystal_example_cpp.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/examples/ncrystal_example_customphysics.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/examples/ncrystal_example_g4sim.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/examples/ncrystal_example_py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.468545 ncrystal-3.6.dev82/ncrystal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-14 18:10:46.000000 ncrystal-3.6.dev82/ncrystal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-07-14 18:10:46.000000 ncrystal-3.6.dev82/ncrystal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:10:46.000000 ncrystal-3.6.dev82/ncrystal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 18:10:46.000000 ncrystal-3.6.dev82/ncrystal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 18:10:46.000000 ncrystal-3.6.dev82/ncrystal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.440544 ncrystal-3.6.dev82/ncrystal_core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.440544 ncrystal-3.6.dev82/ncrystal_core/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.472545 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCAtomData.hh
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCCompositionUtils.hh
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCDataSources.hh
--rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCDefs.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCDump.hh
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCException.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFact.hh
--rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFactImpl.hh
--rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFactRequests.hh
--rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFactTypes.hh
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFmt.hh
--rw-r--r--   0 runner    (1001) docker     (123)    16597 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCImmutBuf.hh
--rw-r--r--   0 runner    (1001) docker     (123)    28964 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCInfo.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCInfoBuilder.hh
--rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCInfoTypes.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCLoadNCMAT.hh
--rw-r--r--   0 runner    (1001) docker     (123)    22448 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCMatCfg.hh
--rw-r--r--   0 runner    (1001) docker     (123)    20439 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCMem.hh
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCNCMATData.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCParseNCMAT.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCPluginBoilerplate.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCPluginMgmt.hh
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCProc.hh
--rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCProcImpl.hh
--rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCRNG.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCSABData.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCSCOrientation.hh
--rw-r--r--   0 runner    (1001) docker     (123)    39147 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCSmallVector.hh
--rw-r--r--   0 runner    (1001) docker     (123)    14618 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCTextData.hh
--rw-r--r--   0 runner    (1001) docker     (123)    37486 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCTypes.hh
--rw-r--r--   0 runner    (1001) docker     (123)    13171 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCVariant.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCVersion.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCrystal.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.480545 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCAbsOOV.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCAtomDB.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCAtomDBExtender.hh
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCAtomUtils.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCBkgdExtCurve.hh
--rw-r--r--   0 runner    (1001) docker     (123)    23020 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCCfgManip.hh
--rw-r--r--   0 runner    (1001) docker     (123)    32290 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCCfgTypes.hh
--rw-r--r--   0 runner    (1001) docker     (123)    35719 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCCfgVars.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCDebyeMSD.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCDynInfoUtils.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCDynLoader.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCElIncScatter.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCElIncXS.hh
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCEqRefl.hh
--rw-r--r--   0 runner    (1001) docker     (123)    19986 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFactoryUtils.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFastConvolve.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFileUtils.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFillHKL.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFreeGas.hh
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFreeGasUtils.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCGasMixUtils.hh
--rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCGaussMos.hh
--rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCGaussOnSphere.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCIofQHelper.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCIter.hh
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCKinUtils.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCLCBragg.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCLCRefModels.hh
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCLCUtils.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCLatticeUtils.hh
--rw-r--r--   0 runner    (1001) docker     (123)    27371 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCMath.hh
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCMatrix.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCOrientUtils.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCPCBragg.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCPlaneProvider.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCPointwiseDist.hh
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCRandUtils.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCRomberg.hh
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCRotMatrix.hh
--rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABEval.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABExtender.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABFactory.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABIntegrator.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABSampler.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABSamplerModels.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABScatter.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABScatterHelper.hh
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABUCN.hh
--rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABUtils.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABXSProvider.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSANSSphScat.hh
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSANSUtils.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSCBragg.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCScatKnlData.hh
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSpan.hh
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSpline.hh
--rw-r--r--   0 runner    (1001) docker     (123)    20113 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCStrView.hh
--rw-r--r--   0 runner    (1001) docker     (123)    15426 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCString.hh
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCVDOSEval.hh
--rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCVDOSGn.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCVDOSToScatKnl.hh
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCVector.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/ncapi.h
--rw-r--r--   0 runner    (1001) docker     (123)    44878 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/ncrystal.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.492546 ncrystal-3.6.dev82/ncrystal_core/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCAbsOOV.cc
--rw-r--r--   0 runner    (1001) docker     (123)    36761 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCAtomDB.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9809 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCAtomDBExtender.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCAtomData.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCAtomUtils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCBkgdExtCurve.cc
--rw-r--r--   0 runner    (1001) docker     (123)    18374 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCCfgManip.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCCfgTypes.cc
--rw-r--r--   0 runner    (1001) docker     (123)    17901 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCCfgVars.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCCompositionUtils.cc
--rw-r--r--   0 runner    (1001) docker     (123)    26184 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCDataSources.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCDebyeMSD.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCDefs.cc
--rw-r--r--   0 runner    (1001) docker     (123)    19704 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCDump.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCDynInfoUtils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCDynLoader.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCElIncScatter.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCElIncXS.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCEqRefl.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCException.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFact.cc
--rw-r--r--   0 runner    (1001) docker     (123)    42888 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFactImpl.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFactRequests.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFactTypes.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFactoryUtils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFactory_NCMAT.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFastConvolve.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFileUtils.cc
--rw-r--r--   0 runner    (1001) docker     (123)    30178 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFillHKL.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFmt.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFreeGas.cc
--rw-r--r--   0 runner    (1001) docker     (123)    39971 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFreeGasUtils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCGasMixFact.cc
--rw-r--r--   0 runner    (1001) docker     (123)    26599 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCGasMixUtils.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCGaussMos.cc
--rw-r--r--   0 runner    (1001) docker     (123)    20586 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCGaussOnSphere.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12554 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCInfo.cc
--rw-r--r--   0 runner    (1001) docker     (123)    57518 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCInfoBuilder.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCIofQHelper.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCKinUtils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCLCBragg.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCLCRefModels.cc
--rw-r--r--   0 runner    (1001) docker     (123)    32322 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCLCUtils.cc
--rw-r--r--   0 runner    (1001) docker     (123)    19509 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCLatticeUtils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCLauLazyFact.cc
--rw-r--r--   0 runner    (1001) docker     (123)    30601 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCLazy.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCLazy.hh
--rw-r--r--   0 runner    (1001) docker     (123)    33272 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCLoadNCMAT.cc
--rw-r--r--   0 runner    (1001) docker     (123)    48483 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCMatCfg.cc
--rw-r--r--   0 runner    (1001) docker     (123)    23835 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCMath.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCMatrix.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCMem.cc
--rw-r--r--   0 runner    (1001) docker     (123)    31787 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCNCMATData.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCOrientUtils.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCPCBragg.cc
--rw-r--r--   0 runner    (1001) docker     (123)    42614 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCParseNCMAT.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCPlaneProvider.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCPluginMgmt.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCPointwiseDist.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCProc.cc
--rw-r--r--   0 runner    (1001) docker     (123)    20199 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCProcImpl.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCQuickFact.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCRNG.cc
--rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCRandUtils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCRomberg.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCRotMatrix.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABData.cc
--rw-r--r--   0 runner    (1001) docker     (123)    31885 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABEval.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABExtender.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABFactory.cc
--rw-r--r--   0 runner    (1001) docker     (123)    23449 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABIntegrator.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABSampler.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12421 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABSamplerModels.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABScatter.cc
--rw-r--r--   0 runner    (1001) docker     (123)    26306 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABUCN.cc
--rw-r--r--   0 runner    (1001) docker     (123)    26746 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABUtils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABXSProvider.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSANSFact.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSANSSphScat.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSANSUtils.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSCBragg.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSCOrientation.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCScatKnlData.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSpline.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCStdAbsFact.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCStdMPScatFact.cc
--rw-r--r--   0 runner    (1001) docker     (123)    18990 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCStdScatFact.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCStrView.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCString.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCTDProd.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCTextData.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCTypes.cc
--rw-r--r--   0 runner    (1001) docker     (123)    25936 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCVDOSEval.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15041 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCVDOSGn.cc
--rw-r--r--   0 runner    (1001) docker     (123)    38631 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCVDOSToScatKnl.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCVector.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCVersion.cc
--rw-r--r--   0 runner    (1001) docker     (123)    72731 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/ncrystal.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.440544 ncrystal-3.6.dev82/ncrystal_geant4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.440544 ncrystal-3.6.dev82/ncrystal_geant4/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.492546 ncrystal-3.6.dev82/ncrystal_geant4/include/G4NCrystal/
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_geant4/include/G4NCrystal/G4NCInstall.hh
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_geant4/include/G4NCrystal/G4NCManager.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_geant4/include/G4NCrystal/G4NCMatHelper.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_geant4/include/G4NCrystal/G4NCrystal.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.492546 ncrystal-3.6.dev82/ncrystal_geant4/src/
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCInstall.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCManager.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15023 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCMatHelper.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCProcWrapper.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCProcWrapper.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.492546 ncrystal-3.6.dev82/ncrystal_mcstas/
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_mcstas/NCrystal_example.instr
--rw-r--r--   0 runner    (1001) docker     (123)    16072 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_mcstas/NCrystal_sample.comp
--rwxr-xr-x   0 runner    (1001) docker     (123)     5054 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_mcstas/ncrystal_preparemcstasdir
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.492546 ncrystal-3.6.dev82/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)    15960 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/ncrystal_cif2ncmat
--rwxr-xr-x   0 runner    (1001) docker     (123)    35171 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/ncrystal_endf2ncmat
--rwxr-xr-x   0 runner    (1001) docker     (123)    73858 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/ncrystal_hfg2ncmat
--rwxr-xr-x   0 runner    (1001) docker     (123)    35971 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/ncrystal_inspectfile
--rwxr-xr-x   0 runner    (1001) docker     (123)    15231 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/ncrystal_ncmat2cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     7659 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/ncrystal_ncmat2hkl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1998 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/ncrystal_onlinedb2ncmat
--rwxr-xr-x   0 runner    (1001) docker     (123)    20289 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/ncrystal_vdos2ncmat
--rwxr-xr-x   0 runner    (1001) docker     (123)    13315 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/ncrystal_verifyatompos
--rwxr-xr-x   0 runner    (1001) docker     (123)    35971 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/nctool
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 18:10:46.492546 ncrystal-3.6.dev82/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:21.094487 ncrystal-3.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:20.986486 ncrystal-3.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:20.994486 ncrystal-3.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-14 17:26:02.000000 ncrystal-3.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-14 17:26:02.000000 ncrystal-3.7.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-14 17:26:02.000000 ncrystal-3.7.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-14 17:26:02.000000 ncrystal-3.7.0/.github/ISSUE_TEMPLATE/request-for-new-material.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:20.994486 ncrystal-3.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-14 17:26:02.000000 ncrystal-3.7.0/.github/workflows/cmake.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-14 17:26:02.000000 ncrystal-3.7.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-14 17:26:02.000000 ncrystal-3.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    80071 2023-07-14 17:26:02.000000 ncrystal-3.7.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)    35343 2023-07-14 17:26:02.000000 ncrystal-3.7.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-14 17:26:02.000000 ncrystal-3.7.0/FILES
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-14 17:26:02.000000 ncrystal-3.7.0/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-07-14 17:26:02.000000 ncrystal-3.7.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:20.998486 ncrystal-3.7.0/NCrystal/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40112 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/_chooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/_coreimpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16356 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/_miscimpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85698 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/_ncmatimpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25999 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/_testimpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/atomdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/cfgstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74600 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/cifutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74942 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/datasrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/mcstasutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11032 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38896 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/ncmat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/obsolete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45843 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NCrystal/vdos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-14 17:26:02.000000 ncrystal-3.7.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-14 17:26:21.094487 ncrystal-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-07-14 17:26:02.000000 ncrystal-3.7.0/README
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 17:26:02.000000 ncrystal-3.7.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:20.998486 ncrystal-3.7.0/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-07-14 17:26:02.000000 ncrystal-3.7.0/cmake/NCrystalConfig.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:20.998486 ncrystal-3.7.0/cmake/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-07-14 17:26:02.000000 ncrystal-3.7.0/cmake/modules/ncrystal_legacyoptions.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-14 17:26:02.000000 ncrystal-3.7.0/cmake/modules/ncrystal_options.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-14 17:26:02.000000 ncrystal-3.7.0/cmake/modules/ncrystal_utils.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-07-14 17:26:02.000000 ncrystal-3.7.0/cmake/ncrystal-config.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-14 17:26:02.000000 ncrystal-3.7.0/cmake/template_setup.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-14 17:26:02.000000 ncrystal-3.7.0/cmake/template_setup.sh.in
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-14 17:26:02.000000 ncrystal-3.7.0/cmake/template_unsetup.sh.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:21.034486 ncrystal-3.7.0/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/AcrylicGlass_C5O2H8.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/AgBr_sg225_SilverBromide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Ag_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Al2O3_sg167_Corundum.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Al4C3_sg166_AluminiumCarbide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/AlN_sg186_AluminumNitride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Al_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Ar_Gas_STP.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Au_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/BaF2_sg225_BariumFluoride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/BaO_sg225_BariumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Ba_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Be3N2_sg206_BerylliumNitride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/BeF2_sg152_Beryllium_Fluoride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/BeO_sg186.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Be_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Bi_sg166.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/C_sg194_pyrolytic_graphite.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/C_sg227_Diamond.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/CaCO3_sg62_Aragonite.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/CaF2_sg225_CalciumFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/CaH2_sg62_CalciumHydride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/CaO2H2_sg164_CalciumHydroxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/CaO_sg225_CalciumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/CaSiO3_sg2_Wollastonite.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Ca_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Ca_sg229_Calcium-gamma.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/CeO2_sg225_CeriumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Cr_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Cu2O_sg224_Cuprite.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Cu_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Dy2O3_sg206_DysprosiumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Epoxy_Araldite506_C18H20O3.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Fe_sg225_Iron-gamma.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Fe_sg229_Iron-alpha.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/GaN_sg186_GalliumNitride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/GaSe_sg194_GalliumSelenide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Ge3Bi4O12_sg220_BismuthGermanate.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Ge_sg227.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/He_Gas_STP.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/HfO2_sg14_HafniumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Ho2O3_sg206_HolmiumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/KBr_sg225_PotassiumBromide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/KF_sg225_PotassiumFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/KOH_sg4_PotassiumHydroxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/K_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Kapton_C22H10N2O5.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Kr_Gas_STP.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/LaBr3_sg176_LanthanumBromide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Li2O_sg225_LithiumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Li3N_sg191_LithiumNitride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/LiF_sg225_LithiumFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/LiH_sg225_LithiumHydride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)  1560968 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/LiquidHeavyWaterD2O_T293.6K.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)   528493 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/LiquidWaterH2O_T293.6K.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Lu2O3_sg206_LutetiumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Lu2SiO5_sg15.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Mg2SiO4_sg62_MagnesiumSilicate.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/MgAl2O4_sg227_MAS.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/MgCO3_sg167_MagnesiumCarbonate.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/MgD2_sg136_MagnesiumDeuteride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/MgF2_sg136_MagnesiumFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/MgH2_sg136_MagnesiumHydride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/MgO2H2_sg164_MagnesiumHydroxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/MgO_sg225_Periclase.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Mg_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Mo_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Na4Si3Al3O12Cl_sg218_Sodalite.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/NaBr_sg225_SodiumBromide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/NaCl_sg225_SodiumChloride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/NaF_sg225_SodiumFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/NaI_sg225_SodiumIodide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Na_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Nb_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Ne_Gas_STP.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Ni_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Nylon11_C11H21NO.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Nylon12_C12H23NO.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Nylon610_C16H30N2O2.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Nylon66or6_C12H22N2O2.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/PEEK_C19H12O3.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/PVC_C2H3Cl.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/PbF2-beta_sg225_BetaLeadFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/PbO-alpha_sg129_Litharge.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/PbO-beta_sg57_Massicot.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/PbS_sg225_LeadSulfide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Pb_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Pd_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Polycarbonate_C16O3H14.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Polyester_C10H8O4.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Polyethylene_CH2.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Polylactide_C3H4O2.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Polypropylene_C3H6.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Polystyrene_C8H8.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Pt_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Rb_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Rubber_C5H8.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Sc_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/SiC-beta_sg216_BetaSiliconCarbide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/SiO2-alpha_sg154_AlphaQuartz.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/SiO2-beta_sg180_BetaQuartz.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Si_sg227.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Sn_sg141.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/SrF2_sg225_StrontiumFluoride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/SrH2_sg62_StrontiumHydride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Sr_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Th3N4_sg166_ThoriumNitride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/ThO2_sg225_ThoriumDioxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Th_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/TiO2_sg136_Rutile.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/TiO2_sg141_Anatase.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Ti_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/TlBr_sg221_ThaliumBromide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Tm2O3_sg206_ThuliumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/UF6_sg62_UraniumHexaflouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/UO2_sg225_UraniumDioxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/V_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/W_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Xe_Gas_STP.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Y2O3_sg206_Yttrium_Oxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Y2SiO5_sg15_YSO.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Y3Al5O12_sg230_YAG.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Y_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/ZnF2_sg136_ZincFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/ZnO_sg186_ZincOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/ZnS_sg216_Sphalerite.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Zn_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/ZrF4-beta_sg84.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/ZrO2_sg137_Zirconia.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/ZrO2_sg14_Zirconia.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/Zr_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-14 17:26:02.000000 ncrystal-3.7.0/data/void.ncmat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:21.034486 ncrystal-3.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    39216 2023-07-14 17:26:02.000000 ncrystal-3.7.0/docs/ncmat_doc.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:21.038486 ncrystal-3.7.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-14 17:26:02.000000 ncrystal-3.7.0/examples/NCrystal_example_mcstas.instr
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-14 17:26:02.000000 ncrystal-3.7.0/examples/ncrystal_example_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-14 17:26:02.000000 ncrystal-3.7.0/examples/ncrystal_example_cpp.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-07-14 17:26:02.000000 ncrystal-3.7.0/examples/ncrystal_example_customphysics.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-14 17:26:02.000000 ncrystal-3.7.0/examples/ncrystal_example_g4sim.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-14 17:26:02.000000 ncrystal-3.7.0/examples/ncrystal_example_py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:21.038486 ncrystal-3.7.0/ncrystal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-14 17:26:20.000000 ncrystal-3.7.0/ncrystal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14431 2023-07-14 17:26:20.000000 ncrystal-3.7.0/ncrystal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:26:20.000000 ncrystal-3.7.0/ncrystal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 17:26:20.000000 ncrystal-3.7.0/ncrystal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 17:26:20.000000 ncrystal-3.7.0/ncrystal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:20.986486 ncrystal-3.7.0/ncrystal_core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:20.986486 ncrystal-3.7.0/ncrystal_core/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:21.050486 ncrystal-3.7.0/ncrystal_core/include/NCrystal/
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCAtomData.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCCompositionUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCDataSources.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCDefs.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCDump.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCException.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCFact.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCFactImpl.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCFactRequests.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCFactTypes.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCFmt.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    16597 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCImmutBuf.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    28964 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCInfo.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCInfoBuilder.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCInfoTypes.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCLoadNCMAT.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    22448 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCMatCfg.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    20439 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCMem.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCNCMATData.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCParseNCMAT.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCPluginBoilerplate.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCPluginMgmt.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCProc.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCProcImpl.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCRNG.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCSABData.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCSCOrientation.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    39147 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCSmallVector.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    14618 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCTextData.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    37486 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCTypes.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    13171 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCVariant.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCVersion.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCrystal.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:21.066487 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCAbsOOV.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCAtomDB.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCAtomDBExtender.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCAtomUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCBkgdExtCurve.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    23020 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCCfgManip.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    32290 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCCfgTypes.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    35719 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCCfgVars.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCDebyeMSD.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCDynInfoUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCDynLoader.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCElIncScatter.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCElIncXS.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCEqRefl.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    19986 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCFactoryUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCFastConvolve.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCFileUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCFillHKL.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCFreeGas.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCFreeGasUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCGasMixUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCGaussMos.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCGaussOnSphere.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCIofQHelper.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCIter.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCKinUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCLCBragg.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCLCRefModels.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCLCUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCLatticeUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    27371 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCMath.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCMatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCOrientUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCPCBragg.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCPlaneProvider.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCPointwiseDist.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCRandUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCRomberg.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCRotMatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABEval.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABExtender.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABFactory.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABIntegrator.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABSampler.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABSamplerModels.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABScatter.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABScatterHelper.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABUCN.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABXSProvider.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSANSSphScat.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSANSUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSCBragg.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCScatKnlData.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSpan.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSpline.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    20113 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCStrView.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    15426 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCString.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCVDOSEval.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCVDOSGn.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCVDOSToScatKnl.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCVector.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/ncapi.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44876 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/include/NCrystal/ncrystal.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:21.090487 ncrystal-3.7.0/ncrystal_core/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCAbsOOV.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    36761 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCAtomDB.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9809 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCAtomDBExtender.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCAtomData.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCAtomUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCBkgdExtCurve.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    18374 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCCfgManip.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCCfgTypes.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    17901 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCCfgVars.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCCompositionUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    26184 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCDataSources.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCDebyeMSD.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCDefs.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    19704 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCDump.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCDynInfoUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCDynLoader.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCElIncScatter.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCElIncXS.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCEqRefl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCException.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCFact.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    42888 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCFactImpl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCFactRequests.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCFactTypes.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCFactoryUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCFactory_NCMAT.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCFastConvolve.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCFileUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    30178 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCFillHKL.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCFmt.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCFreeGas.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    39971 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCFreeGasUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCGasMixFact.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    26599 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCGasMixUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCGaussMos.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    20586 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCGaussOnSphere.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12554 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCInfo.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    57518 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCInfoBuilder.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCIofQHelper.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCKinUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCLCBragg.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCLCRefModels.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    32322 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCLCUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    19509 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCLatticeUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCLauLazyFact.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    30601 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCLazy.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCLazy.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    33272 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCLoadNCMAT.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    48483 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCMatCfg.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23835 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCMath.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCMatrix.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCMem.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    31787 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCNCMATData.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCOrientUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCPCBragg.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    42614 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCParseNCMAT.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCPlaneProvider.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCPluginMgmt.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCPointwiseDist.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCProc.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    20199 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCProcImpl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCQuickFact.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCRNG.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCRandUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCRomberg.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCRotMatrix.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCSABData.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    31885 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCSABEval.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCSABExtender.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCSABFactory.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23449 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCSABIntegrator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCSABSampler.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12421 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCSABSamplerModels.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCSABScatter.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    26306 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCSABUCN.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    26746 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCSABUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCSABXSProvider.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCSANSFact.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCSANSSphScat.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCSANSUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCSCBragg.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCSCOrientation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCScatKnlData.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCSpline.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCStdAbsFact.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCStdMPScatFact.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    18990 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCStdScatFact.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCStrView.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCString.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCTDProd.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCTextData.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCTypes.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    25936 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCVDOSEval.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15041 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCVDOSGn.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    38631 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCVDOSToScatKnl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCVector.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/NCVersion.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    72731 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_core/src/ncrystal.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:20.990486 ncrystal-3.7.0/ncrystal_geant4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:20.986486 ncrystal-3.7.0/ncrystal_geant4/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:21.090487 ncrystal-3.7.0/ncrystal_geant4/include/G4NCrystal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_geant4/include/G4NCrystal/G4NCInstall.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_geant4/include/G4NCrystal/G4NCManager.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_geant4/include/G4NCrystal/G4NCMatHelper.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_geant4/include/G4NCrystal/G4NCrystal.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:21.090487 ncrystal-3.7.0/ncrystal_geant4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_geant4/src/G4NCInstall.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_geant4/src/G4NCManager.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15023 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_geant4/src/G4NCMatHelper.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_geant4/src/G4NCProcWrapper.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_geant4/src/G4NCProcWrapper.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:21.090487 ncrystal-3.7.0/ncrystal_mcstas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_mcstas/NCrystal_example.instr
+-rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_mcstas/NCrystal_sample.comp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5054 2023-07-14 17:26:02.000000 ncrystal-3.7.0/ncrystal_mcstas/ncrystal_preparemcstasdir
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-14 17:26:02.000000 ncrystal-3.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:26:21.094487 ncrystal-3.7.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15960 2023-07-14 17:26:02.000000 ncrystal-3.7.0/scripts/ncrystal_cif2ncmat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35171 2023-07-14 17:26:02.000000 ncrystal-3.7.0/scripts/ncrystal_endf2ncmat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    73858 2023-07-14 17:26:02.000000 ncrystal-3.7.0/scripts/ncrystal_hfg2ncmat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35971 2023-07-14 17:26:02.000000 ncrystal-3.7.0/scripts/ncrystal_inspectfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15231 2023-07-14 17:26:02.000000 ncrystal-3.7.0/scripts/ncrystal_ncmat2cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7659 2023-07-14 17:26:02.000000 ncrystal-3.7.0/scripts/ncrystal_ncmat2hkl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1998 2023-07-14 17:26:02.000000 ncrystal-3.7.0/scripts/ncrystal_onlinedb2ncmat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20289 2023-07-14 17:26:02.000000 ncrystal-3.7.0/scripts/ncrystal_vdos2ncmat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13315 2023-07-14 17:26:02.000000 ncrystal-3.7.0/scripts/ncrystal_verifyatompos
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35971 2023-07-14 17:26:02.000000 ncrystal-3.7.0/scripts/nctool
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:26:21.094487 ncrystal-3.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-14 17:26:02.000000 ncrystal-3.7.0/setup.py
```

### Comparing `ncrystal-3.6.dev82/.github/ISSUE_TEMPLATE/feature_request.md` & `ncrystal-3.7.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/.github/ISSUE_TEMPLATE/request-for-new-material.md` & `ncrystal-3.7.0/.github/ISSUE_TEMPLATE/request-for-new-material.md`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/.github/workflows/cmake.yml` & `ncrystal-3.7.0/.github/workflows/cmake.yml`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/CHANGELOG` & `ncrystal-3.7.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,54 @@
+v3.7.0 2023-07-14
+      * The main feature of this release is that NCrystal now can be optionally
+        built and installed using standard Python-centric toolchains. Work on
+        this feature was spearheaded by Milan Klausz, and is associated with
+        newly added setup.py and pyproject.toml files, using skbuild behind the
+        scenes. Additionally, Python modules and script were moved out of the
+        ncrystal_python directory and into directories named NCrystal and
+        scripts, respectively (solving github issue #127). Finally, existing
+        Python modules and the ncrystal-config script were modified to support
+        such builds and installation. As a result, it is now possible to do "pip
+        install <path-to-ncrystal-src>", and get a fully-fledged NCrystal
+        release. The only difference with respect to e.g. a conda installation
+        of NCrystal, is that downstream CMake-based projecs won't detect the
+        installation, unless the directory reported by "ncrystal-config --show
+        cmakedir" is manually added to the CMAKE_PREFIX_PATH.
+      * Work is ongoing by Milan Klausz to setup workflows at GitHUB to
+        automatically build binary wheels for PyPI, similar to how binary
+        packages are now built automatically at conda-forge. Once this is
+        completed, it will be possible to install prebuilt NCrystal packages via
+        "pip install ncrystal" (solving github issue #93).
+      * Note that setup.py maps NCrystal releases with minor number >= 80 to a
+        development version lke "3.6.dev80", with the intention of preventing
+        "pip install ncrystal" from automatically picking up release candidates.
+      * Rewrote the aligned allocator code used internally when implementing
+        convenience containers such as SmallVector. This was done in response to
+        fix compilation errors with gcc12 (github issue #125). This new version
+        avoid the previous incorrect reliance of a non-standard feature of
+        std::free, and overall the new version is more portable, as it relies on
+        nothing except std::malloc and std::free.
+      * Updated the SmallVector::clear method, in order to work around what
+        appears to be a false-positive compilation error by gcc12.
+      * For completeness, added more functions like ekin2k, constexpr_ekin2k,
+        k2ekin, and k2wl functions in the C++ and Python API's.
+      * Bugfixes (C++ API): NeutronEnergy::k() now actually returns the
+        wavenumber k, and not the squared of k, as it did previously. Also, the
+        free-standing ekin2wl(..) function is no longer constexpr (since
+        std::sqrt is not actually constexpr), but there is a new
+        constexpr_ekin2wl which is.
+      * Added new standard testing facilities, for checking an installation for
+        presence of commandline scripts (solving github issue #110) and that
+        downstream CMake/C++ projects can find and use NCrystal (after getting
+        CMAKE_PREFIX_PATH from ncrystal-config). To invoke all tests, run
+        "python3 -mNCrystal.test all". For other options, run "python3
+        -mNCrystal.test all".
+      * Add ncrystal_setup.sh/ncrystal_unsetup.sh files in addition to the
+        ambiguously named setup.sh/unsetup.sh files. (github issue #126).
+
 v3.6.82 2023-07-13
       * RC3 for release 3.7.0.
 
 v3.6.81 2023-06-23
       * RC2 for release 3.7.0.
 
 v3.6.80 2023-06-07
```

### Comparing `ncrystal-3.6.dev82/CMakeLists.txt` & `ncrystal-3.7.0/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 list( APPEND _project_metadata DESCRIPTION "Library for thermal neutron transport in crystals and other materials" )
 if( "${CMAKE_VERSION}" VERSION_GREATER_EQUAL "3.12.0" )
   list( APPEND _project_metadata HOMEPAGE_URL "https://github.com/mctools/ncrystal" )
 endif()
 
 cmake_policy( SET CMP0048 NEW )#Not sure if this is really needed
 
-project( NCrystal VERSION 3.6.82 ${_project_metadata} )
+project( NCrystal VERSION 3.7.0 ${_project_metadata} )
 
 unset( _project_metadata )
 
 if( NOT NCRYSTAL_NOTOUCH_CMAKE_BUILD_TYPE )
   if ( NOT gen_is_multicfg )
     if ( NOT CMAKE_BUILD_TYPE )
       #This can happen if parent project called the project(..) function before
```

### Comparing `ncrystal-3.6.dev82/FILES` & `ncrystal-3.7.0/FILES`

 * *Files 20% similar despite different names*

```diff
@@ -30,8 +30,10 @@
                       and a script to prepare a given McStas rundir for using it.
 NCrystal/...........: NCrystal python modules.
 scripts/............: Command-line scripts, including the nctool command and
                       various tools for NCMAT file preparation.
 docs/...............: Extra documentation. Currently this is just ncmat_doc.md
                       with a thorough description of the NCMAT format.
 cmake/..............: Other files needed for CMake configuration.
-
+setup.py............: Support building and installing via standard Python
+                      tool-chains.
+pyproject.toml......: Like setup.py, needed for the standard Python tool-chains.
```

### Comparing `ncrystal-3.6.dev82/INSTALL` & `ncrystal-3.7.0/INSTALL`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/LICENSE` & `ncrystal-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/__init__.py` & `ncrystal-3.7.0/NCrystal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 ##  See the License for the specific language governing permissions and       ##
 ##  limitations under the License.                                            ##
 ##                                                                            ##
 ################################################################################
 
 #NB: Synchronize meta-data below with fields in setup.py+template_setup.py.in meta data:
 __license__ = "Apache 2.0, http://www.apache.org/licenses/LICENSE-2.0"
-__version__ = '3.6.82'
+__version__ = '3.7.0'
 __status__ = "Production"
 __author__ = "NCrystal developers (Thomas Kittelmann, Xiao Xiao Cai)"
 __copyright__ = "Copyright 2015-2023 %s"%__author__
 __maintainer__ = __author__
 __email__ = "ncrystal-developers@cern.ch"
 
 #Place f-string here to catch python <3.6 in a more obvious way than a syntax error below:
```

### Comparing `ncrystal-3.6.dev82/NCrystal/_chooks.py` & `ncrystal-3.7.0/NCrystal/_chooks.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/_common.py` & `ncrystal-3.7.0/NCrystal/_common.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/_coreimpl.py` & `ncrystal-3.7.0/NCrystal/_coreimpl.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/_miscimpl.py` & `ncrystal-3.7.0/NCrystal/_miscimpl.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/_ncmatimpl.py` & `ncrystal-3.7.0/NCrystal/_ncmatimpl.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/_numpy.py` & `ncrystal-3.7.0/NCrystal/_numpy.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/_testimpl.py` & `ncrystal-3.7.0/NCrystal/_testimpl.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/api.py` & `ncrystal-3.7.0/NCrystal/api.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/atomdata.py` & `ncrystal-3.7.0/NCrystal/atomdata.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/cfgstr.py` & `ncrystal-3.7.0/NCrystal/cfgstr.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/cifutils.py` & `ncrystal-3.7.0/NCrystal/cifutils.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/constants.py` & `ncrystal-3.7.0/NCrystal/constants.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/core.py` & `ncrystal-3.7.0/NCrystal/core.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/datasrc.py` & `ncrystal-3.7.0/NCrystal/datasrc.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/exceptions.py` & `ncrystal-3.7.0/NCrystal/exceptions.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/mcstasutils.py` & `ncrystal-3.7.0/NCrystal/mcstasutils.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/misc.py` & `ncrystal-3.7.0/NCrystal/misc.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/ncmat.py` & `ncrystal-3.7.0/NCrystal/ncmat.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/obsolete.py` & `ncrystal-3.7.0/NCrystal/obsolete.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/plot.py` & `ncrystal-3.7.0/NCrystal/plot.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/plugins.py` & `ncrystal-3.7.0/NCrystal/plugins.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/test.py` & `ncrystal-3.7.0/NCrystal/test.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NCrystal/vdos.py` & `ncrystal-3.7.0/NCrystal/vdos.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/NOTICE` & `ncrystal-3.7.0/NOTICE`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/PKG-INFO` & `ncrystal-3.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncrystal
-Version: 3.6.dev82
+Version: 3.7.0
 Summary: Library for thermal neutron transport in crystals and other materials.
 Home-page: https://github.com/mctools/ncrystal/wiki
 Author: NCrystal developers (Thomas Kittelmann, Xiao Xiao Cai)
 License: Apache-2.0
 Keywords: neutron,montecarlo,science
 Requires-Python: >=3.6, <4
 License-File: LICENSE
```

### Comparing `ncrystal-3.6.dev82/README` & `ncrystal-3.7.0/README`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/cmake/NCrystalConfig.cmake.in` & `ncrystal-3.7.0/cmake/NCrystalConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/cmake/modules/ncrystal_legacyoptions.cmake` & `ncrystal-3.7.0/cmake/modules/ncrystal_legacyoptions.cmake`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/cmake/modules/ncrystal_options.cmake` & `ncrystal-3.7.0/cmake/modules/ncrystal_options.cmake`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/cmake/modules/ncrystal_utils.cmake` & `ncrystal-3.7.0/cmake/modules/ncrystal_utils.cmake`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/cmake/ncrystal-config.in` & `ncrystal-3.7.0/cmake/ncrystal-config.in`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/cmake/template_setup.py.in` & `ncrystal-3.7.0/cmake/template_setup.py.in`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/cmake/template_setup.sh.in` & `ncrystal-3.7.0/cmake/template_setup.sh.in`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/cmake/template_unsetup.sh.in` & `ncrystal-3.7.0/cmake/template_unsetup.sh.in`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/AcrylicGlass_C5O2H8.ncmat` & `ncrystal-3.7.0/data/AcrylicGlass_C5O2H8.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/AgBr_sg225_SilverBromide.ncmat` & `ncrystal-3.7.0/data/AgBr_sg225_SilverBromide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Ag_sg225.ncmat` & `ncrystal-3.7.0/data/Ag_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Al2O3_sg167_Corundum.ncmat` & `ncrystal-3.7.0/data/Al2O3_sg167_Corundum.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Al4C3_sg166_AluminiumCarbide.ncmat` & `ncrystal-3.7.0/data/Al4C3_sg166_AluminiumCarbide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/AlN_sg186_AluminumNitride.ncmat` & `ncrystal-3.7.0/data/AlN_sg186_AluminumNitride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Al_sg225.ncmat` & `ncrystal-3.7.0/data/Al_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Ar_Gas_STP.ncmat` & `ncrystal-3.7.0/data/Ar_Gas_STP.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Au_sg225.ncmat` & `ncrystal-3.7.0/data/Au_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/BaF2_sg225_BariumFluoride.ncmat` & `ncrystal-3.7.0/data/BaF2_sg225_BariumFluoride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/BaO_sg225_BariumOxide.ncmat` & `ncrystal-3.7.0/data/BaO_sg225_BariumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Ba_sg229.ncmat` & `ncrystal-3.7.0/data/Ba_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Be3N2_sg206_BerylliumNitride.ncmat` & `ncrystal-3.7.0/data/Be3N2_sg206_BerylliumNitride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/BeF2_sg152_Beryllium_Fluoride.ncmat` & `ncrystal-3.7.0/data/BeF2_sg152_Beryllium_Fluoride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/BeO_sg186.ncmat` & `ncrystal-3.7.0/data/BeO_sg186.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Be_sg194.ncmat` & `ncrystal-3.7.0/data/Be_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Bi_sg166.ncmat` & `ncrystal-3.7.0/data/Bi_sg166.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/C_sg194_pyrolytic_graphite.ncmat` & `ncrystal-3.7.0/data/C_sg194_pyrolytic_graphite.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/C_sg227_Diamond.ncmat` & `ncrystal-3.7.0/data/C_sg227_Diamond.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/CaCO3_sg62_Aragonite.ncmat` & `ncrystal-3.7.0/data/CaCO3_sg62_Aragonite.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/CaF2_sg225_CalciumFlouride.ncmat` & `ncrystal-3.7.0/data/CaF2_sg225_CalciumFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/CaH2_sg62_CalciumHydride.ncmat` & `ncrystal-3.7.0/data/CaH2_sg62_CalciumHydride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/CaO2H2_sg164_CalciumHydroxide.ncmat` & `ncrystal-3.7.0/data/CaO2H2_sg164_CalciumHydroxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/CaO_sg225_CalciumOxide.ncmat` & `ncrystal-3.7.0/data/CaO_sg225_CalciumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/CaSiO3_sg2_Wollastonite.ncmat` & `ncrystal-3.7.0/data/CaSiO3_sg2_Wollastonite.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Ca_sg225.ncmat` & `ncrystal-3.7.0/data/Ca_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Ca_sg229_Calcium-gamma.ncmat` & `ncrystal-3.7.0/data/Ca_sg229_Calcium-gamma.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/CeO2_sg225_CeriumOxide.ncmat` & `ncrystal-3.7.0/data/CeO2_sg225_CeriumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Cr_sg229.ncmat` & `ncrystal-3.7.0/data/Cr_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Cu2O_sg224_Cuprite.ncmat` & `ncrystal-3.7.0/data/Cu2O_sg224_Cuprite.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Cu_sg225.ncmat` & `ncrystal-3.7.0/data/Cu_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Dy2O3_sg206_DysprosiumOxide.ncmat` & `ncrystal-3.7.0/data/Dy2O3_sg206_DysprosiumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Epoxy_Araldite506_C18H20O3.ncmat` & `ncrystal-3.7.0/data/Epoxy_Araldite506_C18H20O3.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Fe_sg225_Iron-gamma.ncmat` & `ncrystal-3.7.0/data/Fe_sg225_Iron-gamma.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Fe_sg229_Iron-alpha.ncmat` & `ncrystal-3.7.0/data/Fe_sg229_Iron-alpha.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/GaN_sg186_GalliumNitride.ncmat` & `ncrystal-3.7.0/data/GaN_sg186_GalliumNitride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/GaSe_sg194_GalliumSelenide.ncmat` & `ncrystal-3.7.0/data/GaSe_sg194_GalliumSelenide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Ge3Bi4O12_sg220_BismuthGermanate.ncmat` & `ncrystal-3.7.0/data/Ge3Bi4O12_sg220_BismuthGermanate.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Ge_sg227.ncmat` & `ncrystal-3.7.0/data/Ge_sg227.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/He_Gas_STP.ncmat` & `ncrystal-3.7.0/data/He_Gas_STP.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/HfO2_sg14_HafniumOxide.ncmat` & `ncrystal-3.7.0/data/HfO2_sg14_HafniumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Ho2O3_sg206_HolmiumOxide.ncmat` & `ncrystal-3.7.0/data/Ho2O3_sg206_HolmiumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/KBr_sg225_PotassiumBromide.ncmat` & `ncrystal-3.7.0/data/KBr_sg225_PotassiumBromide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/KF_sg225_PotassiumFlouride.ncmat` & `ncrystal-3.7.0/data/KF_sg225_PotassiumFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/KOH_sg4_PotassiumHydroxide.ncmat` & `ncrystal-3.7.0/data/KOH_sg4_PotassiumHydroxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/K_sg229.ncmat` & `ncrystal-3.7.0/data/K_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Kapton_C22H10N2O5.ncmat` & `ncrystal-3.7.0/data/Kapton_C22H10N2O5.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Kr_Gas_STP.ncmat` & `ncrystal-3.7.0/data/Kr_Gas_STP.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/LaBr3_sg176_LanthanumBromide.ncmat` & `ncrystal-3.7.0/data/LaBr3_sg176_LanthanumBromide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Li2O_sg225_LithiumOxide.ncmat` & `ncrystal-3.7.0/data/Li2O_sg225_LithiumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Li3N_sg191_LithiumNitride.ncmat` & `ncrystal-3.7.0/data/Li3N_sg191_LithiumNitride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/LiF_sg225_LithiumFlouride.ncmat` & `ncrystal-3.7.0/data/LiF_sg225_LithiumFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/LiH_sg225_LithiumHydride.ncmat` & `ncrystal-3.7.0/data/LiH_sg225_LithiumHydride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/LiquidHeavyWaterD2O_T293.6K.ncmat` & `ncrystal-3.7.0/data/LiquidHeavyWaterD2O_T293.6K.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/LiquidWaterH2O_T293.6K.ncmat` & `ncrystal-3.7.0/data/LiquidWaterH2O_T293.6K.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Lu2O3_sg206_LutetiumOxide.ncmat` & `ncrystal-3.7.0/data/Lu2O3_sg206_LutetiumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Lu2SiO5_sg15.ncmat` & `ncrystal-3.7.0/data/Lu2SiO5_sg15.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Mg2SiO4_sg62_MagnesiumSilicate.ncmat` & `ncrystal-3.7.0/data/Mg2SiO4_sg62_MagnesiumSilicate.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/MgAl2O4_sg227_MAS.ncmat` & `ncrystal-3.7.0/data/MgAl2O4_sg227_MAS.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/MgCO3_sg167_MagnesiumCarbonate.ncmat` & `ncrystal-3.7.0/data/MgCO3_sg167_MagnesiumCarbonate.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/MgD2_sg136_MagnesiumDeuteride.ncmat` & `ncrystal-3.7.0/data/MgD2_sg136_MagnesiumDeuteride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/MgF2_sg136_MagnesiumFlouride.ncmat` & `ncrystal-3.7.0/data/MgF2_sg136_MagnesiumFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/MgH2_sg136_MagnesiumHydride.ncmat` & `ncrystal-3.7.0/data/MgH2_sg136_MagnesiumHydride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/MgO2H2_sg164_MagnesiumHydroxide.ncmat` & `ncrystal-3.7.0/data/MgO2H2_sg164_MagnesiumHydroxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/MgO_sg225_Periclase.ncmat` & `ncrystal-3.7.0/data/MgO_sg225_Periclase.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Mg_sg194.ncmat` & `ncrystal-3.7.0/data/Mg_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Mo_sg229.ncmat` & `ncrystal-3.7.0/data/Mo_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Na4Si3Al3O12Cl_sg218_Sodalite.ncmat` & `ncrystal-3.7.0/data/Na4Si3Al3O12Cl_sg218_Sodalite.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/NaBr_sg225_SodiumBromide.ncmat` & `ncrystal-3.7.0/data/NaBr_sg225_SodiumBromide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/NaCl_sg225_SodiumChloride.ncmat` & `ncrystal-3.7.0/data/NaCl_sg225_SodiumChloride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/NaF_sg225_SodiumFlouride.ncmat` & `ncrystal-3.7.0/data/NaF_sg225_SodiumFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/NaI_sg225_SodiumIodide.ncmat` & `ncrystal-3.7.0/data/NaI_sg225_SodiumIodide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Na_sg229.ncmat` & `ncrystal-3.7.0/data/Na_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Nb_sg229.ncmat` & `ncrystal-3.7.0/data/Nb_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Ne_Gas_STP.ncmat` & `ncrystal-3.7.0/data/Ne_Gas_STP.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Ni_sg225.ncmat` & `ncrystal-3.7.0/data/Ni_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Nylon11_C11H21NO.ncmat` & `ncrystal-3.7.0/data/Nylon11_C11H21NO.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Nylon12_C12H23NO.ncmat` & `ncrystal-3.7.0/data/Nylon12_C12H23NO.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Nylon610_C16H30N2O2.ncmat` & `ncrystal-3.7.0/data/Nylon610_C16H30N2O2.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Nylon66or6_C12H22N2O2.ncmat` & `ncrystal-3.7.0/data/Nylon66or6_C12H22N2O2.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/PEEK_C19H12O3.ncmat` & `ncrystal-3.7.0/data/PEEK_C19H12O3.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/PVC_C2H3Cl.ncmat` & `ncrystal-3.7.0/data/PVC_C2H3Cl.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/PbF2-beta_sg225_BetaLeadFlouride.ncmat` & `ncrystal-3.7.0/data/PbF2-beta_sg225_BetaLeadFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/PbO-alpha_sg129_Litharge.ncmat` & `ncrystal-3.7.0/data/PbO-alpha_sg129_Litharge.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/PbO-beta_sg57_Massicot.ncmat` & `ncrystal-3.7.0/data/PbO-beta_sg57_Massicot.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/PbS_sg225_LeadSulfide.ncmat` & `ncrystal-3.7.0/data/PbS_sg225_LeadSulfide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Pb_sg225.ncmat` & `ncrystal-3.7.0/data/Pb_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Pd_sg225.ncmat` & `ncrystal-3.7.0/data/Pd_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Polycarbonate_C16O3H14.ncmat` & `ncrystal-3.7.0/data/Polycarbonate_C16O3H14.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Polyester_C10H8O4.ncmat` & `ncrystal-3.7.0/data/Polyester_C10H8O4.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Polyethylene_CH2.ncmat` & `ncrystal-3.7.0/data/Polyethylene_CH2.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Polylactide_C3H4O2.ncmat` & `ncrystal-3.7.0/data/Polylactide_C3H4O2.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Polypropylene_C3H6.ncmat` & `ncrystal-3.7.0/data/Polypropylene_C3H6.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Polystyrene_C8H8.ncmat` & `ncrystal-3.7.0/data/Polystyrene_C8H8.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Pt_sg225.ncmat` & `ncrystal-3.7.0/data/Pt_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Rb_sg229.ncmat` & `ncrystal-3.7.0/data/Rb_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Rubber_C5H8.ncmat` & `ncrystal-3.7.0/data/Rubber_C5H8.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Sc_sg194.ncmat` & `ncrystal-3.7.0/data/Sc_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/SiC-beta_sg216_BetaSiliconCarbide.ncmat` & `ncrystal-3.7.0/data/SiC-beta_sg216_BetaSiliconCarbide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/SiO2-alpha_sg154_AlphaQuartz.ncmat` & `ncrystal-3.7.0/data/SiO2-alpha_sg154_AlphaQuartz.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/SiO2-beta_sg180_BetaQuartz.ncmat` & `ncrystal-3.7.0/data/SiO2-beta_sg180_BetaQuartz.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Si_sg227.ncmat` & `ncrystal-3.7.0/data/Si_sg227.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Sn_sg141.ncmat` & `ncrystal-3.7.0/data/Sn_sg141.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/SrF2_sg225_StrontiumFluoride.ncmat` & `ncrystal-3.7.0/data/SrF2_sg225_StrontiumFluoride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/SrH2_sg62_StrontiumHydride.ncmat` & `ncrystal-3.7.0/data/SrH2_sg62_StrontiumHydride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Sr_sg225.ncmat` & `ncrystal-3.7.0/data/Sr_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Th3N4_sg166_ThoriumNitride.ncmat` & `ncrystal-3.7.0/data/Th3N4_sg166_ThoriumNitride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/ThO2_sg225_ThoriumDioxide.ncmat` & `ncrystal-3.7.0/data/ThO2_sg225_ThoriumDioxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Th_sg225.ncmat` & `ncrystal-3.7.0/data/Th_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/TiO2_sg136_Rutile.ncmat` & `ncrystal-3.7.0/data/TiO2_sg136_Rutile.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/TiO2_sg141_Anatase.ncmat` & `ncrystal-3.7.0/data/TiO2_sg141_Anatase.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Ti_sg194.ncmat` & `ncrystal-3.7.0/data/Ti_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/TlBr_sg221_ThaliumBromide.ncmat` & `ncrystal-3.7.0/data/TlBr_sg221_ThaliumBromide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Tm2O3_sg206_ThuliumOxide.ncmat` & `ncrystal-3.7.0/data/Tm2O3_sg206_ThuliumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/UF6_sg62_UraniumHexaflouride.ncmat` & `ncrystal-3.7.0/data/UF6_sg62_UraniumHexaflouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/UO2_sg225_UraniumDioxide.ncmat` & `ncrystal-3.7.0/data/UO2_sg225_UraniumDioxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/V_sg229.ncmat` & `ncrystal-3.7.0/data/V_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/W_sg229.ncmat` & `ncrystal-3.7.0/data/W_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Xe_Gas_STP.ncmat` & `ncrystal-3.7.0/data/Xe_Gas_STP.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Y2O3_sg206_Yttrium_Oxide.ncmat` & `ncrystal-3.7.0/data/Y2O3_sg206_Yttrium_Oxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Y2SiO5_sg15_YSO.ncmat` & `ncrystal-3.7.0/data/Y2SiO5_sg15_YSO.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Y3Al5O12_sg230_YAG.ncmat` & `ncrystal-3.7.0/data/Y3Al5O12_sg230_YAG.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Y_sg194.ncmat` & `ncrystal-3.7.0/data/Y_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/ZnF2_sg136_ZincFlouride.ncmat` & `ncrystal-3.7.0/data/ZnF2_sg136_ZincFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/ZnO_sg186_ZincOxide.ncmat` & `ncrystal-3.7.0/data/ZnO_sg186_ZincOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/ZnS_sg216_Sphalerite.ncmat` & `ncrystal-3.7.0/data/ZnS_sg216_Sphalerite.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Zn_sg194.ncmat` & `ncrystal-3.7.0/data/Zn_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/ZrF4-beta_sg84.ncmat` & `ncrystal-3.7.0/data/ZrF4-beta_sg84.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/ZrO2_sg137_Zirconia.ncmat` & `ncrystal-3.7.0/data/ZrO2_sg137_Zirconia.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/ZrO2_sg14_Zirconia.ncmat` & `ncrystal-3.7.0/data/ZrO2_sg14_Zirconia.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/Zr_sg194.ncmat` & `ncrystal-3.7.0/data/Zr_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/data/void.ncmat` & `ncrystal-3.7.0/data/void.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/docs/ncmat_doc.md` & `ncrystal-3.7.0/docs/ncmat_doc.md`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/examples/NCrystal_example_mcstas.instr` & `ncrystal-3.7.0/examples/NCrystal_example_mcstas.instr`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/examples/ncrystal_example_c.c` & `ncrystal-3.7.0/examples/ncrystal_example_c.c`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/examples/ncrystal_example_cpp.cc` & `ncrystal-3.7.0/examples/ncrystal_example_cpp.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/examples/ncrystal_example_customphysics.cc` & `ncrystal-3.7.0/examples/ncrystal_example_customphysics.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/examples/ncrystal_example_g4sim.cc` & `ncrystal-3.7.0/examples/ncrystal_example_g4sim.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/examples/ncrystal_example_py` & `ncrystal-3.7.0/examples/ncrystal_example_py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal.egg-info/PKG-INFO` & `ncrystal-3.7.0/ncrystal.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncrystal
-Version: 3.6.dev82
+Version: 3.7.0
 Summary: Library for thermal neutron transport in crystals and other materials.
 Home-page: https://github.com/mctools/ncrystal/wiki
 Author: NCrystal developers (Thomas Kittelmann, Xiao Xiao Cai)
 License: Apache-2.0
 Keywords: neutron,montecarlo,science
 Requires-Python: >=3.6, <4
 License-File: LICENSE
```

### Comparing `ncrystal-3.6.dev82/ncrystal.egg-info/SOURCES.txt` & `ncrystal-3.7.0/ncrystal.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 pyproject.toml
 setup.py
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/request-for-new-material.md
 .github/workflows/cmake.yml
+.github/workflows/pypi.yml
 NCrystal/__init__.py
 NCrystal/_chooks.py
 NCrystal/_common.py
 NCrystal/_coreimpl.py
 NCrystal/_miscimpl.py
 NCrystal/_ncmatimpl.py
 NCrystal/_numpy.py
```

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCAtomData.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCAtomData.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCCompositionUtils.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCCompositionUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCDataSources.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCDataSources.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCDefs.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCDefs.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCDump.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCDump.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCException.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCException.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFact.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCFact.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFactImpl.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCFactImpl.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFactRequests.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCFactRequests.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFactTypes.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCFactTypes.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFmt.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCFmt.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCImmutBuf.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCImmutBuf.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCInfo.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCInfo.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCInfoBuilder.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCInfoBuilder.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCInfoTypes.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCInfoTypes.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCLoadNCMAT.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCLoadNCMAT.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCMatCfg.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCMatCfg.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCMem.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCMem.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCNCMATData.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCNCMATData.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCParseNCMAT.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCParseNCMAT.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCPluginBoilerplate.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCPluginBoilerplate.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCPluginMgmt.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCPluginMgmt.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCProc.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCProc.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCProcImpl.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCProcImpl.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCRNG.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCRNG.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCSABData.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCSABData.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCSCOrientation.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCSCOrientation.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCSmallVector.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCSmallVector.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCTextData.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCTextData.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCTypes.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCTypes.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCVariant.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCVariant.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCVersion.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCVersion.hh`

 * *Files 3% similar despite different names*

```diff
@@ -34,18 +34,18 @@
 #  undef NCRYSTAL_VERSION
 #endif
 #ifdef NCRYSTAL_VERSION_STR
 #  undef NCRYSTAL_VERSION_STR
 #endif
 
 #define NCRYSTAL_VERSION_MAJOR 3
-#define NCRYSTAL_VERSION_MINOR 6
-#define NCRYSTAL_VERSION_PATCH 82
-#define NCRYSTAL_VERSION   3006082 /* (1000000*MAJOR+1000*MINOR+PATCH)   */
-#define NCRYSTAL_VERSION_STR "3.6.82"
+#define NCRYSTAL_VERSION_MINOR 7
+#define NCRYSTAL_VERSION_PATCH 0
+#define NCRYSTAL_VERSION   3007000 /* (1000000*MAJOR+1000*MINOR+PATCH)   */
+#define NCRYSTAL_VERSION_STR "3.7.0"
 
 #include "NCrystal/ncapi.h"
 #include <stdexcept>
 
 namespace NCrystal {
 
   //Function which returns NCRYSTAL_VERSION. If it does not, it indicates symbol
```

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCrystal.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/NCrystal.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCAbsOOV.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCAbsOOV.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCAtomDB.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCAtomDB.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCAtomDBExtender.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCAtomDBExtender.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCAtomUtils.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCAtomUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCBkgdExtCurve.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCBkgdExtCurve.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCCfgManip.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCCfgManip.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCCfgTypes.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCCfgTypes.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCCfgVars.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCCfgVars.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCDebyeMSD.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCDebyeMSD.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCDynInfoUtils.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCDynInfoUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCDynLoader.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCDynLoader.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCElIncScatter.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCElIncScatter.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCElIncXS.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCElIncXS.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCEqRefl.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCEqRefl.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFactoryUtils.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCFactoryUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFastConvolve.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCFastConvolve.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFileUtils.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCFileUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFillHKL.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCFillHKL.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFreeGas.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCFreeGas.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFreeGasUtils.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCFreeGasUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCGasMixUtils.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCGasMixUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCGaussMos.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCGaussMos.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCGaussOnSphere.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCGaussOnSphere.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCIofQHelper.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCIofQHelper.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCIter.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCIter.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCKinUtils.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCKinUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCLCBragg.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCLCBragg.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCLCRefModels.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCLCRefModels.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCLCUtils.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCLCUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCLatticeUtils.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCLatticeUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCMath.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCMath.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCMatrix.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCMatrix.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCOrientUtils.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCOrientUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCPCBragg.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCPCBragg.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCPlaneProvider.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCPlaneProvider.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCPointwiseDist.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCPointwiseDist.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCRandUtils.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCRandUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCRomberg.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCRomberg.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCRotMatrix.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCRotMatrix.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABEval.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABEval.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABExtender.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABExtender.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABFactory.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABFactory.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABIntegrator.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABIntegrator.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABSampler.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABSampler.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABSamplerModels.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABSamplerModels.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABScatter.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABScatter.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABScatterHelper.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABScatterHelper.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABUCN.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABUCN.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABUtils.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABXSProvider.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSABXSProvider.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSANSSphScat.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSANSSphScat.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSANSUtils.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSANSUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSCBragg.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSCBragg.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCScatKnlData.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCScatKnlData.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSpan.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSpan.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSpline.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCSpline.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCStrView.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCStrView.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCString.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCString.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCVDOSEval.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCVDOSEval.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCVDOSGn.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCVDOSGn.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCVDOSToScatKnl.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCVDOSToScatKnl.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCVector.hh` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/internal/NCVector.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/ncapi.h` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/ncapi.h`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/ncrystal.h` & `ncrystal-3.7.0/ncrystal_core/include/NCrystal/ncrystal.h`

 * *Files 0% similar despite different names*

```diff
@@ -575,18 +575,18 @@
 #ifdef NCRYSTAL_VERSION
 #  undef NCRYSTAL_VERSION
 #endif
 #ifdef NCRYSTAL_VERSION_STR
 #  undef NCRYSTAL_VERSION_STR
 #endif
 #define NCRYSTAL_VERSION_MAJOR 3
-#define NCRYSTAL_VERSION_MINOR 6
-#define NCRYSTAL_VERSION_PATCH 82
-#define NCRYSTAL_VERSION   3006082 /* (1000000*MAJOR+1000*MINOR+PATCH)             */
-#define NCRYSTAL_VERSION_STR "3.6.82"
+#define NCRYSTAL_VERSION_MINOR 7
+#define NCRYSTAL_VERSION_PATCH 0
+#define NCRYSTAL_VERSION   3007000 /* (1000000*MAJOR+1000*MINOR+PATCH)             */
+#define NCRYSTAL_VERSION_STR "3.7.0"
   NCRYSTAL_API int ncrystal_version(); /* returns NCRYSTAL_VERSION                  */
   NCRYSTAL_API const char * ncrystal_version_str(); /* returns NCRYSTAL_VERSION_STR */
 
   /* Load raw NCMAT data into JSON structures. Must deallocate with call to        */
   /* ncrystal_dealloc_string as usual. (WARNING: JSON is incomplete for now!!!!!)  */
   NCRYSTAL_API char * ncrystal_ncmat2json( const char * textdataname );
```

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCAbsOOV.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCAbsOOV.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCAtomDB.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCAtomDB.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCAtomDBExtender.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCAtomDBExtender.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCAtomData.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCAtomData.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCAtomUtils.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCAtomUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCBkgdExtCurve.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCBkgdExtCurve.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCCfgManip.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCCfgManip.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCCfgTypes.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCCfgTypes.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCCfgVars.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCCfgVars.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCCompositionUtils.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCCompositionUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCDataSources.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCDataSources.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCDebyeMSD.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCDebyeMSD.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCDefs.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCDefs.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCDump.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCDump.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCDynInfoUtils.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCDynInfoUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCDynLoader.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCDynLoader.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCElIncScatter.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCElIncScatter.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCElIncXS.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCElIncXS.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCEqRefl.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCEqRefl.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCException.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCException.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCFact.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCFactImpl.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCFactImpl.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCFactRequests.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCFactRequests.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCFactTypes.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCFactTypes.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCFactoryUtils.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCFactoryUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCFactory_NCMAT.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCFactory_NCMAT.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCFastConvolve.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCFastConvolve.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCFileUtils.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCFileUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCFillHKL.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCFillHKL.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCFmt.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCFmt.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCFreeGas.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCFreeGas.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCFreeGasUtils.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCFreeGasUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCGasMixFact.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCGasMixFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCGasMixUtils.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCGasMixUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCGaussMos.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCGaussMos.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCGaussOnSphere.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCGaussOnSphere.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCInfo.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCInfo.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCInfoBuilder.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCInfoBuilder.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCIofQHelper.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCIofQHelper.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCKinUtils.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCKinUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCLCBragg.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCLCBragg.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCLCRefModels.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCLCRefModels.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCLCUtils.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCLCUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCLatticeUtils.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCLatticeUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCLauLazyFact.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCLauLazyFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCLazy.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCLazy.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCLazy.hh` & `ncrystal-3.7.0/ncrystal_core/src/NCLazy.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCLoadNCMAT.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCLoadNCMAT.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCMatCfg.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCMatCfg.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCMath.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCMath.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCMatrix.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCMatrix.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCMem.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCMem.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCNCMATData.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCNCMATData.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCOrientUtils.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCOrientUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCPCBragg.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCPCBragg.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCParseNCMAT.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCParseNCMAT.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCPlaneProvider.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCPlaneProvider.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCPluginMgmt.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCPluginMgmt.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCPointwiseDist.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCPointwiseDist.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCProc.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCProc.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCProcImpl.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCProcImpl.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCQuickFact.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCQuickFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCRNG.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCRNG.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCRandUtils.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCRandUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCRomberg.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCRomberg.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCRotMatrix.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCRotMatrix.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCSABData.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCSABData.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCSABEval.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCSABEval.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCSABExtender.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCSABExtender.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCSABFactory.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCSABFactory.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCSABIntegrator.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCSABIntegrator.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCSABSampler.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCSABSampler.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCSABSamplerModels.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCSABSamplerModels.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCSABScatter.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCSABScatter.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCSABUCN.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCSABUCN.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCSABUtils.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCSABUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCSABXSProvider.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCSABXSProvider.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCSANSFact.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCSANSFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCSANSSphScat.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCSANSSphScat.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCSANSUtils.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCSANSUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCSCBragg.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCSCBragg.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCSCOrientation.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCSCOrientation.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCScatKnlData.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCScatKnlData.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCSpline.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCSpline.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCStdAbsFact.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCStdAbsFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCStdMPScatFact.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCStdMPScatFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCStdScatFact.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCStdScatFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCStrView.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCStrView.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCString.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCString.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCTDProd.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCTDProd.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCTextData.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCTextData.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCTypes.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCTypes.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCVDOSEval.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCVDOSEval.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCVDOSGn.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCVDOSGn.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCVDOSToScatKnl.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCVDOSToScatKnl.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCVector.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCVector.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/NCVersion.cc` & `ncrystal-3.7.0/ncrystal_core/src/NCVersion.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_core/src/ncrystal.cc` & `ncrystal-3.7.0/ncrystal_core/src/ncrystal.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_geant4/include/G4NCrystal/G4NCInstall.hh` & `ncrystal-3.7.0/ncrystal_geant4/include/G4NCrystal/G4NCInstall.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_geant4/include/G4NCrystal/G4NCManager.hh` & `ncrystal-3.7.0/ncrystal_geant4/include/G4NCrystal/G4NCManager.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_geant4/include/G4NCrystal/G4NCMatHelper.hh` & `ncrystal-3.7.0/ncrystal_geant4/include/G4NCrystal/G4NCMatHelper.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_geant4/include/G4NCrystal/G4NCrystal.hh` & `ncrystal-3.7.0/ncrystal_geant4/include/G4NCrystal/G4NCrystal.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCInstall.cc` & `ncrystal-3.7.0/ncrystal_geant4/src/G4NCInstall.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCManager.cc` & `ncrystal-3.7.0/ncrystal_geant4/src/G4NCManager.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCMatHelper.cc` & `ncrystal-3.7.0/ncrystal_geant4/src/G4NCMatHelper.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCProcWrapper.cc` & `ncrystal-3.7.0/ncrystal_geant4/src/G4NCProcWrapper.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCProcWrapper.hh` & `ncrystal-3.7.0/ncrystal_geant4/src/G4NCProcWrapper.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_mcstas/NCrystal_example.instr` & `ncrystal-3.7.0/ncrystal_mcstas/NCrystal_example.instr`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/ncrystal_mcstas/NCrystal_sample.comp` & `ncrystal-3.7.0/ncrystal_mcstas/NCrystal_sample.comp`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 *  limitations under the License.
 *
 *
 * Component: NCrystal_sample
 *
 * %I
 * Written by: NCrystal developers
-* Version: 3.6.82
+* Version: 3.7.0
 * Origin: NCrystal Developers (European Spallation Source ERIC and DTU Nutech)
 *
 * McStas sample component for the NCrystal library for thermal neutron transport
 * (<a href="https://github.com/mctools/ncrystal">www</a>).
 *
 * %D
 * McStas sample component for the NCrystal scattering library.
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 Version 2.0 (the "License"); * you may not use this file except in compliance
 with the License. * You may obtain a copy of the License at * * http://
 www.apache.org/licenses/LICENSE-2.0 * * Unless required by applicable law or
 agreed to in writing, software * distributed under the License is distributed
 on an "AS IS" BASIS, * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 express or implied. * See the License for the specific language governing
 permissions and * limitations under the License. * * * Component:
-NCrystal_sample * * %I * Written by: NCrystal developers * Version: 3.6.82 *
+NCrystal_sample * * %I * Written by: NCrystal developers * Version: 3.7.0 *
 Origin: NCrystal Developers (European Spallation Source ERIC and DTU Nutech) *
 * McStas sample component for the NCrystal library for thermal neutron
 transport * (www). * * %D * McStas sample component for the NCrystal scattering
 library. * Find more information at the_NCrystal_wiki. * In particular, browse
 the available datafiles at Data-library * and read about the format of the
 configuration string expected in * the "cfg" parameter at Using-NCrystal. * *
 NCrystal is available under the Apache_2.0_license. * Depending on the
```

### Comparing `ncrystal-3.6.dev82/ncrystal_mcstas/ncrystal_preparemcstasdir` & `ncrystal-3.7.0/ncrystal_mcstas/ncrystal_preparemcstasdir`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/pyproject.toml` & `ncrystal-3.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/scripts/ncrystal_cif2ncmat` & `ncrystal-3.7.0/scripts/ncrystal_cif2ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/scripts/ncrystal_endf2ncmat` & `ncrystal-3.7.0/scripts/ncrystal_endf2ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/scripts/ncrystal_hfg2ncmat` & `ncrystal-3.7.0/scripts/ncrystal_hfg2ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/scripts/ncrystal_inspectfile` & `ncrystal-3.7.0/scripts/ncrystal_inspectfile`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/scripts/ncrystal_ncmat2cpp` & `ncrystal-3.7.0/scripts/ncrystal_ncmat2cpp`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/scripts/ncrystal_ncmat2hkl` & `ncrystal-3.7.0/scripts/ncrystal_ncmat2hkl`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/scripts/ncrystal_onlinedb2ncmat` & `ncrystal-3.7.0/scripts/ncrystal_onlinedb2ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/scripts/ncrystal_vdos2ncmat` & `ncrystal-3.7.0/scripts/ncrystal_vdos2ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/scripts/ncrystal_verifyatompos` & `ncrystal-3.7.0/scripts/ncrystal_verifyatompos`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/scripts/nctool` & `ncrystal-3.7.0/scripts/nctool`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.dev82/setup.py` & `ncrystal-3.7.0/setup.py`

 * *Files identical despite different names*

