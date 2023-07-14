# Comparing `tmp/ncrystal-3.6.80.tar.gz` & `tmp/ncrystal-3.6.dev82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncrystal-3.6.80.tar", last modified: Fri Jun  9 09:35:39 2023, max compression
+gzip compressed data, was "ncrystal-3.6.dev82.tar", last modified: Fri Jul 14 18:10:46 2023, max compression
```

## Comparing `ncrystal-3.6.80.tar` & `ncrystal-3.6.dev82.tar`

### file list

```diff
@@ -1,433 +1,433 @@
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.636108 ncrystal-3.6.80/
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.396107 ncrystal-3.6.80/.github/
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.424107 ncrystal-3.6.80/.github/ISSUE_TEMPLATE/
--rw-r-----   0 tkittel   (1001) tkittel   (1001)      337 2021-06-17 07:53:55.000000 ncrystal-3.6.80/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r-----   0 tkittel   (1001) tkittel   (1001)      196 2022-10-06 10:17:33.000000 ncrystal-3.6.80/.github/ISSUE_TEMPLATE/config.yml
--rw-r-----   0 tkittel   (1001) tkittel   (1001)      604 2021-06-17 07:53:55.000000 ncrystal-3.6.80/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r-----   0 tkittel   (1001) tkittel   (1001)      665 2021-06-17 07:53:55.000000 ncrystal-3.6.80/.github/ISSUE_TEMPLATE/request-for-new-material.md
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.428107 ncrystal-3.6.80/.github/workflows/
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5502 2023-05-16 21:29:32.000000 ncrystal-3.6.80/.github/workflows/cmake.yml
--rw-r-----   0 tkittel   (1001) tkittel   (1001)      136 2022-11-23 14:47:20.000000 ncrystal-3.6.80/.gitignore
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    76662 2023-06-07 13:12:12.000000 ncrystal-3.6.80/CHANGELOG
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    35134 2023-06-07 13:12:12.000000 ncrystal-3.6.80/CMakeLists.txt
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2365 2023-06-07 13:12:12.000000 ncrystal-3.6.80/FILES
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5490 2023-06-07 13:12:12.000000 ncrystal-3.6.80/INSTALL
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    11509 2023-06-07 13:12:12.000000 ncrystal-3.6.80/LICENSE
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.440107 ncrystal-3.6.80/NCrystal/
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4006 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/__init__.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    40112 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/_chooks.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    13849 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/_common.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5861 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/_coreimpl.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    16356 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/_miscimpl.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    85698 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/_ncmatimpl.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2631 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/_numpy.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    17151 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/_testimpl.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2872 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/api.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     8066 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/atomdata.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3741 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/cfgstr.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    74600 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/cifutils.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5682 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/constants.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    74942 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/core.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     9702 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/datasrc.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2685 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/exceptions.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    17208 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/mcstasutils.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    11032 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/misc.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    38934 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/ncmat.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3437 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/obsolete.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    19521 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/plot.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2435 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/plugins.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     1733 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/test.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    45870 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NCrystal/vdos.py
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     1667 2023-06-07 13:12:12.000000 ncrystal-3.6.80/NOTICE
--rw-r-----   0 tkittel   (1001) tkittel   (1001)      914 2023-06-09 09:35:39.636108 ncrystal-3.6.80/PKG-INFO
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    13326 2023-06-07 13:12:12.000000 ncrystal-3.6.80/README
--rw-r-----   0 tkittel   (1001) tkittel   (1001)        7 2023-06-07 13:12:12.000000 ncrystal-3.6.80/VERSION
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.440107 ncrystal-3.6.80/cmake/
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     6890 2023-06-07 13:12:12.000000 ncrystal-3.6.80/cmake/NCrystalConfig.cmake.in
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.444107 ncrystal-3.6.80/cmake/modules/
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3725 2023-06-07 13:12:12.000000 ncrystal-3.6.80/cmake/modules/ncrystal_legacyoptions.cmake
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3756 2023-06-07 13:12:12.000000 ncrystal-3.6.80/cmake/modules/ncrystal_options.cmake
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4296 2023-06-07 13:12:12.000000 ncrystal-3.6.80/cmake/modules/ncrystal_utils.cmake
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    13730 2023-06-07 13:12:12.000000 ncrystal-3.6.80/cmake/ncrystal-config.in
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2690 2023-06-07 13:12:12.000000 ncrystal-3.6.80/cmake/template_setup.py.in
--rw-r-----   0 tkittel   (1001) tkittel   (1001)      525 2023-06-07 13:12:12.000000 ncrystal-3.6.80/cmake/template_setup.sh.in
--rw-r-----   0 tkittel   (1001) tkittel   (1001)      593 2023-06-07 13:12:12.000000 ncrystal-3.6.80/cmake/template_unsetup.sh.in
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.512107 ncrystal-3.6.80/data/
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4088 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/AcrylicGlass_C5O2H8.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4496 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/AgBr_sg225_SilverBromide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2771 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Ag_sg225.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7677 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Al2O3_sg167_Corundum.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4185 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Al4C3_sg166_AluminiumCarbide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3625 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/AlN_sg186_AluminumNitride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3487 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Al_sg225.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)      756 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Ar_Gas_STP.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     1475 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Au_sg225.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4411 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/BaF2_sg225_BariumFluoride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4887 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/BaO_sg225_BariumOxide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2275 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Ba_sg229.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5540 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Be3N2_sg206_BerylliumNitride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7338 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/BeF2_sg152_Beryllium_Fluoride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3938 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/BeO_sg186.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     1690 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Be_sg194.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2321 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Bi_sg166.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3596 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/C_sg194_pyrolytic_graphite.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3104 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/C_sg227_Diamond.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     9379 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/CaCO3_sg62_Aragonite.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3997 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/CaF2_sg225_CalciumFlouride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4549 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/CaH2_sg62_CalciumHydride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5716 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/CaO2H2_sg164_CalciumHydroxide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3665 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/CaO_sg225_CalciumOxide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     1858 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/CaSiO3_sg2_Wollastonite.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2433 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Ca_sg225.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)      941 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Ca_sg229_Calcium-gamma.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4050 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/CeO2_sg225_CeriumOxide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     1895 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Cr_sg229.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     6705 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Cu2O_sg224_Cuprite.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2483 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Cu_sg225.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5582 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Dy2O3_sg206_DysprosiumOxide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3327 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Epoxy_Araldite506_C18H20O3.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3184 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Fe_sg225_Iron-gamma.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4298 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Fe_sg229_Iron-alpha.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4228 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/GaN_sg186_GalliumNitride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4327 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/GaSe_sg194_GalliumSelenide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7731 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Ge3Bi4O12_sg220_BismuthGermanate.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4724 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Ge_sg227.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)      778 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/He_Gas_STP.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4353 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/HfO2_sg14_HafniumOxide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5885 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Ho2O3_sg206_HolmiumOxide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2698 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/KBr_sg225_PotassiumBromide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3452 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/KF_sg225_PotassiumFlouride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5979 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/KOH_sg4_PotassiumHydroxide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2318 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/K_sg229.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3168 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Kapton_C22H10N2O5.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)      757 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Kr_Gas_STP.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3534 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/LaBr3_sg176_LanthanumBromide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3266 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Li2O_sg225_LithiumOxide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3436 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Li3N_sg191_LithiumNitride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3627 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/LiF_sg225_LithiumFlouride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5087 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/LiH_sg225_LithiumHydride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)  1560968 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/LiquidHeavyWaterD2O_T293.6K.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)   528493 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/LiquidWaterH2O_T293.6K.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5600 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Lu2O3_sg206_LutetiumOxide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7337 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Lu2SiO5_sg15.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5987 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Mg2SiO4_sg62_MagnesiumSilicate.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7228 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/MgAl2O4_sg227_MAS.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     6653 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/MgCO3_sg167_MagnesiumCarbonate.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4982 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/MgD2_sg136_MagnesiumDeuteride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4083 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/MgF2_sg136_MagnesiumFlouride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     6130 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/MgH2_sg136_MagnesiumHydride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     6563 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/MgO2H2_sg164_MagnesiumHydroxide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7167 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/MgO_sg225_Periclase.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     1423 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Mg_sg194.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     1921 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Mo_sg229.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    10379 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Na4Si3Al3O12Cl_sg218_Sodalite.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3143 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/NaBr_sg225_SodiumBromide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3901 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/NaCl_sg225_SodiumChloride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3586 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/NaF_sg225_SodiumFlouride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3495 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/NaI_sg225_SodiumIodide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2372 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Na_sg229.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     1937 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Nb_sg229.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)      758 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Ne_Gas_STP.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2024 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Ni_sg225.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3472 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Nylon11_C11H21NO.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3408 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Nylon12_C12H23NO.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3425 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Nylon610_C16H30N2O2.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3794 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Nylon66or6_C12H22N2O2.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3008 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/PEEK_C19H12O3.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3340 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/PVC_C2H3Cl.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5058 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/PbF2-beta_sg225_BetaLeadFlouride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4155 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/PbO-alpha_sg129_Litharge.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     6502 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/PbO-beta_sg57_Massicot.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3894 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/PbS_sg225_LeadSulfide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2447 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Pb_sg225.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     1722 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Pd_sg225.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3297 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Polycarbonate_C16O3H14.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3698 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Polyester_C10H8O4.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5022 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Polyethylene_CH2.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3292 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Polylactide_C3H4O2.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3331 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Polypropylene_C3H6.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3348 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Polystyrene_C8H8.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2189 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Pt_sg225.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2630 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Rb_sg229.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3291 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Rubber_C5H8.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3309 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Sc_sg194.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3890 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/SiC-beta_sg216_BetaSiliconCarbide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     6995 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/SiO2-alpha_sg154_AlphaQuartz.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4957 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/SiO2-beta_sg180_BetaQuartz.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2517 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Si_sg227.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     1594 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Sn_sg141.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4547 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/SrF2_sg225_StrontiumFluoride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4394 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/SrH2_sg62_StrontiumHydride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2330 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Sr_sg225.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4735 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Th3N4_sg166_ThoriumNitride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4280 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/ThO2_sg225_ThoriumDioxide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2081 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Th_sg225.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4194 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/TiO2_sg136_Rutile.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4122 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/TiO2_sg141_Anatase.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2960 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Ti_sg194.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3878 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/TlBr_sg221_ThaliumBromide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5510 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Tm2O3_sg206_ThuliumOxide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3928 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/UF6_sg62_UraniumHexaflouride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4949 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/UO2_sg225_UraniumDioxide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3084 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/V_sg229.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2482 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/W_sg229.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)      758 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Xe_Gas_STP.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7134 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Y2O3_sg206_Yttrium_Oxide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7283 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Y2SiO5_sg15_YSO.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     8335 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Y3Al5O12_sg230_YAG.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3443 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Y_sg194.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3719 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/ZnF2_sg136_ZincFlouride.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5606 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/ZnO_sg186_ZincOxide.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4164 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/ZnS_sg216_Sphalerite.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2564 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Zn_sg194.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5917 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/ZrF4-beta_sg84.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5387 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/ZrO2_sg137_Zirconia.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4185 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/ZrO2_sg14_Zirconia.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3994 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/Zr_sg194.ncmat
--rw-r-----   0 tkittel   (1001) tkittel   (1001)      858 2023-06-07 13:12:12.000000 ncrystal-3.6.80/data/void.ncmat
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.516108 ncrystal-3.6.80/docs/
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    39216 2023-06-07 13:12:12.000000 ncrystal-3.6.80/docs/ncmat_doc.md
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.520108 ncrystal-3.6.80/examples/
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4012 2023-06-07 13:12:12.000000 ncrystal-3.6.80/examples/NCrystal_example_mcstas.instr
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3685 2023-06-07 13:12:12.000000 ncrystal-3.6.80/examples/ncrystal_example_c.c
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     6227 2023-06-07 13:12:12.000000 ncrystal-3.6.80/examples/ncrystal_example_cpp.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    11501 2023-06-07 13:12:12.000000 ncrystal-3.6.80/examples/ncrystal_example_customphysics.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     8045 2023-06-07 13:12:12.000000 ncrystal-3.6.80/examples/ncrystal_example_g4sim.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2737 2023-06-07 13:12:12.000000 ncrystal-3.6.80/examples/ncrystal_example_py
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.520108 ncrystal-3.6.80/ncrystal.egg-info/
--rw-r-----   0 tkittel   (1001) tkittel   (1001)      914 2023-06-09 09:35:39.000000 ncrystal-3.6.80/ncrystal.egg-info/PKG-INFO
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    14404 2023-06-09 09:35:39.000000 ncrystal-3.6.80/ncrystal.egg-info/SOURCES.txt
--rw-r-----   0 tkittel   (1001) tkittel   (1001)        1 2023-06-09 09:35:39.000000 ncrystal-3.6.80/ncrystal.egg-info/dependency_links.txt
--rw-r-----   0 tkittel   (1001) tkittel   (1001)        6 2023-06-09 09:35:39.000000 ncrystal-3.6.80/ncrystal.egg-info/requires.txt
--rw-r-----   0 tkittel   (1001) tkittel   (1001)        9 2023-06-09 09:35:39.000000 ncrystal-3.6.80/ncrystal.egg-info/top_level.txt
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.400107 ncrystal-3.6.80/ncrystal_core/
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.400107 ncrystal-3.6.80/ncrystal_core/include/
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.536108 ncrystal-3.6.80/ncrystal_core/include/NCrystal/
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     9738 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCAtomData.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7607 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCCompositionUtils.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    10124 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCDataSources.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    50651 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCDefs.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2296 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCDump.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     8763 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCException.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4437 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCFact.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    12315 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCFactImpl.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    11741 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCFactRequests.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    10401 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCFactTypes.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     9309 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCFmt.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    16338 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCImmutBuf.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    28964 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCInfo.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5695 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCInfoBuilder.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    16845 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCInfoTypes.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4232 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCLoadNCMAT.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    22448 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCMatCfg.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    14874 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCMem.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7411 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCNCMATData.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2503 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCParseNCMAT.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4593 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCPluginBoilerplate.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3892 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCPluginMgmt.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     9058 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCProc.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    20012 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCProcImpl.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     8881 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCRNG.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3745 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCSABData.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5817 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCSCOrientation.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    38333 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCSmallVector.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    14618 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCTextData.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    36928 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCTypes.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    13171 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCVariant.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3135 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCVersion.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3965 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCrystal.hh
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.572108 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2639 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCAbsOOV.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2998 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCAtomDB.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4434 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCAtomDBExtender.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     6211 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCAtomUtils.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2505 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCBkgdExtCurve.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    23020 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCCfgManip.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    32290 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCCfgTypes.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    35719 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCCfgVars.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2479 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCDebyeMSD.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3907 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCDynInfoUtils.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3787 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCDynLoader.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4442 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCElIncScatter.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5851 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCElIncXS.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     6565 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCEqRefl.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    19986 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCFactoryUtils.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2887 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCFastConvolve.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3185 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCFileUtils.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4004 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCFillHKL.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3252 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCFreeGas.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7720 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCFreeGasUtils.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4680 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCGasMixUtils.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    10441 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCGaussMos.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    10270 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCGaussOnSphere.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5287 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCIofQHelper.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3651 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCIter.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     8433 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCKinUtils.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3244 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCLCBragg.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4021 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCLCRefModels.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    12681 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCLCUtils.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5378 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCLatticeUtils.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    27371 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCMath.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7060 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCMatrix.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2577 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCOrientUtils.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3551 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCPCBragg.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5786 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCPlaneProvider.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3957 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCPointwiseDist.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     8124 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCRandUtils.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3880 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCRomberg.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7446 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCRotMatrix.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    18011 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABEval.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3641 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABExtender.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2801 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABFactory.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3357 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABIntegrator.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4211 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABSampler.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5564 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABSamplerModels.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3619 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABScatter.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2777 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABScatterHelper.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     9712 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABUCN.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    14765 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABUtils.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2524 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABXSProvider.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3444 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSANSSphScat.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7882 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSANSUtils.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3301 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSCBragg.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5222 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCScatKnlData.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     6947 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSpan.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     8836 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSpline.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    20113 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCStrView.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    15426 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCString.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     6756 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCVDOSEval.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7527 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCVDOSGn.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3697 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCVDOSToScatKnl.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     9623 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCVector.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4111 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/ncapi.h
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    44878 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/include/NCrystal/ncrystal.h
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.628108 ncrystal-3.6.80/ncrystal_core/src/
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3152 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCAbsOOV.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    36761 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCAtomDB.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     9809 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCAtomDBExtender.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    11555 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCAtomData.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    14903 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCAtomUtils.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2638 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCBkgdExtCurve.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    18374 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCCfgManip.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7380 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCCfgTypes.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    17901 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCCfgVars.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    12257 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCCompositionUtils.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    26184 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCDataSources.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4317 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCDebyeMSD.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3413 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/src/NCDefs.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    19704 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCDump.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    13146 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCDynInfoUtils.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     6827 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCDynLoader.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     9488 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCElIncScatter.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7907 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCElIncXS.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4952 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCEqRefl.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2613 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/src/NCException.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3339 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCFact.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    42888 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCFactImpl.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    13433 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCFactRequests.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3761 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCFactTypes.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     6059 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCFactoryUtils.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2647 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/src/NCFactory_NCMAT.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    11222 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCFastConvolve.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7384 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCFileUtils.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    30178 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCFillHKL.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7794 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/src/NCFmt.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3716 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCFreeGas.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    39971 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCFreeGasUtils.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     6261 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCGasMixFact.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    26599 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCGasMixUtils.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    10567 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCGaussMos.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    20586 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCGaussOnSphere.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    12554 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCInfo.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    57518 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/src/NCInfoBuilder.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3507 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCIofQHelper.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2495 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCKinUtils.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     6008 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/src/NCLCBragg.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7084 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCLCRefModels.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    32322 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCLCUtils.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    19509 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCLatticeUtils.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3223 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCLauLazyFact.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    30601 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCLazy.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3277 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCLazy.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    33272 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/src/NCLoadNCMAT.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    48483 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCMatCfg.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    23835 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCMath.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4593 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCMatrix.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4201 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/src/NCMem.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    31787 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/src/NCNCMATData.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2407 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCOrientUtils.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    11539 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCPCBragg.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    42614 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/src/NCParseNCMAT.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     8467 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCPlaneProvider.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     8658 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCPluginMgmt.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5437 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCPointwiseDist.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3125 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCProc.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    20199 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCProcImpl.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    14830 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCQuickFact.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    13265 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCRNG.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    20337 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCRandUtils.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     6792 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCRomberg.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5878 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCRotMatrix.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3197 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCSABData.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    31885 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCSABEval.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2376 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCSABExtender.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5986 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCSABFactory.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    23449 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCSABIntegrator.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    10767 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCSABSampler.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    12421 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCSABSamplerModels.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4819 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCSABScatter.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    26306 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCSABUCN.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    26746 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCSABUtils.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5022 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCSABXSProvider.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5166 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCSANSFact.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    11876 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCSANSSphScat.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     8168 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCSANSUtils.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    13235 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCSCBragg.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3522 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCSCOrientation.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5050 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCScatKnlData.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     8314 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCSpline.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3302 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/src/NCStdAbsFact.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4997 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCStdMPScatFact.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    18990 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCStdScatFact.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7601 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCStrView.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    15206 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCString.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     9143 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCTDProd.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7672 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCTextData.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3374 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/src/NCTypes.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    25936 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/src/NCVDOSEval.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    15041 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/src/NCVDOSGn.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    38631 2023-06-07 13:12:11.000000 ncrystal-3.6.80/ncrystal_core/src/NCVDOSToScatKnl.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     1887 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCVector.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     1633 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/NCVersion.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    72731 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_core/src/ncrystal.cc
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.400107 ncrystal-3.6.80/ncrystal_geant4/
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.400107 ncrystal-3.6.80/ncrystal_geant4/include/
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.628108 ncrystal-3.6.80/ncrystal_geant4/include/G4NCrystal/
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2813 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_geant4/include/G4NCrystal/G4NCInstall.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     6896 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_geant4/include/G4NCrystal/G4NCManager.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2486 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_geant4/include/G4NCrystal/G4NCMatHelper.hh
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2196 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_geant4/include/G4NCrystal/G4NCrystal.hh
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.628108 ncrystal-3.6.80/ncrystal_geant4/src/
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     5504 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_geant4/src/G4NCInstall.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4959 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_geant4/src/G4NCManager.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    15023 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_geant4/src/G4NCMatHelper.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     7467 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_geant4/src/G4NCProcWrapper.cc
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     2644 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_geant4/src/G4NCProcWrapper.hh
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.632108 ncrystal-3.6.80/ncrystal_mcstas/
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     4012 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_mcstas/NCrystal_example.instr
--rw-r-----   0 tkittel   (1001) tkittel   (1001)    16072 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_mcstas/NCrystal_sample.comp
--rwxr-x---   0 tkittel   (1001) tkittel   (1001)     5054 2023-06-07 13:12:12.000000 ncrystal-3.6.80/ncrystal_mcstas/ncrystal_preparemcstasdir
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     1690 2023-06-07 13:12:12.000000 ncrystal-3.6.80/pyproject.toml
-drwxr-x---   0 tkittel   (1001) tkittel   (1001)        0 2023-06-09 09:35:39.636108 ncrystal-3.6.80/scripts/
--rwxr-x---   0 tkittel   (1001) tkittel   (1001)    15960 2023-06-07 13:12:12.000000 ncrystal-3.6.80/scripts/ncrystal_cif2ncmat
--rwxr-x---   0 tkittel   (1001) tkittel   (1001)    35171 2023-06-07 13:12:12.000000 ncrystal-3.6.80/scripts/ncrystal_endf2ncmat
--rwxr-x---   0 tkittel   (1001) tkittel   (1001)    73858 2023-06-07 13:12:12.000000 ncrystal-3.6.80/scripts/ncrystal_hfg2ncmat
--rwxr-x---   0 tkittel   (1001) tkittel   (1001)    35971 2023-06-07 13:12:12.000000 ncrystal-3.6.80/scripts/ncrystal_inspectfile
--rwxr-x---   0 tkittel   (1001) tkittel   (1001)    15231 2023-06-07 13:12:12.000000 ncrystal-3.6.80/scripts/ncrystal_ncmat2cpp
--rwxr-x---   0 tkittel   (1001) tkittel   (1001)     7659 2023-06-07 13:12:12.000000 ncrystal-3.6.80/scripts/ncrystal_ncmat2hkl
--rwxr-x---   0 tkittel   (1001) tkittel   (1001)     1998 2023-06-07 13:12:12.000000 ncrystal-3.6.80/scripts/ncrystal_onlinedb2ncmat
--rwxr-x---   0 tkittel   (1001) tkittel   (1001)    20289 2023-06-07 13:12:12.000000 ncrystal-3.6.80/scripts/ncrystal_vdos2ncmat
--rwxr-x---   0 tkittel   (1001) tkittel   (1001)    13315 2023-06-07 13:12:12.000000 ncrystal-3.6.80/scripts/ncrystal_verifyatompos
--rwxr-x---   0 tkittel   (1001) tkittel   (1001)    35971 2023-06-07 13:12:12.000000 ncrystal-3.6.80/scripts/nctool
--rw-r-----   0 tkittel   (1001) tkittel   (1001)       38 2023-06-09 09:35:39.636108 ncrystal-3.6.80/setup.cfg
--rw-r-----   0 tkittel   (1001) tkittel   (1001)     3918 2023-06-07 13:12:12.000000 ncrystal-3.6.80/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.492546 ncrystal-3.6.dev82/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.436545 ncrystal-3.6.dev82/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.440544 ncrystal-3.6.dev82/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/.github/ISSUE_TEMPLATE/request-for-new-material.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.440544 ncrystal-3.6.dev82/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/.github/workflows/cmake.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    76764 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)    35344 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/FILES
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.444545 ncrystal-3.6.dev82/NCrystal/
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40112 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/_chooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/_coreimpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16356 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/_miscimpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85698 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/_ncmatimpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25999 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/_testimpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/atomdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/cfgstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74600 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/cifutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74942 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/datasrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/mcstasutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11032 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38896 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/ncmat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/obsolete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45843 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NCrystal/vdos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-14 18:10:46.492546 ncrystal-3.6.dev82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/README
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.444545 ncrystal-3.6.dev82/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/cmake/NCrystalConfig.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.444545 ncrystal-3.6.dev82/cmake/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/cmake/modules/ncrystal_legacyoptions.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/cmake/modules/ncrystal_options.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/cmake/modules/ncrystal_utils.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/cmake/ncrystal-config.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/cmake/template_setup.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/cmake/template_setup.sh.in
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/cmake/template_unsetup.sh.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.464545 ncrystal-3.6.dev82/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/AcrylicGlass_C5O2H8.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/AgBr_sg225_SilverBromide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ag_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Al2O3_sg167_Corundum.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Al4C3_sg166_AluminiumCarbide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/AlN_sg186_AluminumNitride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Al_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ar_Gas_STP.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Au_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/BaF2_sg225_BariumFluoride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/BaO_sg225_BariumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ba_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Be3N2_sg206_BerylliumNitride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/BeF2_sg152_Beryllium_Fluoride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/BeO_sg186.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Be_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Bi_sg166.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/C_sg194_pyrolytic_graphite.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/C_sg227_Diamond.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/CaCO3_sg62_Aragonite.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/CaF2_sg225_CalciumFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/CaH2_sg62_CalciumHydride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/CaO2H2_sg164_CalciumHydroxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/CaO_sg225_CalciumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/CaSiO3_sg2_Wollastonite.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ca_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ca_sg229_Calcium-gamma.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/CeO2_sg225_CeriumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Cr_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Cu2O_sg224_Cuprite.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Cu_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Dy2O3_sg206_DysprosiumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Epoxy_Araldite506_C18H20O3.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Fe_sg225_Iron-gamma.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Fe_sg229_Iron-alpha.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/GaN_sg186_GalliumNitride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/GaSe_sg194_GalliumSelenide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ge3Bi4O12_sg220_BismuthGermanate.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ge_sg227.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/He_Gas_STP.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/HfO2_sg14_HafniumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ho2O3_sg206_HolmiumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/KBr_sg225_PotassiumBromide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/KF_sg225_PotassiumFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/KOH_sg4_PotassiumHydroxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/K_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Kapton_C22H10N2O5.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Kr_Gas_STP.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/LaBr3_sg176_LanthanumBromide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Li2O_sg225_LithiumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Li3N_sg191_LithiumNitride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/LiF_sg225_LithiumFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/LiH_sg225_LithiumHydride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)  1560968 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/LiquidHeavyWaterD2O_T293.6K.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)   528493 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/LiquidWaterH2O_T293.6K.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Lu2O3_sg206_LutetiumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Lu2SiO5_sg15.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Mg2SiO4_sg62_MagnesiumSilicate.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/MgAl2O4_sg227_MAS.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/MgCO3_sg167_MagnesiumCarbonate.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/MgD2_sg136_MagnesiumDeuteride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/MgF2_sg136_MagnesiumFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/MgH2_sg136_MagnesiumHydride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/MgO2H2_sg164_MagnesiumHydroxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/MgO_sg225_Periclase.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Mg_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Mo_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Na4Si3Al3O12Cl_sg218_Sodalite.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/NaBr_sg225_SodiumBromide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/NaCl_sg225_SodiumChloride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/NaF_sg225_SodiumFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/NaI_sg225_SodiumIodide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Na_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Nb_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ne_Gas_STP.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ni_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Nylon11_C11H21NO.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Nylon12_C12H23NO.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Nylon610_C16H30N2O2.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Nylon66or6_C12H22N2O2.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/PEEK_C19H12O3.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/PVC_C2H3Cl.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/PbF2-beta_sg225_BetaLeadFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/PbO-alpha_sg129_Litharge.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/PbO-beta_sg57_Massicot.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/PbS_sg225_LeadSulfide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Pb_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Pd_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Polycarbonate_C16O3H14.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Polyester_C10H8O4.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Polyethylene_CH2.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Polylactide_C3H4O2.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Polypropylene_C3H6.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Polystyrene_C8H8.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Pt_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Rb_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Rubber_C5H8.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Sc_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/SiC-beta_sg216_BetaSiliconCarbide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/SiO2-alpha_sg154_AlphaQuartz.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/SiO2-beta_sg180_BetaQuartz.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Si_sg227.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Sn_sg141.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/SrF2_sg225_StrontiumFluoride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/SrH2_sg62_StrontiumHydride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Sr_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Th3N4_sg166_ThoriumNitride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/ThO2_sg225_ThoriumDioxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Th_sg225.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/TiO2_sg136_Rutile.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/TiO2_sg141_Anatase.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Ti_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/TlBr_sg221_ThaliumBromide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Tm2O3_sg206_ThuliumOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/UF6_sg62_UraniumHexaflouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/UO2_sg225_UraniumDioxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/V_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/W_sg229.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Xe_Gas_STP.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Y2O3_sg206_Yttrium_Oxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Y2SiO5_sg15_YSO.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Y3Al5O12_sg230_YAG.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Y_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/ZnF2_sg136_ZincFlouride.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/ZnO_sg186_ZincOxide.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/ZnS_sg216_Sphalerite.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Zn_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/ZrF4-beta_sg84.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/ZrO2_sg137_Zirconia.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/ZrO2_sg14_Zirconia.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/Zr_sg194.ncmat
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/data/void.ncmat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.464545 ncrystal-3.6.dev82/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    39216 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/docs/ncmat_doc.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.468545 ncrystal-3.6.dev82/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/examples/NCrystal_example_mcstas.instr
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/examples/ncrystal_example_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/examples/ncrystal_example_cpp.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/examples/ncrystal_example_customphysics.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/examples/ncrystal_example_g4sim.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/examples/ncrystal_example_py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.468545 ncrystal-3.6.dev82/ncrystal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-14 18:10:46.000000 ncrystal-3.6.dev82/ncrystal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-07-14 18:10:46.000000 ncrystal-3.6.dev82/ncrystal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:10:46.000000 ncrystal-3.6.dev82/ncrystal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 18:10:46.000000 ncrystal-3.6.dev82/ncrystal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 18:10:46.000000 ncrystal-3.6.dev82/ncrystal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.440544 ncrystal-3.6.dev82/ncrystal_core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.440544 ncrystal-3.6.dev82/ncrystal_core/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.472545 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCAtomData.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCCompositionUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCDataSources.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCDefs.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCDump.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCException.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFact.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFactImpl.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFactRequests.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFactTypes.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFmt.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    16597 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCImmutBuf.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    28964 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCInfo.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCInfoBuilder.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCInfoTypes.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCLoadNCMAT.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    22448 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCMatCfg.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    20439 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCMem.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCNCMATData.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCParseNCMAT.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCPluginBoilerplate.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCPluginMgmt.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCProc.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCProcImpl.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCRNG.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCSABData.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCSCOrientation.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    39147 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCSmallVector.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    14618 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCTextData.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    37486 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCTypes.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    13171 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCVariant.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCVersion.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCrystal.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.480545 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCAbsOOV.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCAtomDB.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCAtomDBExtender.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCAtomUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCBkgdExtCurve.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    23020 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCCfgManip.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    32290 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCCfgTypes.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    35719 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCCfgVars.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCDebyeMSD.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCDynInfoUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCDynLoader.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCElIncScatter.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCElIncXS.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCEqRefl.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    19986 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFactoryUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFastConvolve.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFileUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFillHKL.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFreeGas.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFreeGasUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCGasMixUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCGaussMos.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCGaussOnSphere.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCIofQHelper.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCIter.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCKinUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCLCBragg.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCLCRefModels.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCLCUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCLatticeUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    27371 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCMath.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCMatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCOrientUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCPCBragg.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCPlaneProvider.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCPointwiseDist.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCRandUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCRomberg.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCRotMatrix.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABEval.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABExtender.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABFactory.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABIntegrator.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABSampler.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABSamplerModels.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABScatter.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABScatterHelper.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABUCN.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABXSProvider.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSANSSphScat.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSANSUtils.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSCBragg.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCScatKnlData.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSpan.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSpline.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    20113 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCStrView.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    15426 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCString.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCVDOSEval.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCVDOSGn.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCVDOSToScatKnl.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCVector.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/ncapi.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44878 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/ncrystal.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.492546 ncrystal-3.6.dev82/ncrystal_core/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCAbsOOV.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    36761 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCAtomDB.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9809 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCAtomDBExtender.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCAtomData.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCAtomUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCBkgdExtCurve.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    18374 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCCfgManip.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCCfgTypes.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    17901 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCCfgVars.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCCompositionUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    26184 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCDataSources.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCDebyeMSD.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCDefs.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    19704 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCDump.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCDynInfoUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCDynLoader.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCElIncScatter.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCElIncXS.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCEqRefl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCException.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFact.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    42888 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFactImpl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFactRequests.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFactTypes.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFactoryUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFactory_NCMAT.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFastConvolve.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFileUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    30178 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFillHKL.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFmt.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFreeGas.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    39971 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCFreeGasUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCGasMixFact.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    26599 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCGasMixUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCGaussMos.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    20586 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCGaussOnSphere.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12554 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCInfo.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    57518 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCInfoBuilder.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCIofQHelper.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCKinUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCLCBragg.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCLCRefModels.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    32322 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCLCUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    19509 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCLatticeUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCLauLazyFact.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    30601 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCLazy.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCLazy.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    33272 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCLoadNCMAT.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    48483 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCMatCfg.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23835 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCMath.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCMatrix.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCMem.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    31787 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCNCMATData.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCOrientUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCPCBragg.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    42614 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCParseNCMAT.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCPlaneProvider.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCPluginMgmt.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCPointwiseDist.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCProc.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    20199 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCProcImpl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCQuickFact.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCRNG.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCRandUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCRomberg.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCRotMatrix.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABData.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    31885 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABEval.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABExtender.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABFactory.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23449 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABIntegrator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABSampler.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12421 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABSamplerModels.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABScatter.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    26306 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABUCN.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    26746 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSABXSProvider.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSANSFact.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSANSSphScat.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSANSUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSCBragg.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSCOrientation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCScatKnlData.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCSpline.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCStdAbsFact.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCStdMPScatFact.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    18990 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCStdScatFact.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCStrView.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCString.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCTDProd.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCTextData.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCTypes.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    25936 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCVDOSEval.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15041 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCVDOSGn.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    38631 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCVDOSToScatKnl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCVector.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/NCVersion.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    72731 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_core/src/ncrystal.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.440544 ncrystal-3.6.dev82/ncrystal_geant4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.440544 ncrystal-3.6.dev82/ncrystal_geant4/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.492546 ncrystal-3.6.dev82/ncrystal_geant4/include/G4NCrystal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_geant4/include/G4NCrystal/G4NCInstall.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_geant4/include/G4NCrystal/G4NCManager.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_geant4/include/G4NCrystal/G4NCMatHelper.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_geant4/include/G4NCrystal/G4NCrystal.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.492546 ncrystal-3.6.dev82/ncrystal_geant4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCInstall.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCManager.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15023 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCMatHelper.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCProcWrapper.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCProcWrapper.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.492546 ncrystal-3.6.dev82/ncrystal_mcstas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_mcstas/NCrystal_example.instr
+-rw-r--r--   0 runner    (1001) docker     (123)    16072 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_mcstas/NCrystal_sample.comp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5054 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/ncrystal_mcstas/ncrystal_preparemcstasdir
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:10:46.492546 ncrystal-3.6.dev82/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15960 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/ncrystal_cif2ncmat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35171 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/ncrystal_endf2ncmat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    73858 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/ncrystal_hfg2ncmat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35971 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/ncrystal_inspectfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15231 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/ncrystal_ncmat2cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7659 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/ncrystal_ncmat2hkl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1998 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/ncrystal_onlinedb2ncmat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20289 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/ncrystal_vdos2ncmat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13315 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/ncrystal_verifyatompos
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35971 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/scripts/nctool
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 18:10:46.492546 ncrystal-3.6.dev82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-14 18:10:34.000000 ncrystal-3.6.dev82/setup.py
```

### Comparing `ncrystal-3.6.80/.github/ISSUE_TEMPLATE/feature_request.md` & `ncrystal-3.6.dev82/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/.github/ISSUE_TEMPLATE/request-for-new-material.md` & `ncrystal-3.6.dev82/.github/ISSUE_TEMPLATE/request-for-new-material.md`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/.github/workflows/cmake.yml` & `ncrystal-3.6.dev82/.github/workflows/cmake.yml`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/CHANGELOG` & `ncrystal-3.6.dev82/CHANGELOG`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v3.6.82 2023-07-13
+      * RC3 for release 3.7.0.
+
+v3.6.81 2023-06-23
+      * RC2 for release 3.7.0.
+
 v3.6.80 2023-06-07
       * RC1 for release 3.7.0.
 
 v3.6.1 2023-05-16
       * Tiny update with a quick workaround for gcc12 compilation issues
         (github issue #125).
```

### Comparing `ncrystal-3.6.80/CMakeLists.txt` & `ncrystal-3.6.dev82/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ##                                                                            ##
 ################################################################################
 
 ##################################################################################
 #                                                                                #
 # CMake file which can be used to compile and link all files distributed with    #
 # NCrystal, and which provides CMake configuration files and setup.sh/unsetup.sh #
-# for subsequent usage.                                                          #
+# for subsequent usage (also ncrystal_setup.sh/ncrystal_unsetup.sh).             #
 #                                                                                #
 # One way to invoke cmake to build and install would be like this (run this from #
 # a temporary build dir)                                                         #
 #                                                                                #
 #  $> cmake /path/to/sourcedir -DCMAKE_INSTALL_PREFIX=/path/to/installdir        #
 #                                                                                #
 # Followed by (replace the number 8 by the number of processes you want to       #
@@ -82,15 +82,15 @@
 list( APPEND _project_metadata DESCRIPTION "Library for thermal neutron transport in crystals and other materials" )
 if( "${CMAKE_VERSION}" VERSION_GREATER_EQUAL "3.12.0" )
   list( APPEND _project_metadata HOMEPAGE_URL "https://github.com/mctools/ncrystal" )
 endif()
 
 cmake_policy( SET CMP0048 NEW )#Not sure if this is really needed
 
-project( NCrystal VERSION 3.6.80 ${_project_metadata} )
+project( NCrystal VERSION 3.6.82 ${_project_metadata} )
 
 unset( _project_metadata )
 
 if( NOT NCRYSTAL_NOTOUCH_CMAKE_BUILD_TYPE )
   if ( NOT gen_is_multicfg )
     if ( NOT CMAKE_BUILD_TYPE )
       #This can happen if parent project called the project(..) function before
@@ -694,14 +694,16 @@
 
 
 if ( NCRYSTAL_ENABLE_SETUPSH )
   configure_file( "${PROJECT_SOURCE_DIR}/cmake/template_setup.sh.in" "${PROJECT_BINARY_DIR}/generated_setup.sh" @ONLY )
   configure_file( "${PROJECT_SOURCE_DIR}/cmake/template_unsetup.sh.in" "${PROJECT_BINARY_DIR}/generated_unsetup.sh" @ONLY )
   ncinstall( FILES "${PROJECT_BINARY_DIR}/generated_setup.sh" DESTINATION . RENAME setup.sh )
   ncinstall( FILES "${PROJECT_BINARY_DIR}/generated_unsetup.sh" DESTINATION . RENAME unsetup.sh )
+  ncinstall( FILES "${PROJECT_BINARY_DIR}/generated_setup.sh" DESTINATION . RENAME ncrystal_setup.sh )
+  ncinstall( FILES "${PROJECT_BINARY_DIR}/generated_unsetup.sh" DESTINATION . RENAME ncrystal_unsetup.sh )
 endif()
 
 if ( NOT NCRYSTAL_QUIET )
   foreach( optname ${_NCrystal_all_opts} )
     message( STATUS "NCrystal-cfg: ${optname}=${${optname}}" )
   endforeach()
 endif()
```

### Comparing `ncrystal-3.6.80/FILES` & `ncrystal-3.6.dev82/FILES`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/INSTALL` & `ncrystal-3.6.dev82/INSTALL`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/LICENSE` & `ncrystal-3.6.dev82/LICENSE`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/NCrystal/__init__.py` & `ncrystal-3.6.dev82/NCrystal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 ##  See the License for the specific language governing permissions and       ##
 ##  limitations under the License.                                            ##
 ##                                                                            ##
 ################################################################################
 
 #NB: Synchronize meta-data below with fields in setup.py+template_setup.py.in meta data:
 __license__ = "Apache 2.0, http://www.apache.org/licenses/LICENSE-2.0"
-__version__ = '3.6.80'
+__version__ = '3.6.82'
 __status__ = "Production"
 __author__ = "NCrystal developers (Thomas Kittelmann, Xiao Xiao Cai)"
 __copyright__ = "Copyright 2015-2023 %s"%__author__
 __maintainer__ = __author__
 __email__ = "ncrystal-developers@cern.ch"
 
 #Place f-string here to catch python <3.6 in a more obvious way than a syntax error below:
```

### Comparing `ncrystal-3.6.80/NCrystal/_chooks.py` & `ncrystal-3.6.dev82/NCrystal/_chooks.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/NCrystal/_common.py` & `ncrystal-3.6.dev82/NCrystal/_common.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/NCrystal/_coreimpl.py` & `ncrystal-3.6.dev82/NCrystal/_coreimpl.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/NCrystal/_miscimpl.py` & `ncrystal-3.6.dev82/NCrystal/_miscimpl.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/NCrystal/_ncmatimpl.py` & `ncrystal-3.6.dev82/NCrystal/_ncmatimpl.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/NCrystal/_numpy.py` & `ncrystal-3.6.dev82/NCrystal/_numpy.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/NCrystal/api.py` & `ncrystal-3.6.dev82/NCrystal/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,20 +33,20 @@
 ################################################################################
 
 #NB: reduce imported symbols here a bit in a future release (possibly by
 #wrapping the removed function and placing in obsolete.py);
 from .exceptions import *
 from .core import *
 from .datasrc import *
-from .constants import wl2ekin, ekin2wl, ekin2ksq, wl2k, wl2ksq, constant_boltzmann #TODO: only wl2ekin, ekin2wl
+from .constants import wl2ekin, ekin2wl, ekin2ksq, wl2k, wl2ksq, constant_boltzmann #TODO: only wl2ekin, ekin2wl (or all?)
 from .atomdata import atomDB, iterateAtomDB
 from .cfgstr import normaliseCfg, decodeCfg, generateCfgStrDoc
 from .ncmat import NCMATComposer, formatVectorForNCMAT
 from .plugins import hasFactory, browsePlugins
-from ._testimpl import test
+from ._testimpl import *
 from .vdos import createVDOSDebye, debyeIsotropicMSD, PhononDOSAnalyser, debyeTempFromIsotropicMSD, analyseVDOS
 from .obsolete import *
 
 #Some modules are left out on purpose (due to esoteric usage or non-standard
 #dependencies that most users might not need):
 #
 # from .cifutils import *
```

### Comparing `ncrystal-3.6.80/NCrystal/atomdata.py` & `ncrystal-3.6.dev82/NCrystal/atomdata.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/NCrystal/cfgstr.py` & `ncrystal-3.6.dev82/NCrystal/cfgstr.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/NCrystal/cifutils.py` & `ncrystal-3.6.dev82/NCrystal/cifutils.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/NCrystal/constants.py` & `ncrystal-3.6.dev82/NCrystal/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 ##  distributed under the License is distributed on an "AS IS" BASIS,         ##
 ##  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  ##
 ##  See the License for the specific language governing permissions and       ##
 ##  limitations under the License.                                            ##
 ##                                                                            ##
 ################################################################################
 
-#some constants (NB: Copied here from NCMath.hh - must keep synchronized!! Also,
-#remember to include in __all__ list above):
+#some constants (NB: Copied here from NCMath.hh - must keep synchronized!!):
 
 constant_c  = 299792458e10#  speed of light in Aa/s
 constant_dalton2kg =  1.660539040e-27#  amu to kg
 constant_dalton2eVc2 =  931494095.17#  amu to eV/c^2
 constant_avogadro = 6.022140857e23#  mol^-1
 constant_boltzmann = 8.6173303e-5#  eV/K
 const_neutron_mass_amu = 1.00866491588#  [amu]
@@ -119,7 +118,15 @@
         return k2Pi * _np.where( wlnonzero, wlinv, kInf )
     else:
         return k2Pi / wl if wl else kInf
 
 def wl2ksq( wl ):
     """Neutron wavelength (angstrom) to wavenumber squared, (k^2, in units of 1/angstrom^2)"""
     return ( wl2k(wl) )**2
+
+def k2wl( k ):
+    """Wavenumber, (k, in units of 1/angstrom) to neutron wavelength (angstrom)"""
+    return wl2k( k )#using that k2wl = wl2k (both are f(x)=2pi/x)
+
+def k2ekin( k ):
+    """Wavenumber, (k, in units of 1/angstrom) to neutron energy (eV)"""
+    return ksq2ekin( k * k )
```

### Comparing `ncrystal-3.6.80/NCrystal/core.py` & `ncrystal-3.6.dev82/NCrystal/core.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/NCrystal/datasrc.py` & `ncrystal-3.6.dev82/NCrystal/datasrc.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/NCrystal/exceptions.py` & `ncrystal-3.6.dev82/NCrystal/exceptions.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/NCrystal/mcstasutils.py` & `ncrystal-3.6.dev82/NCrystal/mcstasutils.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/NCrystal/misc.py` & `ncrystal-3.6.dev82/NCrystal/misc.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/NCrystal/ncmat.py` & `ncrystal-3.6.dev82/NCrystal/ncmat.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,17 @@
     the resulting NCMAT data. As a convenience the .write() and .register_as()
     methods can be used to write this data as a physical or virtual file
     respectively, or the .load() method can be used to directly load the
     data. Finally, the .plot_xsect() and .inspect() methods can also be used to
     quickly load and investigate the material. It might also be useful to print
     the output of .create_ncmat(), to understand what material has been created.
 
-    For a more in-depth discussion and usage examples, please refer to the wiki
-    page at https://github.com/mctools/ncrystal/wiki/NCMATComposer [fixme?]
-    TODO: Add link here to online tutorial once it is ready.
+    For a more in-depth discussion and usage examples, please refer to the
+    example Jupyter-Lab notebooks in the
+    https://github.com/mctools/ncrystal-notebooks repository.
 
     Note that the "labels" used in the various methods, to identify different
     atoms in the materials are custom user labels. They are simply a way to
     provide a handle associated with a particular atom role or species in the
     material. For many simple materials, all labels will simply have the name of
     the element or isotope ("Al", "Li6", "D", ...), and each type of element and
     isotope will only appear once in the material. That is certainly OK, for
@@ -75,14 +75,15 @@
     by default have their crystal structure verified for consistency with the
     indicated spacegroup, before it is converted to NCMAT data. For that reason,
     the third-party module "spglib" must be installed in order for this
     verification to take place (note that the .refine_crystal_structure() method
     can also be invoked before the material is used, to detect the spacegroup in
     if it was not provided). Fortunately, "spglib" is available both on PyPI and
     in the conda-forge conda channel.
+
     """
 
     def __init__(self, data = None, fmt = None, quiet = False, plotlabel = None ):
         """Initialise. Either an empty instance, or if data (and possibly fmt)
         is provided, from a variety of data. Typically, the fmt parameter can be
         left out, but occasionally it might be needed to specify it
         explicitly. Supported fmt's are "cif", "cfgstr", "ncmat", (for NCMAT
```

### Comparing `ncrystal-3.6.80/NCrystal/obsolete.py` & `ncrystal-3.6.dev82/NCrystal/obsolete.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/NCrystal/plot.py` & `ncrystal-3.6.dev82/NCrystal/plot.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/NCrystal/plugins.py` & `ncrystal-3.6.dev82/NCrystal/plugins.py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/NCrystal/test.py` & `ncrystal-3.6.dev82/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-"""
-
-Module which is intended to trigger the built-in test from the command line by running python3 -m NCrystal.test
-
-"""
 
 ################################################################################
 ##                                                                            ##
 ##  This file is part of NCrystal (see https://mctools.github.io/ncrystal/)   ##
 ##                                                                            ##
 ##  Copyright 2015-2023 NCrystal developers                                   ##
 ##                                                                            ##
@@ -20,10 +15,21 @@
 ##  distributed under the License is distributed on an "AS IS" BASIS,         ##
 ##  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  ##
 ##  See the License for the specific language governing permissions and       ##
 ##  limitations under the License.                                            ##
 ##                                                                            ##
 ################################################################################
 
-if __name__ == '__main__':
-    from ._testimpl import test
-    test()
+[build-system]
+requires = [
+    "setuptools>=42",
+    "scikit-build>=0.13",
+    "cmake>=3.18",
+    "numpy"
+]
+build-backend = "setuptools.build_meta"
+
+[tool.cibuildwheel]
+test-command = [
+  "python3 -mNCrystal.test all",
+  "nctool --test",
+]
```

### Comparing `ncrystal-3.6.80/NCrystal/vdos.py` & `ncrystal-3.6.dev82/NCrystal/vdos.py`

 * *Files 0% similar despite different names*

```diff
@@ -578,15 +578,14 @@
                     continue
                 c.set_dyninfo_vdos( lblmap[lbl], comment = 'From PhononDOSAnalyser', **o.get_dyninfo_args(lbl) )
             if not color:
                 plot_kwargs['color'] = colorder[iplot%len(colorder)]
             plot_kwargs['labelfct'] = lambda x : thr_description
             c.plot_xsect( **plot_kwargs )
 
-        #fixme: plt_final?
         if do_legend:
             plt.legend()
         if do_grid:
             plt.grid()
         t = 'DOS cutoff effect'
         if cfg_params:
             t += ' (%s)'%cfg_params.strip()
```

### Comparing `ncrystal-3.6.80/NOTICE` & `ncrystal-3.6.dev82/NOTICE`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/PKG-INFO` & `ncrystal-3.6.dev82/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncrystal
-Version: 3.6.80
+Version: 3.6.dev82
 Summary: Library for thermal neutron transport in crystals and other materials.
 Home-page: https://github.com/mctools/ncrystal/wiki
 Author: NCrystal developers (Thomas Kittelmann, Xiao Xiao Cai)
 License: Apache-2.0
 Keywords: neutron,montecarlo,science
 Requires-Python: >=3.6, <4
 License-File: LICENSE
```

### Comparing `ncrystal-3.6.80/README` & `ncrystal-3.6.dev82/README`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/cmake/NCrystalConfig.cmake.in` & `ncrystal-3.6.dev82/cmake/NCrystalConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/cmake/modules/ncrystal_legacyoptions.cmake` & `ncrystal-3.6.dev82/cmake/modules/ncrystal_legacyoptions.cmake`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/cmake/modules/ncrystal_options.cmake` & `ncrystal-3.6.dev82/cmake/modules/ncrystal_options.cmake`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/cmake/modules/ncrystal_utils.cmake` & `ncrystal-3.6.dev82/cmake/modules/ncrystal_utils.cmake`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/cmake/ncrystal-config.in` & `ncrystal-3.6.dev82/cmake/ncrystal-config.in`

 * *Files 5% similar despite different names*

```diff
@@ -92,23 +92,24 @@
         f = NCrystal.__file__
     except ImportError:
         f = None
     if f:
         f = pathlib.Path(f).parent / 'ncrystal_pyinst_data'
         if not f.exists() or not f.is_dir():
             f = None
-        if not ( f / 'lib' / nfo['libname'] ).exists():
+        if not f or not ( f / 'lib' / nfo['libname'] ).exists():
             f = None
     if f is None:
         raise SystemExit('Invalid installation. Could not locate the NCrystal library.')
     #Ok, let us fix up stuff:
     d = {}
     d['libdir'] = f / 'lib'
     if nfo['datadir'] is not None:
-        d['datadir'] = f / 'data' / 'NCrystal' /  'data'#Fixme verify this!!!
+        d['datadir'] = f / 'stdlib_data'# NB: Does not 100% work, since libNCrystal.so can
+                                        #     not find it unless NCRYSTAL_DATADIR is set.
     if nfo['mcstasdir'] is not None:
         d['mcstasdir'] = f / 'data' / 'NCrystal' / 'mcstas'
     d['pythonpath'] = f.parent.parent
     d['cmakedir'] = f / 'lib' / 'cmake' / 'NCrystal'
     d['prefix'] = None
     d['includedir'] = f / 'include'
     d['libpath'] =  f / 'lib' / nfo['libname']
```

### Comparing `ncrystal-3.6.80/cmake/template_setup.py.in` & `ncrystal-3.6.dev82/cmake/template_setup.py.in`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/cmake/template_setup.sh.in` & `ncrystal-3.6.dev82/cmake/template_setup.sh.in`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/cmake/template_unsetup.sh.in` & `ncrystal-3.6.dev82/cmake/template_unsetup.sh.in`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/AcrylicGlass_C5O2H8.ncmat` & `ncrystal-3.6.dev82/data/AcrylicGlass_C5O2H8.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/AgBr_sg225_SilverBromide.ncmat` & `ncrystal-3.6.dev82/data/AgBr_sg225_SilverBromide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Ag_sg225.ncmat` & `ncrystal-3.6.dev82/data/Ag_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Al2O3_sg167_Corundum.ncmat` & `ncrystal-3.6.dev82/data/Al2O3_sg167_Corundum.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Al4C3_sg166_AluminiumCarbide.ncmat` & `ncrystal-3.6.dev82/data/Al4C3_sg166_AluminiumCarbide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/AlN_sg186_AluminumNitride.ncmat` & `ncrystal-3.6.dev82/data/AlN_sg186_AluminumNitride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Al_sg225.ncmat` & `ncrystal-3.6.dev82/data/Al_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Ar_Gas_STP.ncmat` & `ncrystal-3.6.dev82/data/Ar_Gas_STP.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Au_sg225.ncmat` & `ncrystal-3.6.dev82/data/Au_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/BaF2_sg225_BariumFluoride.ncmat` & `ncrystal-3.6.dev82/data/BaF2_sg225_BariumFluoride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/BaO_sg225_BariumOxide.ncmat` & `ncrystal-3.6.dev82/data/BaO_sg225_BariumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Ba_sg229.ncmat` & `ncrystal-3.6.dev82/data/Ba_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Be3N2_sg206_BerylliumNitride.ncmat` & `ncrystal-3.6.dev82/data/Be3N2_sg206_BerylliumNitride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/BeF2_sg152_Beryllium_Fluoride.ncmat` & `ncrystal-3.6.dev82/data/BeF2_sg152_Beryllium_Fluoride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/BeO_sg186.ncmat` & `ncrystal-3.6.dev82/data/BeO_sg186.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Be_sg194.ncmat` & `ncrystal-3.6.dev82/data/Be_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Bi_sg166.ncmat` & `ncrystal-3.6.dev82/data/Bi_sg166.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/C_sg194_pyrolytic_graphite.ncmat` & `ncrystal-3.6.dev82/data/C_sg194_pyrolytic_graphite.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/C_sg227_Diamond.ncmat` & `ncrystal-3.6.dev82/data/C_sg227_Diamond.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/CaCO3_sg62_Aragonite.ncmat` & `ncrystal-3.6.dev82/data/CaCO3_sg62_Aragonite.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/CaF2_sg225_CalciumFlouride.ncmat` & `ncrystal-3.6.dev82/data/CaF2_sg225_CalciumFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/CaH2_sg62_CalciumHydride.ncmat` & `ncrystal-3.6.dev82/data/CaH2_sg62_CalciumHydride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/CaO2H2_sg164_CalciumHydroxide.ncmat` & `ncrystal-3.6.dev82/data/CaO2H2_sg164_CalciumHydroxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/CaO_sg225_CalciumOxide.ncmat` & `ncrystal-3.6.dev82/data/CaO_sg225_CalciumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/CaSiO3_sg2_Wollastonite.ncmat` & `ncrystal-3.6.dev82/data/CaSiO3_sg2_Wollastonite.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Ca_sg225.ncmat` & `ncrystal-3.6.dev82/data/Ca_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Ca_sg229_Calcium-gamma.ncmat` & `ncrystal-3.6.dev82/data/Ca_sg229_Calcium-gamma.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/CeO2_sg225_CeriumOxide.ncmat` & `ncrystal-3.6.dev82/data/CeO2_sg225_CeriumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Cr_sg229.ncmat` & `ncrystal-3.6.dev82/data/Cr_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Cu2O_sg224_Cuprite.ncmat` & `ncrystal-3.6.dev82/data/Cu2O_sg224_Cuprite.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Cu_sg225.ncmat` & `ncrystal-3.6.dev82/data/Cu_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Dy2O3_sg206_DysprosiumOxide.ncmat` & `ncrystal-3.6.dev82/data/Dy2O3_sg206_DysprosiumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Epoxy_Araldite506_C18H20O3.ncmat` & `ncrystal-3.6.dev82/data/Epoxy_Araldite506_C18H20O3.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Fe_sg225_Iron-gamma.ncmat` & `ncrystal-3.6.dev82/data/Fe_sg225_Iron-gamma.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Fe_sg229_Iron-alpha.ncmat` & `ncrystal-3.6.dev82/data/Fe_sg229_Iron-alpha.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/GaN_sg186_GalliumNitride.ncmat` & `ncrystal-3.6.dev82/data/GaN_sg186_GalliumNitride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/GaSe_sg194_GalliumSelenide.ncmat` & `ncrystal-3.6.dev82/data/GaSe_sg194_GalliumSelenide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Ge3Bi4O12_sg220_BismuthGermanate.ncmat` & `ncrystal-3.6.dev82/data/Ge3Bi4O12_sg220_BismuthGermanate.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Ge_sg227.ncmat` & `ncrystal-3.6.dev82/data/Ge_sg227.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/He_Gas_STP.ncmat` & `ncrystal-3.6.dev82/data/He_Gas_STP.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/HfO2_sg14_HafniumOxide.ncmat` & `ncrystal-3.6.dev82/data/HfO2_sg14_HafniumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Ho2O3_sg206_HolmiumOxide.ncmat` & `ncrystal-3.6.dev82/data/Ho2O3_sg206_HolmiumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/KBr_sg225_PotassiumBromide.ncmat` & `ncrystal-3.6.dev82/data/KBr_sg225_PotassiumBromide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/KF_sg225_PotassiumFlouride.ncmat` & `ncrystal-3.6.dev82/data/KF_sg225_PotassiumFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/KOH_sg4_PotassiumHydroxide.ncmat` & `ncrystal-3.6.dev82/data/KOH_sg4_PotassiumHydroxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/K_sg229.ncmat` & `ncrystal-3.6.dev82/data/K_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Kapton_C22H10N2O5.ncmat` & `ncrystal-3.6.dev82/data/Kapton_C22H10N2O5.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Kr_Gas_STP.ncmat` & `ncrystal-3.6.dev82/data/Kr_Gas_STP.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/LaBr3_sg176_LanthanumBromide.ncmat` & `ncrystal-3.6.dev82/data/LaBr3_sg176_LanthanumBromide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Li2O_sg225_LithiumOxide.ncmat` & `ncrystal-3.6.dev82/data/Li2O_sg225_LithiumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Li3N_sg191_LithiumNitride.ncmat` & `ncrystal-3.6.dev82/data/Li3N_sg191_LithiumNitride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/LiF_sg225_LithiumFlouride.ncmat` & `ncrystal-3.6.dev82/data/LiF_sg225_LithiumFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/LiH_sg225_LithiumHydride.ncmat` & `ncrystal-3.6.dev82/data/LiH_sg225_LithiumHydride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/LiquidHeavyWaterD2O_T293.6K.ncmat` & `ncrystal-3.6.dev82/data/LiquidHeavyWaterD2O_T293.6K.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/LiquidWaterH2O_T293.6K.ncmat` & `ncrystal-3.6.dev82/data/LiquidWaterH2O_T293.6K.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Lu2O3_sg206_LutetiumOxide.ncmat` & `ncrystal-3.6.dev82/data/Lu2O3_sg206_LutetiumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Lu2SiO5_sg15.ncmat` & `ncrystal-3.6.dev82/data/Lu2SiO5_sg15.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Mg2SiO4_sg62_MagnesiumSilicate.ncmat` & `ncrystal-3.6.dev82/data/Mg2SiO4_sg62_MagnesiumSilicate.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/MgAl2O4_sg227_MAS.ncmat` & `ncrystal-3.6.dev82/data/MgAl2O4_sg227_MAS.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/MgCO3_sg167_MagnesiumCarbonate.ncmat` & `ncrystal-3.6.dev82/data/MgCO3_sg167_MagnesiumCarbonate.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/MgD2_sg136_MagnesiumDeuteride.ncmat` & `ncrystal-3.6.dev82/data/MgD2_sg136_MagnesiumDeuteride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/MgF2_sg136_MagnesiumFlouride.ncmat` & `ncrystal-3.6.dev82/data/MgF2_sg136_MagnesiumFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/MgH2_sg136_MagnesiumHydride.ncmat` & `ncrystal-3.6.dev82/data/MgH2_sg136_MagnesiumHydride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/MgO2H2_sg164_MagnesiumHydroxide.ncmat` & `ncrystal-3.6.dev82/data/MgO2H2_sg164_MagnesiumHydroxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/MgO_sg225_Periclase.ncmat` & `ncrystal-3.6.dev82/data/MgO_sg225_Periclase.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Mg_sg194.ncmat` & `ncrystal-3.6.dev82/data/Mg_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Mo_sg229.ncmat` & `ncrystal-3.6.dev82/data/Mo_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Na4Si3Al3O12Cl_sg218_Sodalite.ncmat` & `ncrystal-3.6.dev82/data/Na4Si3Al3O12Cl_sg218_Sodalite.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/NaBr_sg225_SodiumBromide.ncmat` & `ncrystal-3.6.dev82/data/NaBr_sg225_SodiumBromide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/NaCl_sg225_SodiumChloride.ncmat` & `ncrystal-3.6.dev82/data/NaCl_sg225_SodiumChloride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/NaF_sg225_SodiumFlouride.ncmat` & `ncrystal-3.6.dev82/data/NaF_sg225_SodiumFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/NaI_sg225_SodiumIodide.ncmat` & `ncrystal-3.6.dev82/data/NaI_sg225_SodiumIodide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Na_sg229.ncmat` & `ncrystal-3.6.dev82/data/Na_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Nb_sg229.ncmat` & `ncrystal-3.6.dev82/data/Nb_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Ne_Gas_STP.ncmat` & `ncrystal-3.6.dev82/data/Ne_Gas_STP.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Ni_sg225.ncmat` & `ncrystal-3.6.dev82/data/Ni_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Nylon11_C11H21NO.ncmat` & `ncrystal-3.6.dev82/data/Nylon11_C11H21NO.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Nylon12_C12H23NO.ncmat` & `ncrystal-3.6.dev82/data/Nylon12_C12H23NO.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Nylon610_C16H30N2O2.ncmat` & `ncrystal-3.6.dev82/data/Nylon610_C16H30N2O2.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Nylon66or6_C12H22N2O2.ncmat` & `ncrystal-3.6.dev82/data/Nylon66or6_C12H22N2O2.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/PEEK_C19H12O3.ncmat` & `ncrystal-3.6.dev82/data/PEEK_C19H12O3.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/PVC_C2H3Cl.ncmat` & `ncrystal-3.6.dev82/data/PVC_C2H3Cl.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/PbF2-beta_sg225_BetaLeadFlouride.ncmat` & `ncrystal-3.6.dev82/data/PbF2-beta_sg225_BetaLeadFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/PbO-alpha_sg129_Litharge.ncmat` & `ncrystal-3.6.dev82/data/PbO-alpha_sg129_Litharge.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/PbO-beta_sg57_Massicot.ncmat` & `ncrystal-3.6.dev82/data/PbO-beta_sg57_Massicot.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/PbS_sg225_LeadSulfide.ncmat` & `ncrystal-3.6.dev82/data/PbS_sg225_LeadSulfide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Pb_sg225.ncmat` & `ncrystal-3.6.dev82/data/Pb_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Pd_sg225.ncmat` & `ncrystal-3.6.dev82/data/Pd_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Polycarbonate_C16O3H14.ncmat` & `ncrystal-3.6.dev82/data/Polycarbonate_C16O3H14.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Polyester_C10H8O4.ncmat` & `ncrystal-3.6.dev82/data/Polyester_C10H8O4.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Polyethylene_CH2.ncmat` & `ncrystal-3.6.dev82/data/Polyethylene_CH2.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Polylactide_C3H4O2.ncmat` & `ncrystal-3.6.dev82/data/Polylactide_C3H4O2.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Polypropylene_C3H6.ncmat` & `ncrystal-3.6.dev82/data/Polypropylene_C3H6.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Polystyrene_C8H8.ncmat` & `ncrystal-3.6.dev82/data/Polystyrene_C8H8.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Pt_sg225.ncmat` & `ncrystal-3.6.dev82/data/Pt_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Rb_sg229.ncmat` & `ncrystal-3.6.dev82/data/Rb_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Rubber_C5H8.ncmat` & `ncrystal-3.6.dev82/data/Rubber_C5H8.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Sc_sg194.ncmat` & `ncrystal-3.6.dev82/data/Sc_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/SiC-beta_sg216_BetaSiliconCarbide.ncmat` & `ncrystal-3.6.dev82/data/SiC-beta_sg216_BetaSiliconCarbide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/SiO2-alpha_sg154_AlphaQuartz.ncmat` & `ncrystal-3.6.dev82/data/SiO2-alpha_sg154_AlphaQuartz.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/SiO2-beta_sg180_BetaQuartz.ncmat` & `ncrystal-3.6.dev82/data/SiO2-beta_sg180_BetaQuartz.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Si_sg227.ncmat` & `ncrystal-3.6.dev82/data/Si_sg227.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Sn_sg141.ncmat` & `ncrystal-3.6.dev82/data/Sn_sg141.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/SrF2_sg225_StrontiumFluoride.ncmat` & `ncrystal-3.6.dev82/data/SrF2_sg225_StrontiumFluoride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/SrH2_sg62_StrontiumHydride.ncmat` & `ncrystal-3.6.dev82/data/SrH2_sg62_StrontiumHydride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Sr_sg225.ncmat` & `ncrystal-3.6.dev82/data/Sr_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Th3N4_sg166_ThoriumNitride.ncmat` & `ncrystal-3.6.dev82/data/Th3N4_sg166_ThoriumNitride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/ThO2_sg225_ThoriumDioxide.ncmat` & `ncrystal-3.6.dev82/data/ThO2_sg225_ThoriumDioxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Th_sg225.ncmat` & `ncrystal-3.6.dev82/data/Th_sg225.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/TiO2_sg136_Rutile.ncmat` & `ncrystal-3.6.dev82/data/TiO2_sg136_Rutile.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/TiO2_sg141_Anatase.ncmat` & `ncrystal-3.6.dev82/data/TiO2_sg141_Anatase.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Ti_sg194.ncmat` & `ncrystal-3.6.dev82/data/Ti_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/TlBr_sg221_ThaliumBromide.ncmat` & `ncrystal-3.6.dev82/data/TlBr_sg221_ThaliumBromide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Tm2O3_sg206_ThuliumOxide.ncmat` & `ncrystal-3.6.dev82/data/Tm2O3_sg206_ThuliumOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/UF6_sg62_UraniumHexaflouride.ncmat` & `ncrystal-3.6.dev82/data/UF6_sg62_UraniumHexaflouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/UO2_sg225_UraniumDioxide.ncmat` & `ncrystal-3.6.dev82/data/UO2_sg225_UraniumDioxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/V_sg229.ncmat` & `ncrystal-3.6.dev82/data/V_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/W_sg229.ncmat` & `ncrystal-3.6.dev82/data/W_sg229.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Xe_Gas_STP.ncmat` & `ncrystal-3.6.dev82/data/Xe_Gas_STP.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Y2O3_sg206_Yttrium_Oxide.ncmat` & `ncrystal-3.6.dev82/data/Y2O3_sg206_Yttrium_Oxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Y2SiO5_sg15_YSO.ncmat` & `ncrystal-3.6.dev82/data/Y2SiO5_sg15_YSO.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Y3Al5O12_sg230_YAG.ncmat` & `ncrystal-3.6.dev82/data/Y3Al5O12_sg230_YAG.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Y_sg194.ncmat` & `ncrystal-3.6.dev82/data/Y_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/ZnF2_sg136_ZincFlouride.ncmat` & `ncrystal-3.6.dev82/data/ZnF2_sg136_ZincFlouride.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/ZnO_sg186_ZincOxide.ncmat` & `ncrystal-3.6.dev82/data/ZnO_sg186_ZincOxide.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/ZnS_sg216_Sphalerite.ncmat` & `ncrystal-3.6.dev82/data/ZnS_sg216_Sphalerite.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Zn_sg194.ncmat` & `ncrystal-3.6.dev82/data/Zn_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/ZrF4-beta_sg84.ncmat` & `ncrystal-3.6.dev82/data/ZrF4-beta_sg84.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/ZrO2_sg137_Zirconia.ncmat` & `ncrystal-3.6.dev82/data/ZrO2_sg137_Zirconia.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/ZrO2_sg14_Zirconia.ncmat` & `ncrystal-3.6.dev82/data/ZrO2_sg14_Zirconia.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/Zr_sg194.ncmat` & `ncrystal-3.6.dev82/data/Zr_sg194.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/data/void.ncmat` & `ncrystal-3.6.dev82/data/void.ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/docs/ncmat_doc.md` & `ncrystal-3.6.dev82/docs/ncmat_doc.md`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/examples/NCrystal_example_mcstas.instr` & `ncrystal-3.6.dev82/examples/NCrystal_example_mcstas.instr`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/examples/ncrystal_example_c.c` & `ncrystal-3.6.dev82/examples/ncrystal_example_c.c`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/examples/ncrystal_example_cpp.cc` & `ncrystal-3.6.dev82/examples/ncrystal_example_cpp.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/examples/ncrystal_example_customphysics.cc` & `ncrystal-3.6.dev82/examples/ncrystal_example_customphysics.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/examples/ncrystal_example_g4sim.cc` & `ncrystal-3.6.dev82/examples/ncrystal_example_g4sim.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/examples/ncrystal_example_py` & `ncrystal-3.6.dev82/examples/ncrystal_example_py`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal.egg-info/PKG-INFO` & `ncrystal-3.6.dev82/ncrystal.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncrystal
-Version: 3.6.80
+Version: 3.6.dev82
 Summary: Library for thermal neutron transport in crystals and other materials.
 Home-page: https://github.com/mctools/ncrystal/wiki
 Author: NCrystal developers (Thomas Kittelmann, Xiao Xiao Cai)
 License: Apache-2.0
 Keywords: neutron,montecarlo,science
 Requires-Python: >=3.6, <4
 License-File: LICENSE
```

### Comparing `ncrystal-3.6.80/ncrystal.egg-info/SOURCES.txt` & `ncrystal-3.6.dev82/ncrystal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCAtomData.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCAtomData.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCCompositionUtils.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCCompositionUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCDataSources.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCDataSources.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCDefs.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCDefs.hh`

 * *Files 3% similar despite different names*

```diff
@@ -53,24 +53,30 @@
 #endif
 #ifndef NCrystal_NCMem_hh
 #  include "NCrystal/NCMem.hh"
 #endif
 
 namespace NCrystal {
 
-  //Utility functions for converting between neutron wavelength [Aa], kinetic
-  //energy [eV], and wavenumber k=2pi/lambda [1/Aa]:
-  NCRYSTAL_API constexpr double wl2ekin( double wl ) noexcept;     //cost: 1 branch + 1 division + 1 mult
-  NCRYSTAL_API constexpr double ekin2wl( double ekin ) noexcept;   //cost: 1 branch + 1 division + 1 sqrt
+  //Untyped utility functions for converting between neutron wavelength [Aa],
+  //kinetic energy [eV], and wavenumber k=2pi/lambda [1/Aa]:
+  NCRYSTAL_API constexpr double wl2ekin( double wl ) noexcept; //cost: 1 branch + 1 division + 1 mult
+  NCRYSTAL_API double ekin2wl( double ekin ) noexcept; //cost: 1 branch + 1 division + 1 sqrt
+  NCRYSTAL_API constexpr double constexpr_ekin2wl( double ekin ) noexcept;//expensive, use only compiletime
   NCRYSTAL_API constexpr double ekin2wlsq( double ekin ) noexcept; //cost: 1 branch + 1 division
   NCRYSTAL_API constexpr double ekin2wlsqinv( double ekin ) noexcept; //cost: 1 multiplication
-  NCRYSTAL_API constexpr double wlsq2ekin( double wl ) noexcept;   //cost: 1 branch + 1 division
-  NCRYSTAL_API constexpr double ekin2ksq( double ekin ) noexcept;   //cost: 1 multiplication
-  NCRYSTAL_API constexpr double ksq2ekin( double ksq ) noexcept;   //cost: 1 multiplication
-  NCRYSTAL_API constexpr double wl2k( double wl ) noexcept;     //cost: 1 branch + 1 division
+  NCRYSTAL_API constexpr double wlsq2ekin( double wl ) noexcept; //cost: 1 branch + 1 division
+  NCRYSTAL_API constexpr double ekin2ksq( double ekin ) noexcept; //cost: 1 multiplication
+  NCRYSTAL_API double ekin2k( double ekin ) noexcept; //cost: 1 multiplication + 1 sqrt
+  NCRYSTAL_API constexpr double constexpr_ekin2k( double ekin ) noexcept;//expensive, use only compiletime
+  NCRYSTAL_API constexpr double ksq2ekin( double ksq ) noexcept; //cost: 1 multiplication
+  NCRYSTAL_API constexpr double k2ekin( double k ) noexcept; //cost: 2 multiplications
+  NCRYSTAL_API constexpr double wl2k( double wl ) noexcept; //cost: 1 branch + 1 division
+  NCRYSTAL_API constexpr double wl2ksq( double wl ) noexcept; //cost: 1 branch + 1 division + 1 multiplication
+  NCRYSTAL_API constexpr double k2wl( double wl ) noexcept; //cost: 1 branch + 1 division
 
   //Physics constants (more are in internal NCMath.hh header):
   constexpr double constant_boltzmann = 8.6173303e-5;  // eV/K
   constexpr double const_neutron_mass_amu = 1.00866491588; // [amu]
   constexpr double const_inv_neutron_mass_amu = 1.0/const_neutron_mass_amu; // [amu]
   constexpr double constant_dalton2kg =  1.660539040e-27; // amu to kg (source: NIST/CODATA 2018)
 
@@ -704,23 +710,28 @@
 namespace NCrystal {
 
   inline constexpr double detail_sqrtNR(double x, double xc, double xp)
   {
     return xc == xp ? xc : detail_sqrtNR(x, 0.5 * (xc + x / xc), xc);
   }
 
-  inline constexpr double constexpr_sqrt(double x)
+  inline constexpr double constexpr_abs(double x)
   {
-    //TODO: Mark consteval in c++20.
-    return detail_sqrtNR(x, x, 0.);
+    return x < 0 ? -x : x;
   }
 
-  inline constexpr double constexpr_abs(double x)
+  inline constexpr bool constexpr_isinf(double x)
   {
-    return x < 0 ? -x : x;
+    return constexpr_abs(x) >= std::numeric_limits<double>::infinity();
+  }
+
+  inline constexpr double constexpr_sqrt(double x)
+  {
+    //TODO: Mark consteval in c++20.
+    return constexpr_isinf( x ) ? x : detail_sqrtNR(x, x, 0.);
   }
 
   template <typename TVal>
   inline constexpr TVal ncconstexpr_max(TVal a,TVal b)
   {
     return a > b ? a : b;
   }
@@ -774,20 +785,27 @@
 
   inline constexpr double wl2ekin( double wl) noexcept
   {
     //angstrom to eV
     return wlsq2ekin( wl * wl );
   }
 
-  inline constexpr double ekin2wl( double ekin) noexcept
+  inline double ekin2wl( double ekin) noexcept
   {
+    //NB: std::sqrt is NOT constexpr!
     //eV to angstrom
     return ekin ? std::sqrt( 0.081804209605330899 / ekin ) : kInfinity;
   }
 
+  inline constexpr double constexpr_ekin2wl( double ekin) noexcept
+  {
+    //eV to angstrom
+    return ekin ? constexpr_sqrt( 0.081804209605330899 / ekin ) : kInfinity;
+  }
+
   inline constexpr double wlsq2ekin( double wlsq ) noexcept
   {
     //angstrom^2 to eV
     return (wlsq ? ( 0.081804209605330899 / wlsq )  : kInfinity);
   }
 
   inline constexpr double ekin2wlsq( double ekin) noexcept
@@ -809,24 +827,45 @@
   }
 
   inline constexpr double ekin2ksq( double ekin ) noexcept
   {
     return ekin * detail::const_ekin2ksq_factor;
   }
 
+  inline double ekin2k( double ekin ) noexcept
+  {
+    //NB: std::sqrt is NOT constexpr!
+    return std::sqrt( ekin * detail::const_ekin2ksq_factor );
+  }
+
+  inline constexpr double constexpr_ekin2k( double ekin ) noexcept
+  {
+    return constexpr_sqrt( ekin * detail::const_ekin2ksq_factor );
+  }
+
   inline constexpr double ksq2ekin( double ksq ) noexcept
   {
     return detail::const_ksq2ekin_factor * ksq;
   }
 
+  inline constexpr double k2ekin( double k ) noexcept
+  {
+    return detail::const_ksq2ekin_factor * ( k * k );
+  }
+
   inline constexpr double wl2k( double wl ) noexcept
   {
     return wl ? k2Pi / wl : kInfinity;
   }
 
+  inline constexpr double k2wl( double k ) noexcept
+  {
+    return k ? k2Pi / k : kInfinity;
+  }
+
   inline constexpr double wl2ksq( double wl ) noexcept
   {
     return detail::constexpr_square_hlpr( wl2k(wl) );
   }
 
   //Some obscure compilers like to complain about unused constants defined
   //through function calls rather than literal constants. Workaround is to mark
```

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCDump.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCDump.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCException.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCException.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCFact.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFact.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCFactImpl.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFactImpl.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCFactRequests.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFactRequests.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCFactTypes.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFactTypes.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCFmt.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCFmt.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCImmutBuf.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCImmutBuf.hh`

 * *Files 3% similar despite different names*

```diff
@@ -23,32 +23,34 @@
 
 #include "NCrystal/NCDefs.hh"
 
 namespace NCrystal {
 
   /////////////////////////////////////////////////////////////////////////////////
   //                                                                             //
-  // Immutable buffer with custom alignment and SBO. If needed, remote storage   //
-  // is kept in a shared ptr, so copying of buffer objects will always happen    //
-  // safely and malloc's. Note that the data length is NOT stored on the object, //
-  // so the code using ImmutableBuffer's are responsible for not using data      //
-  // beyond the length. It is optionally possible to store a trivial meta data   //
-  // object (such as an integer) on the object, which is both for convenience    //
-  // and to ensure any padding between the buffer and the metadata object are    //
-  // used to increase the size of the local buffer. Minimum local buffer size    //
-  // and required buffer alignment should be specified as template parameters.   //
-  // Note that a single char is used internally keep track of local vs. remote   //
-  // mode, so optimal LOCALBUF_MINSIZE will value will typically be 1 less than  //
-  // a power of two.                                                             //
+  // Immutable buffer with custom alignment and SBO (small buffer                //
+  // optimisation). If needed, remote storage is kept in a shared ptr, so        //
+  // copying of buffer objects will always happen safely and malloc's are        //
+  // reduced. Note that the data length is NOT stored on the object, so the code //
+  // using ImmutableBuffer's are responsible for not using data beyond the       //
+  // length. It is optionally possible to store a trivial meta data object (such //
+  // as an integer) on the object, which is both for convenience and to ensure   //
+  // any padding between the buffer and the metadata object are used to increase //
+  // the size of the local buffer. Minimum local buffer size and required buffer //
+  // alignment should be specified as template parameters.  Note that a single   //
+  // char is used internally keep track of local vs. remote mode, so optimal     //
+  // LOCALBUF_MINSIZE will value will typically be 1 less than a power of two.   //
   //                                                                             //
   // NB: On most platforms, only powers of two (1, 2, 4, 8, 16, ...) are valid   //
   // BUF_ALIGNMENT choices, but on some platforms e.g. long double apparently    //
   // has alignment of 10, so we don't static assert on it. It is always          //
-  // recommended to set BUF_ALIGNMENT to the alignment of the data to be         //
-  // stored, extracted using alignof(..).                                        //
+  // recommended to set BUF_ALIGNMENT to the alignment of the data to be stored, //
+  // extracted using alignof(..). UPDATE 2023: The underlying allignedAlloc code //
+  // now static_asserts on powers of two, so the code will need to be updated if //
+  // we encounter such platforms.                                                //
   //                                                                             //
   /////////////////////////////////////////////////////////////////////////////////
 
   template< std::size_t LOCALBUF_MINSIZE = 15, std::size_t BUF_ALIGNMENT=1, class TMetaData = NullOptType >
   class NCRYSTAL_API ImmutableBuffer {
     class RemoteBuf;
     using TRemotePtr = std::shared_ptr<const RemoteBuf>;
@@ -180,16 +182,16 @@
     initBuffer(src,len);
   }
 
   template<std::size_t LOCALBUF_MINSIZE, std::size_t BUF_ALIGNMENT, class TMetaData>
   class ImmutableBuffer<LOCALBUF_MINSIZE,BUF_ALIGNMENT,TMetaData>::RemoteBuf : private NoCopyMove {
     char * m_data;
   public:
-    RemoteBuf(const char * src, size_type len ) : m_data((char*)alignedAlloc(BUF_ALIGNMENT,len)) { std::memcpy(m_data,src,len); }
-    ~RemoteBuf() { std::free(m_data); }
+    RemoteBuf(const char * src, size_type len ) : m_data((char*)AlignedAlloc::alignedAllocFixedAlign<BUF_ALIGNMENT>(len)) { std::memcpy(m_data,src,len); }
+    ~RemoteBuf() { AlignedAlloc::freeAlignedAllocFixedAlign<BUF_ALIGNMENT>(static_cast<void*>(m_data)); }
     const char * data() const noexcept { return m_data; }
   };
 
   template<std::size_t LBMS, std::size_t BA, class MD>
   inline void ImmutableBuffer<LBMS,BA,MD>::unsetIfRemote() noexcept {
     if (isRemote()) {
       TRemotePtr* rp = &remotePtr();
```

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCInfo.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCInfo.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCInfoBuilder.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCInfoBuilder.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCInfoTypes.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCInfoTypes.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCLoadNCMAT.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCLoadNCMAT.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCMatCfg.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCMatCfg.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCNCMATData.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCNCMATData.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCParseNCMAT.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCParseNCMAT.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCPluginBoilerplate.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCPluginBoilerplate.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCPluginMgmt.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCPluginMgmt.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCProc.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCProc.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCProcImpl.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCProcImpl.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCRNG.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCRNG.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCSABData.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCSABData.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCSCOrientation.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCSCOrientation.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCSmallVector.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCSmallVector.hh`

 * *Files 0% similar despite different names*

```diff
@@ -299,34 +299,49 @@
 
     class DetachedHeap {
       TValue * m_begin;
       TValue * m_end;
       size_type m_capacity;
     public:
       DetachedHeap(TValue*b,TValue*e,size_type cc) : m_begin(b), m_end(e), m_capacity(cc) {}
-      ncconstexpr17 TValue * begin() noexcept { return m_begin; }
-      ncconstexpr17 TValue * end() noexcept { return m_end; }
-      constexpr size_type capacity() const noexcept { return m_capacity; }
+      ncconstexpr17 TValue * begin() noexcept
+      {
+        assert( m_begin != nullptr );
+        return m_begin;
+      }
+      ncconstexpr17 TValue * end() noexcept
+      {
+        assert( m_end != nullptr );
+        return m_end;
+      }
+      constexpr size_type capacity() const noexcept
+      {
+#if __cplusplus >= 201402L // assert in constexpr requires C++14
+        assert( m_begin != nullptr);
+#endif
+        return m_capacity;
+      }
       TValue * release() { TValue * d = m_begin; m_begin=m_end=nullptr; return d; }
       template<typename ...Args>
       void emplace_back( Args&& ...args )
       {
+        assert( m_begin != nullptr );
         //NB: calling code is responsible for ensuring adequate capacity.
         new (m_end) TValue(std::forward<Args>(args)...);
         ++m_end;//on line after TValue constructor (in case it throws)
         assert( m_end <= m_begin + m_capacity );
       }
 
       ~DetachedHeap()
       {
         if ( m_begin ) {
           auto it(m_begin), itE(m_end);
           for ( ; it!=itE; ++it )
             it->~TValue();
-          std::free(m_begin);
+          AlignedAlloc::freeAlignedAlloc<TValue>( m_begin );
         }
       }
     };
 
     static void adoptHeap(SmallVector* THIS,DetachedHeap& heap) noexcept
     {
       size_type count = std::distance( heap.begin(), heap.end() );
@@ -336,15 +351,15 @@
       THIS->setBeginPtr( THIS->m_data.large.data = heap.release() );
       THIS->m_count = count;
     }
 
     static DetachedHeap createNewDetachedHeap( size_type capacity )
     {
       //Can throw std::bad_alloc
-      TValue * b = alignedAlloc<TValue>(capacity);
+      TValue * b = AlignedAlloc::alignedAlloc<TValue>(capacity);
       return DetachedHeap(b,b,capacity);
     }
 
     static DetachedHeap detachHeapDataAndClear(SmallVector * THIS) noexcept
     {
       assert(large(THIS));
       TValue * b = THIS->m_data.large.data;
@@ -379,27 +394,35 @@
       THIS->setBeginPtr(smallDataBegin(THIS));
     }
 
     static void clear(SmallVector * THIS ) noexcept
     {
       //Call destructors, release heap alloction (if any) and set count to
       //0. It is noexcept since destructors should not throw.
-      if ( THIS->m_count > 0 ) {
-        auto it = THIS->begin();
-        auto itE = THIS->end();
-        for (;it!=itE;++it)
-          it->~TValue();
+      if ( THIS->m_count == 0 )
+        return;
+
+      if ( large(THIS) ) {
+        //Since v3.7.0 (summer 2023) we release the large area like this, to
+        //avoid what looks like a spurious error with gcc 12 (see
+        //https://github.com/mctools/ncrystal/issues/125). Doing it like this
+        //seems to avoid this issue for some obscure reason, perhaps because it
+        //lets gcc focus on one RAII class at a time. Also, it is important
+        //(apparently!) that the "THIS->m_count == 0" check above comes first.
+        Impl::detachHeapDataAndClear(THIS);
+        return;
       }
-      if ( large(THIS) )
-        std::free(THIS->m_data.large.data);
+
+      nclikely auto itE = THIS->end();
+      for ( auto it = THIS->begin(); it!=itE ; ++it )
+        it->~TValue();
       THIS->m_count = 0;
       setBeginPtrSmallData(THIS);
     }
 
-
     static void resizeDown( SmallVector * THIS, size_type n ) noexcept
     {
       assert ( THIS->m_count >= n );
       if ( THIS->m_count == n )
         return;
       if  ( n > NSMALL || THIS->m_count <= NSMALL ) {
         //Can peel entries off without changing storage mode:
```

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCTextData.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCTextData.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCTypes.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCTypes.hh`

 * *Files 1% similar despite different names*

```diff
@@ -135,33 +135,36 @@
   class NeutronEnergy;
 
   class NCRYSTAL_API NeutronWavelength final : public EncapsulatedValue<NeutronWavelength> {
     //Neutron wavelength in angstrom
   public:
     using EncapsulatedValue::EncapsulatedValue;
     static constexpr const char * unit() noexcept { return "Aa"; }
-    //Automatic conversions from/to energy:
-    constexpr NeutronWavelength(NeutronEnergy) noexcept;
+    //Automatic conversions from/to energy (not constexpr, since std::sqrt is not constexpr):
+    NeutronWavelength(NeutronEnergy) noexcept;
     void validate() const;
     ncnodiscard17 constexpr NeutronEnergy energy() const noexcept;
     ncnodiscard17 constexpr double k() const noexcept;//Corresponding wavenumber (k) in units of 1/Aa
     ncnodiscard17 constexpr double ksq() const noexcept;//Corresponding squared wavenumber (k^2) in units of 1/Aa^2
   };
 
   class NCRYSTAL_API NeutronEnergy final : public EncapsulatedValue<NeutronEnergy> {
   public:
     //Neutron kinetic energy in electronvolt
     using EncapsulatedValue::EncapsulatedValue;
     static constexpr const char * unit() noexcept { return "eV"; }
     //Automatic conversions from/to wavelength:
     constexpr NeutronEnergy(NeutronWavelength) noexcept;
     void validate() const;
-    ncnodiscard17 constexpr NeutronWavelength wavelength() const noexcept;
-    ncnodiscard17 constexpr double k() const noexcept;//Corresponding wavenumber (k) in units of 1/Aa
+    ncnodiscard17 NeutronWavelength wavelength() const noexcept;
+    ncnodiscard17 double k() const noexcept;//Corresponding wavenumber (k) in units of 1/Aa
     ncnodiscard17 constexpr double ksq() const noexcept;//Corresponding squared wavenumber (k^2) in units of 1/Aa^2
+    //Constexpr versions (do not use in runtime!):
+    ncnodiscard17 constexpr NeutronWavelength constexpr_wavelength() const noexcept;
+    ncnodiscard17 constexpr double constexpr_k() const noexcept;
   };
 
   class NCRYSTAL_API CosineScatAngle final : public EncapsulatedValue<CosineScatAngle> {
   public:
     //Cosine of scattering angle (aka "mu")
     using EncapsulatedValue::EncapsulatedValue;
     static constexpr const char * unit() noexcept { return ""; }
@@ -635,22 +638,32 @@
   }
 
   inline constexpr NeutronEnergy NeutronWavelength::energy() const noexcept
   {
     return *this;
   }
 
-  inline constexpr NeutronWavelength NeutronEnergy::wavelength() const noexcept
+  inline NeutronWavelength NeutronEnergy::wavelength() const noexcept
   {
     return *this;
   }
 
-  inline constexpr double NeutronEnergy::k() const noexcept
+  inline constexpr NeutronWavelength NeutronEnergy::constexpr_wavelength() const noexcept
   {
-    return ekin2ksq(m_value);
+    return NeutronWavelength{ constexpr_ekin2wl( this->get() ) };
+  }
+
+  inline double NeutronEnergy::k() const noexcept
+  {
+    return ekin2k(m_value);
+  }
+
+  inline constexpr double NeutronEnergy::constexpr_k() const noexcept
+  {
+    return constexpr_ekin2k(m_value);
   }
 
   inline constexpr double NeutronEnergy::ksq() const noexcept
   {
     return ekin2ksq(m_value);
   }
 
@@ -660,16 +673,17 @@
   }
 
   inline constexpr double NeutronWavelength::ksq() const noexcept
   {
     return wl2ksq(m_value);
   }
 
-  //Using nc_as_const so it can also be constexpr in C++11
-  inline constexpr NeutronWavelength::NeutronWavelength(NeutronEnergy ekin) noexcept
+  //Using nc_as_const so it can also be constexpr in C++11 [update: it can't
+  //anyway, since std::sqrt is not constexpr and so ekin2wl is not]:
+  inline NeutronWavelength::NeutronWavelength(NeutronEnergy ekin) noexcept
     : EncapsulatedValue(ekin2wl(nc_as_const(ekin).get())) {}
   inline constexpr NeutronEnergy::NeutronEnergy(NeutronWavelength wl) noexcept
     : EncapsulatedValue(wl2ekin(nc_as_const(wl).get())) {}
   inline constexpr MosaicityFWHM::MosaicityFWHM(MosaicitySigma mos) noexcept
     : EncapsulatedValue( nc_as_const(mos).get() * kSigma2FWHM ) {}
   inline constexpr MosaicitySigma::MosaicitySigma(MosaicityFWHM mos) noexcept
     : EncapsulatedValue( nc_as_const(mos).get() * kFWHM2Sigma ) {}
```

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCVariant.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCVariant.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCVersion.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCVersion.hh`

 * *Files 1% similar despite different names*

```diff
@@ -35,17 +35,17 @@
 #endif
 #ifdef NCRYSTAL_VERSION_STR
 #  undef NCRYSTAL_VERSION_STR
 #endif
 
 #define NCRYSTAL_VERSION_MAJOR 3
 #define NCRYSTAL_VERSION_MINOR 6
-#define NCRYSTAL_VERSION_PATCH 80
-#define NCRYSTAL_VERSION   3006080 /* (1000000*MAJOR+1000*MINOR+PATCH)   */
-#define NCRYSTAL_VERSION_STR "3.6.80"
+#define NCRYSTAL_VERSION_PATCH 82
+#define NCRYSTAL_VERSION   3006082 /* (1000000*MAJOR+1000*MINOR+PATCH)   */
+#define NCRYSTAL_VERSION_STR "3.6.82"
 
 #include "NCrystal/ncapi.h"
 #include <stdexcept>
 
 namespace NCrystal {
 
   //Function which returns NCRYSTAL_VERSION. If it does not, it indicates symbol
```

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/NCrystal.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/NCrystal.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCAbsOOV.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCAbsOOV.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCAtomDB.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCAtomDB.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCAtomDBExtender.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCAtomDBExtender.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCAtomUtils.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCAtomUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCBkgdExtCurve.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCBkgdExtCurve.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCCfgManip.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCCfgManip.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCCfgTypes.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCCfgTypes.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCCfgVars.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCCfgVars.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCDebyeMSD.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCDebyeMSD.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCDynInfoUtils.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCDynInfoUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCDynLoader.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCDynLoader.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCElIncScatter.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCElIncScatter.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCElIncXS.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCElIncXS.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCEqRefl.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCEqRefl.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCFactoryUtils.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFactoryUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCFastConvolve.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFastConvolve.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCFileUtils.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFileUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCFillHKL.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFillHKL.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCFreeGas.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFreeGas.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCFreeGasUtils.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCFreeGasUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCGasMixUtils.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCGasMixUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCGaussMos.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCGaussMos.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCGaussOnSphere.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCGaussOnSphere.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCIofQHelper.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCIofQHelper.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCIter.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCIter.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCKinUtils.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCKinUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCLCBragg.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCLCBragg.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCLCRefModels.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCLCRefModels.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCLCUtils.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCLCUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCLatticeUtils.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCLatticeUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCMath.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCMath.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCMatrix.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCMatrix.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCOrientUtils.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCOrientUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCPCBragg.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCPCBragg.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCPlaneProvider.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCPlaneProvider.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCPointwiseDist.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCPointwiseDist.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCRandUtils.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCRandUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCRomberg.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCRomberg.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCRotMatrix.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCRotMatrix.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABEval.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABEval.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABExtender.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABExtender.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABFactory.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABFactory.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABIntegrator.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABIntegrator.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABSampler.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABSampler.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABSamplerModels.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABSamplerModels.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABScatter.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABScatter.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABScatterHelper.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABScatterHelper.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABUCN.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABUCN.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABUtils.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSABXSProvider.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSABXSProvider.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSANSSphScat.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSANSSphScat.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSANSUtils.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSANSUtils.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSCBragg.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSCBragg.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCScatKnlData.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCScatKnlData.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSpan.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSpan.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCSpline.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCSpline.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCStrView.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCStrView.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCString.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCString.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCVDOSEval.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCVDOSEval.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCVDOSGn.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCVDOSGn.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCVDOSToScatKnl.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCVDOSToScatKnl.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/internal/NCVector.hh` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/internal/NCVector.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/ncapi.h` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/ncapi.h`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/include/NCrystal/ncrystal.h` & `ncrystal-3.6.dev82/ncrystal_core/include/NCrystal/ncrystal.h`

 * *Files 0% similar despite different names*

```diff
@@ -576,17 +576,17 @@
 #  undef NCRYSTAL_VERSION
 #endif
 #ifdef NCRYSTAL_VERSION_STR
 #  undef NCRYSTAL_VERSION_STR
 #endif
 #define NCRYSTAL_VERSION_MAJOR 3
 #define NCRYSTAL_VERSION_MINOR 6
-#define NCRYSTAL_VERSION_PATCH 80
-#define NCRYSTAL_VERSION   3006080 /* (1000000*MAJOR+1000*MINOR+PATCH)             */
-#define NCRYSTAL_VERSION_STR "3.6.80"
+#define NCRYSTAL_VERSION_PATCH 82
+#define NCRYSTAL_VERSION   3006082 /* (1000000*MAJOR+1000*MINOR+PATCH)             */
+#define NCRYSTAL_VERSION_STR "3.6.82"
   NCRYSTAL_API int ncrystal_version(); /* returns NCRYSTAL_VERSION                  */
   NCRYSTAL_API const char * ncrystal_version_str(); /* returns NCRYSTAL_VERSION_STR */
 
   /* Load raw NCMAT data into JSON structures. Must deallocate with call to        */
   /* ncrystal_dealloc_string as usual. (WARNING: JSON is incomplete for now!!!!!)  */
   NCRYSTAL_API char * ncrystal_ncmat2json( const char * textdataname );
```

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCAbsOOV.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCAbsOOV.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCAtomDB.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCAtomDB.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCAtomDBExtender.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCAtomDBExtender.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCAtomData.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCAtomData.cc`

 * *Files 1% similar despite different names*

```diff
@@ -37,25 +37,27 @@
   {
     Component* it = THIS->m_components;
     nc_assert( it != nullptr );
     for ( auto i : ncrange( THIS->nComponents() ) ) {
       (void)i;
       (it++)->~Component();
     }
-    std::free(THIS->m_components);
-    THIS->m_components = nullptr;
+    if ( THIS->m_components ) {
+      AlignedAlloc::freeAlignedAlloc<Component>( THIS->m_components );
+      THIS->m_components = nullptr;
+    }
   }
   static void setComponents(AtomData* THIS, const Component* o_begin, unsigned n )
   {
     if ( THIS->m_components )
       clearComponents(THIS);
     if ( n == 0)
       return;
     nc_assert_always( n < static_cast<unsigned>(-std::numeric_limits<decltype(m_classify)>::lowest()) );
-    Component * it = alignedAlloc<Component>(n);
+    Component * it = AlignedAlloc::alignedAlloc<Component>(n);
     //RAII, start at m_classify=0 so destructor won't clean up something we didn't construct.
     THIS->m_components = it;
     THIS->m_classify = 0;
     for ( auto i : ncrange( n ) ) {
       (void)i;
       new ( it++ ) Component( *(o_begin++) );//copy construct in place
       --(THIS->m_classify);//one more ready to destruct
```

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCAtomUtils.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCAtomUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCBkgdExtCurve.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCBkgdExtCurve.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCCfgManip.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCCfgManip.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCCfgTypes.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCCfgTypes.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCCfgVars.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCCfgVars.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCCompositionUtils.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCCompositionUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCDataSources.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCDataSources.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCDebyeMSD.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCDebyeMSD.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCDefs.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCDefs.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCDump.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCDump.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCDynInfoUtils.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCDynInfoUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCDynLoader.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCDynLoader.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCElIncScatter.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCElIncScatter.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCElIncXS.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCElIncXS.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCEqRefl.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCEqRefl.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCException.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCException.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCFact.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCFactImpl.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCFactImpl.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCFactRequests.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCFactRequests.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCFactTypes.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCFactTypes.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCFactoryUtils.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCFactoryUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCFactory_NCMAT.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCFactory_NCMAT.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCFastConvolve.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCFastConvolve.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCFileUtils.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCFileUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCFillHKL.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCFillHKL.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCFmt.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCFmt.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCFreeGas.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCFreeGas.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCFreeGasUtils.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCFreeGasUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCGasMixFact.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCGasMixFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCGasMixUtils.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCGasMixUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCGaussMos.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCGaussMos.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCGaussOnSphere.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCGaussOnSphere.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCInfo.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCInfo.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCInfoBuilder.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCInfoBuilder.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCIofQHelper.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCIofQHelper.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCKinUtils.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCKinUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCLCBragg.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCLCBragg.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCLCRefModels.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCLCRefModels.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCLCUtils.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCLCUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCLatticeUtils.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCLatticeUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCLauLazyFact.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCLauLazyFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCLazy.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCLazy.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCLazy.hh` & `ncrystal-3.6.dev82/ncrystal_core/src/NCLazy.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCLoadNCMAT.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCLoadNCMAT.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCMatCfg.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCMatCfg.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCMath.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCMath.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCMatrix.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCMatrix.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCNCMATData.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCNCMATData.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCOrientUtils.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCOrientUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCPCBragg.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCPCBragg.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCParseNCMAT.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCParseNCMAT.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCPlaneProvider.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCPlaneProvider.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCPluginMgmt.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCPluginMgmt.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCPointwiseDist.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCPointwiseDist.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCProc.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCProc.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCProcImpl.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCProcImpl.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCQuickFact.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCQuickFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCRNG.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCRNG.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCRandUtils.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCRandUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCRomberg.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCRomberg.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCRotMatrix.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCRotMatrix.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCSABData.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCSABData.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCSABEval.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCSABEval.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCSABExtender.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCSABExtender.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCSABFactory.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCSABFactory.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCSABIntegrator.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCSABIntegrator.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCSABSampler.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCSABSampler.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCSABSamplerModels.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCSABSamplerModels.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCSABScatter.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCSABScatter.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCSABUCN.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCSABUCN.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCSABUtils.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCSABUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCSABXSProvider.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCSABXSProvider.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCSANSFact.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCSANSFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCSANSSphScat.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCSANSSphScat.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCSANSUtils.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCSANSUtils.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCSCBragg.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCSCBragg.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCSCOrientation.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCSCOrientation.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCScatKnlData.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCScatKnlData.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCSpline.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCSpline.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCStdAbsFact.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCStdAbsFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCStdMPScatFact.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCStdMPScatFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCStdScatFact.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCStdScatFact.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCStrView.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCStrView.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCString.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCString.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCTDProd.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCTDProd.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCTextData.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCTextData.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCTypes.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCTypes.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCVDOSEval.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCVDOSEval.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCVDOSGn.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCVDOSGn.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCVDOSToScatKnl.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCVDOSToScatKnl.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCVector.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCVector.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/NCVersion.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/NCVersion.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_core/src/ncrystal.cc` & `ncrystal-3.6.dev82/ncrystal_core/src/ncrystal.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_geant4/include/G4NCrystal/G4NCInstall.hh` & `ncrystal-3.6.dev82/ncrystal_geant4/include/G4NCrystal/G4NCInstall.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_geant4/include/G4NCrystal/G4NCManager.hh` & `ncrystal-3.6.dev82/ncrystal_geant4/include/G4NCrystal/G4NCManager.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_geant4/include/G4NCrystal/G4NCMatHelper.hh` & `ncrystal-3.6.dev82/ncrystal_geant4/include/G4NCrystal/G4NCMatHelper.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_geant4/include/G4NCrystal/G4NCrystal.hh` & `ncrystal-3.6.dev82/ncrystal_geant4/include/G4NCrystal/G4NCrystal.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_geant4/src/G4NCInstall.cc` & `ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCInstall.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_geant4/src/G4NCManager.cc` & `ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCManager.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_geant4/src/G4NCMatHelper.cc` & `ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCMatHelper.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_geant4/src/G4NCProcWrapper.cc` & `ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCProcWrapper.cc`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_geant4/src/G4NCProcWrapper.hh` & `ncrystal-3.6.dev82/ncrystal_geant4/src/G4NCProcWrapper.hh`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_mcstas/NCrystal_example.instr` & `ncrystal-3.6.dev82/ncrystal_mcstas/NCrystal_example.instr`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/ncrystal_mcstas/NCrystal_sample.comp` & `ncrystal-3.6.dev82/ncrystal_mcstas/NCrystal_sample.comp`

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
-* Version: 3.6.80
+* Version: 3.6.82
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
-NCrystal_sample * * %I * Written by: NCrystal developers * Version: 3.6.80 *
+NCrystal_sample * * %I * Written by: NCrystal developers * Version: 3.6.82 *
 Origin: NCrystal Developers (European Spallation Source ERIC and DTU Nutech) *
 * McStas sample component for the NCrystal library for thermal neutron
 transport * (www). * * %D * McStas sample component for the NCrystal scattering
 library. * Find more information at the_NCrystal_wiki. * In particular, browse
 the available datafiles at Data-library * and read about the format of the
 configuration string expected in * the "cfg" parameter at Using-NCrystal. * *
 NCrystal is available under the Apache_2.0_license. * Depending on the
```

### Comparing `ncrystal-3.6.80/ncrystal_mcstas/ncrystal_preparemcstasdir` & `ncrystal-3.6.dev82/ncrystal_mcstas/ncrystal_preparemcstasdir`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/scripts/ncrystal_cif2ncmat` & `ncrystal-3.6.dev82/scripts/ncrystal_cif2ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/scripts/ncrystal_endf2ncmat` & `ncrystal-3.6.dev82/scripts/ncrystal_endf2ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/scripts/ncrystal_hfg2ncmat` & `ncrystal-3.6.dev82/scripts/ncrystal_hfg2ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/scripts/ncrystal_inspectfile` & `ncrystal-3.6.dev82/scripts/ncrystal_inspectfile`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/scripts/ncrystal_ncmat2cpp` & `ncrystal-3.6.dev82/scripts/ncrystal_ncmat2cpp`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/scripts/ncrystal_ncmat2hkl` & `ncrystal-3.6.dev82/scripts/ncrystal_ncmat2hkl`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/scripts/ncrystal_onlinedb2ncmat` & `ncrystal-3.6.dev82/scripts/ncrystal_onlinedb2ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/scripts/ncrystal_vdos2ncmat` & `ncrystal-3.6.dev82/scripts/ncrystal_vdos2ncmat`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/scripts/ncrystal_verifyatompos` & `ncrystal-3.6.dev82/scripts/ncrystal_verifyatompos`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/scripts/nctool` & `ncrystal-3.6.dev82/scripts/nctool`

 * *Files identical despite different names*

### Comparing `ncrystal-3.6.80/setup.py` & `ncrystal-3.6.dev82/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,48 +16,55 @@
 ##  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  ##
 ##  See the License for the specific language governing permissions and       ##
 ##  limitations under the License.                                            ##
 ##                                                                            ##
 ################################################################################
 
 from skbuild import setup  # This line replaces 'from setuptools import setup'
-import codecs
-import os.path
 
-def read(rel_path):
-    here = os.path.abspath(os.path.dirname(__file__))
-    with codecs.open(os.path.join(here, rel_path), 'r') as fp:
-        return fp.read()
+def _extract_version():
+    import pathlib
+    p = pathlib.Path(__file__).parent / 'NCrystal' / '__init__.py'
+    if not p.exists():
+        raise RuntimeError("Unable to find NCrystal/__init__.py (for version string extraction).")
+    version_str = None
+    for l in p.read_text().splitlines():
+        if l.startswith('__version__'):
+            delim = '"' if '"' in l else "'"
+            version_str = l.split(delim)[1]
+            break
+    if not version_str:
+        raise RuntimeError(f'Unable to find version string in {p}.')
+    v = tuple( int(i) for i in version_str.split('.') )
+    if not len(v)==3:
+        raise RuntimeError(f'Invalid version string extracted from {p}.')
+    return v
 
-def get_version(rel_path):
-    for line in read(rel_path).splitlines():
-        if line.startswith('__version__'):
-            delim = '"' if '"' in line else "'"
-            return line.split(delim)[1]
-    else:
-        raise RuntimeError("Unable to find version string.")
+def get_version():
+    x,y,z = _extract_version()
+    return f'{x}.{y}.dev{z}' if z>=80 else f'{x}.{y}.{z}'
 
 setup(
     name="ncrystal",
-    version=get_version("NCrystal/__init__.py"),
+    version=get_version(),
     author='NCrystal developers (Thomas Kittelmann, Xiao Xiao Cai)',
     license = "Apache-2.0",
     description='Library for thermal neutron transport in crystals and other materials.',
     url='https://github.com/mctools/ncrystal/wiki',
     keywords='neutron,montecarlo,science',
     packages=['NCrystal'],
     python_requires='>=3.6, <4',
     install_requires=['numpy'],
     long_description='NCrystal is a library and associated tools which enables calculations for Monte Carlo simulations of thermal neutrons in crystals and other materials, supporting a range of physics including both coherent, incoherent, elastic and inelastic scatterings in a wide range of materials, including crystal powders, mosaic single crystals, layered single crystals, amorphous solids, and liquids. Multiphase materials or isotopically enriched materials are supported as well, and the framework furthermore supports phase-contrast (SANS) physics.',
     cmake_args=['-DNCRYSTAL_NOTOUCH_CMAKE_BUILD_TYPE=ON',
                 '-DNCRYSTAL_MODIFY_RPATH=OFF',
                 '-DNCRYSTAL_ENABLE_SETUPSH=OFF',
-                '-DNCRYSTAL_ENABLE_DATA=EMBED',
+                '-DNCRYSTAL_ENABLE_DATA=EMBED',#the c++ library can not currently locate the files if not embedding
                 '-DNCRYSTAL_ENABLE_MCSTAS=OFF',#Explicitly disable for now (was already moved into upstream McStas)
                 '-DNCRYSTAL_ENABLE_GEANT4=OFF',#Explicitly disable for now (planning to move out of core NCrystal repo)
                 '-DNCRYSTAL_SKIP_PYMODINST=ON',
                 '-DCMAKE_INSTALL_LIBDIR=NCrystal/ncrystal_pyinst_data/lib',
                 '-DCMAKE_INSTALL_INCLUDEDIR=NCrystal/ncrystal_pyinst_data/include',
                 '-DCMAKE_INSTALL_DATADIR=NCrystal/ncrystal_pyinst_data/data',
                 '-DNCrystal_DATAFILESDIR=NCrystal/ncrystal_pyinst_data/stdlib_data',
-    ]
+                ]
 )
```

