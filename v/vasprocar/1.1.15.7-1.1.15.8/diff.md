# Comparing `tmp/vasprocar-1.1.15.7.tar.gz` & `tmp/vasprocar-1.1.15.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vasprocar-1.1.15.7.tar", last modified: Mon Jul 10 21:49:23 2023, max compression
+gzip compressed data, was "vasprocar-1.1.15.8.tar", last modified: Fri Jul 14 15:15:13 2023, max compression
```

## Comparing `vasprocar-1.1.15.7.tar` & `vasprocar-1.1.15.8.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 21:49:23.491193 vasprocar-1.1.15.7/
--rw-rw-rw-   0        0        0    35822 2023-01-01 17:34:12.000000 vasprocar-1.1.15.7/LICENSE.txt
--rw-rw-rw-   0        0        0     2220 2023-07-10 21:49:23.491193 vasprocar-1.1.15.7/PKG-INFO
--rw-rw-rw-   0        0        0     1589 2023-01-17 12:07:08.000000 vasprocar-1.1.15.7/README.md
--rw-rw-rw-   0        0        0      167 2023-07-10 21:49:23.491193 vasprocar-1.1.15.7/setup.cfg
--rw-rw-rw-   0        0        0     1234 2023-07-10 21:49:06.000000 vasprocar-1.1.15.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 21:49:23.347075 vasprocar-1.1.15.7/vasprocar/
--rw-rw-rw-   0        0        0      360 2023-04-28 15:54:36.000000 vasprocar-1.1.15.7/vasprocar/BibTeX.dat
--rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 vasprocar-1.1.15.7/vasprocar/DOI.png
--rw-rw-rw-   0        0        0     4569 2023-07-10 21:47:53.000000 vasprocar-1.1.15.7/vasprocar/VASProcar.py
--rw-rw-rw-   0        0        0      201 2023-03-10 21:53:46.000000 vasprocar-1.1.15.7/vasprocar/__init__.py
--rw-rw-rw-   0        0        0     4569 2023-07-10 21:47:53.000000 vasprocar-1.1.15.7/vasprocar/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 21:49:23.396126 vasprocar-1.1.15.7/vasprocar/src/
-drwxrwxrwx   0        0        0        0 2023-07-10 21:49:23.428205 vasprocar-1.1.15.7/vasprocar/src/_VASP/
--rw-rw-rw-   0        0        0    18256 2023-04-26 12:33:54.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/_info.py
--rw-rw-rw-   0        0        0    13975 2023-02-01 18:32:31.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/_info_b.py
--rw-rw-rw-   0        0        0    15757 2023-07-10 18:09:15.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/_label.py
--rw-rw-rw-   0        0        0    31402 2023-04-16 15:59:10.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/_nscf.py
--rw-rw-rw-   0        0        0     9428 2023-02-07 22:29:38.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/_var_kpoints.py
--rw-rw-rw-   0        0        0    20778 2023-07-03 13:16:41.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/chgcar.py
--rw-rw-rw-   0        0        0    32155 2023-02-06 18:01:33.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/contribuicao.py
--rw-rw-rw-   0        0        0    14022 2023-02-07 16:02:48.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/dielectric_function.py
--rw-rw-rw-   0        0        0    26717 2023-07-10 19:38:20.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/dos_pdos_ldos.py
--rw-rw-rw-   0        0        0    28742 2023-07-10 19:40:51.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/dos_pdos_ldos_[polarizado].py
--rw-rw-rw-   0        0        0    24344 2023-04-01 21:06:45.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/kpoints_2D_3D.py
--rw-rw-rw-   0        0        0    15068 2023-05-04 13:02:49.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/parchg.py
--rw-rw-rw-   0        0        0     8140 2023-04-27 16:07:00.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/poscar_replace.py
--rw-rw-rw-   0        0        0     4159 2023-07-03 14:06:19.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/postar_combination.py
--rw-rw-rw-   0        0        0    14843 2023-05-04 13:03:13.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/potencial.py
--rw-rw-rw-   0        0        0    15029 2023-05-04 13:03:33.000000 vasprocar-1.1.15.7/vasprocar/src/_VASP/wave_function.py
--rw-rw-rw-   0        0        0      626 2023-02-07 16:00:07.000000 vasprocar-1.1.15.7/vasprocar/src/_loop.py
--rw-rw-rw-   0        0        0    17882 2023-07-10 21:37:23.000000 vasprocar-1.1.15.7/vasprocar/src/_settings.py
--rw-rw-rw-   0        0        0     2897 2023-03-23 12:12:59.000000 vasprocar-1.1.15.7/vasprocar/src/_update.py
--rw-rw-rw-   0        0        0    17818 2023-07-10 19:22:09.000000 vasprocar-1.1.15.7/vasprocar/src/bandas_2D.py
--rw-rw-rw-   0        0        0    16604 2023-02-07 22:46:17.000000 vasprocar-1.1.15.7/vasprocar/src/bandas_3D.py
--rw-rw-rw-   0        0        0    14962 2023-02-07 22:46:24.000000 vasprocar-1.1.15.7/vasprocar/src/bandas_4D.py
--rw-rw-rw-   0        0        0     2100 2023-02-06 17:36:59.000000 vasprocar-1.1.15.7/vasprocar/src/correction_file.py
-drwxrwxrwx   0        0        0        0 2023-07-10 21:49:23.428205 vasprocar-1.1.15.7/vasprocar/src/etc/
--rw-rw-rw-   0        0        0      360 2023-04-28 15:54:36.000000 vasprocar-1.1.15.7/vasprocar/src/etc/BibTeX.dat
--rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 vasprocar-1.1.15.7/vasprocar/src/etc/DOI.png
--rw-rw-rw-   0        0        0   374410 2022-06-01 18:31:32.000000 vasprocar-1.1.15.7/vasprocar/src/etc/Greek_alphabet.jpg
--rw-rw-rw-   0        0        0    20078 2023-02-07 22:46:33.000000 vasprocar-1.1.15.7/vasprocar/src/fermi_surface.py
-drwxrwxrwx   0        0        0        0 2023-07-10 21:49:23.428205 vasprocar-1.1.15.7/vasprocar/src/inputs/
--rw-rw-rw-   0        0        0     1010 2023-07-10 21:45:59.000000 vasprocar-1.1.15.7/vasprocar/src/inputs/inputs.py
--rw-rw-rw-   0        0        0     3625 2023-07-10 21:43:57.000000 vasprocar-1.1.15.7/vasprocar/src/inputs/inputs_files.py
--rw-rw-rw-   0        0        0    16978 2023-04-27 19:31:37.000000 vasprocar-1.1.15.7/vasprocar/src/level_countour.py
-drwxrwxrwx   0        0        0        0 2023-07-10 21:49:23.475081 vasprocar-1.1.15.7/vasprocar/src/plot/
-drwxrwxrwx   0        0        0        0 2023-07-10 21:49:23.491193 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/
--rw-rw-rw-   0        0        0     5204 2023-04-28 13:13:46.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_bandas_2D.py
--rw-rw-rw-   0        0        0     4322 2023-05-04 14:16:22.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_chgcar.py
--rw-rw-rw-   0        0        0     4960 2023-04-28 13:17:27.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_dielectric_function.py
--rw-rw-rw-   0        0        0    13180 2023-04-28 13:22:43.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_dos_pdos_ldos.py
--rw-rw-rw-   0        0        0    13278 2023-04-28 15:25:56.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py
--rw-rw-rw-   0        0        0    11204 2023-04-28 15:27:51.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py
--rw-rw-rw-   0        0        0     3883 2023-05-03 16:43:07.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_parchg.py
--rw-rw-rw-   0        0        0     3807 2023-04-28 15:30:54.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_potencial.py
--rw-rw-rw-   0        0        0     6272 2023-04-28 15:35:06.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_projecao_localizacao.py
--rw-rw-rw-   0        0        0    11195 2023-04-28 15:41:27.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_projecao_orbitais.py
--rw-rw-rw-   0        0        0     6149 2023-04-28 15:45:01.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_projecao_psi.py
--rw-rw-rw-   0        0        0    10949 2023-04-28 15:49:29.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_projecao_spin.py
--rw-rw-rw-   0        0        0     4002 2023-04-28 15:51:35.000000 vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_wave_function.py
--rw-rw-rw-   0        0        0     6459 2023-04-26 19:46:07.000000 vasprocar-1.1.15.7/vasprocar/src/plot/_plot_settings.py
--rw-rw-rw-   0        0        0     5859 2023-04-26 19:52:01.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_bandas_2D.py
--rw-rw-rw-   0        0        0     5094 2023-04-27 16:26:15.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_bandas_3D_matplotlib.py
--rw-rw-rw-   0        0        0     5789 2023-04-27 16:25:56.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_bandas_3D_plotly.py
--rw-rw-rw-   0        0        0     5212 2023-04-27 16:30:27.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_bandas_4D_plotly.py
--rw-rw-rw-   0        0        0     5022 2023-05-04 14:15:37.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_chgcar.py
--rw-rw-rw-   0        0        0     4311 2023-04-27 16:32:25.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_dielectric_function.py
--rw-rw-rw-   0        0        0    12937 2023-04-27 16:41:40.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_dos_pdos_ldos.py
--rw-rw-rw-   0        0        0    34063 2023-04-27 16:53:46.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_dos_pdos_ldos_[polarizado].py
--rw-rw-rw-   0        0        0     8368 2023-04-27 16:59:55.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_fermi_surface.py
--rw-rw-rw-   0        0        0     6527 2023-04-27 17:03:00.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_level_countour.py
--rw-rw-rw-   0        0        0     4693 2023-05-03 16:43:27.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_parchg.py
--rw-rw-rw-   0        0        0     4693 2023-04-27 17:09:05.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_potencial.py
--rw-rw-rw-   0        0        0    14161 2023-04-27 18:34:47.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_projecao_localizacao.py
--rw-rw-rw-   0        0        0    26915 2023-04-27 18:40:15.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_projecao_orbitais.py
--rw-rw-rw-   0        0        0    14283 2023-04-27 18:48:44.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_projecao_psi.py
--rw-rw-rw-   0        0        0     7782 2023-04-27 18:53:12.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_projecao_spin.py
--rw-rw-rw-   0        0        0    11866 2023-04-27 19:17:24.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_2D.py
--rw-rw-rw-   0        0        0     9865 2023-04-27 19:05:41.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_3D.py
--rw-rw-rw-   0        0        0     6287 2023-04-27 19:06:44.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_4D.py
--rw-rw-rw-   0        0        0     6345 2023-04-27 19:08:37.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_4D_[iso].py
--rw-rw-rw-   0        0        0    15772 2023-04-27 19:29:40.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_contour.py
--rw-rw-rw-   0        0        0    17321 2023-04-27 19:30:01.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_contour_video.py
--rw-rw-rw-   0        0        0     4600 2023-04-27 17:12:08.000000 vasprocar-1.1.15.7/vasprocar/src/plot/plot_wave_function.py
--rw-rw-rw-   0        0        0    26728 2023-02-09 23:53:36.000000 vasprocar-1.1.15.7/vasprocar/src/projecao_localizacao.py
--rw-rw-rw-   0        0        0    28470 2023-07-10 19:37:56.000000 vasprocar-1.1.15.7/vasprocar/src/projecao_orbitais.py
--rw-rw-rw-   0        0        0    33246 2023-02-14 20:05:13.000000 vasprocar-1.1.15.7/vasprocar/src/projecao_psi.py
--rw-rw-rw-   0        0        0    25231 2023-07-10 19:36:12.000000 vasprocar-1.1.15.7/vasprocar/src/projecao_spin.py
--rw-rw-rw-   0        0        0    22748 2023-02-14 20:11:56.000000 vasprocar-1.1.15.7/vasprocar/src/spin_texture.py
--rw-rw-rw-   0        0        0    22318 2023-04-27 19:32:03.000000 vasprocar-1.1.15.7/vasprocar/src/spin_texture_contour.py
--rw-rw-rw-   0        0        0    23728 2023-04-27 19:32:28.000000 vasprocar-1.1.15.7/vasprocar/src/spin_texture_contour_video.py
-drwxrwxrwx   0        0        0        0 2023-07-10 21:49:23.380541 vasprocar-1.1.15.7/vasprocar.egg-info/
--rw-rw-rw-   0        0        0     2220 2023-07-10 21:49:23.000000 vasprocar-1.1.15.7/vasprocar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3244 2023-07-10 21:49:23.000000 vasprocar-1.1.15.7/vasprocar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 21:49:23.000000 vasprocar-1.1.15.7/vasprocar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-10 21:49:23.000000 vasprocar-1.1.15.7/vasprocar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       91 2023-07-10 21:49:23.000000 vasprocar-1.1.15.7/vasprocar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-10 21:49:23.000000 vasprocar-1.1.15.7/vasprocar.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 15:15:13.768681 vasprocar-1.1.15.8/
+-rw-rw-rw-   0        0        0    35822 2023-01-01 17:34:12.000000 vasprocar-1.1.15.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     2220 2023-07-14 15:15:13.768681 vasprocar-1.1.15.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1589 2023-01-17 12:07:08.000000 vasprocar-1.1.15.8/README.md
+-rw-rw-rw-   0        0        0      167 2023-07-14 15:15:13.769680 vasprocar-1.1.15.8/setup.cfg
+-rw-rw-rw-   0        0        0     1234 2023-07-14 15:15:04.000000 vasprocar-1.1.15.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:15:13.617628 vasprocar-1.1.15.8/vasprocar/
+-rw-rw-rw-   0        0        0      360 2023-04-28 15:54:36.000000 vasprocar-1.1.15.8/vasprocar/BibTeX.dat
+-rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 vasprocar-1.1.15.8/vasprocar/DOI.png
+-rw-rw-rw-   0        0        0     4620 2023-07-14 13:41:10.000000 vasprocar-1.1.15.8/vasprocar/VASProcar.py
+-rw-rw-rw-   0        0        0      201 2023-03-10 21:53:46.000000 vasprocar-1.1.15.8/vasprocar/__init__.py
+-rw-rw-rw-   0        0        0     4620 2023-07-14 13:41:10.000000 vasprocar-1.1.15.8/vasprocar/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:15:13.677622 vasprocar-1.1.15.8/vasprocar/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 15:15:13.702622 vasprocar-1.1.15.8/vasprocar/src/_VASP/
+-rw-rw-rw-   0        0        0    18256 2023-04-26 12:33:54.000000 vasprocar-1.1.15.8/vasprocar/src/_VASP/_info.py
+-rw-rw-rw-   0        0        0    13975 2023-02-01 18:32:31.000000 vasprocar-1.1.15.8/vasprocar/src/_VASP/_info_b.py
+-rw-rw-rw-   0        0        0    15757 2023-07-10 18:09:15.000000 vasprocar-1.1.15.8/vasprocar/src/_VASP/_label.py
+-rw-rw-rw-   0        0        0    31402 2023-04-16 15:59:10.000000 vasprocar-1.1.15.8/vasprocar/src/_VASP/_nscf.py
+-rw-rw-rw-   0        0        0     9428 2023-02-07 22:29:38.000000 vasprocar-1.1.15.8/vasprocar/src/_VASP/_var_kpoints.py
+-rw-rw-rw-   0        0        0    20778 2023-07-03 13:16:41.000000 vasprocar-1.1.15.8/vasprocar/src/_VASP/chgcar.py
+-rw-rw-rw-   0        0        0    32155 2023-02-06 18:01:33.000000 vasprocar-1.1.15.8/vasprocar/src/_VASP/contribuicao.py
+-rw-rw-rw-   0        0        0    14022 2023-02-07 16:02:48.000000 vasprocar-1.1.15.8/vasprocar/src/_VASP/dielectric_function.py
+-rw-rw-rw-   0        0        0    26716 2023-07-14 14:52:10.000000 vasprocar-1.1.15.8/vasprocar/src/_VASP/dos_pdos_ldos.py
+-rw-rw-rw-   0        0        0    28742 2023-07-10 19:40:51.000000 vasprocar-1.1.15.8/vasprocar/src/_VASP/dos_pdos_ldos_[polarizado].py
+-rw-rw-rw-   0        0        0    24344 2023-04-01 21:06:45.000000 vasprocar-1.1.15.8/vasprocar/src/_VASP/kpoints_2D_3D.py
+-rw-rw-rw-   0        0        0    15068 2023-05-04 13:02:49.000000 vasprocar-1.1.15.8/vasprocar/src/_VASP/parchg.py
+-rw-rw-rw-   0        0        0     8140 2023-04-27 16:07:00.000000 vasprocar-1.1.15.8/vasprocar/src/_VASP/poscar_replace.py
+-rw-rw-rw-   0        0        0     4159 2023-07-03 14:06:19.000000 vasprocar-1.1.15.8/vasprocar/src/_VASP/postar_combination.py
+-rw-rw-rw-   0        0        0    14843 2023-05-04 13:03:13.000000 vasprocar-1.1.15.8/vasprocar/src/_VASP/potencial.py
+-rw-rw-rw-   0        0        0    15029 2023-05-04 13:03:33.000000 vasprocar-1.1.15.8/vasprocar/src/_VASP/wave_function.py
+-rw-rw-rw-   0        0        0      626 2023-02-07 16:00:07.000000 vasprocar-1.1.15.8/vasprocar/src/_loop.py
+-rw-rw-rw-   0        0        0    17882 2023-07-14 15:11:57.000000 vasprocar-1.1.15.8/vasprocar/src/_settings.py
+-rw-rw-rw-   0        0        0     2897 2023-03-23 12:12:59.000000 vasprocar-1.1.15.8/vasprocar/src/_update.py
+-rw-rw-rw-   0        0        0    17818 2023-07-10 19:22:09.000000 vasprocar-1.1.15.8/vasprocar/src/bandas_2D.py
+-rw-rw-rw-   0        0        0    16604 2023-02-07 22:46:17.000000 vasprocar-1.1.15.8/vasprocar/src/bandas_3D.py
+-rw-rw-rw-   0        0        0    14962 2023-02-07 22:46:24.000000 vasprocar-1.1.15.8/vasprocar/src/bandas_4D.py
+-rw-rw-rw-   0        0        0     2100 2023-02-06 17:36:59.000000 vasprocar-1.1.15.8/vasprocar/src/correction_file.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:15:13.708646 vasprocar-1.1.15.8/vasprocar/src/etc/
+-rw-rw-rw-   0        0        0      360 2023-04-28 15:54:36.000000 vasprocar-1.1.15.8/vasprocar/src/etc/BibTeX.dat
+-rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 vasprocar-1.1.15.8/vasprocar/src/etc/DOI.png
+-rw-rw-rw-   0        0        0   374410 2022-06-01 18:31:32.000000 vasprocar-1.1.15.8/vasprocar/src/etc/Greek_alphabet.jpg
+-rw-rw-rw-   0        0        0    20078 2023-02-07 22:46:33.000000 vasprocar-1.1.15.8/vasprocar/src/fermi_surface.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:15:13.712625 vasprocar-1.1.15.8/vasprocar/src/inputs/
+-rw-rw-rw-   0        0        0     1022 2023-07-14 13:37:34.000000 vasprocar-1.1.15.8/vasprocar/src/inputs/inputs.py
+-rw-rw-rw-   0        0        0     4099 2023-07-14 13:39:46.000000 vasprocar-1.1.15.8/vasprocar/src/inputs/inputs_files.py
+-rw-rw-rw-   0        0        0    16978 2023-04-27 19:31:37.000000 vasprocar-1.1.15.8/vasprocar/src/level_countour.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:15:13.751685 vasprocar-1.1.15.8/vasprocar/src/plot/
+drwxrwxrwx   0        0        0        0 2023-07-14 15:15:13.767680 vasprocar-1.1.15.8/vasprocar/src/plot/Grace/
+-rw-rw-rw-   0        0        0     5204 2023-04-28 13:13:46.000000 vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_bandas_2D.py
+-rw-rw-rw-   0        0        0     4322 2023-05-04 14:16:22.000000 vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_chgcar.py
+-rw-rw-rw-   0        0        0     4960 2023-04-28 13:17:27.000000 vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_dielectric_function.py
+-rw-rw-rw-   0        0        0    13180 2023-04-28 13:22:43.000000 vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_dos_pdos_ldos.py
+-rw-rw-rw-   0        0        0    13278 2023-04-28 15:25:56.000000 vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py
+-rw-rw-rw-   0        0        0    11204 2023-04-28 15:27:51.000000 vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py
+-rw-rw-rw-   0        0        0     3883 2023-05-03 16:43:07.000000 vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_parchg.py
+-rw-rw-rw-   0        0        0     3807 2023-04-28 15:30:54.000000 vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_potencial.py
+-rw-rw-rw-   0        0        0     6272 2023-04-28 15:35:06.000000 vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_projecao_localizacao.py
+-rw-rw-rw-   0        0        0    11195 2023-04-28 15:41:27.000000 vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_projecao_orbitais.py
+-rw-rw-rw-   0        0        0     6149 2023-04-28 15:45:01.000000 vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_projecao_psi.py
+-rw-rw-rw-   0        0        0    10949 2023-04-28 15:49:29.000000 vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_projecao_spin.py
+-rw-rw-rw-   0        0        0     4002 2023-04-28 15:51:35.000000 vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_wave_function.py
+-rw-rw-rw-   0        0        0     6459 2023-04-26 19:46:07.000000 vasprocar-1.1.15.8/vasprocar/src/plot/_plot_settings.py
+-rw-rw-rw-   0        0        0     5859 2023-04-26 19:52:01.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_bandas_2D.py
+-rw-rw-rw-   0        0        0     5094 2023-04-27 16:26:15.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_bandas_3D_matplotlib.py
+-rw-rw-rw-   0        0        0     5789 2023-04-27 16:25:56.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_bandas_3D_plotly.py
+-rw-rw-rw-   0        0        0     5212 2023-04-27 16:30:27.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_bandas_4D_plotly.py
+-rw-rw-rw-   0        0        0     5022 2023-05-04 14:15:37.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_chgcar.py
+-rw-rw-rw-   0        0        0     4311 2023-04-27 16:32:25.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_dielectric_function.py
+-rw-rw-rw-   0        0        0    12937 2023-04-27 16:41:40.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_dos_pdos_ldos.py
+-rw-rw-rw-   0        0        0    34063 2023-04-27 16:53:46.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_dos_pdos_ldos_[polarizado].py
+-rw-rw-rw-   0        0        0     8368 2023-04-27 16:59:55.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_fermi_surface.py
+-rw-rw-rw-   0        0        0     6527 2023-04-27 17:03:00.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_level_countour.py
+-rw-rw-rw-   0        0        0     4693 2023-05-03 16:43:27.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_parchg.py
+-rw-rw-rw-   0        0        0     4693 2023-04-27 17:09:05.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_potencial.py
+-rw-rw-rw-   0        0        0    14161 2023-04-27 18:34:47.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_projecao_localizacao.py
+-rw-rw-rw-   0        0        0    26915 2023-04-27 18:40:15.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_projecao_orbitais.py
+-rw-rw-rw-   0        0        0    14283 2023-04-27 18:48:44.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_projecao_psi.py
+-rw-rw-rw-   0        0        0     7782 2023-04-27 18:53:12.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_projecao_spin.py
+-rw-rw-rw-   0        0        0    11866 2023-04-27 19:17:24.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_spin_texture_2D.py
+-rw-rw-rw-   0        0        0     9865 2023-04-27 19:05:41.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_spin_texture_3D.py
+-rw-rw-rw-   0        0        0     6287 2023-04-27 19:06:44.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_spin_texture_4D.py
+-rw-rw-rw-   0        0        0     6345 2023-04-27 19:08:37.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_spin_texture_4D_[iso].py
+-rw-rw-rw-   0        0        0    15772 2023-04-27 19:29:40.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_spin_texture_contour.py
+-rw-rw-rw-   0        0        0    17321 2023-04-27 19:30:01.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_spin_texture_contour_video.py
+-rw-rw-rw-   0        0        0     4600 2023-04-27 17:12:08.000000 vasprocar-1.1.15.8/vasprocar/src/plot/plot_wave_function.py
+-rw-rw-rw-   0        0        0    27685 2023-07-14 15:01:46.000000 vasprocar-1.1.15.8/vasprocar/src/projecao_localizacao.py
+-rw-rw-rw-   0        0        0    28470 2023-07-10 19:37:56.000000 vasprocar-1.1.15.8/vasprocar/src/projecao_orbitais.py
+-rw-rw-rw-   0        0        0    33246 2023-02-14 20:05:13.000000 vasprocar-1.1.15.8/vasprocar/src/projecao_psi.py
+-rw-rw-rw-   0        0        0    25231 2023-07-10 19:36:12.000000 vasprocar-1.1.15.8/vasprocar/src/projecao_spin.py
+-rw-rw-rw-   0        0        0    22748 2023-02-14 20:11:56.000000 vasprocar-1.1.15.8/vasprocar/src/spin_texture.py
+-rw-rw-rw-   0        0        0    22318 2023-04-27 19:32:03.000000 vasprocar-1.1.15.8/vasprocar/src/spin_texture_contour.py
+-rw-rw-rw-   0        0        0    23728 2023-04-27 19:32:28.000000 vasprocar-1.1.15.8/vasprocar/src/spin_texture_contour_video.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:15:13.647621 vasprocar-1.1.15.8/vasprocar.egg-info/
+-rw-rw-rw-   0        0        0     2220 2023-07-14 15:15:13.000000 vasprocar-1.1.15.8/vasprocar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3244 2023-07-14 15:15:13.000000 vasprocar-1.1.15.8/vasprocar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 15:15:13.000000 vasprocar-1.1.15.8/vasprocar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-14 15:15:13.000000 vasprocar-1.1.15.8/vasprocar.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       91 2023-07-14 15:15:13.000000 vasprocar-1.1.15.8/vasprocar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 15:15:13.000000 vasprocar-1.1.15.8/vasprocar.egg-info/top_level.txt
```

### Comparing `vasprocar-1.1.15.7/LICENSE.txt` & `vasprocar-1.1.15.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/PKG-INFO` & `vasprocar-1.1.15.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasprocar
-Version: 1.1.15.7
+Version: 1.1.15.8
 Summary: VASProcar is an open-source package written in the Python 3 programming language, which aims to provide an intuitive tool for the post-processing of the output files produced by the DFT VASP code, through an interactive user interface.
 Home-page: https://doi.org/10.5281/zenodo.6343960
 Download-URL: https://doi.org/10.5281/zenodo.6343960
 Author: Augusto de Lelis Araujo and Renan da Paixao Maciel
 Author-email: augusto-lelis@outlook.com, renan.maciel@physics.uu.se
 License: GNU GPLv3
 Description-Content-Type: text/markdown
```

### Comparing `vasprocar-1.1.15.7/README.md` & `vasprocar-1.1.15.8/README.md`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/setup.py` & `vasprocar-1.1.15.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 import json
 from pathlib import Path
 from typing import Optional
 
 setup(
     name = "vasprocar",
-    version = "1.1.15.7",
+    version = "1.1.15.8",
     entry_points={'console_scripts': ['vasprocar = vasprocar:main']},
     description = "VASProcar is an open-source package written in the Python 3 programming language, which aims to provide an intuitive tool for the post-processing of the output files produced by the DFT VASP code, through an interactive user interface.",
     author = "Augusto de Lelis Araujo and Renan da Paixao Maciel", 
     author_email = "augusto-lelis@outlook.com, renan.maciel@physics.uu.se",
     url = "https://doi.org/10.5281/zenodo.6343960",
     download_url = "https://doi.org/10.5281/zenodo.6343960",
     license = "GNU GPLv3",
```

### Comparing `vasprocar-1.1.15.7/vasprocar/DOI.png` & `vasprocar-1.1.15.8/vasprocar/DOI.png`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/VASProcar.py` & `vasprocar-1.1.15.8/vasprocar/VASProcar.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,12 +87,13 @@
 if (len(inputs) > 0):
    for inp in range(len(inputs)): 
        #---------------------------------------------------------------------------
        exec(open(dir_files + '/inputs/' + 'input.vasprocar.' + inputs[inp]).read())
        #---------------------------------------------------------------------------
        if (inputs[inp] == 'bands'):     opcao = -10
        if (inputs[inp] == 'spin'):      opcao = -20  
-       if (inputs[inp] == 'orbitals'):  opcao = -30  
-       if (inputs[inp] == 'dos'):       opcao = -31       
+       if (inputs[inp] == 'orbitals'):  opcao = -30
+       if (inputs[inp] == 'dos'):       opcao = -31  
+       if (inputs[inp] == 'location'):  opcao = -32     
        #--------------------------------------------------------------------
        run = main_dir + '_settings.py'
        exec(open(run).read())
```

### Comparing `vasprocar-1.1.15.7/vasprocar/__main__.py` & `vasprocar-1.1.15.8/vasprocar/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,12 +87,13 @@
 if (len(inputs) > 0):
    for inp in range(len(inputs)): 
        #---------------------------------------------------------------------------
        exec(open(dir_files + '/inputs/' + 'input.vasprocar.' + inputs[inp]).read())
        #---------------------------------------------------------------------------
        if (inputs[inp] == 'bands'):     opcao = -10
        if (inputs[inp] == 'spin'):      opcao = -20  
-       if (inputs[inp] == 'orbitals'):  opcao = -30  
-       if (inputs[inp] == 'dos'):       opcao = -31       
+       if (inputs[inp] == 'orbitals'):  opcao = -30
+       if (inputs[inp] == 'dos'):       opcao = -31  
+       if (inputs[inp] == 'location'):  opcao = -32     
        #--------------------------------------------------------------------
        run = main_dir + '_settings.py'
        exec(open(run).read())
```

### Comparing `vasprocar-1.1.15.7/vasprocar/src/_VASP/_info.py` & `vasprocar-1.1.15.8/vasprocar/src/_VASP/_info.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/_VASP/_info_b.py` & `vasprocar-1.1.15.8/vasprocar/src/_VASP/_info_b.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/_VASP/_label.py` & `vasprocar-1.1.15.8/vasprocar/src/_VASP/_label.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/_VASP/_nscf.py` & `vasprocar-1.1.15.8/vasprocar/src/_VASP/_nscf.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/_VASP/_var_kpoints.py` & `vasprocar-1.1.15.8/vasprocar/src/_VASP/_var_kpoints.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/_VASP/chgcar.py` & `vasprocar-1.1.15.8/vasprocar/src/_VASP/chgcar.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/_VASP/contribuicao.py` & `vasprocar-1.1.15.8/vasprocar/src/_VASP/contribuicao.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/_VASP/dielectric_function.py` & `vasprocar-1.1.15.8/vasprocar/src/_VASP/dielectric_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/_VASP/dos_pdos_ldos.py` & `vasprocar-1.1.15.8/vasprocar/src/_VASP/dos_pdos_ldos.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
                print ("Type in sequence the colors of pDOS Fyx2|Fxyz|Fyz2|Fzz2|Fxz2|Fzx2|Fxx2:      ")
                cor_orb = input ("Colors_of_Orbitals: ")
                #---------------------
                tcor = cor_orb.split()
                c_Fyx2 = int(tcor[0]); c_Fxyz = int(tcor[1]); c_Fyz2 = int(tcor[2]); c_Fzz2 = int(tcor[3])
                c_Fxz2 = int(tcor[4]); c_Fzx2 = int(tcor[5]); c_Fxx2 = int(tcor[6])
                #---------------------
-               print (" ")   
+               print (" ")  
 
    if (len(inputs) == 0):
       print ("##############################################################") 
       print ("with respect to energy, would you like? ======================") 
       print ("[0] Use the default energy value from DFT output =============")
       print ("[1] Shift the Fermi level to 0.0 eV  =========================")
       print ("##############################################################")
```

### Comparing `vasprocar-1.1.15.7/vasprocar/src/_VASP/dos_pdos_ldos_[polarizado].py` & `vasprocar-1.1.15.8/vasprocar/src/_VASP/dos_pdos_ldos_[polarizado].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/_VASP/kpoints_2D_3D.py` & `vasprocar-1.1.15.8/vasprocar/src/_VASP/kpoints_2D_3D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/_VASP/parchg.py` & `vasprocar-1.1.15.8/vasprocar/src/_VASP/parchg.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/_VASP/poscar_replace.py` & `vasprocar-1.1.15.8/vasprocar/src/_VASP/poscar_replace.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/_VASP/postar_combination.py` & `vasprocar-1.1.15.8/vasprocar/src/_VASP/postar_combination.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/_VASP/potencial.py` & `vasprocar-1.1.15.8/vasprocar/src/_VASP/potencial.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/_VASP/wave_function.py` & `vasprocar-1.1.15.8/vasprocar/src/_VASP/wave_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/_loop.py` & `vasprocar-1.1.15.8/vasprocar/src/_loop.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/_settings.py` & `vasprocar-1.1.15.8/vasprocar/src/_settings.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/_update.py` & `vasprocar-1.1.15.8/vasprocar/src/_update.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/bandas_2D.py` & `vasprocar-1.1.15.8/vasprocar/src/bandas_2D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/bandas_3D.py` & `vasprocar-1.1.15.8/vasprocar/src/bandas_3D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/bandas_4D.py` & `vasprocar-1.1.15.8/vasprocar/src/bandas_4D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/correction_file.py` & `vasprocar-1.1.15.8/vasprocar/src/correction_file.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/etc/DOI.png` & `vasprocar-1.1.15.8/vasprocar/src/etc/DOI.png`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/etc/Greek_alphabet.jpg` & `vasprocar-1.1.15.8/vasprocar/src/etc/Greek_alphabet.jpg`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/fermi_surface.py` & `vasprocar-1.1.15.8/vasprocar/src/fermi_surface.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/inputs/inputs.py` & `vasprocar-1.1.15.8/vasprocar/src/inputs/inputs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # VASProcar Copyright (C) 2023
 # GNU GPL-3.0 license
 
-inputs_types = ['bands','spin','orbitals','dos']
+inputs_types = ['bands','spin','orbitals','dos', 'location']
 inputs = []
 
 # ------------------------------------------------------------------------------
 # Checking if the "inputs" folder exists ---------------------------------------
 # ------------------------------------------------------------------------------
 if os.path.isdir(dir_files + '/inputs'):
     folder_input = 'yes'
```

### Comparing `vasprocar-1.1.15.7/vasprocar/src/inputs/inputs_files.py` & `vasprocar-1.1.15.8/vasprocar/src/inputs/inputs_files.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,49 +17,58 @@
 
 print("#######################################################")
 print("# Which input file do you want?                      ##")
 print("#######################################################")
 print("# [1] Bands (Plot 2D)                                ##")
 print("# [2] Projection of Spin components                  ##")
 print("# [3] Projection of Orbitals                         ##")
-print("# [4] DOS                                            ##")
-print("# [5] All input files                                ##")
+print("# [4] Projection of the REGIONS (Location)           ##")
+print("# [5] DOS                                            ##")
+print("# [6] All input files                                ##")
 print("#######################################################")
 tipo = input (" "); tipo = int(tipo)
 print(" ")
 
 #----------------------------------------------------------------------
 # Copy [input files] to the input folder directory --------------------
 #----------------------------------------------------------------------
 
-if (tipo == 1 or tipo == 5):
+if (tipo == 1 or tipo == 6):
    try: f = open(dir_files + '/inputs/input.vasprocar.bands'); f.close(); os.remove(dir_files + '/inputs/input.vasprocar.bands')
    except: 0 == 0
    #--------------------------------------------------
    source = main_dir + '/inputs/input.vasprocar.bands'
    destination = dir_files + '/inputs/input.vasprocar.bands'
    shutil.copyfile(source, destination)
 
-if (tipo == 2 or tipo == 5):
+if (tipo == 2 or tipo == 6):
    try: f = open(dir_files + '/inputs/input.vasprocar.spin'); f.close(); os.remove(dir_files + '/inputs/input.vasprocar.spin')
    except: 0 == 0
    #--------------------------------------------------
    source = main_dir + '/inputs/input.vasprocar.spin'
    destination = dir_files + '/inputs/input.vasprocar.spin'
    shutil.copyfile(source, destination)
 
-if (tipo == 3 or tipo == 5):
+if (tipo == 3 or tipo == 6):
    try: f = open(dir_files + '/inputs/input.vasprocar.orbitals'); f.close(); os.remove(dir_files + '/inputs/input.vasprocar.orbitals')
    except: 0 == 0
    #--------------------------------------------------
    source = main_dir + '/inputs/input.vasprocar.orbitals'
    destination = dir_files + '/inputs/input.vasprocar.orbitals'
    shutil.copyfile(source, destination)
 
-if (tipo == 4 or tipo == 5):
+if (tipo == 4 or tipo == 6):
+   try: f = open(dir_files + '/inputs/input.vasprocar.location'); f.close(); os.remove(dir_files + '/inputs/input.vasprocar.location')
+   except: 0 == 0
+   #--------------------------------------------------
+   source = main_dir + '/inputs/input.vasprocar.location'
+   destination = dir_files + '/inputs/input.vasprocar.location'
+   shutil.copyfile(source, destination)
+
+if (tipo == 5 or tipo == 6):
    try: f = open(dir_files + '/inputs/input.vasprocar.dos'); f.close(); os.remove(dir_files + '/inputs/input.vasprocar.dos')
    except: 0 == 0
    #--------------------------------------------------
    source = main_dir + '/inputs/input.vasprocar.dos'
    destination = dir_files + '/inputs/input.vasprocar.dos'
    shutil.copyfile(source, destination)
```

### Comparing `vasprocar-1.1.15.7/vasprocar/src/level_countour.py` & `vasprocar-1.1.15.8/vasprocar/src/level_countour.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_bandas_2D.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_bandas_2D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_chgcar.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_chgcar.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_dielectric_function.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_dielectric_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_dos_pdos_ldos.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_dos_pdos_ldos.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py` & `vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py` & `vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_parchg.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_parchg.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_potencial.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_potencial.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_projecao_localizacao.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_projecao_localizacao.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_projecao_orbitais.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_projecao_orbitais.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_projecao_psi.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_projecao_psi.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_projecao_spin.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_projecao_spin.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/Grace/plot_wave_function.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/Grace/plot_wave_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/_plot_settings.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/_plot_settings.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_bandas_2D.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_bandas_2D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_bandas_3D_matplotlib.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_bandas_3D_matplotlib.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_bandas_3D_plotly.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_bandas_3D_plotly.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_bandas_4D_plotly.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_bandas_4D_plotly.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_chgcar.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_chgcar.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_dielectric_function.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_dielectric_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_dos_pdos_ldos.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_dos_pdos_ldos.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_dos_pdos_ldos_[polarizado].py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_dos_pdos_ldos_[polarizado].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_fermi_surface.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_fermi_surface.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_level_countour.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_level_countour.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_parchg.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_parchg.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_potencial.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_potencial.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_projecao_localizacao.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_projecao_localizacao.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_projecao_orbitais.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_projecao_orbitais.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_projecao_psi.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_projecao_psi.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_projecao_spin.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_projecao_spin.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_2D.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_spin_texture_2D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_3D.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_spin_texture_3D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_4D.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_spin_texture_4D.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_4D_[iso].py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_spin_texture_4D_[iso].py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_contour.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_spin_texture_contour.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_spin_texture_contour_video.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_spin_texture_contour_video.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/plot/plot_wave_function.py` & `vasprocar-1.1.15.8/vasprocar/src/plot/plot_wave_function.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/projecao_localizacao.py` & `vasprocar-1.1.15.8/vasprocar/src/projecao_localizacao.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,157 +18,165 @@
 #======================================================================
 execute_python_file(filename = DFT + '_info.py')
 
 #----------------------------------------------------------------------
 # Initialization of Variables, Vectors and Matrices -------------------
 #----------------------------------------------------------------------
 
-ion_orb = [[[0]*(n_orb+1) for i in range(ni+1)] for j in range(6+1)]  #  ion_orb[reg][ni][n_orb]
-label_reg = ['null']*(6)
 esc_ions = 0
 
 #======================================================================
 # Get the input from user =============================================
 #======================================================================
 
 print ("##############################################################")
 print ("############ Projection of the REGIONS (Location) ############")
 print ("##############################################################") 
 print (" ")
 
-print ("##############################################################")
-print ("To define a REGION to be projected in the band structure, you ")
-print ("must inform the ions that belong to this region through       ")
-print ("ion_intervals.                                                ")
-print ("==============================================================")
-print ("For a given REGION, you can inform how many ions_intervals you")
-print ("deem necessary.                                               ")
-print ("==============================================================")
-print ("Ions can be added in any order.                               ")
-print ("==============================================================")
-print ("Examples:                                                     ")
-print ("ions_intervals  15:27 28:36 37*                               ")  
-print ("ions_intervals  35:78                                         ")
-print ("ions_intervals  9* 10:14 15*                                  ")
-print ("##############################################################")
-print(" ")
+if (len(inputs) == 0):
+   ion_orb = [[[0]*(n_orb+1) for i in range(ni+1)] for j in range(6+1)]  #  ion_orb[reg][ni][n_orb]
+   label_reg = ['null']*(6)
 
-print ("##############################################################")
-print ("How many REGIONS do you want to analyze? =====================")
-print ("============ (A maximum of 6 REGIONS are allowed) ============")
-print ("##############################################################")
-n_reg = input (" "); n_reg = int(n_reg)
-print(" ")
+if (len(inputs) == 0):
+   print ("##############################################################")
+   print ("To define a REGION to be projected in the band structure, you ")
+   print ("must inform the ions that belong to this region through       ")
+   print ("ion_intervals.                                                ")
+   print ("==============================================================")
+   print ("For a given REGION, you can inform how many ions_intervals you")
+   print ("deem necessary.                                               ")
+   print ("==============================================================")
+   print ("Ions can be added in any order.                               ")
+   print ("==============================================================")
+   print ("Examples:                                                     ")
+   print ("ions_intervals  15:27 28:36 37*                               ")  
+   print ("ions_intervals  35:78                                         ")
+   print ("ions_intervals  9* 10:14 15*                                  ")
+   print ("##############################################################")
+   print(" ")
+
+if (len(inputs) == 0):
+   print ("##############################################################")
+   print ("How many REGIONS do you want to analyze? =====================")
+   print ("============ (A maximum of 6 REGIONS are allowed) ============")
+   print ("##############################################################")
+   n_reg = input (" "); n_reg = int(n_reg)
+   print(" ")
 
 if (n_reg <= 0): n_reg = 1
 if (n_reg > 6):  n_reg = 6
 
-for i in range(1,(n_reg+1)):
+if (len(inputs) == 0):
+   for i in range(1,(n_reg+1)):
     
-    print ("==============================================================")
-    print (f'Enter the REGION_{i} label: ====================================')
-    print ("==============================================================")
-    label_reg[i-1] = input ("rotulo: "); label_reg[i-1] = str(label_reg[i-1])
-    print(" ")
-
-    print ("==============================================================")
-    print (f'Inform the ions_intervals of REGIAO_{i} ========================')
-    print (" ")
-    reg_ion = input ("ions_intervals  ").replace(':', ' ').replace('-', ' ').replace('*', ' *').split( )
-    print (" ")
-
-    loop = int(len(reg_ion)/2)
-
-    for j in range(1,(loop+1)):
-
-        #------------------------------------------
-        loop_i = int(reg_ion[(j-1)*2])
-        if (reg_ion[((j-1)*2) +1] == "*"):
-           reg_ion[((j-1)*2) +1] = reg_ion[(j-1)*2]
-        loop_f = int(reg_ion[((j-1)*2) +1])
-        #----------------------------------------------------------------------------------------
-        if ((loop_i > ni) or (loop_f > ni) or (loop_i < 0) or (loop_f < 0) or (loop_i > loop_f)):
-           print (" ")
-           print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-           print ("ERROR: The informed ion values are incorrect %%%%%%%%%%%%%")
-           print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
-           confirmation = input (" ")
-           exit()
+       print ("==============================================================")
+       print (f'Enter the REGION_{i} label: ====================================')
+       print ("==============================================================")
+       label_reg[i-1] = input ("rotulo: "); label_reg[i-1] = str(label_reg[i-1])
+       print(" ")
+
+       print ("==============================================================")
+       print (f'Inform the ions_intervals of REGIAO_{i} ========================')
+       print (" ")
+       reg_ion = input ("ions_intervals  ").replace(':', ' ').replace('-', ' ').replace('*', ' *').split( )
+       print (" ")
+
+       loop = int(len(reg_ion)/2)
+
+       for j in range(1,(loop+1)):
+
+           #------------------------------------------
+           loop_i = int(reg_ion[(j-1)*2])
+           if (reg_ion[((j-1)*2) +1] == "*"):
+              reg_ion[((j-1)*2) +1] = reg_ion[(j-1)*2]
+           loop_f = int(reg_ion[((j-1)*2) +1])
+           #----------------------------------------------------------------------------------------
+           if ((loop_i > ni) or (loop_f > ni) or (loop_i < 0) or (loop_f < 0) or (loop_i > loop_f)):
+              print (" ")
+              print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+              print ("ERROR: The informed ion values are incorrect %%%%%%%%%%%%%")
+              print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
+              confirmation = input (" ")
+              exit()
            
-        for p in range(loop_i,(loop_f+1)):
-            for m in range (1,(n_orb+1)):                   
-                ion_orb[i][p][m] = 1                    
+           for p in range(loop_i,(loop_f+1)):
+               for m in range (1,(n_orb+1)):                   
+                   ion_orb[i][p][m] = 1                    
  
 # Other input parameters =================================================
 
 if (escolha == -1):
 
-   print ("##################################################################") 
-   print ("Do you want to change the color pattern of the REGIONS projections")
-   print ("[0] NO                                                            ")
-   print ("[1] YES                                                           ")
-   print ("##################################################################") 
-   esc_color = input (" "); esc_color = int(esc_color)
-   print (" ")  
-
-   if (esc_color == 1):
-      print ("##############################################################")
-      print ("Color code:                                                   ")
-      print ("0  White   | 1  Black | 2  Red    | 3  Green  | 4  Blue       ")
-      print ("5  Yellow  | 6  Borwn | 7  Grey   | 8  Violet | 9  Cyan       ")
-      print ("10 Magenta |11 Orange | 12 Indigo | 13 Maroon | 14 Turquesa   ")
-      print ("15 Dark_Green                                                 ")
-      print ("##############################################################")       
-      print ("VASProcar color pattern:                                      ")
-      print ("                                                              ")
-      print ("Color_of_REGIONS 1|2|3|4|5|6:  4 2 3 10 9 5                   ")
-      print ("(Blue, Red, Green, Magenta, Cyan, Yellow)                     ")
-      print ("##############################################################") 
-      print (" ")
-
-      print ("==============================================================") 
-      print ("Type in sequence the colors of the REGIONS that you defined:  ")
-      cor_reg = input ("Color_of_REGIONS: ")
-      #---------------------
-      tcor = cor_reg.split()
-      #-------------------------
-      for i in range(len(tcor)):         
-          if (i == 0): c_Reg1 = int(tcor[0])
-          if (i == 1): c_Reg2 = int(tcor[1])
-          if (i == 2): c_Reg3 = int(tcor[2])
-          if (i == 3): c_Reg4 = int(tcor[3])
-          if (i == 4): c_Reg5 = int(tcor[4])
-          if (i == 5): c_Reg6 = int(tcor[5])
-      #-------------------------------------
-      print (" ") 
+   if (len(inputs) == 0):
+      print ("##################################################################") 
+      print ("Do you want to change the color pattern of the REGIONS projections")
+      print ("[0] NO                                                            ")
+      print ("[1] YES                                                           ")
+      print ("##################################################################") 
+      esc_color = input (" "); esc_color = int(esc_color)
+      print (" ")  
+
+      if (esc_color == 1):
+         print ("##############################################################")
+         print ("Color code:                                                   ")
+         print ("0  White   | 1  Black | 2  Red    | 3  Green  | 4  Blue       ")
+         print ("5  Yellow  | 6  Borwn | 7  Grey   | 8  Violet | 9  Cyan       ")
+         print ("10 Magenta |11 Orange | 12 Indigo | 13 Maroon | 14 Turquesa   ")
+         print ("15 Dark_Green                                                 ")
+         print ("##############################################################")       
+         print ("VASProcar color pattern:                                      ")
+         print ("                                                              ")
+         print ("Color_of_REGIONS 1|2|3|4|5|6:  4 2 3 10 9 5                   ")
+         print ("(Blue, Red, Green, Magenta, Cyan, Yellow)                     ")
+         print ("##############################################################") 
+         print (" ")
+
+         print ("==============================================================") 
+         print ("Type in sequence the colors of the REGIONS that you defined:  ")
+         cor_reg = input ("Color_of_REGIONS: ")
+         #---------------------
+         tcor = cor_reg.split()
+         #-------------------------
+         for i in range(len(tcor)):         
+             if (i == 0): c_Reg1 = int(tcor[0])
+             if (i == 1): c_Reg2 = int(tcor[1])
+             if (i == 2): c_Reg3 = int(tcor[2])
+             if (i == 3): c_Reg4 = int(tcor[3])
+             if (i == 4): c_Reg5 = int(tcor[4])
+             if (i == 5): c_Reg6 = int(tcor[5])
+         #-------------------------------------
+         print (" ") 
 
-   print ("##############################################################")
-   print ("Regarding the Plot of Bands, choose ==========================")
-   print ("[0] Plot/Analyze all bands ===================================")
-   print ("[1] Plot/Analyze selected bands ==============================")
-   print ("##############################################################")
-   esc_bands = input (" "); esc_bands = int(esc_bands)
-   print(" ")
+   if (len(inputs) == 0):
+      print ("##############################################################")
+      print ("Regarding the Plot of Bands, choose ==========================")
+      print ("[0] Plot/Analyze all bands ===================================")
+      print ("[1] Plot/Analyze selected bands ==============================")
+      print ("##############################################################")
+      esc_bands = input (" "); esc_bands = int(esc_bands)
+      print(" ")
 
    if (esc_bands == 0):
       bands_range = '1:' + str(nb)
 
-   if (esc_bands == 1):     
-      print ("##############################################################")
-      print ("Select the bands to be analyzed using intervals:              ")
-      print ("Type as in the examples below =============================== ")
-      print ("------------------------------------------------------------- ")
-      print ("Bands can be added in any order ----------------------------- ")
-      print ("------------------------------------------------------------- ")
-      print ("bands_intervals  35:42                                        ")          
-      print ("bands_intervals  1:15 27:69 18:19 76*                         ")
-      print ("bands_intervals  7* 9* 11* 13* 16:21                          ")
-      print ("##############################################################")
-      bands_range = input ("bands_intervals  ")
-      print (" ")
+   if (esc_bands == 1):  
+      if (len(inputs) == 0):   
+         print ("##############################################################")
+         print ("Select the bands to be analyzed using intervals:              ")
+         print ("Type as in the examples below =============================== ")
+         print ("------------------------------------------------------------- ")
+         print ("Bands can be added in any order ----------------------------- ")
+         print ("------------------------------------------------------------- ")
+         print ("bands_intervals  35:42                                        ")          
+         print ("bands_intervals  1:15 27:69 18:19 76*                         ")
+         print ("bands_intervals  7* 9* 11* 13* 16:21                          ")
+         print ("##############################################################")
+         bands_range = input ("bands_intervals  ")
+         print (" ")
       #------------------------------------------------------------------------------------------
       selected_bands = bands_range.replace(':', ' ').replace('-', ' ').replace('*', ' *').split()
       loop = int(len(selected_bands)/2)
       #------------------------------------------------------------------------------------------
       
       for i in range (1,(loop+1)):
           #--------------------------------------------------------
@@ -181,75 +189,81 @@
              print (" ")
              print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
              print ("ERROR: The values of the informed bands are incorrect %%%%")
              print ("%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%")
              confirmacao = input (" ")
              exit()
 
-   print ("##############################################################") 
-   print ("with respect to energy, would you like? ======================")
-   print ("[0] Use the default energy value from DFT output =============")
-   print ("[1] Shift the Fermi level to 0.0 eV  =========================")
-   print ("##############################################################")
-   esc_fermi = input (" "); esc_fermi = int(esc_fermi)
-   print (" ")   
-
-   print ("##############################################################") 
-   print ("Do you want to modify the energy range to be plotted? ========")
-   print ("[0] NOT                                                       ")
-   print ("[1] YES                                                       ")
-   print ("##############################################################")
-   esc_range_E = input (" "); esc_range_E = int(esc_range_E)
-   print (" ")
+   if (len(inputs) == 0):
+      print ("##############################################################") 
+      print ("with respect to energy, would you like? ======================")
+      print ("[0] Use the default energy value from DFT output =============")
+      print ("[1] Shift the Fermi level to 0.0 eV  =========================")
+      print ("##############################################################")
+      esc_fermi = input (" "); esc_fermi = int(esc_fermi)
+      print (" ")   
 
-   if (esc_range_E == 1):
+   if (len(inputs) == 0):
       print ("##############################################################") 
-      print ("Enter the energy range to be plotted: ========================")
-      print ("Note: Enter the lowest and highest energy value to be plotted ")
-      print ("            in relation to the Fermi Level                    ")
-      print ("Examples:                                                     ")
-      print ("--------------------------------------------------------------")
-      print ("E_min E_max: -3.0 15.0                                        ")
-      print ("E_min E_max: -5.1 5.0                                         ")
-      print ("##############################################################")      
-      range_E = input ("E_min E_max:  ")
+      print ("Do you want to modify the energy range to be plotted? ========")
+      print ("[0] NOT                                                       ")
+      print ("[1] YES                                                       ")
+      print ("##############################################################")
+      esc_range_E = input (" "); esc_range_E = int(esc_range_E)
       print (" ")
+
+   if (esc_range_E == 1):
+      if (len(inputs) == 0):
+         print ("##############################################################") 
+         print ("Enter the energy range to be plotted: ========================")
+         print ("Note: Enter the lowest and highest energy value to be plotted ")
+         print ("            in relation to the Fermi Level                    ")
+         print ("Examples:                                                     ")
+         print ("--------------------------------------------------------------")
+         print ("E_min E_max: -3.0 15.0                                        ")
+         print ("E_min E_max: -5.1 5.0                                         ")
+         print ("##############################################################")      
+         range_E = input ("E_min E_max:  ")
+         print (" ")
       #--------------------------------------------------
       selected_energ = range_E.replace('-', ' -').replace('+', ' +').replace(':', ' ').split()
       E_min = float(selected_energ[0])
       E_max = float(selected_energ[1])
 
-   print ("##############################################################") 
-   print ("Do you want to ignore contributions below a certain amount?   ")
-   print ("[0] NOT                                                       ")
-   print ("[1] YES                                                       ")
-   print ("##############################################################")
-   esc_ignorar = input (" "); esc_ignorar = int(esc_ignorar)
-   print (" ")
+   if (len(inputs) == 0):
+      print ("##############################################################") 
+      print ("Do you want to ignore contributions below a certain amount?   ")
+      print ("[0] NOT                                                       ")
+      print ("[1] YES                                                       ")  
+      print ("##############################################################")
+      esc_ignorar = input (" "); esc_ignorar = int(esc_ignorar)
+      print (" ")
    
    if (esc_ignorar == 0 or esc_ignorar != 1):
       contrib_min = 0.0 
-   if (esc_ignorar == 1):
+   
+   if (esc_ignorar == 1 and len(inputs) == 0):
       print ("##############################################################") 
       print ("Enter the minimum contribution amount to be plotted ==========")
       print ("Note: Enter a value between 0.0 and 1.0 ======================")
       print ("##############################################################")
       contrib_min = input (" "); contrib_min = float(contrib_min)
       print (" ")
 
-   print ("##############################################################")
-   print ("Would you like to label the k-points?                         ")
-   print ("[0] DO NOT label the k-points  ===============================")
-   print ("[1] highlight k-points present in KPOINTS file ===============")
-   print ("[2] Customize: highlight and Label k-points   ================")
-   print ("##############################################################") 
-   dest_k = input (" "); dest_k = int(dest_k)
-   print (" ")
+   if (len(inputs) == 0):
+      print ("##############################################################")
+      print ("Would you like to label the k-points?                         ")
+      print ("[0] DO NOT label the k-points  ===============================")
+      print ("[1] highlight k-points present in KPOINTS file ===============")
+      print ("[2] Customize: highlight and Label k-points   ================")
+      print ("##############################################################") 
+      dest_k = input (" "); dest_k = int(dest_k)
+      print (" ")
 
-   if (DFT == '_QE/' and dest_k == 2):
+   if (DFT == '_QE/' and dest_k == 2 and len(inputs) == 0):
       print ("##############################################################")
       print ("Do you want to insert symmetries as k-point label?            ")
       print ("[0] NOT                                                       ")
       print ("[1] YES                                                       ")
       print ("##############################################################") 
       l_symmetry = input (" "); l_symmetry = int(l_symmetry)
       print (" ") 
@@ -259,41 +273,43 @@
       print ("label.TXT file should be found inside the 'output' folder ====")
       print ("after reading the PROCAR file ================================")
       print ("##############################################################") 
       print (" ")
 
       Dimensao = 1
 
-   if (dest_k != 2):   
+   if (dest_k != 2 and len(inputs) == 0):   
       print ("##############################################################")
       print ("Would you like to choose k-axis units?                        ")
       print ("[1] 2pi/Param. (Param. in Angs.) =============================")
       print ("[2] 1/Angs. ==================================================")
       print ("[3] 1/nm.   ==================================================")
       print ("##############################################################")
       Dimensao = input (" "); Dimensao = int(Dimensao)
       print(" ")
 
-   print ("##############################################################")
-   print ("Enter the weight/size of the spheres in the projection: ======")
-   print ("Enter a value between 0.0 and 1.0 ============================")
-   print ("##############################################################")
-   peso_total = input (" "); peso_total = float(peso_total)
-   print(" ")
+   if (len(inputs) == 0):
+      print ("##############################################################")
+      print ("Enter the weight/size of the spheres in the projection: ======")
+      print ("Enter a value between 0.0 and 1.0 ============================")
+      print ("##############################################################")
+      peso_total = input (" "); peso_total = float(peso_total)
+      print(" ")
 
-   print ("##############################################################")
-   print ("Enter the transparency value to apply to the projections:     ")
-   print ("This option is useful for checking the overlap of orbitals.   ")   
-   print ("Enter a value between 0.0 and 1.0 ============================")
-   print ("==============================================================")
-   print ("Hint: The higher the k-point density, the lower the ==========")
-   print ("      transparency value used, start with 0.5 ================")
-   print ("##############################################################")
-   transp = input (" "); transp = float(transp)
-   print(" ")   
+   if (len(inputs) == 0):
+      print ("##############################################################")
+      print ("Enter the transparency value to apply to the projections:     ")
+      print ("This option is useful for checking the overlap of orbitals.   ")   
+      print ("Enter a value between 0.0 and 1.0 ============================")
+      print ("==============================================================")
+      print ("Hint: The higher the k-point density, the lower the ==========")
+      print ("      transparency value used, start with 0.5 ================")
+      print ("##############################################################")
+      transp = input (" "); transp = float(transp)
+      print(" ")   
 
 if (escolha == 1):
    bands_range = '1:' + str(nb)
    esc_fermi = 1
    esc_range_E = 0
    dest_k = 1
    Dimensao = 1
@@ -474,13 +490,15 @@
 print("= Localizacao.py or .agr files generated in the =============") 
 print("= output/Localizacao folder =================================")
 print("=============================================================")
 
 #-----------------------------------------------------------------
 print(" ")
 print("======================= Completed =======================")
+print(" ")
 #-----------------------------------------------------------------
 
 #=======================================================================
 # User option to perform another calculation or finished the code ======
 #=======================================================================
-execute_python_file(filename = '_loop.py')
+if (len(inputs) == 0):
+   execute_python_file(filename = '_loop.py')
```

### Comparing `vasprocar-1.1.15.7/vasprocar/src/projecao_orbitais.py` & `vasprocar-1.1.15.8/vasprocar/src/projecao_orbitais.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/projecao_psi.py` & `vasprocar-1.1.15.8/vasprocar/src/projecao_psi.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/projecao_spin.py` & `vasprocar-1.1.15.8/vasprocar/src/projecao_spin.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/spin_texture.py` & `vasprocar-1.1.15.8/vasprocar/src/spin_texture.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/spin_texture_contour.py` & `vasprocar-1.1.15.8/vasprocar/src/spin_texture_contour.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar/src/spin_texture_contour_video.py` & `vasprocar-1.1.15.8/vasprocar/src/spin_texture_contour_video.py`

 * *Files identical despite different names*

### Comparing `vasprocar-1.1.15.7/vasprocar.egg-info/PKG-INFO` & `vasprocar-1.1.15.8/vasprocar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vasprocar
-Version: 1.1.15.7
+Version: 1.1.15.8
 Summary: VASProcar is an open-source package written in the Python 3 programming language, which aims to provide an intuitive tool for the post-processing of the output files produced by the DFT VASP code, through an interactive user interface.
 Home-page: https://doi.org/10.5281/zenodo.6343960
 Download-URL: https://doi.org/10.5281/zenodo.6343960
 Author: Augusto de Lelis Araujo and Renan da Paixao Maciel
 Author-email: augusto-lelis@outlook.com, renan.maciel@physics.uu.se
 License: GNU GPLv3
 Description-Content-Type: text/markdown
```

### Comparing `vasprocar-1.1.15.7/vasprocar.egg-info/SOURCES.txt` & `vasprocar-1.1.15.8/vasprocar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

