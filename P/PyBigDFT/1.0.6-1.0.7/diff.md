# Comparing `tmp/pybigdft-1.0.6.tar.gz` & `tmp/pybigdft-1.0.7.tar.gz`

## Comparing `pybigdft-1.0.6.tar` & `pybigdft-1.0.7.tar`

### file list

```diff
@@ -1,519 +1,494 @@
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 pybigdft-1.0.6/.gitrepo
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pybigdft-1.0.6/MANIFEST.in
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pybigdft-1.0.6/Makefile-sphinxbuild
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 pybigdft-1.0.6/conftest.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pybigdft-1.0.6/setup.cfg
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 pybigdft-1.0.6/setup.py
--rw-r--r--   0        0        0    21273 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Atoms.py
--rw-r--r--   0        0        0    10061 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/BZ.py
--rw-r--r--   0        0        0   131061 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/BioQM.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/CDFT.py
--rw-r--r--   0        0        0    30528 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Calculators.py
--rw-r--r--   0        0        0    17573 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Datasets.py
--rw-r--r--   0        0        0    23903 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/DoS.py
--rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Fragments.py
--rw-r--r--   0        0        0    25983 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/IO.py
--rw-r--r--   0        0        0    30908 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/InputActions.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Inputfiles.py
--rw-r--r--   0        0        0    28150 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/LRTDDFT.py
--rwxr-xr-x   0        0        0     6227 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/LogUtils.py
--rw-r--r--   0        0        0    33462 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Logfiles.py
--rw-r--r--   0        0        0     6102 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/PointParticles.py
--rw-r--r--   0        0        0    50145 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/PostProcessing.py
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Spillage.py
--rw-r--r--   0        0        0    22494 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Stats.py
--rw-r--r--   0        0        0    49326 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Systems.py
--rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/UnitCells.py
--rw-r--r--   0        0        0    22352 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Visualization.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/__init__.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/check_examples.py
--rw-r--r--   0        0        0     5852 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/wahba.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/Molecules.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/__init__.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/postprocess.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/AlF.xyz
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Ar.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BF.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BH2.xyz
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BH2Cl.xyz
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BH2F.xyz
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BH3.xyz
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BHF2.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BN.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BO.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BS.xyz
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Be.xyz
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BeH.xyz
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/BeH2.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/C2H.xyz
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/C2H2.xyz
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/C2H3.xyz
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/C2H4.xyz
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/C2H6O.xyz
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/C9H12.xyz
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH2-t.xyz
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH2.xyz
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH2BH.xyz
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH2F.xyz
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH2NH.xyz
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH2PH.xyz
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH3.xyz
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH3BH2.xyz
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH3Cl.xyz
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH3F.xyz
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH3NH2.xyz
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH3O.xyz
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH3OH.xyz
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH3SH.xyz
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CH4.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CN.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CO.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CO2.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CS.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/CSO.xyz
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Cl2.xyz
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/ClCN.xyz
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/ClF.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/F2.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/FCN.xyz
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/FCO.xyz
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/FH-OH.xyz
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/FNO.xyz
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/H.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/H2.xyz
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/H2CN.xyz
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/H2O-Li.xyz
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/H2O.xyz
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HBO.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HBS.xyz
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCCCl.xyz
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCCF.xyz
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCHO.xyz
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCHS.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCN.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCO.xyz
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCONH2.xyz
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCOOH.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCP.xyz
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HCl.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HF.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HNC.xyz
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HNO.xyz
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HNS.xyz
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HO2.xyz
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HOCl.xyz
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HOF.xyz
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/HOOH.xyz
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/He.xyz
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Li.xyz
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Li2.xyz
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/LiBH4.xyz
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/LiCN.xyz
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/LiCl.xyz
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/LiH.xyz
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Mg.xyz
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Mg2.xyz
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/N.xyz
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/N2.xyz
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/N2H2.xyz
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/N2H4.xyz
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NCO.xyz
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NH.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NH2.xyz
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NH2Cl.xyz
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NH2F.xyz
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NH2OH.xyz
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NH3.xyz
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NH3O.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NO.xyz
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NOCl.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NP.xyz
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Na.xyz
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Na2.xyz
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NaCN.xyz
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NaCl.xyz
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NaH.xyz
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/NaLi.xyz
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Ne.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/O2.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/O3.xyz
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/OCl.xyz
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/OCl2.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/OF.xyz
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/OF2.xyz
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/OH.xyz
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/P.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/P2.xyz
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/P2H4.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/PH.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/PH2.xyz
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/PH2OH.xyz
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/PH3.xyz
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/PH3O.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/PS.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/S2.xyz
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/S2H2.xyz
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SCl.xyz
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SCl2.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SF.xyz
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SF2.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SH.xyz
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SH2.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SO-trip.xyz
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SO.xyz
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SO2.xyz
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/Si4.xyz
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SiH3.xyz
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SiH3Cl.xyz
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SiH3F.xyz
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SiH4.xyz
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/XYZs/SiO.xyz
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ag.yaml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Al.yaml
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ar.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.As.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.At.yaml
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Au.yaml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.B.yaml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ba.yaml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Be.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Bi.yaml
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Br.yaml
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.C.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ca.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cd.yaml
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ce.yaml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cl.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Co.yaml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cr.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cs.yaml
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cu.yaml
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Dy.yaml
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Er.yaml
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Eu.yaml
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.F.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Fe.yaml
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ga.yaml
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Gd.yaml
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ge.yaml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.H.yaml
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.He.yaml
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Hf.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Hg.yaml
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ho.yaml
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.I.yaml
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.In.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ir.yaml
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.K.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Kr.yaml
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.La.yaml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Li.yaml
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Lu.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Mg.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Mn.yaml
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Mo.yaml
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.N.yaml
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Na.yaml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Nb.yaml
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Nd.yaml
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ne.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ni.yaml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.O.yaml
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Os.yaml
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.P.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pb.yaml
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pd.yaml
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pm.yaml
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Po.yaml
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pr.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pt.yaml
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Rb.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Re.yaml
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Rh.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Rn.yaml
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ru.yaml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.S.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sb.yaml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sc.yaml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Se.yaml
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Si.yaml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sm.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sn.yaml
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sr.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ta.yaml
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Tb.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Tc.yaml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Te.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ti.yaml
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Tl.yaml
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Tm.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.V.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.W.yaml
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Xe.yaml
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Y.yaml
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Yb.yaml
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Zn.yaml
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Zr.yaml
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ag.yaml
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Al.yaml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ar.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.As.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.At.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Au.yaml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.B.yaml
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ba.yaml
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Be.yaml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Bi.yaml
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Br.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.C.yaml
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ca.yaml
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cd.yaml
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cl.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Co.yaml
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cr.yaml
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cs.yaml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cu.yaml
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.F.yaml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Fe.yaml
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ga.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ge.yaml
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.H.yaml
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.He.yaml
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Hf.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Hg.yaml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.I.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.In.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ir.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.K.yaml
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Kr.yaml
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.La.yaml
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Li.yaml
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Mg.yaml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Mn.yaml
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Mo.yaml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.N.yaml
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Na.yaml
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Nb.yaml
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ne.yaml
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ni.yaml
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.O.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Os.yaml
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.P.yaml
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Pb.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Pd.yaml
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Po.yaml
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Pt.yaml
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Rb.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Re.yaml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Rh.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Rn.yaml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ru.yaml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.S.yaml
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Sb.yaml
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Sc.yaml
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Se.yaml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Si.yaml
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Sn.yaml
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Sr.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ta.yaml
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Tc.yaml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Te.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ti.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Tl.yaml
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.V.yaml
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.W.yaml
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Xe.yaml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Y.yaml
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Zn.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Zr.yaml
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ag.yaml
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Al.yaml
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.B.yaml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Be.yaml
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.C.yaml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ca.yaml
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Cd.yaml
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Cl.yaml
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.F.yaml
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.H.yaml
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.He.yaml
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.K.yaml
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Li.yaml
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Mg.yaml
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Mo.yaml
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.N.yaml
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Nb.yaml
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ne.yaml
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.O.yaml
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.P.yaml
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Pd.yaml
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Rh.yaml
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ru.yaml
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Sc.yaml
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Si.yaml
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Sr.yaml
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Tc.yaml
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ti.yaml
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.V.yaml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Y.yaml
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Zr.yaml
--rw-r--r--   0        0        0     8803 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/ASEInterop.py
--rw-r--r--   0        0        0    18050 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/BabelInterop.py
--rw-r--r--   0        0        0     8527 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/DFTBInterop.py
--rw-r--r--   0        0        0    23836 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/DNAviewerInterop.py
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/DispersionInterop.py
--rw-r--r--   0        0        0     7254 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/MRChemInterop.py
--rw-r--r--   0        0        0    15188 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/OpenMMInterop.py
--rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/PSI4Interop.py
--rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/PolarisInterop.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/RDKitInterop.py
--rw-r--r--   0        0        0    16874 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/XTBInterop.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/Interop/__init__.py
--rw-r--r--   0        0        0     8654 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/DeltaTest.py
--rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/InputGenerator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/__init__.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ag.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Al.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ar.cif
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/As.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Au.cif
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/B.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ba.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Be.cif
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Bi.cif
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Br.cif
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/C.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ca.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Cd.cif
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Cl.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Co.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Cr.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Cs.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Cu.cif
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/F.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Fe.cif
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ga.cif
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ge.cif
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/H.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/He.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Hf.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Hg.cif
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/I.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/In.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ir.cif
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/K.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Kr.cif
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Li.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Lu.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Mg.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Mn.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Mo.cif
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/N.cif
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Na.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Nb.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ne.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ni.cif
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/O.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Os.cif
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/P.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Pb.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Pd.cif
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Po.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Pt.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Rb.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Re.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Rh.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Rn.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ru.cif
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/S.cif
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Sb.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Sc.cif
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Se.cif
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Si.cif
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Sn.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Sr.cif
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ta.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Tc.cif
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Te.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Ti.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Tl.cif
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/V.cif
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/W.cif
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Xe.cif
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Y.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Zn.cif
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/CIFs/Zr.cif
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/__init__.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Ag
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Al
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.B
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Be
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.C
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Ca
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Cd
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Cl
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.F
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.H
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.He
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.K
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Li
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Mg
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Mo
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.N
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Nb
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Ne
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.O
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.P
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Pd
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Rh
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Ru
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Sc
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Si
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Sr
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Tc
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Ti
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.V
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Y
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Zr
--rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/conf.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/docGeneration.rst
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/index.rst
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/requirements.txt
--rw-r--r--   0        0        0   334081 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/BandStructure.ipynb
--rw-r--r--   0        0        0   280632 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/BandStructure.pdf
--rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/BandStructure.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/CH4_posinp.xyz
--rw-r--r--   0        0        0    21304 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/FragmentStudio.ipynb
--rw-r--r--   0        0        0     5541 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/GeometryOptimization.ipynb
--rw-r--r--   0        0        0    51537 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/LinearCubicComparison.ipynb
--rw-r--r--   0        0        0    18637 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/Link with Fortran and BigDFT in Notebooks.ipynb
--rw-r--r--   0        0        0   159640 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/Logfile-basics.pdf
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/Logfile-basics.py
--rw-r--r--   0        0        0     7222 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/QMMM-Fragments.ipynb
--rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/QMMM-Fragments.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/README
--rw-r--r--   0        0        0   291676 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/Spin-Polarization.ipynb
--rw-r--r--   0        0        0    45853 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/Tutorial-N2.ipynb
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/posinp.xyz
--rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/0004.xyz
--rw-r--r--   0        0        0   379025 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/BigCase.xyz
--rw-r--r--   0        0        0   234946 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/GEOPT-all_sqnmbiomode.out.ref.yaml
--rw-r--r--   0        0        0   495823 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/log-Graphene.yaml
--rw-r--r--   0        0        0    71825 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/log-HBDMI.yaml
--rw-r--r--   0        0        0  1963112 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/log-K.yaml
--rw-r--r--   0        0        0  4801577 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/log-snap02000-fullQM.yaml
--rw-r--r--   0        0        0   300521 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/newbig-rigid.xyz
--rw-r--r--   0        0        0     8481 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/newcenters2.xyz
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/psppar.N
--rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/three.xyz
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/notebooks/testfiles/two.xyz
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/sphinx_static/bigdft-logo-reduced.svg
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/sphinx_static/custom.css
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/sphinx_static/logo-bigdft-white.svg
--rw-r--r--   0        0        0     9142 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/sphinx_static/logo_header.png
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pybigdft-1.0.6/source/templates/module.rst_t
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 pybigdft-1.0.6/.gitignore
--rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 pybigdft-1.0.6/COPYING
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pybigdft-1.0.6/ReadMe.md
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 pybigdft-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     9951 2020-02-02 00:00:00.000000 pybigdft-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 pybigdft-1.0.7/.gitrepo
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pybigdft-1.0.7/MANIFEST.in
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pybigdft-1.0.7/Makefile-sphinxbuild
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 pybigdft-1.0.7/conftest.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pybigdft-1.0.7/setup.cfg
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 pybigdft-1.0.7/setup.py
+-rw-r--r--   0        0        0    21273 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Atoms.py
+-rw-r--r--   0        0        0    10061 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/BZ.py
+-rw-r--r--   0        0        0   131163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/BioQM.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/CDFT.py
+-rw-r--r--   0        0        0    30528 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Calculators.py
+-rw-r--r--   0        0        0    17573 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Datasets.py
+-rw-r--r--   0        0        0    23903 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/DoS.py
+-rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Fragments.py
+-rw-r--r--   0        0        0    25983 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/IO.py
+-rw-r--r--   0        0        0    30908 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/InputActions.py
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Inputfiles.py
+-rw-r--r--   0        0        0    28150 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/LRTDDFT.py
+-rwxr-xr-x   0        0        0     6227 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/LogUtils.py
+-rw-r--r--   0        0        0    33462 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Logfiles.py
+-rw-r--r--   0        0        0     6102 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/PointParticles.py
+-rw-r--r--   0        0        0    50145 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/PostProcessing.py
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Spillage.py
+-rw-r--r--   0        0        0    22494 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Stats.py
+-rw-r--r--   0        0        0    49379 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Systems.py
+-rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/UnitCells.py
+-rw-r--r--   0        0        0    22352 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Visualization.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/__init__.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/check_examples.py
+-rw-r--r--   0        0        0     5852 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/wahba.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/Molecules.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/__init__.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/postprocess.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/AlF.xyz
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/Ar.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/BF.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/BH2.xyz
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/BH2Cl.xyz
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/BH2F.xyz
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/BH3.xyz
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/BHF2.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/BN.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/BO.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/BS.xyz
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/Be.xyz
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/BeH.xyz
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/BeH2.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/C2H.xyz
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/C2H2.xyz
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/C2H3.xyz
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/C2H4.xyz
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/C2H6O.xyz
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/C9H12.xyz
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CH2-t.xyz
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CH2.xyz
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CH2BH.xyz
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CH2F.xyz
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CH2NH.xyz
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CH2PH.xyz
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CH3.xyz
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CH3BH2.xyz
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CH3Cl.xyz
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CH3F.xyz
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CH3NH2.xyz
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CH3O.xyz
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CH3OH.xyz
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CH3SH.xyz
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CH4.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CN.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CO.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CO2.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CS.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/CSO.xyz
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/Cl2.xyz
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/ClCN.xyz
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/ClF.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/F2.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/FCN.xyz
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/FCO.xyz
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/FH-OH.xyz
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/FNO.xyz
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/H.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/H2.xyz
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/H2CN.xyz
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/H2O-Li.xyz
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/H2O.xyz
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HBO.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HBS.xyz
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HCCCl.xyz
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HCCF.xyz
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HCHO.xyz
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HCHS.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HCN.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HCO.xyz
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HCONH2.xyz
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HCOOH.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HCP.xyz
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HCl.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HF.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HNC.xyz
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HNO.xyz
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HNS.xyz
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HO2.xyz
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HOCl.xyz
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HOF.xyz
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/HOOH.xyz
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/He.xyz
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/Li.xyz
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/Li2.xyz
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/LiBH4.xyz
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/LiCN.xyz
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/LiCl.xyz
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/LiH.xyz
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/Mg.xyz
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/Mg2.xyz
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/N.xyz
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/N2.xyz
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/N2H2.xyz
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/N2H4.xyz
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/NCO.xyz
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/NH.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/NH2.xyz
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/NH2Cl.xyz
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/NH2F.xyz
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/NH2OH.xyz
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/NH3.xyz
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/NH3O.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/NO.xyz
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/NOCl.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/NP.xyz
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/Na.xyz
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/Na2.xyz
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/NaCN.xyz
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/NaCl.xyz
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/NaH.xyz
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/NaLi.xyz
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/Ne.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/O2.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/O3.xyz
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/OCl.xyz
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/OCl2.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/OF.xyz
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/OF2.xyz
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/OH.xyz
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/P.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/P2.xyz
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/P2H4.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/PH.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/PH2.xyz
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/PH2OH.xyz
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/PH3.xyz
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/PH3O.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/PS.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/S2.xyz
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/S2H2.xyz
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/SCl.xyz
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/SCl2.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/SF.xyz
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/SF2.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/SH.xyz
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/SH2.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/SO-trip.xyz
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/SO.xyz
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/SO2.xyz
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/Si4.xyz
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/SiH3.xyz
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/SiH3Cl.xyz
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/SiH3F.xyz
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/SiH4.xyz
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/XYZs/SiO.xyz
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ag.yaml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Al.yaml
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ar.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.As.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.At.yaml
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Au.yaml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.B.yaml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ba.yaml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Be.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Bi.yaml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Br.yaml
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.C.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ca.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Cd.yaml
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ce.yaml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Cl.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Co.yaml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Cr.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Cs.yaml
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Cu.yaml
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Dy.yaml
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Er.yaml
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Eu.yaml
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.F.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Fe.yaml
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ga.yaml
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Gd.yaml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ge.yaml
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.H.yaml
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.He.yaml
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Hf.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Hg.yaml
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ho.yaml
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.I.yaml
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.In.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ir.yaml
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.K.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Kr.yaml
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.La.yaml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Li.yaml
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Lu.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Mg.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Mn.yaml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Mo.yaml
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.N.yaml
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Na.yaml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Nb.yaml
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Nd.yaml
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ne.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ni.yaml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.O.yaml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Os.yaml
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.P.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Pb.yaml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Pd.yaml
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Pm.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Po.yaml
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Pr.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Pt.yaml
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Rb.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Re.yaml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Rh.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Rn.yaml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ru.yaml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.S.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Sb.yaml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Sc.yaml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Se.yaml
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Si.yaml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Sm.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Sn.yaml
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Sr.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ta.yaml
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Tb.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Tc.yaml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Te.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ti.yaml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Tl.yaml
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Tm.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.V.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.W.yaml
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Xe.yaml
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Y.yaml
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Yb.yaml
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Zn.yaml
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Zr.yaml
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ag.yaml
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Al.yaml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ar.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.As.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.At.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Au.yaml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.B.yaml
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ba.yaml
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Be.yaml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Bi.yaml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Br.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.C.yaml
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ca.yaml
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Cd.yaml
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Cl.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Co.yaml
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Cr.yaml
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Cs.yaml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Cu.yaml
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.F.yaml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Fe.yaml
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ga.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ge.yaml
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.H.yaml
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.He.yaml
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Hf.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Hg.yaml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.I.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.In.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ir.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.K.yaml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Kr.yaml
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.La.yaml
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Li.yaml
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Mg.yaml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Mn.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Mo.yaml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.N.yaml
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Na.yaml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Nb.yaml
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ne.yaml
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ni.yaml
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.O.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Os.yaml
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.P.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Pb.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Pd.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Po.yaml
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Pt.yaml
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Rb.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Re.yaml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Rh.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Rn.yaml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ru.yaml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.S.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Sb.yaml
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Sc.yaml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Se.yaml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Si.yaml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Sn.yaml
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Sr.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ta.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Tc.yaml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Te.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ti.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Tl.yaml
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.V.yaml
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.W.yaml
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Xe.yaml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Y.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Zn.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Zr.yaml
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Ag.yaml
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Al.yaml
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.B.yaml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Be.yaml
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.C.yaml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Ca.yaml
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Cd.yaml
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Cl.yaml
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.F.yaml
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.H.yaml
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.He.yaml
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.K.yaml
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Li.yaml
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Mg.yaml
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Mo.yaml
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.N.yaml
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Nb.yaml
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Ne.yaml
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.O.yaml
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.P.yaml
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Pd.yaml
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Rh.yaml
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Ru.yaml
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Sc.yaml
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Si.yaml
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Sr.yaml
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Tc.yaml
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Ti.yaml
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.V.yaml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Y.yaml
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Zr.yaml
+-rw-r--r--   0        0        0     8803 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Interop/ASEInterop.py
+-rw-r--r--   0        0        0    18050 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Interop/BabelInterop.py
+-rw-r--r--   0        0        0     8527 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Interop/DFTBInterop.py
+-rw-r--r--   0        0        0    23836 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Interop/DNAviewerInterop.py
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Interop/DispersionInterop.py
+-rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Interop/MRChemInterop.py
+-rw-r--r--   0        0        0     9934 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Interop/NWChemInterop.py
+-rw-r--r--   0        0        0    15188 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Interop/OpenMMInterop.py
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Interop/PSI4Interop.py
+-rw-r--r--   0        0        0    12732 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Interop/PolarisInterop.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Interop/RDKitInterop.py
+-rw-r--r--   0        0        0    16874 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Interop/XTBInterop.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/Interop/__init__.py
+-rw-r--r--   0        0        0     8654 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/DeltaTest.py
+-rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/InputGenerator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/__init__.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Ag.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Al.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Ar.cif
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/As.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Au.cif
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/B.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Ba.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Be.cif
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Bi.cif
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Br.cif
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/C.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Ca.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Cd.cif
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Cl.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Co.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Cr.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Cs.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Cu.cif
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/F.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Fe.cif
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Ga.cif
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Ge.cif
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/H.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/He.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Hf.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Hg.cif
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/I.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/In.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Ir.cif
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/K.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Kr.cif
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Li.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Lu.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Mg.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Mn.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Mo.cif
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/N.cif
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Na.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Nb.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Ne.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Ni.cif
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/O.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Os.cif
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/P.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Pb.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Pd.cif
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Po.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Pt.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Rb.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Re.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Rh.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Rn.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Ru.cif
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/S.cif
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Sb.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Sc.cif
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Se.cif
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Si.cif
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Sn.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Sr.cif
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Ta.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Tc.cif
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Te.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Ti.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Tl.cif
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/V.cif
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/W.cif
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Xe.cif
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Y.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Zn.cif
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/CIFs/Zr.cif
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/__init__.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Ag
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Al
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.B
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Be
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.C
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Ca
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Cd
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Cl
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.F
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.H
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.He
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.K
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Li
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Mg
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Mo
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.N
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Nb
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Ne
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.O
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.P
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Pd
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Rh
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Ru
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Sc
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Si
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Sr
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Tc
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Ti
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.V
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Y
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Zr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pybigdft-1.0.7/source/BigDFT_log.yaml
+-rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 pybigdft-1.0.7/source/conf.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 pybigdft-1.0.7/source/coverage_log.yaml
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 pybigdft-1.0.7/source/docGeneration.rst
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 pybigdft-1.0.7/source/index.rst
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pybigdft-1.0.7/source/requirements.txt
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 pybigdft-1.0.7/source/sphinx_static/bigdft-logo-reduced.svg
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 pybigdft-1.0.7/source/sphinx_static/custom.css
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 pybigdft-1.0.7/source/sphinx_static/logo-bigdft-white.svg
+-rw-r--r--   0        0        0     9142 2020-02-02 00:00:00.000000 pybigdft-1.0.7/source/sphinx_static/logo_header.png
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pybigdft-1.0.7/source/templates/module.rst_t
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 pybigdft-1.0.7/.gitignore
+-rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 pybigdft-1.0.7/COPYING
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pybigdft-1.0.7/ReadMe.md
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 pybigdft-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     9951 2020-02-02 00:00:00.000000 pybigdft-1.0.7/PKG-INFO
```

### Comparing `pybigdft-1.0.6/Makefile-sphinxbuild` & `pybigdft-1.0.7/Makefile-sphinxbuild`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/conftest.py` & `pybigdft-1.0.7/conftest.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/setup.py` & `pybigdft-1.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 setup(name="PyBigDFT",
       version="1.0",
       description="Python module for BigDFT drivers and analysis",
       author="Luigi Genovese",
       author_email="luigi.genovese@cea.fr",
       url="www.bigdft.org",
       license='GNU-GPL',
-      packages=setuptools.find_packages(),
+      packages=setuptools.find_namespace_packages(),
       install_requires=['numpy', 'scipy', 'PyFutile'],
       # setup_requires = ['pytest-runner'],
       tests_require=['nbval'],
       # 'package' package must contain files (see list above)
       # I called the package 'package' thus cleverly confusing the whole issue
       # This dict maps the package name =to=> directories
       # It says, package *needs* these files.
```

### Comparing `pybigdft-1.0.6/BigDFT/Atoms.py` & `pybigdft-1.0.7/BigDFT/Atoms.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/BZ.py` & `pybigdft-1.0.7/BigDFT/BZ.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/BioQM.py` & `pybigdft-1.0.7/BigDFT/BioQM.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,26 +355,28 @@
            residues of the structure. Some of the fragments may be missing as
            they may have been merged of not associated to elements of the
            sequence. The second list is the list of the ordered residues.
     """
     from BigDFT.Atoms import AU_to_A
     import numpy as np
     reslist = []
-    centroids_dict = {frag: system[frag].centroid * AU_to_A for frag in system}
+    centroids_dict = {frag: np.array(system[frag].centroid) * AU_to_A
+                      for frag in system}
     original_residues = []
     for residue in structure.get_residues():
         restuple = construct_res_tuple(residue)
         centroid = sum([a.coord for a in residue.get_atoms()]) / len(residue)
         found = False
         for frag in centroids_dict:
             fragtuple = construct_frag_tuple(frag)
             if not strict:
                 found = restuple == fragtuple
             else:
-                found = np.linalg.norm(centroids_dict[frag] - centroid) < 1.e-4
+                found = np.linalg.norm(
+                    centroids_dict[frag] - np.array(centroid)) < 1.e-4
             if found:
                 reslist.append(frag)
                 centroids_dict.pop(frag)
                 break
         if not found:
             reslist.append(None)
         original_residues.append(residue)
@@ -2188,14 +2190,15 @@
         Retrieve the information about the fragments which have not been
         matched inside the sequence
 
         Returns:
            dict: a Dictionary of the fragment that have not been recognized
         """
         from BigDFT.Atoms import AU_to_A
+        from numpy import array
         info = {'expected': {}, 'found': {}}
         expected = []
         for inum, (frag, residue) in enumerate(zip(self.frag_to_residues,
                                                    self.residues)):
             if frag is not None:
                 letter = self.fragment_letters[self.fragment_names.index(frag)]
             if frag is not None and letter is not None:
@@ -2205,15 +2208,15 @@
                  'centroid': list(centroid), 'nat': len(residue),
                  'residue': residue}
             expected += [{at.element: list(at.coord/AU_to_A), 'units': 'bohr'}
                          for at in residue.get_atoms()]
         found = System()
         for frag in self.unmatched_fragments:
             info['found'][frag] = {'centroid':
-                                   list(self[frag].centroid*AU_to_A),
+                                   list(array(self[frag].centroid)*AU_to_A),
                                    'nat': len(self[frag]),
                                    'fragment': self[frag]}
             found[frag] = self[frag]
         if len(expected) > 0:
             info['lookup'] = found.compute_matching(atlist=expected)
         return info
```

### Comparing `pybigdft-1.0.6/BigDFT/CDFT.py` & `pybigdft-1.0.7/BigDFT/CDFT.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Calculators.py` & `pybigdft-1.0.7/BigDFT/Calculators.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Datasets.py` & `pybigdft-1.0.7/BigDFT/Datasets.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/DoS.py` & `pybigdft-1.0.7/BigDFT/DoS.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Fragments.py` & `pybigdft-1.0.7/BigDFT/Fragments.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/IO.py` & `pybigdft-1.0.7/BigDFT/IO.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/InputActions.py` & `pybigdft-1.0.7/BigDFT/InputActions.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Inputfiles.py` & `pybigdft-1.0.7/BigDFT/Inputfiles.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/LRTDDFT.py` & `pybigdft-1.0.7/BigDFT/LRTDDFT.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/LogUtils.py` & `pybigdft-1.0.7/BigDFT/LogUtils.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Logfiles.py` & `pybigdft-1.0.7/BigDFT/Logfiles.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/PointParticles.py` & `pybigdft-1.0.7/BigDFT/PointParticles.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/PostProcessing.py` & `pybigdft-1.0.7/BigDFT/PostProcessing.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Spillage.py` & `pybigdft-1.0.7/BigDFT/Spillage.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Stats.py` & `pybigdft-1.0.7/BigDFT/Stats.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Systems.py` & `pybigdft-1.0.7/BigDFT/Systems.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,16 @@
 
         Returns:
           (str): the name of the fragment.
           (Fragment): the fragment object
         """
         import numpy as np
         CMs = [frag.centroid for frag in self.values()]
-        idx = np.argmin([np.dot(dd, dd.T) for dd in (CMs - self.centroid)])
+        idx = np.argmin([np.dot(dd, dd.T)
+                         for dd in (CMs - np.array(self.centroid))])
         return list(self.keys())[idx], list(self.values())[idx]
 
     def get_external_potential(self, units="bohr", charge_offset=False):
         """
         Transform the system information into a dictionary ready to be
         put as an external potential.
 
@@ -966,15 +967,15 @@
     nsubplots = len(cns)
     if axs is None:
         fig, axs = plt.subplots(1, nsubplots)
     else:
         fig = None
     for ax, cn, title in zip(axs, cns, titles):
         ax.set_title(title)
-        system_violinplot(cn, ax, widths=1.0)
+        system_violinplot(cn, ax, reuse_ticks=True, widths=1.0)
     if fig is not None:
         fig.tight_layout()
     return axs
 
 
 def validate_dataframe_representation(sys, df):
     """
```

### Comparing `pybigdft-1.0.6/BigDFT/UnitCells.py` & `pybigdft-1.0.7/BigDFT/UnitCells.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Visualization.py` & `pybigdft-1.0.7/BigDFT/Visualization.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/check_examples.py` & `pybigdft-1.0.7/BigDFT/check_examples.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,17 +37,21 @@
                 # Import the module we found
                 module = __import__(modname, fromlist="dummy")
 
                 # See if it has an example routine.
                 if hasattr(module, "_example"):
                     name = modname.replace(".", "_").replace("/", "")
                     # Skip some of the interop modules.
-                    if any([x in name for x in ["ASEInterop", "BabelInterop",
-                                                "DFTBInterop", "MRChemInterop",
-                                                "PSI4Interop", "XTBInterop",
+                    if any([x in name for x in ["ASEInterop",
+                                                "BabelInterop",
+                                                "DFTBInterop",
+                                                "MRChemInterop",
+                                                "NWChemInterop",
+                                                "PSI4Interop",
+                                                "XTBInterop",
                                                 "Visualization"]]):
                         continue
                     dict["test_" + name] = gen_test(name, module)
             except ModuleNotFoundError:
                 continue
 
         return type.__new__(mcs, name, bases, dict)
```

### Comparing `pybigdft-1.0.6/BigDFT/wahba.py` & `pybigdft-1.0.7/BigDFT/wahba.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/Molecules.py` & `pybigdft-1.0.7/BigDFT/Database/Molecules.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/postprocess.yaml` & `pybigdft-1.0.7/BigDFT/Database/postprocess.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/XYZs/C9H12.xyz` & `pybigdft-1.0.7/BigDFT/Database/XYZs/C9H12.xyz`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ag.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ag.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Al.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Al.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ar.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ar.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.As.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.As.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.At.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.At.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Au.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Au.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.B.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.B.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ba.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ba.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Be.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Be.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Bi.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Bi.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Br.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Br.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.C.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.C.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ca.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ca.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cd.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Cd.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ce.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ce.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cl.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Cl.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Co.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Co.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cr.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Cr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cs.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Cs.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Cu.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Cu.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Dy.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Dy.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Er.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Er.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Eu.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Eu.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.F.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.F.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Fe.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Fe.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ga.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ga.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Gd.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Gd.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ge.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ge.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Hf.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Hf.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Hg.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Hg.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ho.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ho.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.I.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.I.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.In.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.In.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ir.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ir.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.K.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.K.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Kr.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Kr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.La.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.La.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Li.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Li.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Lu.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Lu.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Mg.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Mg.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Mn.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Mn.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Mo.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Mo.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.N.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.N.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Na.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Na.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Nb.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Nb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Nd.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Nd.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ne.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ne.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ni.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ni.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.O.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.O.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Os.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Os.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.P.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.P.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pb.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Pb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pd.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Pd.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pm.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Pm.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Po.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Po.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pr.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Pr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Pt.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Pt.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Rb.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Rb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Re.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Re.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Rh.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Rh.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Rn.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Rn.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ru.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ru.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.S.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.S.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sb.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Sb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sc.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Sc.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Se.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Se.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Si.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Si.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sm.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Sm.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sn.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Sn.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Sr.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Sr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ta.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ta.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Tb.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Tb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Tc.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Tc.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Te.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Te.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Ti.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Ti.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Tl.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Tl.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Tm.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Tm.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.V.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.V.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.W.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.W.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Xe.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Xe.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Y.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Y.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Yb.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Yb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Zn.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Zn.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/LDA/psppar.Zr.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/LDA/psppar.Zr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ag.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ag.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Al.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Al.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ar.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ar.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.As.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.As.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.At.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.At.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Au.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Au.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.B.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.B.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ba.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ba.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Bi.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Bi.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Br.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Br.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.C.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.C.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ca.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ca.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cd.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Cd.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cl.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Cl.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Co.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Co.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cr.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Cr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cs.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Cs.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Cu.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Cu.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.F.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.F.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Fe.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Fe.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ga.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ga.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ge.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ge.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Hf.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Hf.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Hg.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Hg.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.I.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.I.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.In.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.In.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ir.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ir.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.K.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.K.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Kr.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Kr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.La.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.La.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Mg.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Mg.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Mn.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Mn.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Mo.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Mo.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.N.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.N.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Na.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Na.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Nb.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Nb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ne.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ne.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ni.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ni.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.O.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.O.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Os.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Os.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.P.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.P.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Pb.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Pb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Pd.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Pd.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Po.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Po.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Pt.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Pt.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Rb.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Rb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Re.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Re.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Rh.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Rh.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Rn.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Rn.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ru.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ru.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.S.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.S.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Sb.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Sb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Sc.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Sc.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Se.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Se.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Si.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Si.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Sn.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Sn.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Sr.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Sr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ta.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ta.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Tc.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Tc.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Te.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Te.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Ti.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Ti.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Tl.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Tl.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.V.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.V.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.W.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.W.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Xe.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Xe.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Y.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Y.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Zn.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Zn.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/Krack/PBE/psppar.Zr.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/Krack/PBE/psppar.Zr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ag.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Ag.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Al.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Al.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.B.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.B.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Be.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Be.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.C.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.C.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ca.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Ca.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Cd.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Cd.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Cl.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Cl.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.F.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.F.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.K.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.K.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Li.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Li.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Mg.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Mg.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Mo.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Mo.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.N.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.N.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Nb.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Nb.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ne.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Ne.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.O.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.O.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.P.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.P.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Pd.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Pd.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Rh.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Rh.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ru.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Ru.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Sc.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Sc.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Si.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Si.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Sr.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Sr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Tc.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Tc.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Ti.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Ti.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.V.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.V.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Y.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Y.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Database/psppar/SS/psppar.Zr.yaml` & `pybigdft-1.0.7/BigDFT/Database/psppar/SS/psppar.Zr.yaml`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Interop/ASEInterop.py` & `pybigdft-1.0.7/BigDFT/Interop/ASEInterop.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Interop/BabelInterop.py` & `pybigdft-1.0.7/BigDFT/Interop/BabelInterop.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Interop/DFTBInterop.py` & `pybigdft-1.0.7/BigDFT/Interop/DFTBInterop.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Interop/DNAviewerInterop.py` & `pybigdft-1.0.7/BigDFT/Interop/DNAviewerInterop.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Interop/DispersionInterop.py` & `pybigdft-1.0.7/BigDFT/Interop/DispersionInterop.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Interop/MRChemInterop.py` & `pybigdft-1.0.7/BigDFT/Interop/MRChemInterop.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 from BigDFT.Calculators import Runner
 from futile.Utils import write as safe_print
 
 
 class MRChemLogfile(dict):
     """
-    This class stores the values of the result.tag generated by DFTB+.
+    This class stores the detailed output from MRChem.
 
     Attributes:
         energy (float): the energy of the system
     """
     def __init__(self, logname):
         self._process_values(logname)
 
@@ -119,15 +119,15 @@
         return {'logname': join(self.run_dir, self._get_logname())}
 
     def post_processing(self, logname, command):
         """
         Post processing the calculation.
 
         Returns:
-            (BigDFT.Interop.DFTBInterop.DFTBLogfile): a representation of the
+            (BigDFT.Interop.MRChemLogfile): a representation of the
             detailed output.
         """
         from json import JSONDecodeError
         from os.path import join
 
         try:
             logname = join(self.run_dir, self._get_logname())
```

### Comparing `pybigdft-1.0.6/BigDFT/Interop/OpenMMInterop.py` & `pybigdft-1.0.7/BigDFT/Interop/OpenMMInterop.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Interop/PSI4Interop.py` & `pybigdft-1.0.7/BigDFT/Interop/PSI4Interop.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Interop/PolarisInterop.py` & `pybigdft-1.0.7/BigDFT/Interop/PolarisInterop.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Interop/RDKitInterop.py` & `pybigdft-1.0.7/BigDFT/Interop/RDKitInterop.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/Interop/XTBInterop.py` & `pybigdft-1.0.7/BigDFT/Interop/XTBInterop.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/DeltaTest.py` & `pybigdft-1.0.7/BigDFT/scripts/DeltaTest.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/InputGenerator.py` & `pybigdft-1.0.7/BigDFT/scripts/InputGenerator.py`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ag.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Ag.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Al.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Al.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ar.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Ar.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/As.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/As.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Au.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Au.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/B.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/B.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ba.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Ba.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Be.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Be.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Bi.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Bi.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Br.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Br.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/C.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/C.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ca.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Ca.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Cd.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Cd.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Cl.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Cl.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Co.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Co.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Cr.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Cr.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Cs.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Cs.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Cu.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Cu.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/F.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/F.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Fe.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Fe.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ga.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Ga.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ge.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Ge.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/H.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/H.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/He.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/He.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Hf.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Hf.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Hg.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Hg.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/I.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/I.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/In.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/In.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ir.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Ir.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/K.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/K.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Kr.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Kr.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Li.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Li.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Lu.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Lu.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Mg.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Mg.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Mn.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Mn.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Mo.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Mo.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/N.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/N.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Na.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Na.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Nb.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Nb.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ne.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Ne.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ni.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Ni.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/O.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/O.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Os.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Os.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/P.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/P.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Pb.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Pb.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Pd.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Pd.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Po.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Po.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Pt.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Pt.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Rb.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Rb.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Re.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Re.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Rh.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Rh.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Rn.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Rn.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ru.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Ru.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/S.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/S.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Sb.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Sb.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Sc.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Sc.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Se.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Se.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Si.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Si.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Sn.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Sn.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Sr.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Sr.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ta.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Ta.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Tc.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Tc.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Te.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Te.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Ti.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Ti.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Tl.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Tl.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/V.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/V.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/W.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/W.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Xe.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Xe.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Y.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Y.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Zn.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Zn.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/CIFs/Zr.cif` & `pybigdft-1.0.7/BigDFT/scripts/CIFs/Zr.cif`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Ag` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Ag`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Al` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Al`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Ca` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Ca`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Cd` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Cd`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Cl` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Cl`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.K` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.K`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Mg` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Mg`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Mo` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Mo`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Nb` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Nb`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.P` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.P`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Pd` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Pd`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Rh` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Rh`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Ru` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Ru`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Sc` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Sc`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Si` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Si`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Sr` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Sr`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Tc` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Tc`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Ti` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Ti`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.V` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.V`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Y` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Y`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/BigDFT/scripts/psppar/psppar.Zr` & `pybigdft-1.0.7/BigDFT/scripts/psppar/psppar.Zr`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/source/conf.py` & `pybigdft-1.0.7/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from os import path as p
 import sys
 sourcepath = p.dirname(p.abspath(__file__))
 pybigdftpath = p.dirname(sourcepath)
 bigdftsuitepath = p.abspath(p.join(pybigdftpath, '..'))
 sys.path.insert(0, p.abspath(p.join(bigdftsuitepath, 'futile', 'python')))
 sys.path.insert(0, p.abspath(pybigdftpath))
-sys.path.insert(0, p.abspath(p.join(pybigdftpath, 'notebooks')))
 sys.path.insert(0, p.abspath(p.join(bigdftsuitepath, 'Coverage')))
 
 from Coverage import CoverageHandler
 
 print('#' * 72)
 # -- General configuration ------------------------------------------------
```

### Comparing `pybigdft-1.0.6/source/docGeneration.rst` & `pybigdft-1.0.7/source/docGeneration.rst`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/source/index.rst` & `pybigdft-1.0.7/source/index.rst`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/source/sphinx_static/bigdft-logo-reduced.svg` & `pybigdft-1.0.7/source/sphinx_static/bigdft-logo-reduced.svg`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/source/sphinx_static/logo-bigdft-white.svg` & `pybigdft-1.0.7/source/sphinx_static/logo-bigdft-white.svg`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/source/sphinx_static/logo_header.png` & `pybigdft-1.0.7/source/sphinx_static/logo_header.png`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/.gitignore` & `pybigdft-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/COPYING` & `pybigdft-1.0.7/COPYING`

 * *Files identical despite different names*

### Comparing `pybigdft-1.0.6/pyproject.toml` & `pybigdft-1.0.7/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyBigDFT"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="William Dawson", email="william.dawson@riken.jp"},
   { name="Damien Caliste", email="Damien.Caliste@cea.fr"},
   { name="Luigi Genovese", email="Luigi.Genovese@cea.fr"},
 ]
 
 description="Python utilities for BigDFT"
```

### Comparing `pybigdft-1.0.6/PKG-INFO` & `pybigdft-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBigDFT
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python utilities for BigDFT
 Project-URL: Homepage, https://bigdft.org
 Project-URL: Bug Tracker, https://gitlab.com/l_sim/bigdft-suite/-/issues
 Author-email: William Dawson <william.dawson@riken.jp>, Damien Caliste <Damien.Caliste@cea.fr>, Luigi Genovese <Luigi.Genovese@cea.fr>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

