# Comparing `tmp/scipion-em-xmipp-23.3.0.3.tar.gz` & `tmp/scipion-em-xmipp-23.7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-xmipp-23.3.0.3.tar", last modified: Tue May  9 10:26:58 2023, max compression
+gzip compressed data, was "scipion-em-xmipp-23.7.0.0.tar", last modified: Fri Jul 14 07:58:46 2023, max compression
```

## Comparing `scipion-em-xmipp-23.3.0.3.tar` & `scipion-em-xmipp-23.7.0.0.tar`

### file list

```diff
@@ -1,237 +1,243 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:26:58.235284 scipion-em-xmipp-23.3.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-09 10:26:58.231284 scipion-em-xmipp-23.3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:26:58.211284 scipion-em-xmipp-23.3.0.3/scipion_em_xmipp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-09 10:26:58.000000 scipion-em-xmipp-23.3.0.3/scipion_em_xmipp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-05-09 10:26:58.000000 scipion-em-xmipp-23.3.0.3/scipion_em_xmipp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:26:58.000000 scipion-em-xmipp-23.3.0.3/scipion_em_xmipp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-09 10:26:58.000000 scipion-em-xmipp-23.3.0.3/scipion_em_xmipp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-09 10:26:58.000000 scipion-em-xmipp-23.3.0.3/scipion_em_xmipp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 10:26:58.000000 scipion-em-xmipp-23.3.0.3/scipion_em_xmipp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 10:26:58.235284 scipion-em-xmipp-23.3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:26:58.211284 scipion-em-xmipp-23.3.0.3/xmipp3/
--rw-r--r--   0 runner    (1001) docker     (123)    13057 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21220 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    26010 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:26:58.211284 scipion-em-xmipp-23.3.0.3/xmipp3/convert/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62027 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/convert/dataimport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/convert/io_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/programs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:26:58.223284 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18950 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_align_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_align_volume_and_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_analyze_local_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)    30302 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_angular_graph_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_apply_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_apply_deformation_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_apply_transformation_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_apply_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_assignment_tilt_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_break_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_center_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)    27226 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_cl2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_cl2d_align.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_classes_2d_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    37013 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_classification_gpuCorr.py
--rw-r--r--   0 runner    (1001) docker     (123)    40366 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_classification_gpuCorr_full.py
--rw-r--r--   0 runner    (1001) docker     (123)    18244 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_classification_gpuCorr_semi.py
--rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_classify_kmeans2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_compare_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_compare_reprojections.py
--rw-r--r--   0 runner    (1001) docker     (123)    31955 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_consensus_classes3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_consensus_local_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_convert_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_core_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_create_gallery.py
--rw-r--r--   0 runner    (1001) docker     (123)    42641 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_ctf_consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_ctf_correct_wiener2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_ctf_defocus_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    28698 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_ctf_micrographs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21324 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_deep_denoising.py
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_deep_hand.py
--rw-r--r--   0 runner    (1001) docker     (123)    21735 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_deep_micrograph_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_denoise_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)    22399 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_eliminate_empty_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    25080 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_enrich.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_extract_asymmetric_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    23503 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_extract_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)    23258 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_extract_particles_movies.py
--rw-r--r--   0 runner    (1001) docker     (123)    29349 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_extract_particles_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18475 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_flexalign.py
--rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_generate_reprojections.py
--rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_helical_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_kerdensom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_kmeans_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_local_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_metaprotocol_create_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32782 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_metaprotocol_golden_highres.py
--rw-r--r--   0 runner    (1001) docker     (123)    17214 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_ml2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    26961 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_movie_gain.py
--rw-r--r--   0 runner    (1001) docker     (123)    17726 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_movie_max_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)    18030 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_movie_opticalflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_movie_split_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_multiple_fscs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27778 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_multireference_alignability.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_normalize_strain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_particle_boxsize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_particle_pick.py
--rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_particle_pick_automatic.py
--rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_particle_pick_consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_particle_pick_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_particle_pick_remove_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_phantom_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_pick_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    15158 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_postProcessing_deepPostProcessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:26:58.223284 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/geometrical_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_add_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_create_mask2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_create_mask3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    23009 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_crop_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)    22928 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_image_operate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_movie_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)    39852 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    24220 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess_micrographs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:26:58.223284 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_projmatch/
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_projmatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_projmatch/projmatch_form.py
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_projmatch/projmatch_initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    34600 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_projmatch/projmatch_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    18096 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_projmatch/protocol_projmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    17030 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_random_conical_tilt.py
--rw-r--r--   0 runner    (1001) docker     (123)    28957 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_ransac.py
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_reconstruct_fourier.py
--rw-r--r--   0 runner    (1001) docker     (123)   107816 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_reconstruct_highres.py
--rw-r--r--   0 runner    (1001) docker     (123)    26462 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_reconstruct_significant.py
--rw-r--r--   0 runner    (1001) docker     (123)    30163 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_reconstruct_swarm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_resolution3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_resolution_bfactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16477 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_resolution_deepres.py
--rw-r--r--   0 runner    (1001) docker     (123)    12893 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_resolution_directional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_resolution_fso.py
--rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_resolution_monogenic_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_rotate_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_rotational_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_rotational_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    88133 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_screen_deepConsensus.py
--rw-r--r--   0 runner    (1001) docker     (123)    17530 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_screen_deeplearning.py
--rw-r--r--   0 runner    (1001) docker     (123)    21002 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_screen_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_shift_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_shift_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_simulate_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)    29287 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_solid_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_split_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    40429 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_split_volume_hierarchical_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_structure_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    22110 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_structure_map_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_subtract_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)    28360 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_tilt_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    16359 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_trigger_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23655 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_validate_fscq.py
--rw-r--r--   0 runner    (1001) docker     (123)    16415 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_validate_nontilt.py
--rw-r--r--   0 runner    (1001) docker     (123)    25116 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_validate_overfitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    17626 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_volume_adjust_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_volume_consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_volume_deform_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_volume_local_sharpening.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_volume_strain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_write_testC.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_write_testP.py
--rw-r--r--   0 runner    (1001) docker     (123)    12552 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:26:58.227284 scipion-em-xmipp-23.3.0.3/xmipp3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44475 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_convert_xmipp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_angular_graph_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_apply_transformation_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_compare_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_consensus_classes3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_ctf_consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_deep_denoising.py
--rw-r--r--   0 runner    (1001) docker     (123)    23298 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_extract_asymmetric_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_monodir.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_multiple_fsc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_multireference_alignability.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_reconstruct_fourier.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_screen_deepConsensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_simulate_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_validate_fscq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_validate_overfitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_add_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_continuousflex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_deepVolPostprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_deepres.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_fso.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_gpuCorr_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_gpuCorr_fullStreaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_gpuCorr_semiStreaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_highres.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_local_defocus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_localdeblur.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_metaprotocol_golden_highres.py
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_mixed_movies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_monores.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_realignment_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_solid_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)    76668 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_xmipp_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)   161922 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_xmipp_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    61131 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_xmipp_mics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_xmipp_movie_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)    35140 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_xmipp_movies.py
--rw-r--r--   0 runner    (1001) docker     (123)    18132 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:26:58.231284 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21483 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_analyze_local_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_cl2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_classes3D.py
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_consensus_classes3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_ctf_consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_deepEMHancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_deep_consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_deep_micrograph_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_eliminate_empty_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_extract_asymmetric_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_local_sharpening.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_metaprotocol_golden_highres.py
--rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_ml2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_movie_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_normalize_strain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_pdb_deform_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    37770 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_projmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_ransac.py
--rw-r--r--   0 runner    (1001) docker     (123)    13184 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_reconstruct_highres.py
--rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_resolution3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_resolution_bfactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_resolution_deepres.py
--rw-r--r--   0 runner    (1001) docker     (123)    20319 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_resolution_directional.py
--rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_resolution_fso.py
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_resolution_monogenic_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_solid_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_split_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    14398 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_structure_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_subtract_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_swarm.py
--rw-r--r--   0 runner    (1001) docker     (123)    18651 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_validate_fscq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_validate_nontilt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_validate_overfitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_volume_consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_volume_deform_zernike3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_volume_strain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_volume_subtraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20151 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)    84496 2023-05-09 10:25:11.000000 scipion-em-xmipp-23.3.0.3/xmipp3/xmipp_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:58:46.235337 scipion-em-xmipp-23.7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-14 07:58:46.235337 scipion-em-xmipp-23.7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:58:46.207335 scipion-em-xmipp-23.7.0.0/scipion_em_xmipp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-14 07:58:46.000000 scipion-em-xmipp-23.7.0.0/scipion_em_xmipp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-07-14 07:58:46.000000 scipion-em-xmipp-23.7.0.0/scipion_em_xmipp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 07:58:46.000000 scipion-em-xmipp-23.7.0.0/scipion_em_xmipp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-14 07:58:46.000000 scipion-em-xmipp-23.7.0.0/scipion_em_xmipp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-14 07:58:46.000000 scipion-em-xmipp-23.7.0.0/scipion_em_xmipp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 07:58:46.000000 scipion-em-xmipp-23.7.0.0/scipion_em_xmipp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 07:58:46.235337 scipion-em-xmipp-23.7.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:58:46.207335 scipion-em-xmipp-23.7.0.0/xmipp3/
+-rw-r--r--   0 runner    (1001) docker     (123)    13059 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21220 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:58:46.211336 scipion-em-xmipp-23.7.0.0/xmipp3/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62027 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/convert/dataimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/convert/io_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/programs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:58:46.223336 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19073 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_align_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_align_volume_and_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_analyze_local_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30302 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_angular_graph_consistency.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8521 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_angular_resolution_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_apply_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_apply_transformation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_apply_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_assignment_tilt_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_break_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_center_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27226 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_cl2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_cl2d_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_classes_2d_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37013 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_classification_gpuCorr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40366 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_classification_gpuCorr_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18244 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_classification_gpuCorr_semi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_compare_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15333 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_compare_reprojections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25092 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_consensus_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_consensus_local_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14775 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_convert_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_core_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_create_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42614 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_ctf_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_ctf_correct_wiener2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_ctf_defocus_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28698 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_ctf_micrographs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_deep_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_deep_center_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21324 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_deep_denoising.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_deep_global_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_deep_global_assignment_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_deep_hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22168 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_deep_micrograph_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_denoise_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22399 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_eliminate_empty_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25080 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_enrich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_extract_asymmetric_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23503 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_extract_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23258 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_extract_particles_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29349 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_extract_particles_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18472 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_flexalign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_generate_reprojections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_helical_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_kerdensom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_local_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_metaprotocol_create_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32782 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_metaprotocol_golden_highres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17214 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_ml2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17826 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_movie_dose_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25732 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_movie_gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17726 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_movie_max_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18030 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_movie_opticalflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_movie_split_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_multiple_fscs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27778 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_multireference_alignability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_normalize_strain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_particle_pick.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_particle_pick_automatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16901 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_particle_pick_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_particle_pick_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_particle_pick_remove_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_phantom_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_pick_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15158 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_postProcessing_deepPostProcessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:58:46.223336 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/geometrical_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_add_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_create_mask2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_create_mask3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25599 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_crop_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22928 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_image_operate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_movie_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39852 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24220 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess_micrographs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:58:46.227337 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_projmatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_projmatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_projmatch/projmatch_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_projmatch/projmatch_initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34600 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_projmatch/projmatch_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18096 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_projmatch/protocol_projmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17030 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_random_conical_tilt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28957 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_ransac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_reconstruct_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107816 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_reconstruct_highres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26462 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_reconstruct_significant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30163 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_reconstruct_swarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_resolution3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_resolution_bfactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16477 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_resolution_deepres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12893 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_resolution_directional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_resolution_fso.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_resolution_monogenic_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_rotate_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_rotational_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88133 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_screen_deepConsensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17530 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_screen_deeplearning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21002 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_screen_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_shift_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_shift_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_simulate_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29287 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_solid_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_split_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_structure_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22110 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_structure_map_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_subtract_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27993 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_tilt_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16359 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_trigger_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23655 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_validate_fscq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16415 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_validate_nontilt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25116 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_validate_overfitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17626 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_volume_adjust_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_volume_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_volume_deform_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_volume_local_sharpening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_volume_strain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_write_testC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_write_testP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:58:46.231337 scipion-em-xmipp-23.7.0.0/xmipp3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44475 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_convert_xmipp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_angular_graph_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_apply_transformation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_compare_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_consensus_classes3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_ctf_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_deep_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_deep_center_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_deep_denoising.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_deep_global_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_deep_global_assignment_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23298 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_extract_asymmetric_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_monodir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_multiple_fsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_multireference_alignability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_reconstruct_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_screen_deepConsensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_simulate_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_validate_fscq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_validate_overfitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_add_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_angular_resolution_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_continuousflex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_deepVolPostprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_deepres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_fso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_gpuCorr_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_gpuCorr_fullStreaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_gpuCorr_semiStreaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_highres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_local_defocus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_localdeblur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_metaprotocol_golden_highres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_mixed_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_monores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_realignment_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_solid_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75260 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_xmipp_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   166280 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_xmipp_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59829 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_xmipp_mics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_xmipp_movie_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38274 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_xmipp_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18132 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:58:46.235337 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19690 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_analyze_local_ctf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5155 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_angular_resolution_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_cl2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_consensus_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_ctf_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_deepEMHancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_deep_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_deep_micrograph_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_dose_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_eliminate_empty_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_extract_asymmetric_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_local_sharpening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_metaprotocol_golden_highres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_ml2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_movie_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_normalize_strain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_pdb_deform_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37634 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_projmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_ransac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13184 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_reconstruct_highres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_resolution3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_resolution_bfactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_resolution_deepres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20319 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_resolution_directional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_resolution_fso.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_resolution_monogenic_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_solid_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_split_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_structure_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_subtract_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_swarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18651 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_validate_fscq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_validate_nontilt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_validate_overfitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_volume_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_volume_deform_zernike3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_volume_strain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_volume_subtraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20343 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84496 2023-07-14 07:56:07.000000 scipion-em-xmipp-23.7.0.0/xmipp3/xmipp_logo.png
```

### Comparing `scipion-em-xmipp-23.3.0.3/LICENSE` & `scipion-em-xmipp-23.7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/PKG-INFO` & `scipion-em-xmipp-23.7.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-xmipp
-Version: 23.3.0.3
+Version: 23.7.0.0
 Summary: Plugin to use Xmipp programs within the Scipion framework (see https://scipion-em.github.io/docs/).
 Home-page: https://github.com/i2pc/scipion-em-xmipp
 Author: I2PC
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: [![Build](https://github.com/I2PC/scipion-em-xmipp/actions/workflows/build.yml/badge.svg)](https://github.com/I2PC/scipion-em-xmipp/actions/workflows/build.yml)
```

### Comparing `scipion-em-xmipp-23.3.0.3/README.md` & `scipion-em-xmipp-23.7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/scipion_em_xmipp.egg-info/PKG-INFO` & `scipion-em-xmipp-23.7.0.0/scipion_em_xmipp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: scipion-em-xmipp
-Version: 23.3.0.3
+Version: 23.7.0.0
 Summary: Plugin to use Xmipp programs within the Scipion framework (see https://scipion-em.github.io/docs/).
 Home-page: https://github.com/i2pc/scipion-em-xmipp
 Author: I2PC
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: [![Build](https://github.com/I2PC/scipion-em-xmipp/actions/workflows/build.yml/badge.svg)](https://github.com/I2PC/scipion-em-xmipp/actions/workflows/build.yml)
```

### Comparing `scipion-em-xmipp-23.3.0.3/scipion_em_xmipp.egg-info/SOURCES.txt` & `scipion-em-xmipp-23.7.0.0/scipion_em_xmipp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-CHANGES.txt
+CHANGES.md
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 scipion_em_xmipp.egg-info/PKG-INFO
 scipion_em_xmipp.egg-info/SOURCES.txt
@@ -24,66 +24,68 @@
 xmipp3/convert/dataimport.py
 xmipp3/convert/io_coordinates.py
 xmipp3/protocols/__init__.py
 xmipp3/protocols/protocol_align_volume.py
 xmipp3/protocols/protocol_align_volume_and_particles.py
 xmipp3/protocols/protocol_analyze_local_ctf.py
 xmipp3/protocols/protocol_angular_graph_consistency.py
+xmipp3/protocols/protocol_angular_resolution_alignment.py
 xmipp3/protocols/protocol_apply_alignment.py
-xmipp3/protocols/protocol_apply_deformation_zernike3d.py
 xmipp3/protocols/protocol_apply_transformation_matrix.py
 xmipp3/protocols/protocol_apply_zernike3d.py
 xmipp3/protocols/protocol_assignment_tilt_pair.py
 xmipp3/protocols/protocol_break_symmetry.py
 xmipp3/protocols/protocol_center_particles.py
 xmipp3/protocols/protocol_cl2d.py
 xmipp3/protocols/protocol_cl2d_align.py
 xmipp3/protocols/protocol_classes_2d_mapping.py
 xmipp3/protocols/protocol_classification_gpuCorr.py
 xmipp3/protocols/protocol_classification_gpuCorr_full.py
 xmipp3/protocols/protocol_classification_gpuCorr_semi.py
-xmipp3/protocols/protocol_classify_kmeans2d.py
 xmipp3/protocols/protocol_compare_angles.py
 xmipp3/protocols/protocol_compare_reprojections.py
-xmipp3/protocols/protocol_consensus_classes3D.py
+xmipp3/protocols/protocol_consensus_classes.py
 xmipp3/protocols/protocol_consensus_local_ctf.py
 xmipp3/protocols/protocol_convert_pdb.py
 xmipp3/protocols/protocol_core_analysis.py
 xmipp3/protocols/protocol_create_gallery.py
 xmipp3/protocols/protocol_ctf_consensus.py
 xmipp3/protocols/protocol_ctf_correct_wiener2d.py
 xmipp3/protocols/protocol_ctf_defocus_group.py
 xmipp3/protocols/protocol_ctf_micrographs.py
+xmipp3/protocols/protocol_deep_center.py
+xmipp3/protocols/protocol_deep_center_predict.py
 xmipp3/protocols/protocol_deep_denoising.py
+xmipp3/protocols/protocol_deep_global_assignment.py
+xmipp3/protocols/protocol_deep_global_assignment_predict.py
 xmipp3/protocols/protocol_deep_hand.py
 xmipp3/protocols/protocol_deep_micrograph_screen.py
 xmipp3/protocols/protocol_denoise_particles.py
 xmipp3/protocols/protocol_eliminate_empty_images.py
 xmipp3/protocols/protocol_enrich.py
 xmipp3/protocols/protocol_extract_asymmetric_unit.py
 xmipp3/protocols/protocol_extract_particles.py
 xmipp3/protocols/protocol_extract_particles_movies.py
 xmipp3/protocols/protocol_extract_particles_pairs.py
 xmipp3/protocols/protocol_flexalign.py
 xmipp3/protocols/protocol_generate_reprojections.py
 xmipp3/protocols/protocol_helical_parameters.py
 xmipp3/protocols/protocol_kerdensom.py
-xmipp3/protocols/protocol_kmeans_clustering.py
 xmipp3/protocols/protocol_local_ctf.py
 xmipp3/protocols/protocol_metaprotocol_create_subset.py
 xmipp3/protocols/protocol_metaprotocol_golden_highres.py
 xmipp3/protocols/protocol_ml2d.py
+xmipp3/protocols/protocol_movie_dose_analysis.py
 xmipp3/protocols/protocol_movie_gain.py
 xmipp3/protocols/protocol_movie_max_shift.py
 xmipp3/protocols/protocol_movie_opticalflow.py
 xmipp3/protocols/protocol_movie_split_frames.py
 xmipp3/protocols/protocol_multiple_fscs.py
 xmipp3/protocols/protocol_multireference_alignability.py
 xmipp3/protocols/protocol_normalize_strain.py
-xmipp3/protocols/protocol_particle_boxsize.py
 xmipp3/protocols/protocol_particle_pick.py
 xmipp3/protocols/protocol_particle_pick_automatic.py
 xmipp3/protocols/protocol_particle_pick_consensus.py
 xmipp3/protocols/protocol_particle_pick_pairs.py
 xmipp3/protocols/protocol_particle_pick_remove_duplicates.py
 xmipp3/protocols/protocol_phantom_create.py
 xmipp3/protocols/protocol_pick_noise.py
@@ -98,25 +100,23 @@
 xmipp3/protocols/protocol_resolution3d.py
 xmipp3/protocols/protocol_resolution_bfactor.py
 xmipp3/protocols/protocol_resolution_deepres.py
 xmipp3/protocols/protocol_resolution_directional.py
 xmipp3/protocols/protocol_resolution_fso.py
 xmipp3/protocols/protocol_resolution_monogenic_signal.py
 xmipp3/protocols/protocol_rotate_volume.py
-xmipp3/protocols/protocol_rotational_spectra.py
 xmipp3/protocols/protocol_rotational_symmetry.py
 xmipp3/protocols/protocol_screen_deepConsensus.py
 xmipp3/protocols/protocol_screen_deeplearning.py
 xmipp3/protocols/protocol_screen_particles.py
 xmipp3/protocols/protocol_shift_particles.py
 xmipp3/protocols/protocol_shift_volume.py
 xmipp3/protocols/protocol_simulate_ctf.py
 xmipp3/protocols/protocol_solid_angles.py
 xmipp3/protocols/protocol_split_volume.py
-xmipp3/protocols/protocol_split_volume_hierarchical_cluster.py
 xmipp3/protocols/protocol_structure_map.py
 xmipp3/protocols/protocol_structure_map_zernike3d.py
 xmipp3/protocols/protocol_subtract_projection.py
 xmipp3/protocols/protocol_tilt_analysis.py
 xmipp3/protocols/protocol_trigger_data.py
 xmipp3/protocols/protocol_validate_fscq.py
 xmipp3/protocols/protocol_validate_nontilt.py
@@ -148,25 +148,30 @@
 xmipp3/tests/__init__.py
 xmipp3/tests/test_convert_xmipp.py
 xmipp3/tests/test_protocol_angular_graph_consistency.py
 xmipp3/tests/test_protocol_apply_transformation_matrix.py
 xmipp3/tests/test_protocol_compare_angles.py
 xmipp3/tests/test_protocol_consensus_classes3D.py
 xmipp3/tests/test_protocol_ctf_consensus.py
+xmipp3/tests/test_protocol_deep_center.py
+xmipp3/tests/test_protocol_deep_center_predict.py
 xmipp3/tests/test_protocol_deep_denoising.py
+xmipp3/tests/test_protocol_deep_global_assignment.py
+xmipp3/tests/test_protocol_deep_global_assignment_predict.py
 xmipp3/tests/test_protocol_extract_asymmetric_unit.py
 xmipp3/tests/test_protocol_monodir.py
 xmipp3/tests/test_protocol_multiple_fsc.py
 xmipp3/tests/test_protocol_multireference_alignability.py
 xmipp3/tests/test_protocol_reconstruct_fourier.py
 xmipp3/tests/test_protocol_screen_deepConsensus.py
 xmipp3/tests/test_protocol_simulate_ctf.py
 xmipp3/tests/test_protocol_validate_fscq.py
 xmipp3/tests/test_protocol_validate_overfitting.py
 xmipp3/tests/test_protocols_add_noise.py
+xmipp3/tests/test_protocols_angular_resolution_alignment.py
 xmipp3/tests/test_protocols_continuousflex.py
 xmipp3/tests/test_protocols_deepVolPostprocessing.py
 xmipp3/tests/test_protocols_deepres.py
 xmipp3/tests/test_protocols_fso.py
 xmipp3/tests/test_protocols_gpuCorr_classifier.py
 xmipp3/tests/test_protocols_gpuCorr_fullStreaming.py
 xmipp3/tests/test_protocols_gpuCorr_semiStreaming.py
@@ -184,21 +189,22 @@
 xmipp3/tests/test_protocols_xmipp_movie_resize.py
 xmipp3/tests/test_protocols_xmipp_movies.py
 xmipp3/tests/test_protocols_zernike3d.py
 xmipp3/viewers/__init__.py
 xmipp3/viewers/plotter.py
 xmipp3/viewers/viewer.py
 xmipp3/viewers/viewer_analyze_local_ctf.py
+xmipp3/viewers/viewer_angular_resolution_alignment.py
 xmipp3/viewers/viewer_cl2d.py
-xmipp3/viewers/viewer_classes3D.py
-xmipp3/viewers/viewer_consensus_classes3D.py
+xmipp3/viewers/viewer_consensus_classes.py
 xmipp3/viewers/viewer_ctf_consensus.py
 xmipp3/viewers/viewer_deepEMHancer.py
 xmipp3/viewers/viewer_deep_consensus.py
 xmipp3/viewers/viewer_deep_micrograph_cleaner.py
+xmipp3/viewers/viewer_dose_analysis.py
 xmipp3/viewers/viewer_eliminate_empty_images.py
 xmipp3/viewers/viewer_extract_asymmetric_unit.py
 xmipp3/viewers/viewer_local_sharpening.py
 xmipp3/viewers/viewer_metaprotocol_golden_highres.py
 xmipp3/viewers/viewer_ml2d.py
 xmipp3/viewers/viewer_movie_alignment.py
 xmipp3/viewers/viewer_normalize_strain.py
```

### Comparing `scipion-em-xmipp-23.3.0.3/setup.py` & `scipion-em-xmipp-23.7.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/__init__.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,18 +34,18 @@
 import pwem
 import pyworkflow.utils as pwutils
 
 from .base import *
 from .constants import XMIPP_HOME, XMIPP_URL, XMIPP_DLTK_NAME
 
 _logo = "xmipp_logo.png"
-_references = ['delaRosaTrevin2013', 'Sorzano2013']
-_currentBinVersion = '3.23.03.0'
-# This will allow scipion to detect the plugin version and print it in the log.
-__version__ = _currentBinVersion[2:] + ".3"  # Set this to ".0" on each xmipp binary release, otherwise increase it --> ".1", ".2", ...
+_references = ['delaRosaTrevin2013', 'Sorzano2013', 'Strelak2021']
+_currentBinVersion = '3.23.07.0'
+__version__ = _currentBinVersion[2:] + ".0"  # Set this to ".0" on each xmipp binary release, otherwise increase it --> ".1", ".2", ...
+
 
 
 class Plugin(pwem.Plugin):
     _homeVar = XMIPP_HOME
     _pathVars = [XMIPP_HOME]
     _supportedVersions = []
     _url = XMIPP_URL
@@ -205,43 +205,42 @@
         try:
             nvidiaDriverVer = subprocess.Popen(["nvidia-smi",
                                                 "--query-gpu=driver_version",
                                                 "--format=csv,noheader"],
                                                env=plugin.getEnviron(),
                                                stdout=subprocess.PIPE
                                                ).stdout.read().decode('utf-8').split(".")[0]
-            try:
-                int(nvidiaDriverVer)
-            except ValueError:
-                nvidiaDriverVer = None
             if int(nvidiaDriverVer) < 390:
                 preMsgs.append("Incompatible driver %s" % nvidiaDriverVer)
                 cudaMsgs.append("Your NVIDIA drivers are too old (<390). "
                                 "Tensorflow was installed without GPU support. "
-                                "Just CPU computations enabled (slow computations).")
+                                "Just CPU computations enabled (slow computations)."
+                                "To enable CUDA (drivers>390 needed), "
+                                "set CUDA=True in 'scipion.conf' file")
                 nvidiaDriverVer = None
-        except Exception as e:
-            preMsgs.append(str(e))
+        except (ValueError, TypeError):
+            nvidiaDriverVer = None
+            preMsgs.append("Not nvidia driver found. Type: "
+                           " nvidia-smi --query-gpu=driver_version --format=csv,noheader")
+            preMsgs.append(
+                "CUDA will NOT be USED. (not found or incompatible)")
+            msg = ("Tensorflow installed without GPU. Just CPU computations "
+                   "enabled (slow computations).")
+            cudaMsgs.append(msg)
+            useGpu = False
 
     if nvidiaDriverVer is not None:
-        preMsgs.append("CUDA support find. Driver version: %s" % nvidiaDriverVer)
-        msg = "Tensorflow installed with CUDA SUPPORT."
+        preMsgs.append("CUDA support found. Driver version: %s" % nvidiaDriverVer)
+        msg = "Tensorflow will be installed with CUDA SUPPORT."
         cudaMsgs.append(msg)
         useGpu = True
-    else:
-        preMsgs.append("CUDA will NOT be USED. (not found or incompatible)")
-        msg = ("Tensorflow installed without GPU. Just CPU computations "
-               "enabled (slow computations). To enable CUDA (drivers>390 needed), "
-               "set CUDA=True in 'scipion.conf' file")
-        cudaMsgs.append(msg)
-        useGpu = False
+
 
     # commands  = [(command, target), (cmd, tgt), ...]
-    cmdsInstall = [(cmd, envName + ".yml") for cmd, envName in
-                   CondaEnvManager.yieldInstallAllCmds(useGpu=useGpu)]
+    cmdsInstall = list(CondaEnvManager.yieldInstallAllCmds(useGpu=useGpu))
 
     now = datetime.now()
     installDLvars = {'modelsUrl': "http://scipion.cnb.csic.es/downloads/scipion/software/em",
                      'syncBin': plugin.getHome('bin/xmipp_sync_data'),
                      'modelsDir': plugin.getHome('models'),
                      'modelsPrefix': "models_UPDATED_on",
                      'xmippLibToken': 'xmippLibToken',
@@ -263,10 +262,10 @@
     xmippInstallCheck = ("if ls %(libXmipp)s > /dev/null ; "
                          "then touch %(xmippLibToken)s; echo ' > %(preMsgsStr)s' ; "
                          "else echo ; echo ' > Xmipp installation not found, "
                          "please install it first (xmippSrc or xmippBin*).';echo;"
                          " fi" % installDLvars,           # End of command
                          installDLvars['xmippLibToken'])  # Target
 
-    env.addPackage(XMIPP_DLTK_NAME, version='0.2', urlSuffix='external',
+    env.addPackage(XMIPP_DLTK_NAME, version='1.0', urlSuffix='external',
                    commands=[xmippInstallCheck]+cmdsInstall+[modelsDownloadCmd],
                    deps=[], tar=XMIPP_DLTK_NAME+'.tgz')
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/base.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/bibtex.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/bibtex.py`

 * *Files 2% similar despite different names*

```diff
@@ -600,9 +600,25 @@
 year = {2021},
 issn = {1047-8477},
 doi = {https://doi.org/10.1016/j.jsb.2021.107780},
 url = {https://www.sciencedirect.com/science/article/pii/S104784772100085X},
 author = {E. Fernández-Giménez and M. Martínez and R. Sánchez-García and R. Marabini and E. Ramírez-Aportela and
 P. Conesa and J.M. Carazo and C.O.S. Sorzano},
 }
+
+@Article{Strelak2021,
+AUTHOR = {Strelak, David and Jiménez-Moreno, Amaya and Vilas, José L. and Ramírez-Aportela, Erney and Sánchez-García, Ruben and Maluenda, David and Vargas, Javier and Herreros, David and Fernández-Giménez, Estrella and de Isidro-Gómez, Federico P. and Horacek, Jan and Myska, David and Horacek, Martin and Conesa, Pablo and Fonseca-Reyna, Yunior C. and Jiménez, Jorge and Martínez, Marta and Harastani, Mohamad and Jonić, Slavica and Filipovic, Jiri and Marabini, Roberto and Carazo, José M. and Sorzano, Carlos O. S.},
+TITLE = {Advances in Xmipp for Cryo–Electron Microscopy: From Xmipp to Scipion},
+JOURNAL = {Molecules},
+VOLUME = {26},
+YEAR = {2021},
+NUMBER = {20},
+ARTICLE-NUMBER = {6224},
+URL = {https://www.mdpi.com/1420-3049/26/20/6224},
+PubMedID = {34684805},
+ISSN = {1420-3049},
+DOI = {https://doi.org/10.3390/molecules26206224}
+}
+
+
 """
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/constants.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/convert/__init__.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/convert/convert.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/convert/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/convert/dataimport.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/convert/dataimport.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/convert/io_coordinates.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/convert/io_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/programs.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/programs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/__init__.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,35 +27,36 @@
 # **************************************************************************
 
 from .protocol_preprocess import *
 
 from .protocol_assignment_tilt_pair import XmippProtAssignmentTiltPair
 from .protocol_align_volume import XmippProtAlignVolume, XmippProtAlignVolumeForWeb
 from .protocol_angular_graph_consistency import XmippProtAngularGraphConsistency
+from .protocol_angular_resolution_alignment import XmippProtResolutionAlignment
 from .protocol_preprocess.protocol_add_noise import (XmippProtAddNoiseVolumes,
                                                      XmippProtAddNoiseParticles)
 from .protocol_apply_alignment import XmippProtApplyAlignment
 from .protocol_apply_transformation_matrix import XmippProtApplyTransformationMatrix
 from .protocol_break_symmetry import XmippProtAngBreakSymmetry
 from .protocol_cl2d_align import XmippProtCL2DAlign
 from .protocol_cl2d import XmippProtCL2D
-from .protocol_classify_kmeans2d import XmippProtKmeansClassif2D
+#from .protocol_classify_kmeans2d import XmippProtKmeansClassif2D
 from .protocol_classification_gpuCorr import XmippProtGpuCrrCL2D
 from .protocol_classification_gpuCorr_semi import XmippProtStrGpuCrrSimple
 from .protocol_classification_gpuCorr_full import XmippProtStrGpuCrrCL2D
 from .protocol_ctf_defocus_group import XmippProtCTFDefocusGroup
 from .protocol_compare_reprojections import XmippProtCompareReprojections
 from .protocol_compare_angles import XmippProtCompareAngles
 from .protocol_convert_pdb import XmippProtConvertPdb
 from .protocol_core_analysis import XmippProtCoreAnalysis
 from .protocol_create_gallery import XmippProtCreateGallery
 from .protocol_ctf_consensus import XmippProtCTFConsensus
 from .protocol_ctf_micrographs import XmippProtCTFMicrographs
 from .protocol_ctf_correct_wiener2d import XmippProtCTFCorrectWiener2D
-from .protocol_consensus_classes3D import XmippProtConsensusClasses3D
+from .protocol_consensus_classes import XmippProtConsensusClasses
 from .protocol_denoise_particles import XmippProtDenoiseParticles
 from .protocol_deep_micrograph_screen import  XmippProtDeepMicrographScreen
 from .protocol_eliminate_empty_images import (XmippProtEliminateEmptyParticles,
                                               XmippProtEliminateEmptyClasses)
 from .protocol_enrich import XmippProtEnrich
 from .protocol_extract_particles import XmippProtExtractParticles
 from .protocol_extract_particles_movies import XmippProtExtractMovieParticles
@@ -64,22 +65,23 @@
 from .protocol_helical_parameters import XmippProtHelicalParameters
 from .protocol_kerdensom import XmippProtKerdensom
 from .protocol_ml2d import XmippProtML2D
 from .protocol_movie_gain import XmippProtMovieGain
 from .protocol_flexalign import XmippProtFlexAlign
 from .protocol_movie_opticalflow import XmippProtOFAlignment, ProtMovieAlignment
 from .protocol_movie_max_shift import XmippProtMovieMaxShift
+from .protocol_movie_dose_analysis import XmippProtMovieDoseAnalysis
 from .protocol_movie_split_frames import XmippProtSplitFrames
 from .protocol_multiple_fscs import XmippProtMultipleFSCs
 from .protocol_multireference_alignability import XmippProtMultiRefAlignability
 from .protocol_normalize_strain import XmippProtNormalizeStrain
 from .protocol_particle_pick_automatic import XmippParticlePickingAutomatic
 from .protocol_particle_pick_consensus import XmippProtConsensusPicking
 from .protocol_pick_noise import XmippProtPickNoise
-from .protocol_particle_boxsize import XmippProtParticleBoxsize
+#from .protocol_particle_boxsize import XmippProtParticleBoxsize
 from .protocol_particle_pick import XmippProtParticlePicking
 from .protocol_particle_pick_pairs import XmippProtParticlePickingPairs
 from .protocol_phantom_create import XmippProtPhantom
 from .protocol_preprocess_micrographs import XmippProtPreprocessMicrographs
 from .protocol_projmatch import XmippProtProjMatch
 from .protocol_random_conical_tilt import XmippProtRCT
 from .protocol_ransac import XmippProtRansac
@@ -92,15 +94,15 @@
 from .protocol_resolution_bfactor import XmippProtbfactorResolution
 from .protocol_resolution_directional import XmippProtMonoDir
 from .protocol_resolution_fso import XmippProtFSO
 from .protocol_resolution_monogenic_signal import XmippProtMonoRes
 from .protocol_resolution_deepres import XmippProtDeepRes
 from .protocol_postProcessing_deepPostProcessing import XmippProtDeepVolPostProc
 from .protocol_rotate_volume import XmippProtRotateVolume
-from .protocol_rotational_spectra import XmippProtRotSpectra
+#from .protocol_rotational_spectra import XmippProtRotSpectra
 from .protocol_rotational_symmetry import XmippProtRotationalSymmetry
 from .protocol_screen_particles import XmippProtScreenParticles
 from .protocol_screen_deepConsensus import XmippProtScreenDeepConsensus, XmippProtDeepConsSubSet
 from .protocol_screen_deeplearning import XmippProtScreenDeepLearning
 from .protocol_shift_particles import XmippProtShiftParticles
 from .protocol_shift_volume import XmippProtShiftVolume
 from .protocol_simulate_ctf import XmippProtSimulateCTF
@@ -115,15 +117,14 @@
 from .protocol_validate_fscq import XmippProtValFit
 from .protocol_volume_local_sharpening import XmippProtLocSharp
 from .protocol_volume_strain import XmippProtVolumeStrain
 from .protocol_write_testC import XmippProtWriteTestC
 from .protocol_write_testP import XmippProtWriteTestP
 from .protocol_generate_reprojections import XmippProtGenerateReprojections
 from .protocol_deep_denoising import XmippProtDeepDenoising  # deepDenoising has to be after XmippProtGenerateReprojections and XmippProtCompareReprojections
-from .protocol_split_volume_hierarchical_cluster import XmippProtSplitVolumeHierarchical
 from .protocol_metaprotocol_create_subset import XmippMetaProtCreateSubset
 from .protocol_volume_deform_zernike3d import XmippProtVolumeDeformZernike3D
 from .protocol_structure_map_zernike3d import XmippProtStructureMapZernike3D
 from .protocol_align_volume_and_particles import XmippProtAlignVolumeParticles
 from .protocol_local_ctf import XmippProtLocalCTF
 from .protocol_analyze_local_ctf import XmippProtAnalyzeLocalCTF
 from .protocol_consensus_local_ctf import XmippProtConsensusLocalCTF
@@ -133,7 +134,11 @@
 # from .protocol_kmeans_clustering import XmippProtKmeansSPH
 from .protocol_structure_map import XmippProtStructureMap
 from .protocol_apply_zernike3d import XmippApplyZernike3D
 from .protocol_volume_adjust_sub import XmippProtVolAdjust, XmippProtVolSubtraction
 from .protocol_volume_consensus import XmippProtVolConsensus
 from .protocol_classes_2d_mapping import XmippProtCL2DMap
 from .protocol_deep_hand import XmippProtDeepHand
+from .protocol_deep_center import XmippProtDeepCenter
+from .protocol_deep_center_predict import XmippProtDeepCenterPredict
+from .protocol_deep_global_assignment import XmippProtDeepGlobalAssignment
+from .protocol_deep_global_assignment_predict import XmippProtDeepGlobalAssignmentPredict
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_align_volume.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_align_volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import pyworkflow.protocol.params as params
 from pyworkflow.protocol import STEPS_PARALLEL
 
 from pwem.protocols import ProtAlignVolume
 from pwem.objects import Volume, Transform, SetOfVolumes
 
 from xmipp3.convert import getImageLocation
+from pyworkflow import BETA, UPDATED, NEW, PROD
 
 
 ALIGN_MASK_CIRCULAR = 0
 ALIGN_MASK_BINARY_FILE = 1
 
 ALIGN_ALGORITHM_EXHAUSTIVE = 0
 ALIGN_ALGORITHM_LOCAL = 1
@@ -47,14 +48,16 @@
     """ 
     Aligns a set of volumes using cross correlation 
     or a Fast Fourier method. 
 
      """
     _label = 'align volume'
     nVols = 0
+    _devStatus = UPDATED
+
     
     def __init__(self, **args):
         ProtAlignVolume.__init__(self, **args)
         self.stepsExecutionMode = STEPS_PARALLEL
     
     #--------------------------- DEFINE param functions --------------------------------------------
     def _defineParams(self, form):
@@ -196,15 +199,17 @@
         vols = []
         idx=1
         for vol in self._iterInputVolumes():
             outVol = Volume()
             fnOutVol = self._getExtraPath("vol%02d.mrc"%idx)
             outVol.setLocation(fnOutVol)
             outVol.setObjComment(vol.getObjComment())
-            #set transformation matrix             
+            outVol.setObjLabel(vol.getObjLabel())
+
+            #set transformation matrix
             fhInputTranMat = self._getExtraPath('transformation-matrix_vol%06d.txt'%idx)
             transMatFromFile = np.loadtxt(fhInputTranMat)
             transformationMat = np.reshape(transMatFromFile,(4,4))
             transform = Transform()
             transform.setMatrix(transformationMat)
             outVol.setTransform(transform)            
             vols.append(outVol)
@@ -325,15 +330,15 @@
             if self.maskType == ALIGN_MASK_CIRCULAR:
                 maskArgs+=" --mask circular -%d" % self.maskRadius
             else:
                 maskArgs+=" --mask binary_file %s" % self.maskFile.get().getFileName()
         return maskArgs
     
     def _getAlignArgs(self):
-        alignArgs = ''
+        alignArgs = ' --dontWrap'
         
         if self.alignmentAlgorithm == ALIGN_ALGORITHM_FAST_FOURIER:
             alignArgs += " --frm"
             
         elif self.alignmentAlgorithm == ALIGN_ALGORITHM_LOCAL:
             alignArgs += " --local --rot %f %f 1 --tilt %f %f 1 --psi %f %f 1 -x %f %f 1 -y %f %f 1 -z %f %f 1" %\
                (self.initialRotAngle, self.initialRotAngle,
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_align_volume_and_particles.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_align_volume_and_particles.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,11 +252,11 @@
     #--------------------------- UTILS functions -------------------------------
     def _getMaskArgs(self):
         maskArgs = ''
         if self.applyMask:
             if self.maskType == ALIGN_MASK_CIRCULAR:
                 maskArgs+=" --mask circular -%d" % self.maskRadius
             else:
-                maskArgs+=" --mask binary_file %s" % self.volMask
+                maskArgs+=" --mask binary_file %s" % self.maskFile.get().getFileName()
         return maskArgs
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_analyze_local_ctf.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_analyze_local_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_angular_graph_consistency.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_angular_graph_consistency.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_apply_alignment.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_apply_alignment.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_apply_deformation_zernike3d.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_volume_consensus.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,113 +1,127 @@
-# # *************************************************
-# # * This protocol will be offered in future releases (more testing is needed)
-# # * TODO: If this protocol is added, check that sampling rate is properly set in header of mrc
-# # *************************************************
-
-# # **************************************************************************
-# # *
-# # * Authors:     David Herreros Calero (dherreros@cnb.csic.es)
-# # *
-# # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
-# # *
-# # * This program is free software; you can redistribute it and/or modify
-# # * it under the terms of the GNU General Public License as published by
-# # * the Free Software Foundation; either version 2 of the License, or
-# # * (at your option) any later version.
-# # *
-# # * This program is distributed in the hope that it will be useful,
-# # * but WITHOUT ANY WARRANTY; without even the implied warranty of
-# # * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# # * GNU General Public License for more details.
-# # *
-# # * You should have received a copy of the GNU General Public License
-# # * along with this program; if not, write to the Free Software
-# # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
-# # * 02111-1307  USA
-# # *
-# # *  All comments concerning this program package may be sent to the
-# # *  e-mail address 'scipion@cnb.csic.es'
-# # *
-# # **************************************************************************
-#
-# import os, glob
-# import numpy as np
-#
-# from pwem.protocols import ProtAnalysis3D
-# from pwem.objects import Volume, Integer
-# import pwem.emlib.metadata as md
-# import pyworkflow.protocol.params as params
-# import pyworkflow.utils as pwutils
-#
-#
-# class XmippProtApplyZernike3D(ProtAnalysis3D):
-#     """ Protocol to apply the deformation computed through spherical harmonics to
-#     EM maps. """
-#     _label = 'apply deformation - Zernike3D'
-#
-#     # --------------------------- DEFINE param functions --------------------------------------------
-#     def _defineParams(self, form):
-#         form.addSection(label='Input')
-#         form.addParam('inputVol', params.PointerParam, label="Input volume",
-#                       pointerClass='Volume', important=True,
-#                       help='Select a Volume to be deformed.')
-#         form.addParam('inputClasses', params.PointerParam, pointerClass='SetOfClasses2D',
-#                       label="Input Coefficients", important=True,
-#                       help='Specify a path to the deformation coefficients metadata.')
-#
-#     # --------------------------- INSERT steps functions -----------------------
-#     def _insertAllSteps(self):
-#         self._insertFunctionStep("deformStep")
-#         self._insertFunctionStep("createOutputStep")
-#
-#     # --------------------------- STEPS functions ------------------------------
-#     def deformStep(self):
-#         self.samplingRate_Volume = self.inputVol.get().getSamplingRate()
-#         self.outParams = []
-#         classes = self.inputClasses.get()
-#         self.samplingRate_Coefficients = classes.getSamplingRate()
-#         correctionFactor = self.samplingRate_Coefficients / self.samplingRate_Volume
-#         for rep in classes.iterItems():
-#             basisParams = [rep.L1, rep.L2, rep.Rmax]
-#             coeffs = rep.getRepresentative().get()
-#             coeffs = np.fromstring(coeffs, sep=',')
-#             coeffs = correctionFactor * coeffs
-#             idx = rep.getObjId() + 1
-#             file = self._getTmpPath('coeffs.txt')
-#             # np.savetxt(file, coeffs)
-#             with open(file, 'w') as fid:
-#                 fid.write(' '.join(map(str, basisParams)) + "\n")
-#                 fid.write(' '.join(map(str, coeffs)) + "\n")
-#             outFile = pwutils.removeBaseExt(self.inputVol.get().getFileName()) + '_%d_deformed.mrc' % idx
-#             params = ' -i %s --clnm %s -o %s' % \
-#                      (self.inputVol.get().getFileName(), file, self._getExtraPath(outFile))
-#             self.runJob("xmipp_volume_apply_deform_sph", params)
-#             params = ' -i %s --sampling_rate %f' % (self._getExtraPath(outFile), self.samplingRate_Volume)
-#             self.runJob("xmipp_image_header", params)
-#             self.outParams.append((self._getExtraPath(outFile), rep.getSize()))
-#
-#     def createOutputStep(self):
-#         classes3DSet = self._createSetOfClasses3D(self.inputClasses.get().getImages())
-#         classes3DSet.classifyItems(updateItemCallback=self._updateParticle,
-#                                    updateClassCallback=self._updateClass,
-#                                    itemDataIterator=self.iterClassesId())
-#         result = {'outputClasses': classes3DSet}
-#         self._defineOutputs(**result)
-#         self._defineSourceRelation(self.inputClasses, classes3DSet)
-#         self._defineOutputs(**result)
-#         self._defineSourceRelation(self.inputVol, classes3DSet)
-#
-#     # ------------------------------- UTILS functions -------------------------------
-#     def _updateParticle(self, item, idc):
-#         item.setClassId(idc)
-#
-#     def _updateClass(self, item):
-#         representative = item.getRepresentative()
-#         volumeFile = pwutils.removeBaseExt(self.inputVol.get().getFileName()) + '_%d_deformed.mrc' \
-#                      % (item.getObjId() + 1)
-#         volumeFile = self._getExtraPath(volumeFile)
-#         representative.setSamplingRate(self.samplingRate_Volume)
-#         representative.setLocation(volumeFile)
-#
-#     def iterClassesId(self):
-#         for img in self.inputClasses.get().iterClassItems():
-#             yield img.getClassId()
+# -*- coding: utf-8 -*-
+# **************************************************************************
+# *
+# * Authors:  Estrella Fernandez Gimenez (me.fernandez@cnb.csic.es)
+# *
+# * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
+# *
+# * This program is free software; you can redistribute it and/or modify
+# * it under the terms of the GNU General Public License as published by
+# * the Free Software Foundation; either version 2 of the License, or
+# * (at your option) any later version.
+# *
+# * This program is distributed in the hope that it will be useful,
+# * but WITHOUT ANY WARRANTY; without even the implied warranty of
+# * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# * GNU General Public License for more details.
+# *
+# * You should have received a copy of the GNU General Public License
+# * along with this program; if not, write to the Free Software
+# * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
+# * 02111-1307  USA
+# *
+# *  All comments concerning this program package may be sent to the
+# *  e-mail address 'scipion@cnb.csic.es'
+# *
+# **************************************************************************
+
+from os.path import exists
+from pyworkflow.protocol.params import MultiPointerParam
+from pwem.objects import Volume, Transform
+from pwem.protocols import ProtInitialVolume
+
+
+class XmippProtVolConsensus(ProtInitialVolume):
+    """ This protocol performs a fusion of all the input volumes, which should be preprocessed with protocol 'volume
+    substraction' saving volume 2, in order to be as similar as possible before the fusion. The output of
+    this protocol is the consensus volume and another volume which indicates the maximun difference between input
+    volumes in each voxel."""
+
+    _label = 'volume consensus'
+
+    # --------------------------- DEFINE param functions --------------------------------------------
+    def _defineParams(self, form):
+        form.addSection(label='Input')
+        form.addParam('vols', MultiPointerParam, pointerClass='Volume', label="Volumes",
+                      help='Select the volumes for the consensus.')
+
+    # --------------------------- INSERT steps functions --------------------------------------------
+    def _insertAllSteps(self):
+        self._insertFunctionStep('fusionStep')
+        self._insertFunctionStep('createOutputStep')
+        self._insertFunctionStep("createChimeraScript")
+
+    # --------------------------- STEPS functions ---------------------------------------------------
+    def fusionStep(self):
+        inputVols = self._getExtraPath("input_volumes.txt")
+        fhInputVols = open(inputVols, 'w')
+        for i, vol in enumerate(self.vols):
+            fileName = vol.get().getFileName()
+            if fileName.endswith(':mrc'):
+                fileName = fileName[:-4]
+            fhInputVols.write(fileName + '\n')
+        fhInputVols.close()
+        outVolFn = self._getExtraPath("consensus_volume.mrc")
+        args = " -i %s -o %s" % (inputVols, outVolFn)
+        self.runJob("xmipp_volume_consensus", args)
+
+    def createOutputStep(self):
+        outVol = Volume()
+        outVol.setSamplingRate(self.vols[0].get().getSamplingRate())
+        outVol.setFileName(self._getExtraPath("consensus_volume.mrc"))
+        if not exists(self._getExtraPath("consensus_volume.mrc")):
+            raise NoOutputGenerated("Consensus volume NOT generated, please check input volumes to ensure they have "
+                                    "equal box size, voxel size and origin.")
+        else:
+            outVol2 = Volume()
+            outVol2.setSamplingRate(self.vols[0].get().getSamplingRate())
+            outVol2.setFileName(self._getExtraPath("consensus_volume_diff.mrc"))
+            self._defineOutputs(outputVolume=outVol)
+            self._defineOutputs(outputVolumeDiff=outVol2)
+
+    def createChimeraScript(self):
+        fnRoot = "extra/"
+        scriptFile = self._getPath('result') + '_fusion_chimera.cxc'
+        fhCmd = open(scriptFile, 'w')
+        fhCmd.write("open %s\n" % (fnRoot+"consensus_volume.mrc"))
+        fhCmd.write("open %s\n" % (fnRoot+"consensus_volume_diff.mrc"))
+        fhCmd.write("vol #2 hide\n")
+        fhCmd.write("color sample #1 map #2 palette rainbow\n")
+        fhCmd.close()
+
+    # --------------------------- INFO functions --------------------------------------------
+    def _summary(self):
+        summary = []
+        if not hasattr(self, 'outputVolume'):
+            summary.append("Output volume not ready yet.")
+        else:
+            for i, vol in enumerate(self.vols):
+                summary.append("Volume %d: %s" % (i+1, vol.get().getFileName()))
+        return summary
+
+    def _methods(self):
+        methods = []
+        if not hasattr(self, 'outputVolume'):
+            methods.append("Output volume not ready yet.")
+        else:
+            methods.append("We compute a consensus volume from %d input volumes at %f A/px" %
+                           (self.vols.getSize(), self.vols[0].get().getSamplingRate()))
+        return methods
+
+    def _validate(self):
+        errors = []
+        voxel_size = []
+        for i, vol in enumerate(self.vols):
+            voxel_size.append(round(vol.get().getSamplingRate(), 2))
+        result = all(element == voxel_size[0] for element in voxel_size)
+        if not result:
+            errors.append('Pixel size should be the same for all input volumes.')
+        return errors
+
+    def _citations(self):
+        return ['Fernandez-Gimenez2021']
+
+
+class NoOutputGenerated(Exception):
+    """No output generation error"""
+    pass
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_apply_transformation_matrix.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_apply_transformation_matrix.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_apply_zernike3d.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_apply_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_assignment_tilt_pair.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_assignment_tilt_pair.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_break_symmetry.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_break_symmetry.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_center_particles.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_center_particles.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,28 +25,31 @@
 # *
 # ******************************************************************************
 
 import numpy as np
 import os
 from pyworkflow import VERSION_2_0
 from pwem.constants import ALIGN_2D
-from pwem.objects import Class2D, Particle, Coordinate, Transform
+from pwem.objects import Class2D, Particle, Coordinate, Transform, SetOfClasses2D, SetOfParticles
 from pwem.protocols import ProtClassify2D
 import pwem.emlib.metadata as md
 import pyworkflow.protocol.params as params
 
 from pwem.emlib import MD_APPEND
 from xmipp3.convert import (rowToAlignment, alignmentToRow,
                             rowToParticle, writeSetOfClasses2D, xmippToLocation)
 
+OUTPUT_CLASSES = 'outputClasses'
+OUTPUT_PARTICLES = 'outputParticles'
 
 class XmippProtCenterParticles(ProtClassify2D):
     """ Realignment of un-centered particles. """
     _label = 'center particles'
     _lastUpdateVersion = VERSION_2_0
+    _possibleOutputs = {OUTPUT_CLASSES:SetOfClasses2D, OUTPUT_PARTICLES:SetOfParticles}
 
     # --------------------------- DEFINE param functions -----------------------
     def _defineParams(self, form):
         form.addSection(label='Input')
         form.addParam('inputClasses', params.PointerParam,
                       pointerClass='SetOfClasses2D',
                       important=True,
@@ -172,24 +175,21 @@
         mdImages.write(self._getExtraPath('final_images.xmd'))
 
 
     def createOutputStep(self):
         inputParticles = self.inputClasses.get().getImages()
         outputClasses = self._createSetOfClasses2D(self.inputClasses.get().getImagesPointer())
         self._fillClasses(outputClasses)
-        result = {'outputClasses': outputClasses}
-        self._defineOutputs(**result)
-        self._defineSourceRelation(self.inputClasses, outputClasses)
-
         outputParticles = self._createSetOfParticles()
         outputParticles.copyInfo(inputParticles)
-
         self._fillParticles(outputParticles)
-        result = {'outputParticles': outputParticles}
+
+        result = {OUTPUT_CLASSES: outputClasses, OUTPUT_PARTICLES: outputParticles}
         self._defineOutputs(**result)
+        self._defineSourceRelation(self.inputClasses, outputClasses)
         self._defineSourceRelation(self.inputClasses, outputParticles)
 
     # --------------------------- UTILS functions ------------------------------
     def _fillClasses(self, outputClasses):
         """ Create the SetOfClasses2D """
         inputSet = self.inputClasses.get().getImages()
         myRep = md.MetaData('classes@' + self._getExtraPath(
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_cl2d.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_cl2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_cl2d_align.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_cl2d_align.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_classes_2d_mapping.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_classes_2d_mapping.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_classification_gpuCorr.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_classification_gpuCorr.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_classification_gpuCorr_full.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_classification_gpuCorr_full.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_classification_gpuCorr_semi.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_classification_gpuCorr_semi.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_classify_kmeans2d.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_kerdensom.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# *****************************************************************************
+# **************************************************************************
 # *
-# * Authors:     Tomas Majtner         tmajtner@cnb.csic.es (2017)
+# * Authors:     Josue Gomez Blanco (josue.gomez-blanco@mcgill.ca)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 2 of the License, or
 # * (at your option) any later version.
@@ -18,268 +18,249 @@
 # * along with this program; if not, write to the Free Software
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
-# *****************************************************************************
-
-import os
-
-import pyworkflow.protocol.params as param
-
-from pyworkflow import VERSION_2_0
-
-import pwem.emlib.metadata as md
-import pyworkflow.protocol.constants as cons
-from pyworkflow.object import Set
-from pyworkflow.utils.path import cleanPath
-from pyworkflow.utils.properties import Message
+# **************************************************************************
+from pyworkflow.protocol import (PointerParam, BooleanParam, IntParam,
+                                 LEVEL_ADVANCED, StringParam)
 
+from pwem.emlib.image import ImageHandler
+from pwem.objects import Particle
 from pwem.protocols import ProtClassify2D
-from pwem.objects import SetOfParticles, SetOfClasses2D
-from pwem.constants import ALIGN_NONE
 
-from xmipp3.convert import (writeSetOfParticles, xmippToLocation,
-                            readSetOfParticles)
 
+from pwem import emlib
 
-class XmippProtKmeansClassif2D(ProtClassify2D):
-    """ Classifies a set of particles using a clustering algorithm to subdivide
-    the original dataset into a given number of classes. """
 
-    _label = '2D kmeans clustering'
-    _lastUpdateVersion = VERSION_2_0
+from xmipp3.convert import (writeSetOfParticles, readSetOfClasses2D,
+                            xmippToLocation)
 
-    def __init__(self, **args):
-        ProtClassify2D.__init__(self, **args)
-        self.stepsExecutionMode = param.STEPS_PARALLEL
 
-    # --------------------------- DEFINE param functions -----------------------
+class KendersomBaseClassify(ProtClassify2D):
+    """ Class to create a base template for Kendersom and rotational spectra protocols that share
+    a common structure. 
+    """
+    
+    #--------------------------- DEFINE param functions --------------------------------------------
     def _defineParams(self, form):
-        form.addSection(label=Message.LABEL_INPUT)
-
-        form.addParam('inputParticles', param.PointerParam,
-                      label="Input images",
-                      important=True, pointerClass='SetOfParticles',
-                      help='Select the input images to be classified.')
-        form.addParam('numberOfClasses', param.IntParam, default=10,
-                      label='Number of 2D classes:',
-                      help='Number of 2D classes to be created.')
-        form.addParam('maxObjects', param.IntParam, default=-1,
-                      expertLevel=param.LEVEL_ADVANCED,
-                      label='Threshold for number of particles:',
-                      help='Threshold for number of particles after which the '
-                           'position of clusters will be fixed.')
-
-        form.addParallelSection(threads=1, mpi=1)
-
-    # --------------------------- INSERT steps functions -----------------------
+        form.addSection(label='Input')
+        form.addParam('inputParticles', PointerParam, label="Input images", important=True, 
+                      pointerClass='SetOfParticles', pointerCondition='hasAlignment',
+                      help='Select the input images from the project.'
+                           'It should be a SetOfParticles class')
+        form.addParam('useMask', BooleanParam, default=False,
+                      label='Use a Mask ?', 
+                      help='If you set to *Yes*, you should provide a mask')
+        form.addParam('Mask', PointerParam , condition='useMask',
+                      label="Mask", pointerClass='Mask',
+                      help='Mask image will serve to enhance the classification')
+        
+        line = form.addLine('Dimension of the map', 
+                            help='Josue tiene que meter el help')
+        line.addParam('SomXdim', IntParam, default=7,
+                      label='X')
+        line.addParam('SomYdim', IntParam, default=7,
+                      label='Y')
+               
+        form.addParam('SomReg0', IntParam, default=1000, expertLevel=LEVEL_ADVANCED,
+                      label='Initial regularization factor', 
+                      help='The kerdenSOM algorithm anneals from an initial high regularization factor'
+                      'to a final lower one, in a user-defined number of steps.'
+                      'If the output map is too smooth, lower the regularization factors'
+                      'If the output map is not organized, higher the regularization factors'
+                      'See [[http://xmipp.cnb.uam.es/twiki/bin/view/Xmipp/KerDenSOM][KerDenSOM]]')
+        form.addParam('SomReg1', IntParam, default=200, expertLevel=LEVEL_ADVANCED,
+                      label='Final regularization factor:')
+        form.addParam('SomSteps', IntParam, default=5, expertLevel=LEVEL_ADVANCED,
+                      label='Regularization steps:',
+                      help='Number of steps to lower the regularization factor')
+        form.addParam('extraParams', StringParam, default='', expertLevel=LEVEL_ADVANCED,
+                      label="Additional parameters:", 
+                      help='Additional parameters for kerdensom program. \n For a complete description'
+                      'See [[http://xmipp.cnb.uam.es/twiki/bin/view/Xmipp/KerDenSOM][KerDenSOM]]')
+        self._addParams(form)
+    
+    #--------------------------- INSERT steps functions --------------------------------------------
+    def _prepareParams(self):
+        # Convert input images if necessary
+        self.imgsFn = self._getExtraPath('images.xmd') 
+        self._insertFunctionStep('convertInputStep')  
+        
+        if self.useMask:
+            mask = self.Mask.get().getFileName()
+        else:
+            mask = None
+            
+        self._params = {'oroot': self._getExtraPath("kerdensom"),
+                        'imgsFn': self.imgsFn,
+                        'mask': mask,
+                        'SomXdim': self.SomXdim.get(),
+                        'SomYdim': self.SomYdim.get(),
+                        'SomReg0': self.SomReg0.get(),
+                        'SomReg1': self.SomReg1.get(),
+                        'SomSteps': self.SomSteps.get(),
+                        'extraParams': self.extraParams.get(),
+                        'vectors': self._getExtraPath("vectors.xmd"),
+                        'classes': self._getExtraPath("classes.stk"),
+                        'averages': self._getExtraPath("averages.stk"),
+                        'kvectors': self._getExtraPath("kerdensom_vectors.xmd"),
+                        'kclasses': self._getExtraPath("kerdensom_classes.xmd")
+                       }
+    
     def _insertAllSteps(self):
-        self.finished = False
-        self.insertedDict = {}
-        self.SetOfParticles = [m.clone() for m in self.inputParticles.get()]
-        partsSteps = self._insertNewPartsSteps(self.insertedDict,
-                                               self.SetOfParticles)
-        self._insertFunctionStep('createOutputStep',
-                                 prerequisites=partsSteps, wait=True)
-
+        self._prepareParams()
+        self._insertProccesStep()
+        self._insertFunctionStep('rewriteClassBlockStep')
+        self._insertFunctionStep('createOutputStep')
+    
+    def _insertKerdensomStep(self):
+        args = '-i %(vectors)s --oroot %(oroot)s --xdim %(SomXdim)d --ydim %(SomYdim)d' + \
+               ' --deterministic_annealing %(SomSteps)f %(SomReg0)f %(SomReg1)f %(extraParams)s'
+        self._insertRunJobStep("xmipp_classify_kerdensom", args % self._params)
+#        deleteFiles([self._getExtraPath("vectors.xmd"),self._getExtraPath("vectors.vec")], True)
+    
+    #--------------------------- STEPS functions ---------------------------------------------------
+    def convertInputStep(self):
+        writeSetOfParticles(self.inputParticles.get(),self.imgsFn) 
+
+    #--------------------------- INFO functions ----------------------------------------------------
+    def rewriteClassBlockStep(self):
+        firstImage = self.inputParticles.get().getFirstItem()
+        fnClasses = self._params['kclasses']
+        mdClasses = "classes@%s" % fnClasses
+        fnClassStack = self._params['classes']
+        fnAverageStack = self._params['averages']      
+        
+        md = emlib.MetaData(mdClasses)
+        image = ImageHandler().createImage()
+        
+        counter = 1
+        
+        for objId in md:
+            imageName =  "%06d@%s" % (counter, fnClassStack)
+            averageName = "%06d@%s" % (counter, fnAverageStack)
+            
+            if md.getValue(emlib.MDL_CLASS_COUNT, objId) > 0:
+                # compute the average of images assigned to this class
+                classPrefix = 'class%06d' % counter
+                classMd = '%s_images@%s' % (classPrefix, fnClasses)
+                classRoot = self._getTmpPath(classPrefix)
+                self.runJob('xmipp_image_statistics', 
+                            '-i %s --save_image_stats %s -v 0' % (classMd, classRoot))
+                image.read(classRoot + 'average.xmp')
+            else:
+                # Create emtpy image as average
+                image.read(firstImage.getLocation()) # just to take the right dimensions and datatype
+                image.initConstant(0.)
+                
+            image.write(averageName)
+            md.setValue(emlib.MDL_IMAGE, imageName, objId)
+            md.setValue(emlib.MDL_IMAGE2, averageName, objId)
+            
+            counter += 1
+            
+        md.write(mdClasses, emlib.MD_APPEND)
+        
+    def _preprocessClass(self, classItem, classRow):
+        classItem.average = Particle()
+        classItem.average.setLocation(xmippToLocation(classRow.getValue(emlib.MDL_IMAGE2)))
+        
     def createOutputStep(self):
-        pass
-
-    def _getFirstJoinStepName(self):
-        # This function will be used for streaming, to check which is
-        # the first function that need to wait for all particles
-        # to have completed, this can be overriden in subclasses
-        # (e.g., in Xmipp 'sortPSDStep')
-        return 'createOutputStep'
-
-    def _getFirstJoinStep(self):
-        for s in self._steps:
-            if s.funcName == self._getFirstJoinStepName():
-                return s
-        return None
-
-    def _insertNewPartsSteps(self, insertedDict, inputParticles):
-        deps = []
-        writeSetOfParticles([m.clone() for m in inputParticles],
-                            self._getExtraPath("allDone.xmd"),
-                            alignType=ALIGN_NONE)
-        writeSetOfParticles([m.clone() for m in inputParticles
-                             if int(m.getObjId()) not in insertedDict],
-                            self._getExtraPath("newDone.xmd"),
-                            alignType=ALIGN_NONE)
-
-        stepId = \
-            self._insertFunctionStep('kmeansClassifyStep',
-                                     self._getExtraPath("newDone.xmd"),
-                                     prerequisites=[])
-        deps.append(stepId)
-        for part in inputParticles:
-            if part.getObjId() not in insertedDict:
-                insertedDict[part.getObjId()] = stepId
-        return deps
-
-    def _stepsCheck(self):
-        # Input particles set can be loaded or None when checked for new inputs
-        # If None, we load it
-        self._checkNewInput()
-        self._checkNewOutput()
-
-    def _checkNewInput(self):
-        # Check if there are new particles to process from the input set
-        partsFile = self.inputParticles.get().getFileName()
-        partsSet = SetOfParticles(filename=partsFile)
-        partsSet.loadAllProperties()
-        self.SetOfParticles = [m.clone() for m in partsSet]
-        self.streamClosed = partsSet.isStreamClosed()
-        partsSet.close()
-        partsSet = self._createSetOfParticles()
-        readSetOfParticles(self._getExtraPath("allDone.xmd"), partsSet)
-        newParts = any(m.getObjId() not in partsSet
-                       for m in self.SetOfParticles)
-        outputStep = self._getFirstJoinStep()
-        if newParts:
-            fDeps = self._insertNewPartsSteps(self.insertedDict,
-                                              self.SetOfParticles)
-            if outputStep is not None:
-                outputStep.addPrerequisites(*fDeps)
-            self.updateSteps()
-
-    def _checkNewOutput(self):
-        if getattr(self, 'finished', False):
-            return
-        # Load previously done items (from text file)
-        doneList = self._readDoneList()
-        # Check for newly done items
-        partsSet = self._createSetOfParticles()
-        readSetOfParticles(self._getExtraPath("allDone.xmd"), partsSet)
-        newDone = [m.clone() for m in self.SetOfParticles
-                   if int(m.getObjId()) not in doneList]
-        self.finished = self.streamClosed and (len(doneList) == len(partsSet))
-        if newDone:
-            self._writeDoneList(newDone)
-        elif not self.finished:
-            # If we are not finished and no new output have been produced
-            # it does not make sense to proceed and updated the outputs
-            # so we exit from the function here
-            return
-        if self.finished:  # Unlock createOutputStep if finished all jobs
-            outputStep = self._getFirstJoinStep()
-            if outputStep and outputStep.isWaiting():
-                outputStep.setStatus(cons.STATUS_NEW)
-
-    def _loadOutputSet(self, SetClass, baseName):
-        setFile = self._getPath(baseName)
-        if os.path.exists(setFile):
-            outputSet = SetClass(filename=setFile)
-            outputSet.loadAllProperties()
-            outputSet.enableAppend()
-        else:
-            outputSet = SetClass(filename=setFile)
-            outputSet.setStreamState(outputSet.STREAM_OPEN)
-
-        inputs = self.inputParticles.get()
-        outputSet.copyInfo(inputs)
-        return outputSet
-
-    def _updateOutputSet(self, outputName, outputSet, state=Set.STREAM_OPEN):
-        outputSet.setStreamState(state)
-        if self.hasAttribute(outputName):
-            outputSet.write()  # Write to commit changes
-            outputAttr = getattr(self, outputName)
-            # Copy the properties to the object contained in the protocol
-            outputAttr.copy(outputSet, copyId=False)
-            # Persist changes
-            self._store(outputAttr)
-        else:
-            set2D = self._createSetOfClasses2D(self.inputParticles.get())
-            self._fillClassesFromLevel(set2D)
-
-            outputSet = {'outputClasses': set2D}
-            self._defineOutputs(**outputSet)
-            self._defineSourceRelation(self.inputParticles, set2D)
-
-    def kmeansClassifyStep(self, fnInputMd):
-        iteration = 0
-        args = "-i %s -k %d -m %d" % (fnInputMd, self.numberOfClasses.get(),
-                                      self.maxObjects.get())
-        self.runJob("xmipp_classify_kmeans_2d", args)
-        cleanPath(self._getExtraPath("level_00"))
-        blocks = md.getBlocksInMetaDataFile(self._getExtraPath("output.xmd"))
-        fnDir = self._getExtraPath()
-        # Gather all images in block
-        for b in blocks:
-            if b.startswith('class0'):
-                args = "-i %s@%s --iter 5 --distance correlation " \
-                       "--classicalMultiref --nref 1 --odir %s --oroot %s" % \
-                       (b, self._getExtraPath("output.xmd"), fnDir, b)
-                if iteration == 0:
-                    args += " --nref0 1"
-                else:
-                    args += " --ref0 %s" % \
-                            self._getExtraPath("level_00/%s_classes.stk" % b)
-                self.runJob("xmipp_classify_CL2D", args,
-                            numberOfMpi=max(2, self.numberOfMpi.get()))
-                cleanPath(self._getExtraPath("level_00/%s_classes.xmd" % b))
-
-        streamMode = Set.STREAM_CLOSED if self.finished else Set.STREAM_OPEN
-        outSet = self._loadOutputSet(SetOfClasses2D, 'classes2D.sqlite')
-        self._updateOutputSet('outputParticles', outSet, streamMode)
-
-    def _readDoneList(self):
-        """ Read from a file the id's of the items that have been done. """
-        doneFile = self._getAllDone()
-        doneList = []
-        # Check what items have been previously done
-        if os.path.exists(doneFile):
-            with open(doneFile) as f:
-                doneList += [int(line.strip()) for line in f]
-        return doneList
-
-    def _getAllDone(self):
-        return self._getExtraPath('DONE_all.TXT')
-
-    def _writeDoneList(self, partList):
-        """ Write to a text file the items that have been done. """
-        with open(self._getAllDone(), 'a') as f:
-            for part in partList:
-                f.write('%d\n' % part.getObjId())
-
-    def _updateParticle(self, item, row):
-        item.setClassId(row.getValue(md.MDL_REF))
-
-    def _updateClass(self, item):
-        classId = item.getObjId()
-        if classId in self._classesInfo:
-            index, fn, _ = self._classesInfo[classId]
-            item.setAlignment2D()
-            rep = item.getRepresentative()
-            rep.setLocation(index, fn)
-            rep.setSamplingRate(self.inputParticles.get().getSamplingRate())
-
-    def _loadClassesInfo(self, filename, blockId):
-        """ Read some information about the produced 2D classes
-        from the metadata file.
+        """ Store the kenserdom object 
+        as result of the protocol.
         """
-        self._classesInfo = {}  # store classes info, indexed by class id
-        mdClasses = md.MetaData(filename)
-        for classNumber, row in enumerate(md.iterRows(mdClasses)):
-            index, fn = xmippToLocation(row.getValue(md.MDL_IMAGE))
-            self._classesInfo[blockId] = (index, fn, row.clone())
-
-    def _fillClassesFromLevel(self, clsSet):
-        """ Create the SetOfClasses2D from a given iteration. """
-        blocks = md.getBlocksInMetaDataFile(self._getExtraPath('output.xmd'))
-        for bId, b in enumerate(blocks):
-            if b.startswith('class0'):
-                self._loadClassesInfo(
-                    self._getExtraPath("level_00/%s_classes.stk" % b), bId)
-                xmpMd = b + "@" + self._getExtraPath('output.xmd')
-                iterator = md.SetMdIterator(xmpMd,
-                                            sortByLabel=md.MDL_ITEM_ID,
-                                            updateItemCallback=
-                                            self._updateParticle,
-                                            skipDisabled=True)
-                clsSet.classifyItems(updateItemCallback=iterator.updateItem,
-                                     updateClassCallback=self._updateClass)
+        imgSet = self.inputParticles.get()
+        classes2DSet = self._createSetOfClasses2D(imgSet)
+        readSetOfClasses2D(classes2DSet, self._params['kclasses'], 
+                           preprocessClass=self._preprocessClass)
+        self._defineOutputs(outputClasses=classes2DSet)
+        self._defineSourceRelation(self.inputParticles, classes2DSet)
+    
+    #--------------------------- INFO functions ----------------------------------------------------
+    def _validate(self):
+        errors = []
+        if self.SomReg0 < self.SomReg1:
+            errors.append("Regularization must decrease over iterations:")
+            errors.append("    Initial regularization must be larger than final")
+        if self.useMask:
+            mask = self.Mask.get()
+            if mask is None:
+                errors.append("You have selected to use a mask. Select one.")
+        return errors
+    
+    def _summary(self):
+        return self._methods()
+
+    def _methods(self):
+        messages = []  
+        if not hasattr(self, 'outputClasses'):
+            messages.append("Output classification not ready yet.")
+        elif self.inputParticles.get() is None:
+            messages.append('Input not selected yet.')
+        else:    
+            messages.append("*Kendersom classification*")
+            messages.append('%s particles from %s were classified to obtain %s classes %s.'
+                            % (self.inputParticles.get().getSize(), self.getObjectTag('inputParticles'), self.outputClasses.getSize(), self.getObjectTag('outputClasses')))
+            if self.useMask:
+                messages.append('Mask %s was used in classification.' % self.getObjectTag('Mask'))
+        return messages
+
+
+class XmippProtKerdensom(KendersomBaseClassify):
+    """
+    Classifies a set of images using  Kohonen's Self-Organizing Feature Maps (SOM) 
+    and Fuzzy c-means clustering technique (FCM) .
+    
+    The kerdenSOM algorithm anneals from an initial high regularization factor
+    to a final lower one, in a user-defined number of steps.
+    
+    KerdenSOM is an excellent tool for classification, especially when
+    using a large number of data and classes and when the transition between
+    the classes is almost continuous, with no clear separation between them.
+    
+    The input images must be previously aligned.
+    """
+    _label = 'kerdensom'
+    
+    def __init__(self, **args):
+        KendersomBaseClassify.__init__(self, **args)
+    
+    #--------------------------- DEFINE param functions --------------------------------------------
+    def _addParams(self, form):
+        pass
+    
+    #--------------------------- INSERT steps functions --------------------------------------------
+    def _insertProccesStep(self):
+        self._insertImgToVectorStep()
+        self._insertKerdensomStep()
+        self._insertVectorToImgStep()
+    
+    def _insertImgToVectorStep(self):
+        """ Insert runJob for convert into a vector Md """
+        args = ' -i %(imgsFn)s -o %(vectors)s '
+        if self.useMask:
+            args += ' --mask binary_file %(mask)s'
+        
+        self._insertRunJobStep("xmipp_image_vectorize", args % self._params)
+   
+    def _insertVectorToImgStep(self):
+        args = ' -i %(kvectors)s -o %(classes)s' 
+        if self.useMask:
+            args += ' --mask binary_file %(mask)s'
+        self._insertRunJobStep("xmipp_image_vectorize", args % self._params)
+#        deleteFiles([self._getExtraPath("kerdensom_vectors.xmd"),self._getExtraPath("kerdensom_vectors.vec")], True)
+    
+    #--------------------------- INFO functions ----------------------------------------------------
+    def _validate(self):
+        return KendersomBaseClassify._validate(self)
+    
+    def _summary(self):
+        return KendersomBaseClassify._summary(self)
+    
+    def _methods(self):
+        return KendersomBaseClassify._methods(self)
+    
+    def _citations(self):
+        return ['PascualMontano2001', 'PascualMontano2002']
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_compare_angles.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_compare_angles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_compare_reprojections.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_compare_reprojections.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,19 +261,19 @@
         else:
             return False
 
     def _computeResiduals(self, fnVol):
         if fnVol.endswith('.mrc'):
             fnVol += ':mrc'
         program = "xmipp_subtract_projection"
-        args = '-i %s --ref %s -o %s --save %s --max_resolution %f --sigma %d' % \
-               (self.imgsFn, fnVol, self._getExtraPath("residuals"), self._getExtraPath(''), self.resol.get(),
-                self.sigma.get())
+        args = '-i %s --ref %s -o %s --save %s --max_resolution %f --sigma %d --oroot %s' % \
+               (self.imgsFn, fnVol, self._getExtraPath("residuals.xmd"), self._getExtraPath(''), self.resol.get(),
+                self.sigma.get(), self._getExtraPath("residual_part"))
         self.runJob(program, args, numberOfMpi=1)
-        mrcsresiduals = self._getExtraPath("residuals.mrcs")
+        mrcsresiduals = self._getExtraPath("residuals.xmd")
         args2 = " -i %s -o %s" % (mrcsresiduals, self.fnResiduals)
         self.runJob("xmipp_image_convert", args2, numberOfMpi=1)
         fnNewParticles = self._getExtraPath("images.stk")
         if os.path.exists(fnNewParticles):
             cleanPath(fnNewParticles)
         if os.path.exists(mrcsresiduals):
             cleanPath(mrcsresiduals)
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_consensus_local_ctf.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_split_volume.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# coding=utf-8
 # **************************************************************************
 # *
-# * Authors:     Estrella Fernandez Gimenez (me.fernandez@cnb.csic.es)
-# *              Carlos Oscar Sanchez Sorzano
+# * Authors:     Carlos Oscar Sorzano (coss@cnb.csic.es)
 # *
-# * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia, CSIC
+# * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 2 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
@@ -21,124 +19,94 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-
-import numpy as np
-
-from pyworkflow import VERSION_2_0
-from pyworkflow.object import Float
-from pyworkflow.protocol.params import MultiPointerParam, PointerParam
-
-from pwem.protocols import ProtAnalysis3D
-from pwem import emlib
-
-from xmipp3.convert import setXmippAttribute
-
-
-class XmippProtConsensusLocalCTF(ProtAnalysis3D):
-    """This protocol compares the estimations of local defocus computed by different protocols for a set of particles"""
-    _label = 'consensus local defocus'
-    _lastUpdateVersion = VERSION_2_0
+"""
+Protocol to split a volume in two volumes based on a set of images
+"""
+
+from pyworkflow.protocol.constants import LEVEL_ADVANCED
+from pyworkflow.protocol.params import PointerParam, FloatParam, IntParam, StringParam
+from pyworkflow.utils.path import cleanPath
+from pyworkflow import BETA, UPDATED, NEW, PROD
+from pwem.protocols import ProtClassify3D
+from pwem.objects import Volume
+from pwem.emlib.image import ImageHandler
+from xmipp3.convert import writeSetOfParticles
+
+
+class XmippProtSplitvolume(ProtClassify3D):
+    """Split volume in two"""
+    _label = 'split volume'
+    _devStatus = BETA
 
     def __init__(self, **args):
-        ProtAnalysis3D.__init__(self, **args)
+        ProtClassify3D.__init__(self, **args)
 
     #--------------------------- DEFINE param functions --------------------------------------------
     def _defineParams(self, form):
         form.addSection(label='Input')
-        form.addParam('inputSet', PointerParam,
-                      label="Input particles to assign the consensus defocus",
-                      pointerClass='SetOfParticles',
-                      help="Particle set of interest to estimate the defocus")
-        form.addParam('inputSets', MultiPointerParam,
-                      label="Input defocus estimations",
-                      pointerClass='SetOfParticles',
-                      help="Sets of particles with different local defocus estimations to compare")
-
+        
+        form.addParam('directionalClasses', PointerParam, label="Directional classes", important=True, 
+                      pointerClass='SetOfAverages', pointerCondition='hasAlignmentProj',
+                      help='Select a set of particles with angles. Preferrably the output of a run of directional classes')
+        form.addParam('symmetryGroup', StringParam, default='c1',
+                      label="Symmetry group", 
+                      help='See [[Xmipp Symmetry][http://www2.mrc-lmb.cam.ac.uk/Xmipp/index.php/Conventions_%26_File_formats#Symmetry]] page '
+                           'for a description of the symmetry format accepted by Xmipp') 
+        form.addParam('mask', PointerParam, label="Mask", pointerClass='VolumeMask', allowsNull=True,
+                      help='The mask values must be binary: 0 (remove these voxels) and 1 (let them pass).')
+        form.addParam('Nrec', IntParam, label="Number of reconstructions", default=5000, expertLevel=LEVEL_ADVANCED, 
+                      help="Number of random reconstructions to perform");
+        form.addParam('Nsamples', IntParam, label="Number of images/reconstruction", default=15, expertLevel=LEVEL_ADVANCED, 
+                      help="Number of images per reconstruction. Consider that reconstructions with symmetry c1 will be perfomed");
+        form.addParam('alpha', FloatParam, label="Confidence level", default=0.05, expertLevel=LEVEL_ADVANCED, 
+                      help="This parameter is alpha. Two volumes, one at alpha/2 and another one at 1-alpha/2, will be generated");
+    
     #--------------------------- INSERT steps functions --------------------------------------------
     def _insertAllSteps(self):
-        self._insertFunctionStep("compareDefocus")
-        self._insertFunctionStep("createOutputStep")
+        self._insertFunctionStep('convertInputStep',self.directionalClasses.getObjId())
+        self._insertFunctionStep('generateSplittedVolumes')
+        self._insertFunctionStep('createOutput')
 
     #--------------------------- STEPS functions ---------------------------------------------------
-    def compareDefocus(self):
-        """compare with median, mad and correlation matrix the local defocus value for each pixel estimated by
-        different programs (Xmipp, Relion, gCTF, ...)"""
-        allParticlesDef = {}
-        for defsetP in self.inputSets:
-            defset = defsetP.get()
-            for particle in defset:
-                pIDs = []
-                pDefAs = []
-                pIDs.append(particle.getObjId())
-                defU = particle.getCTF().getDefocusU()
-                defV = particle.getCTF().getDefocusV()
-                pDefAs.append((defU+defV)/2)
-                for pId, pDefA in zip(pIDs,pDefAs):
-                    if not pId in allParticlesDef.keys():
-                        allParticlesDef[pId]=[]
-                    allParticlesDef[pId].append(pDefA)
-        self.defMatrix = np.full(shape=(len(allParticlesDef.keys()),len(self.inputSets)),fill_value=np.NaN)
-        i=0
-        self.pMatrixIdx={}
-        for pId,pdefi in allParticlesDef.items():
-            self.pMatrixIdx[pId]=i
-            for j in enumerate(pdefi):
-                self.defMatrix[i,j[0]]=j[1]
-            i+=1
-
-        self.median = np.nanmedian(self.defMatrix, axis=1)
-        self.mad = np.empty_like(self.median)
-        for k in enumerate(self.median):
-            self.mad[k[0]] = np.nanmedian(np.abs(self.defMatrix[k[0],:] - self.median[k[0]]))
-        self.defMatrix = np.hstack((self.defMatrix, self.median.reshape(len(self.median),1)))
-        self.corrMatrix = np.zeros((self.defMatrix.shape[0],self.defMatrix.shape[1]))
-        defMatrixInvalid = np.ma.masked_invalid(self.defMatrix)
-        self.corrMatrix = np.ma.corrcoef(defMatrixInvalid,rowvar=False)
-        np.savetxt(self._getExtraPath("defocusMatrix.txt"),self.defMatrix)
-        np.savetxt(self._getExtraPath("correlationMatrix.txt"),self.corrMatrix)
-
-    def createOutputStep(self):
-        """create as output a setOfParticles with a consensus estimation of local defocus (median) and its median
-        standard deviation (mad)"""
-        imgSet = self.inputSet.get()
-
-        outputSet = self._createSetOfParticles()
-        outputSet.copyInfo(imgSet)
-        # Loop through input set of
-        for part in imgSet.iterItems():
-
-            id = part.getObjId()
-            if id in self.pMatrixIdx:
-                index = self.pMatrixIdx[id]
-                newPart = part.clone()
-                pMedian = Float(self.median[index])
-                pMad = Float(self.mad[index])
-                setXmippAttribute(newPart.getCTF(), emlib.MDL_CTF_DEFOCUSA, pMedian)
-                setXmippAttribute(newPart.getCTF(), emlib.MDL_CTF_DEFOCUS_RESIDUAL, pMad)
-                outputSet.append(newPart)
-
-        self._defineOutputs(outputParticles=outputSet)
-        self._defineSourceRelation(self.inputSet, outputSet)
-
-
-    def _updateItem(self, particle, row):
-        """update each particle in the set with the values computed"""
-        pId = particle.getObjId()
-        setXmippAttribute(particle,emlib.MDL_CTF_DEFOCUSA,self.median[self.pMatrixIdx[pId]])
-        setXmippAttribute(particle,emlib.MDL_CTF_DEFOCUS_RESIDUAL,self.mad[self.pMatrixIdx[pId]])
-
-    #--------------------------- INFO functions --------------------------------------------
-    def _summary(self):
-        summary = []
-        summary.append("Consensus local defocus and residual computed for %s particles" % self.getObjectTag('outputParticles'))
-        return summary
-
-    def _methods(self):
-        methods = []
-        methods.append("The results obtained when local CTF is estimated by different methods are compared here "
-                       "computing the median, MAD and correlation matrix.")
-        return methods
+    def convertInputStep(self, inputParticlesId):
+        writeSetOfParticles(self.directionalClasses.get(),self._getExtraPath("directionalClasses.xmd"))
+
+    def createOutput(self):
+        inputParticles = self.directionalClasses.get()
+        Ts = inputParticles.getSamplingRate()
+        volumesSet = self._createSetOfVolumes()
+        volumesSet.setSamplingRate(Ts)
+        for i in range(2):
+            vol = Volume()
+            fnVol = self._getExtraPath("split_v%d.vol"%(i+1))
+            fnMrc = self._getExtraPath("split_v%d.mrc"%(i+1))
+            self.runJob("xmipp_image_convert","-i %s -o %s -t vol"%(fnVol,fnMrc), numberOfMpi=1)
+            self.runJob("xmipp_image_header","-i %s --sampling_rate %f"%(fnMrc, Ts), numberOfMpi=1)
+            cleanPath(fnVol)
+            vol.setLocation(1, fnMrc)
+            volumesSet.append(vol)
+        
+        self._defineOutputs(outputVolumes=volumesSet)
+        self._defineSourceRelation(inputParticles, volumesSet)
+        
+    def generateSplittedVolumes(self):
+        inputParticles = self.directionalClasses.get()
+        Xdim = inputParticles.getDimensions()[0]
+        fnMask = ""
+        if self.mask.hasValue():
+            fnMask = self._getExtraPath("mask.vol")
+            img=ImageHandler()
+            img.convert(self.mask.get(), fnMask)
+            self.runJob('xmipp_image_resize',"-i %s --dim %d"%(fnMask,Xdim),numberOfMpi=1)
+            self.runJob('xmipp_transform_threshold',"-i %s --select below 0.5 --substitute binarize"%fnMask,numberOfMpi=1)
+
+        args="-i %s --oroot %s --Nrec %d --Nsamples %d --sym %s --alpha %f"%\
+             (self._getExtraPath("directionalClasses.xmd"),self._getExtraPath("split"),self.Nrec.get(),self.Nsamples.get(),
+              self.symmetryGroup.get(), self.alpha.get())
+        if fnMask!="":
+            args+=" --mask binary_file %s"%fnMask
+        self.runJob("xmipp_classify_first_split",args)
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_convert_pdb.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_helical_parameters.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-# -*- coding: utf-8 -*-
 # **************************************************************************
 # *
-# * Authors:  Jesus Cuenca (jcuenca@cnb.csic.es)
-# *           Roberto Marabini (rmarabini@cnb.csic.es)
-# *           Ignacio Foche
-# * 
-# *           
+# * Authors:     Carlos Oscar S. Sorzano (coss@cnb.csic.es)
+# *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 2 of the License, or
 # * (at your option) any later version.
 # *
@@ -24,195 +20,160 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-import os
-
+import pyworkflow.object as pwobj
+from pwem.objects import Volume
+from pwem.emlib.image import ImageHandler
+from pwem.protocols import ProtPreprocessVolumes
 import pyworkflow.protocol.params as params
-import pyworkflow.protocol.constants as const
-from pyworkflow.utils import replaceBaseExt, removeExt, getExt, createLink
+from pyworkflow.protocol.constants import LEVEL_ADVANCED
 
-from pwem.convert import cifToPdb, downloadPdb, headers
-from pwem.objects import Volume, Transform
-from pwem.protocols import ProtInitialVolume
-
-
-class XmippProtConvertPdb(ProtInitialVolume):
-    """ Convert a PDB file into a volume.  """
-    _label = 'convert a PDB'
-    IMPORT_FROM_ID = 0
-    IMPORT_OBJ = 1
-    IMPORT_FROM_FILES = 2 
-       
-    # --------------------------- DEFINE param functions --------------------------------------------
-    def _defineParams(self, form):
-        """ Define the parameters that will be input for the Protocol.
-        This definition is also used to generate automatically the GUI.
-        """
-        form.addSection(label='Input')
-        form.addParam('inputPdbData', params.EnumParam, choices=['id', 'object', 'file'],
-                      label="Retrieve PDB from", default=self.IMPORT_FROM_ID,
-                      display=params.EnumParam.DISPLAY_HLIST,
-                      help='Retrieve PDB data from server, use a pdb Object, or a local file')
-        form.addParam('pdbId', params.StringParam, condition='inputPdbData == IMPORT_FROM_ID',
-                      label="Pdb Id ", allowsNull=True,
-                      help='Type a pdb Id (four alphanumeric characters).')
-        form.addParam('pdbObj', params.PointerParam, pointerClass='AtomStruct',
-                      label="Input pdb ", condition='inputPdbData == IMPORT_OBJ', allowsNull=True,
-                      help='Specify a pdb object.')
-        form.addParam('pdbFile', params.FileParam,
-                      label="File path", condition='inputPdbData == IMPORT_FROM_FILES', allowsNull=True,
-                      help='Specify a path to desired PDB structure.')
-        form.addParam('sampling', params.FloatParam, default=1.0, 
-                      label="Sampling rate (Å/px)",
-                      help='Sampling rate (Angstroms/pixel)')
-        form.addParam('vol', params.BooleanParam, label='Use a volume as an empty template?', default=False,
-                      help='Use an existing volume to define the size and origin for the output volume. If this option'
-                           'is selected, make sure that "Center PDB" in advanced parameters is set to *No*.')
-        form.addParam('volObj', params.PointerParam, pointerClass='Volume',
-                      label="Input volume ", condition='vol', allowsNull=True,
-                      help='The origin and the final size of the output volume will be taken from this volume.')
-        form.addParam('setSize', params.BooleanParam, label='Set final size?', default=False, condition='vol == False')
-        form.addParam('size_z', params.IntParam, condition='setSize', allowsNull=True,
-                      label="Final size (px) Z",
-                      help='Final size in Z in pixels. If no value is provided, protocol will estimate it.')
-        form.addParam('size_y', params.IntParam, condition='setSize', allowsNull=True,
-                      label="Final size (px) Y",
-                      help='Final size in Y in pixels. If no value is provided, protocol will estimate it.')
-        form.addParam('size_x', params.IntParam, condition='setSize', allowsNull=True,
-                      label="Final size (px) X",
-                      help='Final size in X in pixels. If desired output size is x = y = z you can only fill this '
-                           'field. If no value is provided, protocol will estimate it.')
-        form.addParam('centerPdb', params.BooleanParam, default=True, 
-                      expertLevel=const.LEVEL_ADVANCED, 
-                      label="Center PDB",
-                      help='Center PDB with the center of mass')
-        form.addParam('outPdb', params.BooleanParam, default=False, 
-                      expertLevel=const.LEVEL_ADVANCED, 
-                      label="Store centered PDB",
-                      help='Set to \'Yes\' if you want to save centered PDB. '
-                           'It will be stored in the output directory of this protocol')
+from pwem.emlib import MetaData, MDL_ANGLE_ROT, MDL_SHIFT_Z
+from xmipp3.base import HelicalFinder
+from xmipp3.convert import getImageLocation
+
+
+class XmippProtHelicalParameters(ProtPreprocessVolumes, HelicalFinder):
+    """ Estimate helical parameters and symmetrize.
+    
+    Helical symmetry is defined as V(r,rot,z)=V(r,rot+k*DeltaRot,z+k*Deltaz).
+    """
+    _label = 'helical symmetry'
     
-    # --------------------------- INSERT steps functions --------------------------------------------
+    #--------------------------- DEFINE param functions --------------------------------------------
+    def _defineParams(self, form):
+        form.addSection(label='General parameters')
+        form.addParam('inputVolume', params.PointerParam, pointerClass="Volume", label='Input volume')
+        form.addParam('cylinderInnerRadius', params.IntParam,label='Cylinder inner radius', default=-1,
+                      help="The helix is supposed to occupy this radius in voxels around the Z axis. Leave it as -1 for symmetrizing the whole volume")
+        form.addParam('cylinderOuterRadius',params.IntParam,label='Cylinder outer radius', default=-1,
+                      help="The helix is supposed to occupy this radius in voxels around the Z axis. Leave it as -1 for symmetrizing the whole volume")
+        form.addParam('dihedral',params.BooleanParam,default=False,label='Apply dihedral symmetry')
+        form.addParam('forceDihedralX',params.BooleanParam,default=False,expertLevel=LEVEL_ADVANCED, label='Force the dihedral axis to be in X',
+                      help="If this option is chosen, then the dihedral axis is not searched and it is assumed that it is around X.")
+        form.addParam('additionalCn',params.BooleanParam,default=False,label='Apply Cn symmetry')
+        form.addParam('Cn',params.StringParam,default="C2",condition="additionalCn",label='Cn symmetry')
+
+        form.addSection(label='Search limits')
+        form.addParam('heightFraction',params.FloatParam,default=0.9,label='Height fraction',
+                      help="The helical parameters are only sought using the fraction indicated by this number. "\
+                           "In this way, you can avoid including planes that are poorly resolved at the extremes of the volume. " \
+                           "However, note that the algorithm can perfectly work with a fraction of 1.")
+        form.addParam('rot0',params.FloatParam,default=0,label='Minimum rotational angle',help="In degrees")
+        form.addParam('rotF',params.FloatParam,default=360,label='Maximum rotational angle',help="In degrees")
+        form.addParam('rotStep',params.FloatParam,default=5,label='Angular step',help="In degrees")
+        form.addParam('z0',params.FloatParam,default=1,label='Minimum shift Z',help="In Angstroms")
+        form.addParam('zF',params.FloatParam,default=10,label='Maximum shift Z',help="In Angstroms")
+        form.addParam('zStep',params.FloatParam,default=0.5,label='Shift step',help="In Angstroms")
+        self.deltaZ= params.Float()
+        self.deltaRot=params.Float()
+        form.addParallelSection(threads=4, mpi=0)
+
+    #--------------------------- INSERT steps functions --------------------------------------------
     def _insertAllSteps(self):
-        """ In this function the steps that are going to be executed should
-        be defined. Two of the most used functions are: _insertFunctionStep or _insertRunJobStep
-        """
-        if self.inputPdbData == self.IMPORT_FROM_ID:
-            self._insertFunctionStep('pdbDownloadStep')
-        self._insertFunctionStep('convertPdbStep')
+        self._insertFunctionStep('copyInput')
+        self._insertFunctionStep('coarseSearch')
+        self._insertFunctionStep('fineSearch')
+        self._insertFunctionStep('symmetrize')
         self._insertFunctionStep('createOutput')
+        self.fnVol = getImageLocation(self.inputVolume.get())
+        self.fnVolSym=self._getPath('volume_symmetrized.mrc')
+        [self.height,_,_]=self.inputVolume.get().getDim()
+
+    def _getFileName(self, key, **kwargs):
+        if key=="fine":
+            return self._getExtraPath('fineParams.xmd')
+        elif key=="coarse":
+            return self._getExtraPath('coarseParams.xmd')
+        else:
+            return ""
     
-    # --------------------------- STEPS functions --------------------------------------------
-    def pdbDownloadStep(self):
-        """Download all pdb files in file_list and unzip them."""
-        downloadPdb(self.pdbId.get(), self._getPdbFileName(), self._log)
-        
-    def convertPdbStep(self):
-        """ Although is not mandatory, usually is used by the protocol to
-        register the resulting outputs in the database.
-        """
-        pdbFn = self._getPdbFileName()
-        outFile = removeExt(self._getVolName())
-        if getExt(pdbFn)==".cif":
-            pdbFn2=replaceBaseExt(pdbFn, 'pdb')
-            cifToPdb(pdbFn, pdbFn2)
-            pdbFn = pdbFn2
-
-        if " " in pdbFn:
-            pdbFn_extra = self._getExtraPath(os.path.basename(pdbFn.replace(" ", "_")))
+    #--------------------------- STEPS functions --------------------------------------------
+    def copyInput(self):
+        if self.dihedral:
+            if not self.forceDihedralX:
+                self.runJob("xmipp_transform_symmetrize","-i %s -o %s --sym dihedral --dont_wrap" % (self.fnVol, self.fnVolSym))
+            else:
+                self.runJob("xmipp_transform_geometry","-i %s -o %s --rotate_volume axis 180 1 0 0" % (self.fnVol, self.fnVolSym))
+                self.runJob("xmipp_image_operate","-i %s --plus %s -o %s" % (self.fnVol, self.fnVolSym, self.fnVolSym))
+                self.runJob("xmipp_image_operate","-i %s --mult 0.5" % self.fnVolSym)
         else:
-            pdbFn_extra = self._getExtraPath(os.path.basename(pdbFn))
-
-        createLink(pdbFn, pdbFn_extra)
-
-        samplingR = self.sampling.get()
-
-        args = '-i %s --sampling %f -o %s' % (pdbFn_extra, samplingR, outFile)
-        
-        if self.centerPdb:
-            args += ' --centerPDB'
-            if self.outPdb:
-                args += ' --oPDB'
-
-        if self.vol:
-            vol = self.volObj.get()
-            size = vol.getDim()
-            ccp4header = headers.Ccp4Header(vol.getFileName(), readHeader=True)
-            self.shifts = ccp4header.getOrigin()
-            args += ' --size %d %d %d --orig %d %d %d' % (size[2], size[1], size[0],
-                                                          self.shifts[0]/samplingR,
-                                                          self.shifts[1]/samplingR,
-                                                          self.shifts[2]/samplingR)
-
-        if self.setSize:
-            args += ' --size'
-
-        if self.size_x.hasValue() and self.setSize:
-            args += ' %d' % self.size_x.get()
-
-        if self.size_y.hasValue() and self.size_z.hasValue() and self.setSize:
-            args += ' %d %d' % (self.size_y.get(), self.size_z.get())
-
-        self.info("Input file: " + pdbFn)
-        self.info("Output file: " + outFile)
-        
-        program = "xmipp_volume_from_pdb"
-        self.runJob(program, args)
+            ImageHandler().convert(self.inputVolume.get(), self.fnVolSym)
+                        
+    def coarseSearch(self):
+        Cn = "c1"
+        if self.additionalCn:
+            Cn=self.Cn.get()
+        self.runCoarseSearch(self.fnVolSym,self.dihedral.get(),float(self.heightFraction.get()),
+                             float(self.z0.get()),float(self.zF.get()),float(self.zStep.get()),
+                             float(self.rot0.get()),float(self.rotF.get()),float(self.rotStep.get()),
+                             self.numberOfThreads.get(),self._getFileName('coarse'),
+                             int(self.cylinderInnerRadius.get()),int(self.cylinderOuterRadius.get()),int(self.height),
+                             self.inputVolume.get().getSamplingRate(), Cn)
+
+    def fineSearch(self):
+        Cn = "c1"
+        if self.additionalCn:
+            Cn=self.Cn.get()
+        self.runFineSearch(self.fnVolSym, self.dihedral.get(), self._getFileName('coarse'),
+                           self._getFileName('fine'),
+                           float(self.heightFraction.get()),float(self.z0.get()),float(self.zF.get()),
+                           float(self.rot0.get()),float(self.rotF.get()),
+                           int(self.cylinderInnerRadius.get()),int(self.cylinderOuterRadius.get()),int(self.height),
+                           self.inputVolume.get().getSamplingRate(), Cn)
+
+    def symmetrize(self):
+        Cn = "c1"
+        if self.additionalCn:
+            Cn=self.Cn.get()
+        self.runSymmetrize(self.fnVolSym, self.dihedral.get(), self._getFileName('fine'), self.fnVolSym,
+                           float(self.heightFraction.get()),
+                           self.cylinderInnerRadius.get(), self.cylinderOuterRadius.get(), self.height,
+                           self.inputVolume.get().getSamplingRate(), Cn)
 
     def createOutput(self):
         volume = Volume()
-        volume.setSamplingRate(self.sampling.get())
-        volume.setFileName(self._getVolName())
-        if self.vol:
-            origin = Transform()
-            origin.setShiftsTuple(self.shifts)
-            volume.setOrigin(origin)
+        volume.setFileName(self.fnVolSym)
+        Ts = self.inputVolume.get().getSamplingRate()
+        self.runJob("xmipp_image_header","-i %s --sampling_rate %f"%(self.fnVolSym,Ts))
+        volume.copyInfo(self.inputVolume.get())
         self._defineOutputs(outputVolume=volume)
-        if self.inputPdbData == self.IMPORT_OBJ:
-            self._defineSourceRelation(self.pdbObj, volume)
-    
-    # --------------------------- INFO functions --------------------------------------------
+        self._defineTransformRelation(self.inputVolume, self.outputVolume)
+        
+        md = MetaData(self._getFileName('fine'))
+        objId = md.firstObject()
+        self._defineOutputs(deltaRot=pwobj.Float(md.getValue(MDL_ANGLE_ROT, objId)),
+                            deltaZ=pwobj.Float(md.getValue(MDL_SHIFT_Z, objId)))
+
+    #--------------------------- INFO functions --------------------------------------------
     def _summary(self):
-        """ Even if the full set of parameters is available, this function provides
-        summary information about an specific run.
-        """ 
-        summary = []
-        # Add some lines of summary information
-        if not hasattr(self, 'outputVolume'):
-            summary.append("outputVolume not ready yet.")
-        else:
-            if self.inputPdbData == self.IMPORT_FROM_ID:
-                summary.append("Input PDB ID: %s" % self.pdbId.get())
-            elif self.inputPdbData == self.IMPORT_OBJ:
-                summary.append("Input PDB File: %s" % self.pdbObj.get().getFileName())
-            else:
-                summary.append("Input PDB File: %s" % self.pdbFile.get())
-        return summary
-      
+        messages = []
+        if self.deltaZ.hasValue():
+            messages.append('DeltaZ=%f (voxels) %f (Angstroms)'%(self.deltaZ.get()/self.inputVolume.get().getSamplingRate(),self.deltaZ.get()))
+            messages.append('DeltaRot=%f (degrees)'%self.deltaRot.get())      
+        return messages
+
+    def _citations(self):
+        papers=[]
+        return papers
+
     def _validate(self):
-        """ The function of this hook is to add some validation before the protocol
-        is launched to be executed. It should return a list of errors. If the list is
-        empty the protocol can be executed.
-        """
-        errors = []
-        if self.inputPdbData == self.IMPORT_FROM_ID:
-            lenStr = len(self.pdbId.get())
-            if lenStr != 4:
-                errors = ["Pdb id is composed only by four alphanumeric characters"]
-        
-        return errors
-    
-    # --------------------------- UTLIS functions --------------------------------------------
-    def _getPdbFileName(self):
-        if self.inputPdbData == self.IMPORT_FROM_ID:
-            return self._getExtraPath('%s.cif' % self.pdbId.get())
-        elif self.inputPdbData == self.IMPORT_OBJ:
-            return self.pdbObj.get().getFileName()
-        else:
-            return self.pdbFile.get()
-    
-    def _getVolName(self):
-        return self._getExtraPath(replaceBaseExt(self._getPdbFileName().replace(" ", "_"), "vol"))
+        messages=[]
+        if float(self.z0.get())<=0:
+            messages.append("z0 should not be negative or zero")
+        return messages
+
+    def _methods(self):
+        messages = []      
+        messages.append('We looked for the helical symmetry parameters of the volume %s using Xmipp [delaRosaTrevin2013].' % self.getObjectTag('inputVolume'))
+        if self.deltaZ.hasValue():
+            messages.append('We found them to be %f Angstroms and %f degrees.'%(self.deltaZ.get(),self.deltaRot.get()))
+            messages.append('We symmetrized %s with these parameters and produced the volume %s.'%(self.getObjectTag('inputVolume'),
+                                                                                                  self.getObjectTag('outputVolume')))
+            if self.dihedral.get():
+                messages.append('We applied dihedral symmetry.')
+        return messages
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_core_analysis.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_core_analysis.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_create_gallery.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_create_gallery.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_ctf_consensus.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_ctf_consensus.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from pyworkflow.object import Set, Integer, Pointer
 import pyworkflow.protocol.params as params
 import pyworkflow.utils as pwutils
 
 from pwem.protocols import ProtCTFMicrographs
 from pwem.emlib.metadata import Row
 from pyworkflow.protocol.constants import (STATUS_NEW)
+from pyworkflow import BETA, UPDATED, NEW, PROD
 
 from pwem import emlib
 import xmipp3
 from xmipp3.convert import setXmippAttribute, getScipionObj
 
 ACCEPTED = 'Accepted'
 DISCARDED = 'Discarded'
@@ -54,14 +55,15 @@
 class XmippProtCTFConsensus(ProtCTFMicrographs):
     """
     Protocol to make a selection of meaningful CTFs in basis of the defocus
     values, the astigmatism, the resolution, other Xmipp parameters, and
     the agreement with a secondary CTF for the same set of micrographs.
     """
     _label = 'ctf consensus'
+    _devStatus = UPDATED
     _lastUpdateVersion = VERSION_3_0
 
     def __init__(self, **args):
         ProtCTFMicrographs.__init__(self, **args)
         self._freqResol = {}
         self.stepsExecutionMode = params.STEPS_PARALLEL
 
@@ -185,15 +187,15 @@
                       condition="calculateConsensus", default=False,
                       label='Include all secondary metadata?',
                       help='If *Yes*, all metadata in the *Secondary CTF* will '
                            'be included in the resulting CTF.\n '
                            'If *No*, only the primary metadata (plus consensus '
                            'scores) will be in the resulting CTF.')
 
-        form.addParallelSection(threads=1, mpi=1)
+        form.addParallelSection(threads=4, mpi=1)
 
 # --------------------------- INSERT steps functions -------------------------
     def _insertAllSteps(self):
         self.initializeParams()
         if self.calculateConsensus:
             self.ctfFn2 = self.inputCTF2.get().getFileName()
             self.allCtf2 = {}
@@ -654,18 +656,16 @@
             iceness = self._getIceness()
             ctfMargin = self._getCritCtfMargin()
             minNonAstigmatic, maxNonAstigmatic = \
                 self._getCritNonAstigmaticValidity()
 
             if self.xmippCTF == INPUT1:
                 ctfX = ctf
-            elif self.xmippCTF == INPUT2:
-                ctfX = self.allCtf2.get(ctfId)
             else:
-                raise Exception("No xmipp ctf was found")
+                ctfX = self.allCtf2.get(ctfId)
 
 
             secondCondition = (
                 compareValue(ctfX, '_xmipp_ctfCritFirstZero', 'lt', firstZero) or
                 compareValue(ctfX, '_xmipp_ctfCritfirstZeroRatio', 'lt', minFirstZero) or
                 compareValue(ctfX, '_xmipp_ctfCritfirstZeroRatio', 'bt', maxFirstZero) or
                 compareValue(ctfX, '_xmipp_ctfCritCorr13', 'lt', corr) or
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_ctf_correct_wiener2d.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_ctf_correct_wiener2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_ctf_defocus_group.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_ctf_defocus_group.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_ctf_micrographs.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_ctf_micrographs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_deep_denoising.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_deep_denoising.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_deep_hand.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_deep_hand.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from xmipp3.convert import getImageLocation
 
 class XmippProtDeepHand(EMProtocol, XmippProtocol):
     """Protocol to returns handedness of structure from trained deep learning model
     """
 
     _label ="deep hand"
-    _conda_env = "xmipp_deepHand"
+    _conda_env = "xmipp_pyTorch"
 
     def __init__(self, *args, **kwargs):
         EMProtocol.__init__(self, *args, **kwargs)
         XmippProtocol.__init__(self)
         self.vResizedVolFile = 'resizedVol.mrc'
         self.vMaskFile = 'mask.mrc'
         self.vFilteredVolFile = 'filteredVol.mrc'
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_deep_micrograph_screen.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_deep_micrograph_screen.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,15 @@
               if self.useQueueForSteps() or self.useQueue():
                   args += ' -g all '
               else:
                   args += ' -g %s'%(",".join([str(elem) for elem in self.getGpuList()]))
           else:
               args += ' -g -1'
 
+          os.environ['TF_FORCE_GPU_ALLOW_GROWTH'] = 'true'
           self.runJob('xmipp_deep_micrograph_cleaner', args)
 
 
     def _checkNewOutput(self):
         if getattr(self, 'finished', False):
             return
 
@@ -278,37 +279,34 @@
       if self.micsSource==SAME_AS_PICKING or self.useOtherScale.get()==1:
         scale= 1
       else:
         scale=(1./self.getBoxScale())
       return scale
 
     def _updateOutputCoordSet(self, micList, streamMode):
-
         # Do no proceed if there is not micrograph ready
         if not micList:
             return []
 
         outputDir = self._getExtraPath('outputCoords')
         outputCoords = self.getOutput()
 
         # If there are not outputCoordinates yet, it means that is the first
         # time we are updating output coordinates, so we need to first create
         # the output set
         firstTime = outputCoords is None
 
         if firstTime:
-            if self.micsSource==SAME_AS_PICKING or self.useOtherScale.get()==1:
+            if self.useOtherScale.get() == 1:
               boxSize = self.getBoxSize()
-              micSetPtr = self.getInputMicrographs()
             else:
               boxSize = self.inputCoordinates.get().getBoxSize()
-              micSetPtr = self.inputCoordinates.get().getMicrographs()
-              
-            outputCoords = self._createSetOfCoordinates(micSetPtr,
-                                                        suffix=self.getAutoSuffix())
+
+            micSetPtr = self.getInputMicrographsPointer()
+            outputCoords = self._createSetOfCoordinates(micSetPtr, suffix=self.getAutoSuffix())
             outputCoords.copyInfo(self.inputCoordinates.get())
             outputCoords.setBoxSize(boxSize)
         else:
             outputCoords.enableAppend()
         self.info("Reading coordinates from mics: %s" % ','.join([mic.strId() for mic in micList]))
         readSetOfCoordinates(outputDir, micList, outputCoords, scale= self._getScale())
         self.debug(" _updateOutputCoordSet Stream Mode: %s " % streamMode)
@@ -316,33 +314,35 @@
 
         if firstTime:
             self._defineSourceRelation(micSetPtr,
                                        outputCoords)
 
         return micList
 
-
     #--------------------------- INFO functions --------------------------------
-
     def _getStreamingBatchSize(self):
-      self.firstBatch=True
-      if self.streamingBatchSize.get()==-1:
+      self.firstBatch = True
+      if self.streamingBatchSize.get() == -1:
         if not hasattr(self, "actualBatchSize"):
           if self.isInStreaming():
-            self.actualBatchSize= 16
+            self.actualBatchSize = 16
+            batchSize = self.actualBatchSize
           else:
             if self.firstBatch:
-              self.firstBatch=False
-              batchSize= 4
+              self.firstBatch = False
+              batchSize = 4
             else:
               nPickMics = self._getNumPickedMics()
-              self.actualBatchSize= min(50, nPickMics)
-              batchSize= self.actualBatchSize
+              self.actualBatchSize = min(50, nPickMics)
+              batchSize = self.actualBatchSize
+        else:
+            batchSize = self.actualBatchSize
       else:
-        batchSize= self.streamingBatchSize.get()
+        batchSize = self.streamingBatchSize.get()
+
       return batchSize
 
     def _getNumPickedMics(self):
       nPickMics = 0
       lastId=None
       for coord in self.inputCoordinates.get():
         curId=coord.getMicId()
@@ -418,14 +418,24 @@
         """ Return the micrographs associated to the SetOfCoordinates or
         Other micrographs. """
         if not self._micsOther():
             return self.inputCoordinates.get().getMicrographs()
         else:
             return self.inputMicrographs.get()
 
+    def getInputMicrographsPointer(self):
+        """ Return the micrographs pointer associated to the SetOfCoordinates or
+        Other micrographs. """
+        if not self._micsOther():
+            inMicsPointer = Pointer(self.getMapper().getParent(self.inputCoordinates.get().getMicrographs()),
+                                    extended='outputMicrographs')
+            return inMicsPointer
+        else:
+            return self.inputMicrographs
+
     def getCoords(self):
         return self.inputCoordinates.get()
 
     def getAutoSuffix(self):
         return '_Full' if self.threshold.get() < 0 else '_Auto_%03d'%int(self.threshold.get()*100)
 
     def getOutputName(self):
@@ -481,26 +491,23 @@
         return out
 
     def registerCoords(self, coordsDir):
         """ This method is usually inherited by all Pickers
         and it is used from the Java picking GUI to register
         a new SetOfCoordinates when the user click on +Particles button.
         """
-
-        inputset = self.getInputMicrographs()
-        
+        inputset = self.getInputMicrographsPointer()
         mySuffix = '_Manual_%s' % coordsDir.split('manualThresholding_')[1]
         outputName = 'outputCoordinates' + mySuffix
-
         outputset = self._createSetOfCoordinates(inputset, suffix=mySuffix)
         readSetOfCoordinates(coordsDir, outputset.getMicrographs(), outputset)
         # summary = self.getSummary(outputset)
         # outputset.setObjComment(summary)
         outputs = {outputName: outputset}
         self._defineOutputs(**outputs)
 
         # Using a pointer to define the relations is more robust to scheduling
         # and id changes between the protocol run.db and the main project
         # database. The pointer defined below points to the outputset object
-        self._defineSourceRelation(self.getInputMicrographs(),
+        self._defineSourceRelation(inputset,
                                    Pointer(value=self, extended=outputName))
         self._store()
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_denoise_particles.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_denoise_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_eliminate_empty_images.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_eliminate_empty_images.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_enrich.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_enrich.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_extract_asymmetric_unit.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_extract_asymmetric_unit.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_extract_particles.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_extract_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_extract_particles_movies.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_extract_particles_movies.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_extract_particles_pairs.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_extract_particles_pairs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_flexalign.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_flexalign.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 class XmippProtFlexAlign(ProtAlignMovies):
     """
     Wrapper protocol to Xmipp Movie Alignment by cross-correlation
     """
     NO_ROTATION = 0
     NO_FLIP = 0
-    _devStatus = UPDATED
+    _devStatus = PROD
     _label = 'FlexAlign'
     _lastUpdateVersion = VERSION_1_1
 
     def __init__(self, **args):
         ProtAlignMovies.__init__(self, **args)
         self.stepsExecutionMode = cons.STEPS_PARALLEL
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_generate_reprojections.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_generate_reprojections.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_helical_parameters.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_deep_global_assignment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # **************************************************************************
 # *
-# * Authors:     Carlos Oscar S. Sorzano (coss@cnb.csic.es)
+# * Authors:     COS Sorzano and Adrian Sansinena
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 2 of the License, or
 # * (at your option) any later version.
@@ -20,160 +20,157 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-import pyworkflow.object as pwobj
-from pwem.objects import Volume
-from pwem.emlib.image import ImageHandler
-from pwem.protocols import ProtPreprocessVolumes
-import pyworkflow.protocol.params as params
+from pyworkflow import VERSION_3_0
+from pyworkflow.protocol import STEPS_PARALLEL
+from pyworkflow.protocol.params import (PointerParam, StringParam, FloatParam, EnumParam,
+                                        IntParam, BooleanParam, GPU_LIST)
 from pyworkflow.protocol.constants import LEVEL_ADVANCED
+from pyworkflow.utils.path import moveFile, cleanPattern
+from pwem.protocols import ProtAlign2D
+from pwem.emlib.metadata import iterRows, getFirstRow
+import pwem.emlib.metadata as md
+from xmipp3.convert import createItemMatrix, setXmippAttributes, readSetOfParticles, writeSetOfParticles
+from pwem import ALIGN_PROJ
+from pwem import emlib
+from pwem.emlib.image import ImageHandler
+import os
+import sys
+import numpy as np
+import math
+from shutil import copy
+from os import remove
+from os.path import exists, join
+import xmipp3
+from pyworkflow import BETA, UPDATED, NEW, PROD
+
+
+class XmippProtDeepGlobalAssignment(ProtAlign2D, xmipp3.XmippProtocol):
+    """Learns a model to assign angles to particles using deep learning. Particles must be previously centered with respect
+       to a volume, and they must have 3D alignment information. """
+    _label = 'deep global assignment'
+    _lastUpdateVersion = VERSION_3_0
+    _devStatus = BETA
+
+    _conda_env = 'xmipp_DLTK_v1.0'
+    _cond_modelPretrainTrue = 'modelPretrain==True'
+    _cond_modelPretrainFalse = 'modelPretrain==False'
 
-from pwem.emlib import MetaData, MDL_ANGLE_ROT, MDL_SHIFT_Z
-from xmipp3.base import HelicalFinder
-from xmipp3.convert import getImageLocation
-
+    def __init__(self, **args):
+        ProtAlign2D.__init__(self, **args)
 
-class XmippProtHelicalParameters(ProtPreprocessVolumes, HelicalFinder):
-    """ Estimate helical parameters and symmetrize.
-    
-    Helical symmetry is defined as V(r,rot,z)=V(r,rot+k*DeltaRot,z+k*Deltaz).
-    """
-    _label = 'helical symmetry'
-    
-    #--------------------------- DEFINE param functions --------------------------------------------
+    # --------------------------- DEFINE param functions --------------------------------------------
     def _defineParams(self, form):
-        form.addSection(label='General parameters')
-        form.addParam('inputVolume', params.PointerParam, pointerClass="Volume", label='Input volume')
-        form.addParam('cylinderInnerRadius', params.IntParam,label='Cylinder inner radius', default=-1,
-                      help="The helix is supposed to occupy this radius in voxels around the Z axis. Leave it as -1 for symmetrizing the whole volume")
-        form.addParam('cylinderOuterRadius',params.IntParam,label='Cylinder outer radius', default=-1,
-                      help="The helix is supposed to occupy this radius in voxels around the Z axis. Leave it as -1 for symmetrizing the whole volume")
-        form.addParam('dihedral',params.BooleanParam,default=False,label='Apply dihedral symmetry')
-        form.addParam('forceDihedralX',params.BooleanParam,default=False,expertLevel=LEVEL_ADVANCED, label='Force the dihedral axis to be in X',
-                      help="If this option is chosen, then the dihedral axis is not searched and it is assumed that it is around X.")
-        form.addParam('additionalCn',params.BooleanParam,default=False,label='Apply Cn symmetry')
-        form.addParam('Cn',params.StringParam,default="C2",condition="additionalCn",label='Cn symmetry')
-
-        form.addSection(label='Search limits')
-        form.addParam('heightFraction',params.FloatParam,default=0.9,label='Height fraction',
-                      help="The helical parameters are only sought using the fraction indicated by this number. "\
-                           "In this way, you can avoid including planes that are poorly resolved at the extremes of the volume. " \
-                           "However, note that the algorithm can perfectly work with a fraction of 1.")
-        form.addParam('rot0',params.FloatParam,default=0,label='Minimum rotational angle',help="In degrees")
-        form.addParam('rotF',params.FloatParam,default=360,label='Maximum rotational angle',help="In degrees")
-        form.addParam('rotStep',params.FloatParam,default=5,label='Angular step',help="In degrees")
-        form.addParam('z0',params.FloatParam,default=1,label='Minimum shift Z',help="In Angstroms")
-        form.addParam('zF',params.FloatParam,default=10,label='Maximum shift Z',help="In Angstroms")
-        form.addParam('zStep',params.FloatParam,default=0.5,label='Shift step',help="In Angstroms")
-        self.deltaZ= params.Float()
-        self.deltaRot=params.Float()
-        form.addParallelSection(threads=4, mpi=0)
+        form.addHidden(GPU_LIST, StringParam, default='0',
+                       expertLevel=LEVEL_ADVANCED,
+                       label="Choose GPU IDs",
+                       help="GPU may have several cores. Set it to zero"
+                            " if you do not know what we are talking about."
+                            " First core index is 0, second 1 and so on.")
+        form.addSection(label='Input')
+        form.addParam('inputTrainSet', PointerParam, label="Input training set",
+                      pointerClass='SetOfParticles',
+                      pointerCondition='hasAlignment2D or hasAlignmentProj',
+                      help='The set of particles previously aligned to be used as training set')
+
+        form.addParam('Xdim', IntParam, label="Size of the images for training", default=128)
+
+        form.addParam('modelPretrain', BooleanParam, default=False,
+                      label='Choose if you want to use a pretrained model',
+                      help='Set "yes" if you want to use a previously trained model. '
+                           'If you choose "no" new models will be trained.')
+
+        form.addParam('pretrainedModels', PointerParam,
+                      pointerClass='XmippProtDeepGlobalAssignment',
+                      condition=self._cond_modelPretrainTrue,
+                      label='Pretrained model',
+                      help='Select the pretrained model. ')
+
+        form.addSection(label='Training parameters')
+        form.addParam('numAngModels', IntParam,
+                      label="Number of models for angular assignment", default=5,
+                      help="Choose number of models you want to train. More than 1 is recommended only if next step "
+                           "is inference.")
+
+        form.addParam('numEpochs_ang', IntParam,
+                      label="Number of epochs",
+                      default=25, expertLevel=LEVEL_ADVANCED,
+                      help="Number of epochs for training.")
+
+        form.addParam('batchSize', IntParam,
+                      label="Batch size for training",
+                      default=32, expertLevel=LEVEL_ADVANCED,
+                      help="Batch size for training.")
+
+        form.addParam('learningRate', FloatParam,
+                      label="Learning rate",
+                      default=0.001, expertLevel=LEVEL_ADVANCED,
+                      help="Learning rate for training.")
+
+        form.addParam('sigma', FloatParam,
+                      label="Image shifting",
+                      default=2, expertLevel=LEVEL_ADVANCED,
+                      help="Maximum number of pixels that particles can be shifted in each direction from the center.")
+
+        form.addParam('patience', IntParam,
+                      label="Patience",
+                      default=20, expertLevel=LEVEL_ADVANCED,
+                      help="Training will be stopped if the number of epochs without improvement is greater than "
+                           "patience.")
+
+        form.addParallelSection(threads=1, mpi=1)
 
-    #--------------------------- INSERT steps functions --------------------------------------------
+    # --------------------------- INSERT steps functions --------------------------------------------
     def _insertAllSteps(self):
-        self._insertFunctionStep('copyInput')
-        self._insertFunctionStep('coarseSearch')
-        self._insertFunctionStep('fineSearch')
-        self._insertFunctionStep('symmetrize')
-        self._insertFunctionStep('createOutput')
-        self.fnVol = getImageLocation(self.inputVolume.get())
-        self.fnVolSym=self._getPath('volume_symmetrized.mrc')
-        [self.height,_,_]=self.inputVolume.get().getDim()
-
-    def _getFileName(self, key, **kwargs):
-        if key=="fine":
-            return self._getExtraPath('fineParams.xmd')
-        elif key=="coarse":
-            return self._getExtraPath('coarseParams.xmd')
+        self.trainImgsFn = self._getExtraPath('train_input_imgs.xmd')
+        if self.useQueueForSteps() or self.useQueue():
+            myStr = os.environ["CUDA_VISIBLE_DEVICES"]
         else:
-            return ""
-    
-    #--------------------------- STEPS functions --------------------------------------------
-    def copyInput(self):
-        if self.dihedral:
-            if not self.forceDihedralX:
-                self.runJob("xmipp_transform_symmetrize","-i %s -o %s --sym dihedral --dont_wrap" % (self.fnVol, self.fnVolSym))
-            else:
-                self.runJob("xmipp_transform_geometry","-i %s -o %s --rotate_volume axis 180 1 0 0" % (self.fnVol, self.fnVolSym))
-                self.runJob("xmipp_image_operate","-i %s --plus %s -o %s" % (self.fnVol, self.fnVolSym, self.fnVolSym))
-                self.runJob("xmipp_image_operate","-i %s --mult 0.5" % self.fnVolSym)
-        else:
-            ImageHandler().convert(self.inputVolume.get(), self.fnVolSym)
-                        
-    def coarseSearch(self):
-        Cn = "c1"
-        if self.additionalCn:
-            Cn=self.Cn.get()
-        self.runCoarseSearch(self.fnVolSym,self.dihedral.get(),float(self.heightFraction.get()),
-                             float(self.z0.get()),float(self.zF.get()),float(self.zStep.get()),
-                             float(self.rot0.get()),float(self.rotF.get()),float(self.rotStep.get()),
-                             self.numberOfThreads.get(),self._getFileName('coarse'),
-                             int(self.cylinderInnerRadius.get()),int(self.cylinderOuterRadius.get()),int(self.height),
-                             self.inputVolume.get().getSamplingRate(), Cn)
-
-    def fineSearch(self):
-        Cn = "c1"
-        if self.additionalCn:
-            Cn=self.Cn.get()
-        self.runFineSearch(self.fnVolSym, self.dihedral.get(), self._getFileName('coarse'),
-                           self._getFileName('fine'),
-                           float(self.heightFraction.get()),float(self.z0.get()),float(self.zF.get()),
-                           float(self.rot0.get()),float(self.rotF.get()),
-                           int(self.cylinderInnerRadius.get()),int(self.cylinderOuterRadius.get()),int(self.height),
-                           self.inputVolume.get().getSamplingRate(), Cn)
-
-    def symmetrize(self):
-        Cn = "c1"
-        if self.additionalCn:
-            Cn=self.Cn.get()
-        self.runSymmetrize(self.fnVolSym, self.dihedral.get(), self._getFileName('fine'), self.fnVolSym,
-                           float(self.heightFraction.get()),
-                           self.cylinderInnerRadius.get(), self.cylinderOuterRadius.get(), self.height,
-                           self.inputVolume.get().getSamplingRate(), Cn)
-
-    def createOutput(self):
-        volume = Volume()
-        volume.setFileName(self.fnVolSym)
-        Ts = self.inputVolume.get().getSamplingRate()
-        self.runJob("xmipp_image_header","-i %s --sampling_rate %f"%(self.fnVolSym,Ts))
-        volume.copyInfo(self.inputVolume.get())
-        self._defineOutputs(outputVolume=volume)
-        self._defineTransformRelation(self.inputVolume, self.outputVolume)
-        
-        md = MetaData(self._getFileName('fine'))
-        objId = md.firstObject()
-        self._defineOutputs(deltaRot=pwobj.Float(md.getValue(MDL_ANGLE_ROT, objId)),
-                            deltaZ=pwobj.Float(md.getValue(MDL_SHIFT_Z, objId)))
-
-    #--------------------------- INFO functions --------------------------------------------
-    def _summary(self):
-        messages = []
-        if self.deltaZ.hasValue():
-            messages.append('DeltaZ=%f (voxels) %f (Angstroms)'%(self.deltaZ.get()/self.inputVolume.get().getSamplingRate(),self.deltaZ.get()))
-            messages.append('DeltaRot=%f (degrees)'%self.deltaRot.get())      
-        return messages
-
-    def _citations(self):
-        papers=[]
-        return papers
-
-    def _validate(self):
-        messages=[]
-        if float(self.z0.get())<=0:
-            messages.append("z0 should not be negative or zero")
-        return messages
+            myStr = self.gpuList.get()
+            os.environ["CUDA_VISIBLE_DEVICES"] = self.gpuList.get()
+        numGPU = myStr.split(',')
+
+        self._insertFunctionStep("convertStep")
+        self._insertFunctionStep("train", numGPU[0])
+
+    # --------------------------- STEPS functions ---------------------------------------------------
+    def convertStep(self):
+        writeSetOfParticles(self.inputTrainSet.get(), self.trainImgsFn)
+        self.runJob("xmipp_image_resize",
+                    "-i %s -o %s --save_metadata_stack %s --fourier %d" %
+                    (self.trainImgsFn,
+                     self._getExtraPath('trainingResized.stk'),
+                     self._getExtraPath('trainingResized.xmd'),
+                     self.Xdim), numberOfMpi=self.numberOfThreads.get() * self.numberOfMpi.get())
+
+    def train(self, gpuId):
+
+        sig = self.sigma.get()
+
+        self.pretrained = 'no'
+        self.pathToModel = 'none'
+        if self.modelPretrain:
+            self.model = self.pretrainedModels.get()
+            self.pretrained = 'yes'
+            self.pathToModel = self.model._getExtraPath("modelAngular0.h5")
+
+        args = "%s %s %f %d %d %s %d %f %d %s %s" % (
+            self._getExtraPath("trainingResized.xmd"), self._getExtraPath("modelAngular"), sig,
+            self.numEpochs_ang, self.batchSize.get(), gpuId, self.numAngModels.get(), self.learningRate.get(),
+            self.patience.get(), self.pretrained, self.pathToModel)
+        print(args)
+        self.runJob("xmipp_deep_global_assignment", args, numberOfMpi=1, env=self.getCondaEnv())
 
-    def _methods(self):
-        messages = []      
-        messages.append('We looked for the helical symmetry parameters of the volume %s using Xmipp [delaRosaTrevin2013].' % self.getObjectTag('inputVolume'))
-        if self.deltaZ.hasValue():
-            messages.append('We found them to be %f Angstroms and %f degrees.'%(self.deltaZ.get(),self.deltaRot.get()))
-            messages.append('We symmetrized %s with these parameters and produced the volume %s.'%(self.getObjectTag('inputVolume'),
-                                                                                                  self.getObjectTag('outputVolume')))
-            if self.dihedral.get():
-                messages.append('We applied dihedral symmetry.')
-        return messages
+        remove(self._getExtraPath("trainingResized.xmd"))
+        remove(self._getExtraPath("trainingResized.stk"))
 
+    # --------------------------- INFO functions --------------------------------
+    def _methods(self):
+        methods = []
+        if hasattr(self, 'outputParticles'):
+            methods.append("We learned a model to center particles from %i input images (%s)." \
+                           % (self.inputSet.get().getSize(), self.getObjectTag('inputSet')))
+        return methods
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_kerdensom.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_resolution_monogenic_signal.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+# -*- coding: utf-8 -*-
 # **************************************************************************
 # *
-# * Authors:     Josue Gomez Blanco (josue.gomez-blanco@mcgill.ca)
+# * Authors:     J.L. Vilas (jlvilas@cnb.csic.es)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 2 of the License, or
 # * (at your option) any later version.
@@ -19,248 +20,240 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-from pyworkflow.protocol import (PointerParam, BooleanParam, IntParam,
-                                 LEVEL_ADVANCED, StringParam)
+import os
 
-from pwem.emlib.image import ImageHandler
-from pwem.objects import Particle
-from pwem.protocols import ProtClassify2D
+import matplotlib.pyplot as plt
+from matplotlib import cm
+from pwem.wizards import ColorScaleWizardBase
+from pyworkflow.utils import replaceExt
+from os.path import exists
+
+from pyworkflow.protocol.params import (LabelParam, EnumParam, PointerParam,
+                                        IntParam, LEVEL_ADVANCED)
+from pyworkflow.viewer import ProtocolViewer, DESKTOP_TKINTER
+
+from xmipp3.viewers.viewer_resolution_directional import AX_Z
+from pwem.viewers import (LocalResolutionViewer, EmPlotter, ChimeraView,
+                          DataView)
+from pwem.emlib.metadata import MetaData, MDL_X, MDL_COUNT
+
+from xmipp3.protocols.protocol_resolution_monogenic_signal import (
+    XmippProtMonoRes, OUTPUT_RESOLUTION_FILE, FN_METADATA_HISTOGRAM,
+    OUTPUT_RESOLUTION_FILE_CHIMERA)
+from .plotter import XmippPlotter
+from pyworkflow.gui import plotter
 
 
-from pwem import emlib
+class XmippMonoResViewer(LocalResolutionViewer):
+    """
+    Visualization tools for MonoRes results.
+    
+    MonoRes is a Xmipp packagefor computing the local resolution of 3D
+    density maps studied in structural biology, primarily by cryo-electron
+    microscopy (cryo-EM).
+    """
+    _label = 'viewer MonoRes'
+    _targets = [XmippProtMonoRes]
+    _environments = [DESKTOP_TKINTER]
+
+    @staticmethod
+    def getColorMapChoices():
+        return plt.colormaps()
 
+    def __init__(self, *args, **kwargs):
+        ProtocolViewer.__init__(self, *args, **kwargs)
 
-from xmipp3.convert import (writeSetOfParticles, readSetOfClasses2D,
-                            xmippToLocation)
+    def _defineParams(self, form):
+        form.addSection(label='Visualization')
 
+        form.addParam('doShowVolumeSlices', LabelParam,
+                      label="Show resolution slices")
 
-class KendersomBaseClassify(ProtClassify2D):
-    """ Class to create a base template for Kendersom and rotational spectra protocols that share
-    a common structure. 
-    """
-    
-    #--------------------------- DEFINE param functions --------------------------------------------
-    def _defineParams(self, form):
-        form.addSection(label='Input')
-        form.addParam('inputParticles', PointerParam, label="Input images", important=True, 
-                      pointerClass='SetOfParticles', pointerCondition='hasAlignment',
-                      help='Select the input images from the project.'
-                           'It should be a SetOfParticles class')
-        form.addParam('useMask', BooleanParam, default=False,
-                      label='Use a Mask ?', 
-                      help='If you set to *Yes*, you should provide a mask')
-        form.addParam('Mask', PointerParam , condition='useMask',
-                      label="Mask", pointerClass='Mask',
-                      help='Mask image will serve to enhance the classification')
-        
-        line = form.addLine('Dimension of the map', 
-                            help='Josue tiene que meter el help')
-        line.addParam('SomXdim', IntParam, default=7,
-                      label='X')
-        line.addParam('SomYdim', IntParam, default=7,
-                      label='Y')
-               
-        form.addParam('SomReg0', IntParam, default=1000, expertLevel=LEVEL_ADVANCED,
-                      label='Initial regularization factor', 
-                      help='The kerdenSOM algorithm anneals from an initial high regularization factor'
-                      'to a final lower one, in a user-defined number of steps.'
-                      'If the output map is too smooth, lower the regularization factors'
-                      'If the output map is not organized, higher the regularization factors'
-                      'See [[http://xmipp.cnb.uam.es/twiki/bin/view/Xmipp/KerDenSOM][KerDenSOM]]')
-        form.addParam('SomReg1', IntParam, default=200, expertLevel=LEVEL_ADVANCED,
-                      label='Final regularization factor:')
-        form.addParam('SomSteps', IntParam, default=5, expertLevel=LEVEL_ADVANCED,
-                      label='Regularization steps:',
-                      help='Number of steps to lower the regularization factor')
-        form.addParam('extraParams', StringParam, default='', expertLevel=LEVEL_ADVANCED,
-                      label="Additional parameters:", 
-                      help='Additional parameters for kerdensom program. \n For a complete description'
-                      'See [[http://xmipp.cnb.uam.es/twiki/bin/view/Xmipp/KerDenSOM][KerDenSOM]]')
-        self._addParams(form)
-    
-    #--------------------------- INSERT steps functions --------------------------------------------
-    def _prepareParams(self):
-        # Convert input images if necessary
-        self.imgsFn = self._getExtraPath('images.xmd') 
-        self._insertFunctionStep('convertInputStep')  
-        
-        if self.useMask:
-            mask = self.Mask.get().getFileName()
-        else:
-            mask = None
-            
-        self._params = {'oroot': self._getExtraPath("kerdensom"),
-                        'imgsFn': self.imgsFn,
-                        'mask': mask,
-                        'SomXdim': self.SomXdim.get(),
-                        'SomYdim': self.SomYdim.get(),
-                        'SomReg0': self.SomReg0.get(),
-                        'SomReg1': self.SomReg1.get(),
-                        'SomSteps': self.SomSteps.get(),
-                        'extraParams': self.extraParams.get(),
-                        'vectors': self._getExtraPath("vectors.xmd"),
-                        'classes': self._getExtraPath("classes.stk"),
-                        'averages': self._getExtraPath("averages.stk"),
-                        'kvectors': self._getExtraPath("kerdensom_vectors.xmd"),
-                        'kclasses': self._getExtraPath("kerdensom_classes.xmd")
-                       }
-    
-    def _insertAllSteps(self):
-        self._prepareParams()
-        self._insertProccesStep()
-        self._insertFunctionStep('rewriteClassBlockStep')
-        self._insertFunctionStep('createOutputStep')
-    
-    def _insertKerdensomStep(self):
-        args = '-i %(vectors)s --oroot %(oroot)s --xdim %(SomXdim)d --ydim %(SomYdim)d' + \
-               ' --deterministic_annealing %(SomSteps)f %(SomReg0)f %(SomReg1)f %(extraParams)s'
-        self._insertRunJobStep("xmipp_classify_kerdensom", args % self._params)
-#        deleteFiles([self._getExtraPath("vectors.xmd"),self._getExtraPath("vectors.vec")], True)
-    
-    #--------------------------- STEPS functions ---------------------------------------------------
-    def convertInputStep(self):
-        writeSetOfParticles(self.inputParticles.get(),self.imgsFn) 
-
-    #--------------------------- INFO functions ----------------------------------------------------
-    def rewriteClassBlockStep(self):
-        firstImage = self.inputParticles.get().getFirstItem()
-        fnClasses = self._params['kclasses']
-        mdClasses = "classes@%s" % fnClasses
-        fnClassStack = self._params['classes']
-        fnAverageStack = self._params['averages']      
-        
-        md = emlib.MetaData(mdClasses)
-        image = ImageHandler().createImage()
-        
-        counter = 1
-        
-        for objId in md:
-            imageName =  "%06d@%s" % (counter, fnClassStack)
-            averageName = "%06d@%s" % (counter, fnAverageStack)
-            
-            if md.getValue(emlib.MDL_CLASS_COUNT, objId) > 0:
-                # compute the average of images assigned to this class
-                classPrefix = 'class%06d' % counter
-                classMd = '%s_images@%s' % (classPrefix, fnClasses)
-                classRoot = self._getTmpPath(classPrefix)
-                self.runJob('xmipp_image_statistics', 
-                            '-i %s --save_image_stats %s -v 0' % (classMd, classRoot))
-                image.read(classRoot + 'average.xmp')
+        form.addParam('doShowOriginalVolumeSlices', LabelParam,
+                      label="Show original volume slices")
+
+        form.addParam('doShowResHistogram', LabelParam,
+                      label="Show resolution histogram")
+
+        group = form.addGroup('Colored resolution Slices and Volumes')
+
+        group.addParam('sliceAxis', EnumParam, default=AX_Z,
+                       choices=['x', 'y', 'z'],
+                       display=EnumParam.DISPLAY_HLIST,
+                       label='Slice axis')
+
+        group.addParam('doShowVolumeColorSlices', LabelParam,
+                       label="Show colored slices")
+
+        group.addParam('doShowOneColorslice', LabelParam,
+                       expertLevel=LEVEL_ADVANCED,
+                       label='Show selected slice')
+
+        group.addParam('sliceNumber', IntParam, default=-1,
+                       expertLevel=LEVEL_ADVANCED,
+                       label='Show slice number')
+
+        group.addParam('doShowChimera', LabelParam,
+                       label="Show Resolution map in ChimeraX")
+
+        ColorScaleWizardBase.defineColorScaleParams(group, defaultLowest=self.protocol.min_res_init,
+                                                    defaultHighest=self.protocol.max_res_init)
+
+        group.addParam('sharpenedMap', PointerParam, pointerClass='Volume',
+                       label="(Optional) Color a sharpen map by local resolution in ChimeraX",
+                       allowsNull=True,
+                       help='Local resolution should be estimated with the raw maps instead'
+                            ' of sharpen maps. Information about this in (Vilas et al '
+                            'Current Opinion in Structural Biology 2021). This entry parameter '
+                            'allows to color the local resolution in'
+                            'a different map')
+
+    def _getVisualizeDict(self):
+        self.protocol._createFilenameTemplates()
+        return {'doShowOriginalVolumeSlices': self._showOriginalVolumeSlices,
+                'doShowVolumeSlices': self._showVolumeSlices,
+                'doShowVolumeColorSlices': self._showVolumeColorSlices,
+                'doShowOneColorslice': self._showOneColorslice,
+                'doShowResHistogram': self._plotHistogram,
+                'doShowChimera': self._showChimera,
+                }
+
+    def _showVolumeSlices(self, param=None):
+        cm = DataView(self.protocol.resolution_Volume.getFileName())
+
+        return [cm]
+
+    def _showOriginalVolumeSlices(self, param=None):
+        if self.protocol.useHalfVolumes.get():
+            if self.protocol.hasHalfVolumesFile.get():
+                fn1, fn2 = self.protocol.associatedHalves.get().getHalfMaps().split(',')
             else:
-                # Create emtpy image as average
-                image.read(firstImage.getLocation()) # just to take the right dimensions and datatype
-                image.initConstant(0.)
-                
-            image.write(averageName)
-            md.setValue(emlib.MDL_IMAGE, imageName, objId)
-            md.setValue(emlib.MDL_IMAGE2, averageName, objId)
-            
-            counter += 1
-            
-        md.write(mdClasses, emlib.MD_APPEND)
-        
-    def _preprocessClass(self, classItem, classRow):
-        classItem.average = Particle()
-        classItem.average.setLocation(xmippToLocation(classRow.getValue(emlib.MDL_IMAGE2)))
-        
-    def createOutputStep(self):
-        """ Store the kenserdom object 
-        as result of the protocol.
-        """
-        imgSet = self.inputParticles.get()
-        classes2DSet = self._createSetOfClasses2D(imgSet)
-        readSetOfClasses2D(classes2DSet, self._params['kclasses'], 
-                           preprocessClass=self._preprocessClass)
-        self._defineOutputs(outputClasses=classes2DSet)
-        self._defineSourceRelation(self.inputParticles, classes2DSet)
-    
-    #--------------------------- INFO functions ----------------------------------------------------
-    def _validate(self):
-        errors = []
-        if self.SomReg0 < self.SomReg1:
-            errors.append("Regularization must decrease over iterations:")
-            errors.append("    Initial regularization must be larger than final")
-        if self.useMask:
-            mask = self.Mask.get()
-            if mask is None:
-                errors.append("You have selected to use a mask. Select one.")
-        return errors
-    
-    def _summary(self):
-        return self._methods()
+                fn1 = self.protocol.halfMap1.get().getFileName()
+                fn2 = self.protocol.halfMap2.get().getFileName()
+            cm = DataView(fn1)
+            cm2 = DataView(fn2)
+            return [cm, cm2]
+        else:
+            cm = DataView(self.protocol.fullMap.get().getFileName())
+            return [cm]
 
-    def _methods(self):
-        messages = []  
-        if not hasattr(self, 'outputClasses'):
-            messages.append("Output classification not ready yet.")
-        elif self.inputParticles.get() is None:
-            messages.append('Input not selected yet.')
-        else:    
-            messages.append("*Kendersom classification*")
-            messages.append('%s particles from %s were classified to obtain %s classes %s.'
-                            % (self.inputParticles.get().getSize(), self.getObjectTag('inputParticles'), self.outputClasses.getSize(), self.getObjectTag('outputClasses')))
-            if self.useMask:
-                messages.append('Mask %s was used in classification.' % self.getObjectTag('Mask'))
-        return messages
+    def _showVolumeColorSlices(self, param=None):
+        if (exists(self.protocol._getExtraPath("mgresolution.mrc"))):
+            imageFile = self.protocol._getExtraPath("mgresolution.mrc")
+        else:
+            imageFile = self.protocol._getExtraPath(OUTPUT_RESOLUTION_FILE)
+        if not os.path.exists(imageFile):
+            imageFile = replaceExt(imageFile, 'mrc')
+        imgData, min_Res, max_Res, voldim = self.getImgData(imageFile)
+
+        xplotter = XmippPlotter(x=2, y=2, mainTitle="Local Resolution Slices "
+                                                    "along %s-axis."
+                                                    % self._getAxis())
+        # The slices to be shown are close to the center. Volume size is divided in
+        # 9 segments, the fouth central ones are selected i.e. 3,4,5,6
+        for i in range(3, 7):
+            sliceNumber = self.getSlice(i, imgData)
+            a = xplotter.createSubPlot("Slice %s" % (sliceNumber + 1), '', '')
+            matrix = self.getSliceImage(imgData, sliceNumber, self._getAxis())
+            plot = xplotter.plotMatrix(a, matrix, self.lowest.get(), self.highest.get(),
+                                       cmap=self.getColorMap(),
+                                       interpolation="nearest")
+        xplotter.getColorBar(plot)
+        return [xplotter]
+
+    def _showOneColorslice(self, param=None):
+        if (exists(self.protocol._getExtraPath("mgresolution.mrc"))):
+            imageFile = self.protocol._getExtraPath("mgresolution.mrc")
+        else:
+            imageFile = self.protocol._getExtraPath(OUTPUT_RESOLUTION_FILE)
+        if not os.path.exists(imageFile):
+            imageFile = replaceExt(imageFile, 'mrc')
+        imgData, min_Res, max_Res, voldim = self.getImgData(imageFile)
+
+        xplotter = XmippPlotter(x=1, y=1, mainTitle="Local Resolution Slices "
+                                                    "along %s-axis."
+                                                    % self._getAxis())
+        sliceNumber = self.sliceNumber.get()
+        if sliceNumber < 0:
+            sliceNumber = int(voldim[0] / 2)
+        else:
+            sliceNumber -= 1
+        # sliceNumber has no sense to start in zero
+        a = xplotter.createSubPlot("Slice %s" % (sliceNumber + 1), '', '')
+        matrix = self.getSliceImage(imgData, sliceNumber, self._getAxis())
+        plot = xplotter.plotMatrix(a, matrix, self.lowest.get(), self.highest.get(),
+                                   cmap=self.getColorMap(),
+                                   interpolation="nearest")
+        xplotter.getColorBar(plot)
+        return [xplotter]
+
+    def _plotHistogram(self, param=None):
+        md = MetaData()
+        md.read(self.protocol._getExtraPath(FN_METADATA_HISTOGRAM))
+        x_axis = []
+        y_axis = []
+
+        for idx in md:
+            x_axis_ = md.getValue(MDL_X, idx)
+            y_axis_ = md.getValue(MDL_COUNT, idx)
+
+            x_axis.append(x_axis_)
+            y_axis.append(y_axis_)
+
+        _plotter = EmPlotter()
+        _plotter.createSubPlot("Resolutions Histogram",
+                               "Resolution (A)", "# of Counts")
+        if len(x_axis) == 1:
+            barwidth = 0.1
+            _plotter.plotDataBar(x_axis, y_axis, barwidth)
+        else:
+            barwidth = (x_axis[-1] - x_axis[0]) / len(x_axis)
+            _plotter.plotDataBar(x_axis[:-2], y_axis[:-2], barwidth)
 
+        return [_plotter]
 
-class XmippProtKerdensom(KendersomBaseClassify):
-    """
-    Classifies a set of images using  Kohonen's Self-Organizing Feature Maps (SOM) 
-    and Fuzzy c-means clustering technique (FCM) .
-    
-    The kerdenSOM algorithm anneals from an initial high regularization factor
-    to a final lower one, in a user-defined number of steps.
-    
-    KerdenSOM is an excellent tool for classification, especially when
-    using a large number of data and classes and when the transition between
-    the classes is almost continuous, with no clear separation between them.
-    
-    The input images must be previously aligned.
-    """
-    _label = 'kerdensom'
-    
-    def __init__(self, **args):
-        KendersomBaseClassify.__init__(self, **args)
-    
-    #--------------------------- DEFINE param functions --------------------------------------------
-    def _addParams(self, form):
-        pass
-    
-    #--------------------------- INSERT steps functions --------------------------------------------
-    def _insertProccesStep(self):
-        self._insertImgToVectorStep()
-        self._insertKerdensomStep()
-        self._insertVectorToImgStep()
-    
-    def _insertImgToVectorStep(self):
-        """ Insert runJob for convert into a vector Md """
-        args = ' -i %(imgsFn)s -o %(vectors)s '
-        if self.useMask:
-            args += ' --mask binary_file %(mask)s'
-        
-        self._insertRunJobStep("xmipp_image_vectorize", args % self._params)
-   
-    def _insertVectorToImgStep(self):
-        args = ' -i %(kvectors)s -o %(classes)s' 
-        if self.useMask:
-            args += ' --mask binary_file %(mask)s'
-        self._insertRunJobStep("xmipp_image_vectorize", args % self._params)
-#        deleteFiles([self._getExtraPath("kerdensom_vectors.xmd"),self._getExtraPath("kerdensom_vectors.vec")], True)
-    
-    #--------------------------- INFO functions ----------------------------------------------------
-    def _validate(self):
-        return KendersomBaseClassify._validate(self)
-    
-    def _summary(self):
-        return KendersomBaseClassify._summary(self)
-    
-    def _methods(self):
-        return KendersomBaseClassify._methods(self)
-    
-    def _citations(self):
-        return ['PascualMontano2001', 'PascualMontano2002']
+    def _getAxis(self):
+        return self.getEnumText('sliceAxis')
+
+    def _showChimera(self, param=None):
+
+        if (exists(self.protocol._getExtraPath("MG_Chimera_resolution.mrc"))):
+            fnResVol = self.protocol._getExtraPath("MG_Chimera_resolution.mrc")
+        else:
+            fnResVol = self.protocol._getExtraPath(OUTPUT_RESOLUTION_FILE_CHIMERA)
+
+        if self.sharpenedMap.get():
+            fnOrigMap = self.sharpenedMap.get().getFileName()
+            sampRate = self.sharpenedMap.get().getSamplingRate()
+        else:
+            if self.protocol.useHalfVolumes.get():
+                if self.protocol.hasHalfVolumesFile.get():
+                    vol = self.protocol.associatedHalves.get().getHalfMaps()
+                    fnOrigMap, _unused = vol.split(',')
+                    sampRate = self.protocol.associatedHalves.get().getSamplingRate()
+                else:
+                    vol = self.protocol.halfMap1.get()
+                    fnOrigMap = vol.getFileName()
+                    sampRate = vol.getSamplingRate()
+            else:
+                vol = self.protocol.fullMap.get()
+                fnOrigMap = vol.getFileName()
+                sampRate = vol.getSamplingRate()
+
+        cmdFile = self.protocol._getExtraPath('chimera_resolution_map.py')
+        self.createChimeraScript(cmdFile, fnResVol, fnOrigMap, sampRate,
+                                 numColors=self.intervals.get(),
+                                 lowResLimit=self.highest.get(),
+                                 highResLimit=self.lowest.get())
+        view = ChimeraView(cmdFile)
+        return [view]
+
+    def getColorMap(self):
+        cmap = cm.get_cmap(self.colorMap.get())
+        if cmap is None:
+            cmap = cm.jet
+        return cmap
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_local_ctf.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_local_ctf.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                       expertLevel=LEVEL_ADVANCED)
         form.addParam('maxGrayScaleChange', FloatParam, label="Maximum gray scale change", default=1,
                       expertLevel=LEVEL_ADVANCED, help="The reprojection is modified as a*P+b, a is restricted to the "
                                                        "interval [1-maxGrayScale,1+maxGrayScale]")
         form.addParam('maxGrayShiftChange', FloatParam, label="Maximum gray shift change", default=1,
                       expertLevel=LEVEL_ADVANCED, help="The reprojection is modified as a*P+b, b is restricted to the "
                                                        "interval [-maxGrayShift,maxGrayShift]")
-        form.addParam('sameDefocus', BooleanParam, label="Force defocusV to be equal than defocusU", default=True,
+        form.addParam('sameDefocus', BooleanParam, label="Force defocusV to be equal than defocusU", default=False,
                       expertLevel=LEVEL_ADVANCED,
                       help="As the CTF usually suffers from astigmatism (it is not spherical but ellipsoidal), the "
                            "defocus vary if computed in X or Y direction, being defocus U value the defocus in X "
                            "direction and defocus V value the defocus in Y direction.")
         form.addParallelSection(threads=0, mpi=8)
     
     # --------------------------- INSERT steps functions --------------------------------------------
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_metaprotocol_create_subset.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_metaprotocol_create_subset.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_metaprotocol_golden_highres.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_metaprotocol_golden_highres.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_ml2d.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_ml2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_movie_gain.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_movie_gain.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,45 +37,54 @@
                                         BooleanParam, LEVEL_ADVANCED)
 from pyworkflow.utils.properties import Message
 from pyworkflow.utils.path import moveFile
 import pyworkflow.protocol.constants as cons
 
 from pwem.objects import SetOfMovies, Movie, SetOfImages, Image
 from pwem.protocols import EMProtocol, ProtProcessMovies
+from pyworkflow import BETA, UPDATED, NEW, PROD
 
 from pwem import emlib
 import xmipp3.utils as xmutils
 
+OUTPUT_ESTIMATED_GAINS = 'estimatedGains'
+OUTPUT_ORIENTED_GAINS = 'orientedGain'
+OUTPUT_RESIDUAL_GAINS = 'residualGains'
+OUTPUT_MOVIES = 'outputMovies'
 
 class XmippProtMovieGain(ProtProcessMovies):
     """ Estimate the gain image of a camera, directly analyzing one of its movies.
     It can correct the orientation of an external gain image (by comparing it with the estimated).
     Finally, it estimates the residual gain (the gain of the movie after correcting with a gain).
     The gain used in the correction will be preferably the external gain, but can also be the estimated
     gain if the first is not found.
     The same criteria is used for assigning the gain to the output movies (external corrected > external > estimated)
     """
     _label = 'movie gain'
+    _devStatus = UPDATED
     _lastUpdateVersion = VERSION_1_1
-
+    _stepsCheckSecs = 60
     estimatedDatabase = 'estGains.sqlite'
     residualDatabase = 'resGains.sqlite'
+    _possibleOutputs = {OUTPUT_ESTIMATED_GAINS: SetOfImages,
+                        OUTPUT_ORIENTED_GAINS: SetOfImages,
+                        OUTPUT_RESIDUAL_GAINS: SetOfImages,
+                        OUTPUT_MOVIES: SetOfMovies}
 
     def __init__(self, **args):
         EMProtocol.__init__(self, **args)
         self.stepsExecutionMode = STEPS_PARALLEL
 
     # -------------------------- DEFINE param functions ----------------------
     def _defineParams(self, form):
         form.addSection(label=Message.LABEL_INPUT)
 
-        form.addParam('inputMovies', PointerParam, pointerClass='SetOfMovies, '
-                                                                'Movie',
+        form.addParam('inputMovies', PointerParam, pointerClass='SetOfMovies',
                       label=Message.LABEL_INPUT_MOVS,
-                      help='Select one or several movies. A gain image will '
+                      help='Select several movies. A gain image will '
                            'be calculated for each one of them.')
         form.addParam('estimateGain', BooleanParam, default=True,
                       label="Estimate movies gain",
                       help='Estimate the gain from a set of movies using the algorith from xmipp')
         form.addParam('estimateOrientation', BooleanParam, default=True,
                       label="Estimate external gain orientation",
                       help='Estimate the relative orientation between the estimated '
@@ -97,70 +106,63 @@
                       label="Frame step", expertLevel=LEVEL_ADVANCED,
                       help='By default, every 5th frame is used to compute '
                            'the movie gain. If you set this parameter to '
                            '2, 3, ..., then only every 2nd, 3rd, ... '
                            'frame will be used.')
         form.addParam('movieStep', IntParam, default=250,
                       label="Movie step", expertLevel=LEVEL_ADVANCED,
-                      help='By default, every movie (movieStep=1) is used to '
+                      help='By default, every 250 movies (movieStep=250) is used to '
                            'compute the movie gain. If you set '
-                           'this parameter to 2, 3, ..., then only every 2nd, '
+                           'this parameter to 2, 3, ..., then every 2nd, '
                            '3rd, ... movie will be used.')
 
         # It should be in parallel (>2) in order to be able of attaching
         #  new movies to the output while estimating residual gain
         form.addParallelSection(threads=4, mpi=1)
 
     # -------------------------- STEPS functions ------------------------------
     def createOutputStep(self):
         if self.estimateGain.get():
             estGainsSet = self._loadOutputSet(SetOfImages, self.estimatedDatabase)
-            self._updateOutputSet('estimatedGains', estGainsSet, Set.STREAM_CLOSED)
+            self._updateOutputSet(OUTPUT_ESTIMATED_GAINS, estGainsSet, Set.STREAM_CLOSED)
 
         if self.estimateResidualGain.get():
             resGainsSet = self._loadOutputSet(SetOfImages, self.residualDatabase)
-            self._updateOutputSet('residualGains', resGainsSet, Set.STREAM_CLOSED)
+            self._updateOutputSet(OUTPUT_RESIDUAL_GAINS, resGainsSet, Set.STREAM_CLOSED)
 
     def _insertNewMoviesSteps(self, insertedDict, inputMovies):
         """ Insert steps to process new movies (from streaming)
         Params:
             insertedDict: contains already processed movies
             inputMovies: input movies set to be check
         """
         deps = []
-        if isinstance(self.inputMovies.get(), Movie):
-            movie = self.inputMovies.get()
+        if len(insertedDict) == 0 and self.estimateOrientation.get():
+            # Adding a first step to orientate the input gain
+            firstMovie = inputMovies.getFirstItem()
+            movieDict = firstMovie.getObjDict(includeBasic=True)
+            orientStepId = self._insertFunctionStep('estimateOrientationStep',
+                                                    movieDict,
+                                                    prerequisites=self.convertCIStep)
+            # adding orientStep as dependency for all other steps
+            self.convertCIStep.append(orientStepId)
+
+        if len(insertedDict) == 0 and self.normalizeGain.get():
+            # Adding a step to normalize the gain (only one)
+            normStepId = self._insertFunctionStep('normalizeGainStep',
+                                                  prerequisites=self.convertCIStep)
+            # adding normStep as dependency for all other steps
+            self.convertCIStep.append(normStepId)
+        self.estimatedIds, self.estimatedResIds = [], []
+        # For each movie insert the step to process it
+        for movie in inputMovies:
             if movie.getObjId() not in insertedDict:
                 stepId = self._insertMovieStep(movie)
                 deps.append(stepId)
                 insertedDict[movie.getObjId()] = stepId
-        else:
-            if len(insertedDict) == 0 and self.estimateOrientation.get():
-                # Adding a first step to orientate the input gain
-                firstMovie = self.inputMovies.get().getFirstItem()
-                movieDict = firstMovie.getObjDict(includeBasic=True)
-                orientStepId = self._insertFunctionStep('estimateOrientationStep',
-                                                        movieDict,
-                                                        prerequisites=self.convertCIStep)
-                # adding orientStep as dependency for all other steps
-                self.convertCIStep.append(orientStepId)
-
-            if len(insertedDict) == 0 and self.normalizeGain.get():
-                # Adding a step to normalize the gain (only one)
-                normStepId = self._insertFunctionStep('normalizeGainStep',
-                                                      prerequisites=self.convertCIStep)
-                # adding normStep as dependency for all other steps
-                self.convertCIStep.append(normStepId)
-            self.estimatedIds, self.estimatedResIds = [], []
-            # For each movie insert the step to process it
-            for movie in self.inputMovies.get():
-                if movie.getObjId() not in insertedDict:
-                    stepId = self._insertMovieStep(movie)
-                    deps.append(stepId)
-                    insertedDict[movie.getObjId()] = stepId
         return deps
 
     def estimateGainFun(self, movie, noSigma=False, residual=False):
         movieId = movie.getObjId()
         movieFn = movie.getFileName()
 
         # Check which estimated gain matches with the experimental gain
@@ -184,15 +186,15 @@
 
         estGain = xmutils.readImage(estGainFn)
         expGain = xmutils.readImage(expGainFn)
         self.match_orientation(expGain, estGain)
 
         orientedSet = self._loadOutputSet(SetOfImages, 'orientedGain.sqlite')
         orientedSet = self.updateGainsOutput(movie, orientedSet, self.getOrientedGainPath())
-        self._updateOutputSet('orientedGain', orientedSet, Set.STREAM_CLOSED)
+        self._updateOutputSet(OUTPUT_ORIENTED_GAINS, orientedSet, Set.STREAM_CLOSED)
 
     def normalizeGainStep(self):
         gainFn = self.getFinalGainPath()
 
         oriGain = emlib.Image()
         oriGain.read(gainFn)
         oriArray = oriGain.getData()
@@ -210,15 +212,15 @@
         inputGain = self.getInputGain()
 
         if self.estimateGain.get() and not movieId in self.estimatedIds:
                 self.estimatedIds.append(movieId)
                 self.estimateGainFun(movie)
 
         if self.estimateResidualGain.get() and not movieId in self.estimatedResIds:
-            print('\nEstimating residual gain')
+            self.info('\nEstimating residual gain')
             self.estimatedResIds.append(movieId)
             self.estimateGainFun(movie, residual=True)
 
         # If the gain hasn't been oriented or normalized, we still need orientedGain
         if not os.path.exists(self.getOrientedGainPath()):
             # No previous gain: orientedGain is the estimated
             if not inputGain is None:
@@ -264,106 +266,83 @@
             outputSet = SetClass(filename=setFile)
             outputSet.loadAllProperties()
             outputSet.enableAppend()
         else:
             outputSet = SetClass(filename=setFile)
             outputSet.setStreamState(outputSet.STREAM_OPEN)
 
-            if isinstance(self.inputMovies.get(), SetOfMovies) or isinstance(self.inputMovies.get(), Movie):
-                inputMovies = self.inputMovies.get()
-                outputSet.copyInfo(inputMovies)
+            inputMovies = self.inputMovies.get()
+            outputSet.copyInfo(inputMovies)
 
-                if fixGain:
-                    outputSet.setGain(self.getFinalGainPath(tifFlipped=True))
+            if fixGain:
+                outputSet.setGain(self.getFinalGainPath(tifFlipped=True))
 
         return outputSet
 
     def _checkNewInput(self):
-        if isinstance(self.inputMovies.get(), SetOfMovies):
-            ProtProcessMovies._checkNewInput(self)
+        ProtProcessMovies._checkNewInput(self)
 
     def _checkNewOutput(self):
         if getattr(self, 'finished', False):
             return
-        if isinstance(self.inputMovies.get(), Movie):
-            movie = self.inputMovies.get()
-            movieId = movie.getObjId()
-            streamMode = Set.STREAM_CLOSED
-            saveMovie = self.getAttributeValue('doSaveMovie', False)
-            moviesSet = self._loadOutputSet(SetOfMovies, 'movies.sqlite', fixGain=True)
-            moviesSet.append(movie)
-            self._updateOutputSet('outputMovies', moviesSet, streamMode)
 
+        # Load previously done items (from text file)
+        doneList = self._readDoneList()
+        # Check for newly done items
+        newDone = [m.clone() for m in self.listOfMovies
+                   if int(m.getObjId()) not in doneList and
+                   self._isMovieDone(m)]
+
+        allDone = len(doneList) + len(newDone)
+        # We have finished when there is not more input movies
+        # (stream closed) and the number of processed movies is
+        # equal to the number of inputs
+        self.finished = self.streamClosed and \
+                        allDone == len(self.listOfMovies)
+        streamMode = Set.STREAM_CLOSED if self.finished \
+            else Set.STREAM_OPEN
+
+        if newDone:
+            self._writeDoneList(newDone)
+        elif not self.finished:
+            # If we are not finished and no new output have been produced
+            # it does not make sense to proceed and updated the outputs
+            # so we exit from the function here
+            return
+
+        if any([self.doGainProcess(i.getObjId()) for i in newDone]):
+            # update outputGains if any residualGain is processed in newDone
             if self.estimateGain.get():
                 estGainsSet = self._loadOutputSet(SetOfImages, self.estimatedDatabase)
-                estGainsSet = self.updateGainsOutput(movie, estGainsSet, self.getEstimatedGainPath(movieId))
-                self._updateOutputSet('estimatedGains', estGainsSet, streamMode)
             if self.estimateResidualGain.get():
                 resGainsSet = self._loadOutputSet(SetOfImages, self.residualDatabase)
-                resGainsSet = self.updateGainsOutput(movie, resGainsSet, self.getResidualGainPath(movieId))
-                self._updateOutputSet('residualGains', resGainsSet, streamMode)
 
-            outputStep = self._getFirstJoinStep()
-            outputStep.setStatus(cons.STATUS_NEW)
-            self.finished = True
-        else:
-            # Load previously done items (from text file)
-            doneList = self._readDoneList()
-            # Check for newly done items
-            newDone = [m.clone() for m in self.listOfMovies
-                       if int(m.getObjId()) not in doneList and
-                       self._isMovieDone(m)]
-
-            allDone = len(doneList) + len(newDone)
-            # We have finished when there is not more input movies
-            # (stream closed) and the number of processed movies is
-            # equal to the number of inputs
-            self.finished = self.streamClosed and \
-                            allDone == len(self.listOfMovies)
-            streamMode = Set.STREAM_CLOSED if self.finished \
-                else Set.STREAM_OPEN
-
-            if newDone:
-                self._writeDoneList(newDone)
-            elif not self.finished:
-                # If we are not finished and no new output have been produced
-                # it does not make sense to proceed and updated the outputs
-                # so we exit from the function here
-                return
-
-            if any([self.doGainProcess(i.getObjId()) for i in newDone]):
-                # update outputGains if any residualGain is processed in newDone
+            for movie in newDone:
+                movieId = movie.getObjId()
+                if not self.doGainProcess(movieId):
+                    continue
                 if self.estimateGain.get():
-                    estGainsSet = self._loadOutputSet(SetOfImages, self.estimatedDatabase)
+                    estGainsSet = self.updateGainsOutput(movie, estGainsSet, self.getEstimatedGainPath(movieId))
                 if self.estimateResidualGain.get():
-                    resGainsSet = self._loadOutputSet(SetOfImages, self.residualDatabase)
+                    resGainsSet = self.updateGainsOutput(movie, resGainsSet, self.getResidualGainPath(movieId))
 
-                for movie in newDone:
-                    movieId = movie.getObjId()
-                    if not self.doGainProcess(movieId):
-                        continue
-                    if self.estimateGain.get():
-                        estGainsSet = self.updateGainsOutput(movie, estGainsSet, self.getEstimatedGainPath(movieId))
-                    if self.estimateResidualGain.get():
-                        resGainsSet = self.updateGainsOutput(movie, resGainsSet, self.getResidualGainPath(movieId))
-
-                if self.estimateGain.get():
-                    self._updateOutputSet('estimatedGains', estGainsSet, streamMode)
-                if self.estimateResidualGain.get():
-                    self._updateOutputSet('residualGains', resGainsSet, streamMode)
+            if self.estimateGain.get():
+                self._updateOutputSet(OUTPUT_ESTIMATED_GAINS, estGainsSet, streamMode)
+            if self.estimateResidualGain.get():
+                self._updateOutputSet(OUTPUT_RESIDUAL_GAINS, resGainsSet, streamMode)
 
-            moviesSet = self._loadOutputSet(SetOfMovies, 'movies.sqlite', fixGain=True)
-            for movie in newDone:
-                moviesSet.append(movie)
-            self._updateOutputSet('outputMovies', moviesSet, streamMode)
+        moviesSet = self._loadOutputSet(SetOfMovies, 'movies.sqlite', fixGain=True)
+        for movie in newDone:
+            moviesSet.append(movie)
+        self._updateOutputSet(OUTPUT_MOVIES, moviesSet, streamMode)
 
-            if self.finished:  # Unlock createOutputStep if finished all jobs
-                outputStep = self._getFirstJoinStep()
-                if outputStep and outputStep.isWaiting():
-                    outputStep.setStatus(cons.STATUS_NEW)
+        if self.finished:  # Unlock createOutputStep if finished all jobs
+            outputStep = self._getFirstJoinStep()
+            if outputStep and outputStep.isWaiting():
+                outputStep.setStatus(cons.STATUS_NEW)
 
     def updateGainsOutput(self, movie, imgSet, imageFile):
         movieId = movie.getObjId()
         imgOut = Image()
         imgOut.setObjId(movieId)
         imgOut.setSamplingRate(movie.getSamplingRate())
         imgOut.setFileName(imageFile)
@@ -391,15 +370,15 @@
         outputSet.close()
 
     def match_orientation(self, exp_gain, est_gain):
         ''' Calculates the correct orientation of the experimental gain image
             with respect to the estimated
             Input: 2 Xmipp Images
         '''
-        print('\nEstimating best orientation')
+        self.info('\nEstimating best orientation')
         sys.stdout.flush()
         best_cor = 0
         #Building conjugate of FT of estimated gain for correlations
         est_gain_array = est_gain.getData()
         est_gain_array = xmutils.normalize_array(est_gain_array)
         est_gain_array_FT_conj = np.conj(np.fft.fft2(est_gain_array))
 
@@ -426,28 +405,34 @@
                 maxLoc = np.where(correlationFunction == maxVal)
 
                 if abs(minVal) > abs(best_cor):
                     corLoc = translation_correction(minLoc,est_gain_array.shape)
                     best_cor = minVal
                     best_transf = (angle,imir)
                     best_R = R
-                    T = np.asarray([[1, 0, np.asscalar(corLoc[1])], [0, 1, np.asscalar(corLoc[0])], [0, 0, 1]])
+                    # T = np.asarray([[1, 0, np.asscalar(corLoc[1])], [0, 1, np.asscalar(corLoc[0])], [0, 0, 1]])
+                    T = np.asarray([[1, 0, corLoc[1].item()],
+                                    [0, 1, corLoc[0].item()],
+                                    [0, 0, 1]])
                 if abs(maxVal) > abs(best_cor):
                     corLoc = translation_correction(maxLoc, est_gain_array.shape)
                     best_cor = maxVal
                     best_transf = (angle, imir)
                     best_R = R
-                    T = np.asarray([[1, 0, np.asscalar(corLoc[1])], [0, 1, np.asscalar(corLoc[0])], [0, 0, 1]])
+                    # T = np.asarray([[1, 0, np.asscalar(corLoc[1])], [0, 1, np.asscalar(corLoc[0])], [0, 0, 1]])
+                    T = np.asarray([[1, 0, corLoc[1].item()], 
+                                    [0, 1, corLoc[0].item()],
+                                    [0, 0, 1]])
 
         # Multiply by inverse of translation matrix
         best_M = np.matmul(np.linalg.inv(T), best_R)
         best_gain_array = xmutils.applyTransform(np.asarray(exp_gain.getData(), dtype=np.float64), best_M, est_gain_array.shape)
 
-        print('Best correlation: ', best_cor)
-        print('Rotation angle: {}\nHorizontal mirror: {}'.format(best_transf[0],best_transf[1]==1))
+        self.info('Best correlation: %f' %best_cor)
+        self.info('Rotation angle: {}\nHorizontal mirror: {}'.format(best_transf[0],best_transf[1]==1))
 
         inv_best_gain_array = invert_array(best_gain_array)
         if best_cor > 0:
             xmutils.writeImageFromArray(best_gain_array, self.getOrientedGainPath())
             #xmutils.writeImageFromArray(inv_best_gain_array, self.getBestCorrectionPath())
         else:
             xmutils.writeImageFromArray(inv_best_gain_array, self.getOrientedGainPath())
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_movie_max_shift.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_movie_max_shift.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_movie_opticalflow.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_movie_opticalflow.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_movie_split_frames.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_movie_split_frames.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_multiple_fscs.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_multiple_fscs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_multireference_alignability.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_multireference_alignability.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_normalize_strain.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_normalize_strain.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_particle_boxsize.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_consensus_classes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # **************************************************************************
 # *
-# * Authors:     Jose Luis Vilas (jlvilas@cnb.csic.es)
+# * Authors:     J.M. De la Rosa Trevin (jmdelarosa@cnb.csic.es)
+# *              Oier Lauzirika Zarrabeitia (oierlauzi@bizkaia.eu)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 2 of the License, or
 # * (at your option) any later version.
@@ -20,114 +21,125 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-import random
+"""
+This module implement the wrappers around
+visualization program.
+"""
+from pyworkflow.viewer import (ProtocolViewer, DESKTOP_TKINTER, WEB_DJANGO)
+from pyworkflow.protocol.params import Form, Line, LabelParam, IntParam
+from pyworkflow.protocol.params import GE
+
+from pwem.viewers.showj import *
+from pwem.viewers import TableView, ObjectView
+from pwem.objects import SetOfClasses
+
+from xmipp3.protocols.protocol_consensus_classes import XmippProtConsensusClasses
+
+import numpy as np
+import matplotlib.pyplot as plt
+import scipy.spatial
+import scipy.cluster
 
-from pyworkflow import VERSION_2_0
-from pyworkflow.object import Integer
-from pyworkflow.protocol.params import PointerParam, IntParam, LEVEL_ADVANCED
-
-from pwem.protocols import ProtMicrographs
-
-from xmipp3.convert import writeSetOfMicrographs
-import xmipp3
-
-
-class XmippProtParticleBoxsize(ProtMicrographs, xmipp3.XmippProtocol):
-    """ Given a set of micrographs, the protocol estimate the particle box size.
+class XmippConsensusClassesViewer(ProtocolViewer):
+    """ Visualization of results from the consensus classes 3D protocol
     """
-    _label = 'particle boxsize'
-    _lastUpdateVersion = VERSION_2_0
-    _conda_env = 'xmipp_DLTK_v0.3'
-
-    def __init__(self, **args):
-        ProtMicrographs.__init__(self, **args)
-        self.particleBoxsize = None
-
-    # --------------------------- DEFINE param functions ----------------------
-    def _defineParams(self, form):
-        form.addSection(label='Input')
-        form.addParam('inputMicrographs', PointerParam, important=True,
-                      label="Input Micrographs", pointerClass='SetOfMicrographs',
-                      help='Select a set of micrographs for determining the '
-                           'particle boxsize.')
-
-        form.addParam('nMicsToAnalize', IntParam,
-                      label="Number of mics to use for estimation",
-                      default=10, expertLevel=LEVEL_ADVANCED,
-                      help='The boxsize estimation is the median of the boxsize '
-                           'estimations on different micrographs.'
-                           'This number selects a random subset of input '
-                           'micrographs to perform analysis. Use -1 to '
-                           'consider all micrographs')
-
-    # --------------------------- INSERT steps functions -----------------------
-    def _insertAllSteps(self):
-        # Convert input into xmipp Metadata format
-        self._insertFunctionStep('convertInputStep')
-        self._insertFunctionStep('boxsizeStep')
-        self._insertFunctionStep('createOutputStep')
-
-    def convertInputStep(self):
-        writeSetOfMicrographs(self.inputMicrographs.get(),
-                              self._getExtraPath('input_micrographs.xmd'))
-
-    def boxsizeStep(self):
-        particleBoxSizeFn = self._getExtraPath('particle_boxsize.xmd')
-        imgSize = 400  # This should match the img_size used for training weights? Add as metada?
-        weights = self.getModel('boxsize', 'weights.hdf5')
-
-        params = ' --img_size %d' % imgSize
-        params += ' --weights %s' % weights
-        params += ' --output %s' % particleBoxSizeFn
-
-        fileNames = [mic.getFileName().encode() + b'\n' for mic in self.inputMicrographs.get()]
-
-        nMicsToAnalize = self.nMicsToAnalize.get()
-        if nMicsToAnalize != -1:
-            random.shuffle(fileNames)
-            fileNames= fileNames[:min(len(fileNames), nMicsToAnalize)]
-        # TODO: output name is hardcoded
-        micNamesPath = self._getTmpPath('mic_names.csv')
-        with open(micNamesPath, 'wb') as csvFile:
-            csvFile.writelines(fileNames)
-        params += ' --micrographs %s' % micNamesPath
-        self.runJob('xmipp_particle_boxsize', params, env=self.getCondaEnv())
-
-        with open(particleBoxSizeFn, 'r') as fp:
-            self.particleBoxsize = int(fp.read().rstrip('\n'))
-
-        print("\n > Estimated box size: %d \n" % self.particleBoxsize)
-
-    def createOutputStep(self):
-        """ The output is just an Integer. Other protocols can use it in those
-            IntParam if it has set allowsPointer=True
-        """
-        micSet = self.inputMicrographs.get()
-        boxSize = Integer(self.particleBoxsize)
-        self._defineOutputs(boxsize=boxSize)
-        self._defineSourceRelation(micSet, boxSize)
-
-    # --------------------------- INFO functions ------------------------------
-    def _methods(self):
-        messages = []
-        if hasattr(self, 'boxsize'):
-            messages.append('Estimated box size: %s pixels' % self.boxsize)
-        return messages
-
-    def _summary(self):
-        messages = []
-        if hasattr(self, 'boxsize'):
-            messages.append('Estimated box size: %s pixels' % self.boxsize)
-            messages.append("Open 'Analyze results' to see it in context. "
-                            "(The displayed coordinate is just to show the size)")
-        return messages
-
-    def _citations(self):
-        return ['']
-
-    def _validate(self):
-        return self.validateDLtoolkit(model=('boxsize', 'weights.hdf5'))
+    _label = 'viewer consensus classes'
+    _targets = [XmippProtConsensusClasses]
+    _environments = [DESKTOP_TKINTER, WEB_DJANGO]
+
+    def __init__(self, **kwargs):
+        ProtocolViewer.__init__(self, **kwargs)
+
+    def _defineParams(self, form: Form):
+        form.addSection(label='Classes')
+        form.addParam('visualizeClasses', IntParam,
+                      validators=[GE(1)], default=1,
+                      label='Classes' )
+
+        form.addSection(label='Graphs')
+        form.addParam('visualizeDendrogram', LabelParam,
+                       label='Dendrogram' )
+        form.addParam('visualizeCostFunction', LabelParam,
+                       label='Cost function' )
+
+
+    def _getVisualizeDict(self):
+        return {
+            'visualizeClasses': self._visualizeClasses,
+            'visualizeDendrogram': self._visualizeDendrogram,
+            'visualizeCostFunction': self._visualizeCostFunction,
+        }
+    
+    # --------------------------- UTILS functions ------------------------------
+    def _getLinkageMatrix(self) -> np.ndarray:
+        return self.protocol._readLinkageMatrix()
+    
+    def _getElbows(self) -> dict:
+        return self.protocol._readElbows()
+    
+    def _getMergedIntersections(self, size) -> SetOfClasses:
+        return self.protocol._obtainMergedIntersections(size)
+    
+    def _visualizeClasses(self, param=None):
+        count = self.visualizeClasses.get()
+        classes = self._getMergedIntersections(count)
+        return self._showSetOfClasses3D(classes)
+        
+    def _visualizeDendrogram(self, param=None):
+        linkage = self._getLinkageMatrix()
+        elbows = self._getElbows()
+        labels = np.arange(1, len(linkage)+2)
+        y = linkage[:,2]
+        
+        fig, ax = plt.subplots()
+        scipy.cluster.hierarchy.dendrogram(linkage, ax=ax, labels=labels)
+        
+        # Plot the elbows
+        for key, value in elbows.items():
+            index = len(y) - value
+            label = key + ': ' + str(value)
+            ax.axhline((y[index] + y[index+1])/2, label=label, color='black', linestyle='--')
+        
+        ax.legend()
+        ax.set_ylabel('cost')
+        ax.set_xlabel('classId')
+        ax.set_title('Dendrogram')
+        
+        return [fig]
+        
+    def _visualizeCostFunction(self, param=None):
+        linkage = self._getLinkageMatrix()
+        elbows = self._getElbows()
+        y = linkage[:,2]
+        x = np.arange(len(y), 0, -1)
+        
+        fig, ax = plt.subplots()
+        ax.plot(x, y)
+        
+        # Plot the elbows
+        for key, value in elbows.items():
+            index = len(x) - value
+            label = key + ': ' + str(value)
+            ax.scatter([x[index]], [y[index]], label=label)
+        
+        ax.legend()
+        ax.set_ylabel('cost')
+        ax.set_xlabel('class count')
+        ax.set_title('Cost function')
+        
+        return [fig]
+    
+    def _showSetOfClasses3D(self, classes):
+        labels = 'enabled id _size _representative._filename _xmipp_classIntersectionSizePValue _xmipp_classIntersectionRelativeSizePValue'
+        labelRender = '_representative._filename'
+        return [ObjectView( self._project, classes.strId(), classes.getFileName(),
+                            viewParams={ORDER: labels,
+                                        VISIBLE: labels,
+                                        RENDER: labelRender,
+                                        SORT_BY: '_size desc',
+                                        MODE: MODE_MD})]
+
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_particle_pick.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_particle_pick.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_particle_pick_automatic.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_particle_pick_automatic.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,24 +226,18 @@
     def getCoordsDir(self):
         return self._getExtraPath()
     
     def getInputMicrographsPointer(self):
         # Get micrographs to pick
         if self.micsToPick == MICS_SAMEASPICKING:
             inputPicking = self.xmippParticlePicking.get()
-            if inputPicking is None:
-                return None
-            else:
-                return inputPicking.inputMicrographs
+            return inputPicking.inputMicrographs if inputPicking else None
         else:
             return self.inputMicrographs
         
     def getInputMicrographs(self):
         """ Return the input micrographs that can be the same of the supervised
         picking or other ones selected by the user. (This can be used to pick
         a new set of micrographs with the same properties than a previous
         trained ones. )
         """ 
-        if self.getInputMicrographsPointer() is not None:
-            return self.getInputMicrographsPointer().get()
-        else:
-            return None
+        return self.getInputMicrographsPointer().get() if self.getInputMicrographsPointer() else None
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_particle_pick_consensus.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_particle_pick_consensus.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,29 +25,36 @@
 # *
 # **************************************************************************
 """
 Consensus picking protocol
 """
 
 import os
-
+import enum
 from math import sqrt
 import numpy as np
 
 from pyworkflow.object import Set, String, Pointer
 import pyworkflow.protocol.params as params
 from pwem.protocols import ProtParticlePicking
 from pyworkflow.protocol.constants import *
 from pwem.objects import SetOfCoordinates, Coordinate
 from pyworkflow.utils import getFiles, removeBaseExt, moveFile
 
 
 PICK_MODE_LARGER = 0
 PICK_MODE_EQUAL = 1
 
+
+class ProtPickingConsensusOutput(enum.Enum):
+    """ Possible outputs for particle picking protocols
+    """
+    consensusCoordinates = SetOfCoordinates
+
+
 class XmippProtConsensusPicking(ProtParticlePicking):
     """
     Protocol to estimate the agreement between different particle picking
     algorithms. The protocol takes several Sets of Coordinates calculated
     by different programs and/or different parameter settings. Let's say:
     we consider N independent pickings. Then, a coordinate is considered
     to be a correct particle if M pickers have selected the same particle
@@ -61,15 +68,16 @@
     If you want to be very flexible, set M=1, in this way it suffices that
     1 picker has selected the coordinate to be considered as a particle. Note
     that in this way, the cleaning of the dataset has to be performed by other
     means (screen particles, 2D and 3D classification, ...).
     """
 
     _label = 'picking consensus'
-    outputName = 'consensusCoordinates'
+    _possibleOutputs = ProtPickingConsensusOutput
+    outputName = ProtPickingConsensusOutput.consensusCoordinates.name
     FN_PREFIX = 'consensusCoords_'
 
     def __init__(self, **args):
         ProtParticlePicking.__init__(self, **args)
         self.stepsExecutionMode = STEPS_SERIAL
 
     def _defineParams(self, form):
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_particle_pick_pairs.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_particle_pick_pairs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_particle_pick_remove_duplicates.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_particle_pick_remove_duplicates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_phantom_create.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_phantom_create.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_pick_noise.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_pick_noise.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_postProcessing_deepPostProcessing.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_postProcessing_deepPostProcessing.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/__init__.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/geometrical_mask.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/geometrical_mask.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_add_noise.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_add_noise.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_create_mask2d.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_create_mask2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_create_mask3d.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_create_mask3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,14 +204,16 @@
         self._insertFunctionStep('postProcessMaskStep')
         self._insertFunctionStep('createOutputStep')
     
     #--------------------------- STEPS functions -------------------------------
     def createMaskFromVolumeStep(self):
         volume = self.inputVolume.get()
         fnVol = getImageLocation(volume)
+        if fnVol.endswith(".mrc"):
+            fnVol += ":mrc"
         Ts = volume.getSamplingRate()
         
         if self.volumeOperation == OPERATION_THRESHOLD:
             self.runJob("xmipp_transform_threshold",
                         "-i %s -o %s --select below %f --substitute binarize"
                         % (fnVol, self.maskFile, self.threshold.get()))
         elif self.volumeOperation == OPERATION_SEGMENT:
@@ -388,11 +390,15 @@
                             % self.getEnumText('morphologicalOperation'))
         if self.doInvert:
             messages.append("We inverted the mask. ")
         if self.doSmooth:
             messages.append("And, we smoothed it (sigma=%f voxels)."
                             % self.sigmaConvolution.get())
         if self.hasAttribute('outputMask'):
-            messages.append('We refer to the output mask as %s.'
-                            % self.outputMask.getNameId())
+            messages.append('We refer to the output mask as %s.'  % self.outputMask.getNameId())
         return messages
     
+    def _validate(self):
+        errors = []
+        if self.source == SOURCE_VOLUME and not self.inputVolume.get():
+            errors.append("You need to select an input volume")
+            return errors
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_crop_resize.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_crop_resize.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,39 +22,43 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+import os
 
 import pyworkflow.protocol.constants as const
+from pyworkflow.object import String
 from pwem.convert.headers import setMRCSamplingRate
 from pyworkflow.protocol.params import (BooleanParam, EnumParam, FloatParam,
                                         IntParam)
-from pwem.objects import Volume
+from pwem.objects import Volume, SetOfParticles, Mask
 
 from .protocol_process import XmippProcessParticles, XmippProcessVolumes
+from pyworkflow import BETA, UPDATED, NEW, PROD
 
 
 class XmippResizeHelper:
     """ Common features to change dimensions of either SetOfParticles,
     Volume or SetOfVolumes objects.
     """
+    _devStatus = UPDATED
 
     RESIZE_SAMPLINGRATE = 0
     RESIZE_DIMENSIONS = 1
     RESIZE_FACTOR = 2
     RESIZE_PYRAMID = 3
 
     WINDOW_OP_CROP = 0
     WINDOW_OP_WINDOW = 1
-
-    #--------------------------- DEFINE param functions --------------------------------------------
-    @classmethod
+    
+    #--------------------------- DEFINE param functions --------------------------------------------       
+    @classmethod   
     def _defineProcessParams(cls, protocol, form):
         # Resize operation
         form.addParam('doResize', BooleanParam, default=False,
                       label='Resize %s?' % protocol._inputLabel,
                       help='If you set to *Yes*, you should provide a resize option.')
         form.addParam('resizeOption', EnumParam,
                       choices=['Sampling Rate', 'Dimensions', 'Factor', 'Pyramid'],
@@ -238,21 +242,36 @@
     """ get the sampling rate of an object"""
     samplingRate = imgSet.getSamplingRate()
     return samplingRate
 
 
 class XmippProtCropResizeParticles(XmippProcessParticles):
     """ Crop or resize a set of particles """
+    # Protocol constants
+    OUTPUT_PARTICLES_NAME = 'outputParticles'
+    OUTPUT_MASK_NAME = 'outputMask'
+
     _label = 'crop/resize particles'
     _inputLabel = 'particles'
+    _possibleOutputs = {OUTPUT_PARTICLES_NAME: SetOfParticles, OUTPUT_MASK_NAME: Mask}
     
     def __init__(self, **kwargs):
         XmippProcessParticles.__init__(self, **kwargs)
     
     #--------------------------- DEFINE param functions --------------------------------------------
+    def _defineParams(self, form):
+        # Creating super form
+        super()._defineParams(form)
+       
+        # Obtaining input particles param to accept also a mask
+        inputParticles = form.getParam('inputParticles')
+        inputParticles.pointerClass = String(str(inputParticles.pointerClass) + ',Mask')
+        inputParticles.label = String(str(inputParticles.label) + '/Mask')
+        inputParticles.help = String('Input particles or 2D Mask to be cropped/resized.')
+
     def _defineProcessParams(self, form):
         XmippResizeHelper._defineProcessParams(self, form)
         form.addParallelSection(threads=0, mpi=8)
         
     def _insertProcessStep(self):
         XmippResizeHelper._insertProcessStep(self)
      
@@ -261,20 +280,48 @@
         XmippResizeHelper.filterStep(self, self._ioArgs(isFirstStep)+args)
     
     def resizeStep(self, isFirstStep, args):
         XmippResizeHelper.resizeStep(self, self._ioArgs(isFirstStep)+args)
     
     def windowStep(self, isFirstStep, args):
         XmippResizeHelper.windowStep(self, self._ioArgs(isFirstStep)+args)
+    
+    def convertInputStep(self):
+        """ convert if necessary"""
+        if self.isMask():
+            # If input is a Mask, modify filter params
+            self.inputFn = self.inputParticles.get().getFileName()
+            inputName = os.path.splitext(os.path.basename(self.inputFn))[0]
+
+            # Set output mask path
+            self.outputStk = self._getExtraPath(os.path.basename(inputName + '.mrc'))
+            self.outputMd = self._getTmpPath('tmp.xmd')
+        else:
+            # If input is not Mask, keep default behaviour
+            super().convertInputStep()
+    
+    def createOutputStep(self):
+        if self.isMask():
+            # If input is a Mask, create output Mask
+            outputMask = Mask(self.outputStk)
+            outputMask.copyInfo(self.inputParticles.get())
+            self._preprocessOutput(outputMask)
+            self._defineOutputs(**{self.OUTPUT_MASK_NAME: outputMask})
+            self._defineTransformRelation(self.inputParticles.get(), outputMask)
+        else:
+            # If input is not Mask, keep default behaviour
+            super().createOutputStep()
         
     def _preprocessOutput(self, output):
-        """ We need to update the sampling rate of the 
+        """
+        We need to update the sampling rate of the 
         particles if the Resize option was used.
         """
-        self.inputHasAlign = self.inputParticles.get().hasAlignment()
+        if not self.isMask():
+            self.inputHasAlign = self.inputParticles.get().hasAlignment()
         
         if self.doResize:
             output.setSamplingRate(self.samplingRate)
             setMRCSamplingRate(self.outputStk, self.samplingRate)
             
     def _updateItem(self, item, row):
         """ Update also the sampling rate and 
@@ -334,17 +381,30 @@
             methods += ["did nothing to them"]
         str = "%s and %s. Output particles: %s" % (", ".join(methods[:-1]),
                                                    methods[-1],
                                                    self.getObjectTag('outputParticles'))
         return [str]
 
     def _validate(self):
-        return XmippResizeHelper._validate(self)
+        """ This function validates the input parameters so only allowed operations take place. """
+        # Getting default errors
+        errors = XmippResizeHelper._validate(self)
+
+        # Checking if at least one of the operations has been selected
+        if not self.doResize and not self.doWindow.get():
+            errors.append('At least one of the possible operations needs to be selected.')
+        
+        # Returning errors
+        return errors
     
     #--------------------------- UTILS functions ---------------------------------------------------
+    def isMask(self):
+        """ This function returns True if the input object is a Mask. False otherwise. """
+        return isinstance(self.inputParticles.get(), Mask)
+      
     def _ioArgs(self, isFirstStep):
         if isFirstStep:
             return "-i %s -o %s --save_metadata_stack %s --keep_input_columns " % (self.inputFn, self.outputStk, self.outputMd)
         else:
             return "-i %s " % self.outputStk
 
     def _filterArgs(self):
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_filter.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_filter.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_image_operate.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_image_operate.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_mask.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_mask.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_movie_resize.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_movie_resize.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_preprocess.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_preprocess.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess/protocol_process.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess/protocol_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,23 +24,26 @@
 # *
 # **************************************************************************
 
 from pwem.constants import ALIGN_NONE
 from pwem.protocols import ProtProcessParticles, ProtPreprocessVolumes
 from pwem.objects import Volume
 import pwem.emlib.metadata as md
+from pyworkflow import BETA, UPDATED, NEW, PROD
 
 from xmipp3.convert import (writeSetOfParticles, xmippToLocation,
                             writeSetOfVolumes, getImageLocation)
 
 
 class XmippProcessParticles(ProtProcessParticles):
     """ Class to create a base template for Xmipp protocols 
     that process SetOfParticles
     """
+    _devStatus = UPDATED
+
     def __init__(self, **kwargs):
         ProtProcessParticles.__init__(self, **kwargs)
         self._args = "-i %(inputFn)s "
 
     #--------------------------- INSERT steps functions -----------------------
     def _insertAllSteps(self):
         self._defineFilenames()
@@ -83,15 +86,15 @@
         writeSetOfParticles(self.inputParticles.get(), self.inputFn,
                             alignType=ALIGN_NONE)
     
     def createOutputStep(self):
         inputSet = self.inputParticles.get()
         # outputSet could be SetOfParticles, SetOfAverages or any future sub-class of SetOfParticles
         className = inputSet.getClassName()
-        outputSet = self._createSetFromName(className)
+        outputSet = inputSet.createCopy(self._getPath())
         outputSet.copyInfo(inputSet)
 
         self._preprocessOutput(outputSet)
         
         outputSet.copyItems(inputSet, 
                             updateItemCallback=self._updateItem,
                             itemDataIterator=md.iterRows(self.outputMd, sortByLabel=md.MDL_ITEM_ID))
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_preprocess_micrographs.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_preprocess_micrographs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_projmatch/__init__.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_projmatch/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_projmatch/projmatch_form.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_projmatch/projmatch_form.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_projmatch/projmatch_initialize.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_projmatch/projmatch_initialize.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_projmatch/projmatch_steps.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_projmatch/projmatch_steps.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_projmatch/protocol_projmatch.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_projmatch/protocol_projmatch.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_random_conical_tilt.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_random_conical_tilt.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_ransac.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_ransac.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_reconstruct_fourier.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_reconstruct_fourier.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_reconstruct_highres.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_reconstruct_highres.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_reconstruct_significant.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_reconstruct_significant.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_reconstruct_swarm.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_reconstruct_swarm.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_resolution3d.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_resolution3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_resolution_bfactor.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_resolution_bfactor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_resolution_deepres.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_resolution_deepres.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_resolution_directional.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_resolution_directional.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_resolution_fso.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_resolution_fso.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,28 +31,29 @@
 from pyworkflow.utils import getExt
 from pyworkflow.protocol.params import (PointerParam, BooleanParam, FloatParam,
                                         LEVEL_ADVANCED)
 
 from pyworkflow import BETA, UPDATED, NEW, PROD
 from pwem.objects import Volume
 from pwem.protocols import ProtAnalysis3D
+from pyworkflow import BETA, UPDATED, NEW, PROD
 
 OUTPUT_3DFSC = '3dFSC.mrc'
 OUTPUT_DIRECTIONAL_FILTER = 'filteredMap.mrc'
 OUTPUT_DIRECTIONAL_DISTRIBUTION = 'Resolution_Distribution.xmd'
 
 
 class XmippProtFSO(ProtAnalysis3D):
     """    
     Given two half maps the protocol estimates Fourier Shell Occupancy to determine the global anisotropy of the map.
     See more information here: https://github.com/I2PC/xmipp/wiki/FSO---Fourier-Shell-Occupancy
     """
     _label = 'resolution fso'
     _lastUpdateVersion = VERSION_2_0
-    _devStatus = NEW
+    _devStatus = PROD
 
     def __init__(self, **args):
         ProtAnalysis3D.__init__(self, **args)
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineParams(self, form):
         form.addSection(label='Input')
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_resolution_monogenic_signal.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_resolution_monogenic_signal.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_rotate_volume.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_rotate_volume.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_rotational_spectra.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_angular_resolution_alignment.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+# -*- coding: utf-8 -*-
 # **************************************************************************
 # *
-# * Authors:     Josue Gomez Blanco (josue.gomez-blanco@mcgill.ca)
+# * Authors:     Jose Luis Vilas (jlvilas@cnb.csic.es)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 2 of the License, or
 # * (at your option) any later version.
@@ -20,194 +21,184 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-from os.path import join
-import numpy as np
-from pwem.objects import Image
-
-from pyworkflow.utils.path import makePath
-from pyworkflow.gui.plotter import Plotter
-from pyworkflow.protocol.params import EnumParam, IntParam
-
-from pwem import emlib
-import xmipp3
-from xmipp3.convert import readSetOfClasses2D
-from .protocol_kerdensom import KendersomBaseClassify
 
+import os
+from pyworkflow import VERSION_2_0
+from pyworkflow.utils import getExt
+from pyworkflow.protocol.params import (PointerParam, BooleanParam, FloatParam,
+                                        LEVEL_ADVANCED)
+from pwem.protocols import ProtAnalysis3D
 
-class XmippProtRotSpectra(KendersomBaseClassify):
-    """Protocol to compute the rotational spectrum of the given particles.
+RADIAL_RESOLUTION_FN = 'radial_FSC_resolution.xmd'
+
+class XmippProtResolutionAlignment(ProtAnalysis3D):
+    """    
+    Given two half maps the protocol estimates if the reconstruction presents angular
+    alignment errors. To do that, a set of directional FSC along all possible directions
+    are estimated. The result is a curve Resolution-radius. If this curve presents a slope
+    then the map present angular assignment errors, but it the graph is flat (horizontal), the map
+    is error free. Note that this protocol generates a plot, not a Scipion object. Its result
+    can only be visualized.
     """
-    _label = 'rotational spectra'
-    
+    _label = 'resolution alignment'
+    _lastUpdateVersion = VERSION_2_0
+
     def __init__(self, **args):
-        KendersomBaseClassify.__init__(self, **args)
-        
-    #--------------------------- DEFINE param functions --------------------------------------------
-    def _addParams(self, form):
-        form.addSection(label='Spectra')
-        form.addParam('howCenter', EnumParam, 
-                      choices=['Middle of the image', 'Minimize first harmonic'], 
-                      default=xmipp3.constants.ROTSPECTRA_CENTER_FIRST_HARMONIC,
-                      display=EnumParam.DISPLAY_COMBO, 
-                      label='How to find the center of rotation', important=True,  
-                      help='Select how to find the center of rotation.')
-        
-        line = form.addLine('Rotational harmonics radius (px)')
-        line.addParam('spectraInnerRadius', IntParam, default=5,
-                      label='Inner',
-                      help='A percentage of the image radius')
-        line.addParam('spectraOuterRadius', IntParam, default=43,
-                      label='Outer',
-                      help='A percentage of the image radius')
-        
-        line = form.addLine('Harmonics to calculate')
-        line.addParam('spectraLowHarmonic', IntParam, default=1,
-                      label='Lowest')
-        line.addParam('spectraHighHarmonic', IntParam, default=15,
-                      label='Highest') 
-    
-    #--------------------------- INSERT steps functions --------------------------------------------
-    def _prepareParams(self):
-        KendersomBaseClassify._prepareParams(self)
-        self._params['extraDir'] = self._getExtraPath()
-        # we need to convert R1 and R2 to percentage of the radius
-        radius = self.inputParticles.get().getDim()[0] / 2
-        percent = 100. / radius
-        self._params['R1'] = self.spectraInnerRadius.get() * percent
-        self._params['R2'] = self.spectraOuterRadius.get() * percent
-        self._params['spectraLowHarmonic'] = self.spectraLowHarmonic.get()
-        self._params['spectraHighHarmonic'] = self.spectraHighHarmonic.get()
-        self._params['vectors'] = self._getExtraPath("rotSpectra.xmd")
-    
-    def _insertProccesStep(self):
-        imagesFn = self._params['imgsFn']
-        centerFn = self._getExtraPath("center2d_center.xmd")
-        # After any of this steps the file "center2d_center.xmd" should be produced
-        if self.howCenter == xmipp3.constants.ROTSPECTRA_CENTER_MIDDLE:
-            self._insertMiddleStep(imagesFn, centerFn)
+        ProtAnalysis3D.__init__(self, **args)
+
+    # --------------------------- DEFINE param functions ----------------------
+    def _defineParams(self, form):
+        form.addSection(label='Input')
+
+        form.addParam('halfVolumesFile', BooleanParam, default=False,
+                      label="Are the half volumes stored with the input volume?",
+                      help='Usually, the half volumes are stored as properties of '
+                           'the input volume. If this is not the case, set this to '
+                           'False and specify the two halves you want to use.')
+
+        form.addParam('inputHalves', PointerParam, pointerClass='Volume',
+                      label="Input Half Maps",
+                      condition='halfVolumesFile',
+                      help='Select a half maps for determining its '
+                           ' resolution anisotropy and resolution.')
+
+        form.addParam('half1', PointerParam, pointerClass='Volume',
+                      condition="not halfVolumesFile",
+                      label="Half Map 1", important=True,
+                      help='Select one map for determining the '
+                           'directional FSC resolution.')
+
+        form.addParam('half2', PointerParam, pointerClass='Volume',
+                      condition="not halfVolumesFile",
+                      label="Half Map 2", important=True,
+                      help='Select the second map for determining the '
+                           'directional FSC resolution.')
+
+        form.addParam('mask', PointerParam, pointerClass='VolumeMask',
+                      allowsNull=True,
+                      label="Mask",
+                      help='The mask determines which points are specimen'
+                           ' and which are not')
+
+        form.addParam('helicalReconstruction', BooleanParam, default=False,
+                      label="Is a the protein a helix",
+                      help='blablabla')
+
+        form.addParam('limRadius', BooleanParam, default=True,
+                      expertLevel=LEVEL_ADVANCED,
+                      label="Limit the protein radius",
+                      help='blablabla')
+
+        form.addParam('usedirectionalfsc', BooleanParam, default=True,
+                      expertLevel=LEVEL_ADVANCED,
+                      label="use directional fsc",
+                      help='blablabla')
+
+        form.addParam('coneAngle', FloatParam, default=17.0,
+                      expertLevel=LEVEL_ADVANCED,
+                      label="Cone Angle",
+                      help='Angle between the axis of the cone and the generatrix. '
+                           'An angle of 17 degrees is the best angle (see publication'
+                           'Vilas 2021) to measuare directional FSCs')
+
+        form.addParam('threshold', FloatParam, expertLevel=LEVEL_ADVANCED,
+                      default=0.143,
+                      label="FSC Threshold",
+                      help='Threshold for the fsc. By default the standard 0.143. '
+                           'Other common thresholds are 0.5 and 0.3.')
+
+        form.addParallelSection(threads=4, mpi=0)
+
+    # --------------------------- INSERT steps functions --------------------------------------------
+    def _insertAllSteps(self):
+        self._insertFunctionStep(self.convertInputStep)
+        self._insertFunctionStep(self.angularResolutionAlignmentStep)
+
+    def convertInputStep(self):
+        """ This function sets the maps properly into mrc
+        """
+
+        if self.halfVolumesFile:
+            self.vol1Fn, self.vol2Fn = self.inputHalves.get().getHalfMaps().split(',')
         else:
-            self._insertFunctionStep('centerFirstHarmonicStep', imagesFn, centerFn)
-        # Produce "rotSpectra.xmd" vectors
-        self._insertFunctionStep('calculateSpectraStep', imagesFn, centerFn, self._params['vectors'])
-        # Call kerdensom for classification
-        self._insertKerdensomStep()
-    
-    def _insertMiddleStep(self, imagesFn, outputCenter):
-        R2 = self._params['R2']
-        
-        if R2 + 20 > 100:
-            R3 = R2 + (100 - R2) / 2
-            R4 = 100
+            self.vol1Fn = self.half1.get().getFileName()
+            self.vol2Fn = self.half2.get().getFileName()
+
+        extVol1 = getExt(self.vol1Fn)
+        extVol2 = getExt(self.vol2Fn)
+
+        if (extVol1 == '.mrc') or (extVol1 == '.map'):
+            self.vol1Fn = self.vol1Fn + ':mrc'
+        if (extVol2 == '.mrc') or (extVol2 == '.map'):
+            self.vol2Fn = self.vol2Fn + ':mrc'
+
+        if self.mask.hasValue():
+            self.maskFn = self.mask.get().getFileName()
+            extMask = getExt(self.maskFn)
+            if (extMask == '.mrc') or (extMask == '.map'):
+                self.maskFn = self.maskFn + ':mrc'
+
+    def angularResolutionAlignmentStep(self):
+        """
+        This function runs the algorithm to detect misalignment
+        """
+        fndir = self._getExtraPath("fsc")
+
+        os.mkdir(fndir)
+
+        params = ' --half1 "%s"' % self.vol1Fn
+        params += ' --half2 "%s"' % self.vol2Fn
+        params += ' -o %s' % self._getExtraPath(RADIAL_RESOLUTION_FN)
+        if self.halfVolumesFile:
+            params += ' --sampling %f' % self.inputHalves.get().getSamplingRate()
         else:
-            R3 = R2 + 10
-            R4 = R2 + 20
-        self._params['R3'] = R3
-        self._params['R4'] = R4
-        
-        program = 'xmipp_image_find_center'
-        args = '-i ' + imagesFn
-        args += ' --oroot %(extraDir)s/center2d --r1 %(R1)d --r2 %(R2)d --r3 %(R3)d --r4 %(R4)d'
-        # Run the command with formatted parameters
-        self._insertRunJobStep(program, args % self._params)
-    
-    #--------------------------- STEPS functions ---------------------------------------------------
-    def centerFirstHarmonicStep(self, imagesFn, outputCenter):
-        dims = emlib.MetaDataInfo(str(imagesFn))
-        md = emlib.MetaData()
-        objId = md.addObject()
-        md.setValue(emlib.MDL_X, float(dims[0] / 2), objId)
-        md.setValue(emlib.MDL_Y, float(dims[1] / 2), objId)
-        md.write(outputCenter)
-        return [outputCenter] # this file should exists after the step
-            
-    def calculateSpectraStep(self, imagesFn, inputCenter, outputSpectra):     
-        md = emlib.MetaData(inputCenter)
-        objId = md.firstObject()
-        self._params['xOffset'] = md.getValue(emlib.MDL_X, objId)
-        self._params['yOffset'] = md.getValue(emlib.MDL_Y, objId)
-        
-        program = 'xmipp_image_rotational_spectra'
-        args = "-i %s -o %s" % (imagesFn, outputSpectra)
-        args += ' --x0 %(xOffset)s --y0 %(yOffset)s --r1 %(R1)d --r2 %(R2)d' + \
-                     ' --low %(spectraLowHarmonic)d --high %(spectraHighHarmonic)d'
-        # Run the command with formatted parameters
-        self.runJob(program, args % self._params)
-        return [outputSpectra]
-    
-    def createOutputStep(self):
-        self.plotsDir = self._getExtraPath('plots')
-        makePath(self.plotsDir)
-        
-        fnClassVectors = self._params['kvectors'].replace('xmd', 'vec')
-        f = open(fnClassVectors)
-        self.classArray = np.fromfile(f, dtype=np.float32)
-        f.close()
-        
-        fnImgVectors = self._params['vectors'].replace('xmd', 'vec')
-        f = open(fnImgVectors)
-        self.imgArray = np.fromfile(f, dtype=np.float32)
-        f.close()
-        self.imgCount = 0
-        
-        imgSet = self.inputParticles.get()
-        classes2DSet = self._createSetOfClasses2D(imgSet)
-        readSetOfClasses2D(classes2DSet, self._params['kclasses'], 
-                           preprocessClass=self._preprocessClass,
-                           postprocessImageRow=self._postprocessImageRow)
-        self._defineOutputs(outputClasses=classes2DSet)
-        self._defineSourceRelation(self.inputParticles, classes2DSet)
-                
-    def _preprocessClass(self, classItem, classRow):
-        KendersomBaseClassify._preprocessClass(self, classItem, classRow)
-        ref = classRow.getValue(emlib.MDL_REF) # get class number
-        classItem.spectraPlot = Image()
-        classItem.spectraPlot.setFileName(self._createSpectraPlot('class', 
-                                                                  self.classArray, 
-                                                                  ref))
-        
-    def _postprocessImageRow(self, img, imgRow):
-        self.imgCount += 1
-        img.spectraPlot = Image()
-        img.spectraPlot.setFileName(self._createSpectraPlot('image', 
-                                                            self.imgArray, 
-                                                            self.imgCount, 
-                                                            img.getObjId()))
-        
-    def _createSpectraPlot(self, label, array, index, objId=None):
-        if objId is None:
-            objId = index
-        # Number of harmonics calculated
-        plotter = Plotter()
-        a = plotter.createSubPlot('Spectrum for %s %d' % (label, objId), 
-                                  xlabel='Harmonics', ylabel='Energy')
-        
-        n = self.spectraHighHarmonic.get() - self.spectraLowHarmonic.get() + 1
-        i1 = (index-1) * n
-        i2 = i1 + n
-        xdata = range(self.spectraLowHarmonic.get(), self.spectraHighHarmonic.get()+1)
-        ydata = array[i1:i2]
-        a.plot(xdata, ydata)
-        
-        plotFile = join(self.plotsDir, 'spectra_%s%06d.png' % (label, objId))
-        plotter.savefig(plotFile)
-        plotter.close()
-        
-        return plotFile
-        
-    #--------------------------- INFO functions ----------------------------------------------------
+            params += ' --sampling %f' % self.half1.get().getSamplingRate()
+
+        if self.helicalReconstruction.get():
+            params += ' --helix '
+
+        if self.mask.hasValue():
+            params += ' --mask "%s"' % self.maskFn
+        if self.limRadius.get():
+            params += ' --limit_radius '
+        if self.usedirectionalfsc.get():
+            params += ' --directional_resolution '
+            params += ' --anglecone %f' % self.coneAngle.get()
+
+        params += ' --threshold %s' % self.threshold.get()
+        params += ' --threads %s' % self.numberOfThreads.get()
+
+        self.runJob('xmipp_angular_resolution_alignment', params)
+
+    # --------------------------- INFO functions ------------------------------
+
+    def _methods(self):
+        messages = []
+        ARTICLE_URL = 'Pending on publication'
+        messages.append('Information about the method/article in ' + ARTICLE_URL)
+
+        return messages
+
     def _validate(self):
-        return KendersomBaseClassify._validate(self)
-    
-    def _citations(self):
-        return ['Pascual2000']
-    
+        errors = []
+
+        if self.halfVolumesFile.get():
+            if not self.inputHalves.get():
+                errors.append("You need to select the Associated halves")
+        else:
+            if not self.half1.get():
+                errors.append("You need to select the half1")
+            if not self.half2.get():
+                errors.append("You need to select the half2")
+
+        return errors
+
     def _summary(self):
-        return KendersomBaseClassify._summary(self)
-    
-    def _methods(self):
-        return KendersomBaseClassify._methods(self)
-   
+        summary = []
+        summary.append("This protocol does not produce Scipion Objects as output. Click on Analyze results to visualize the results")
+        return summary
+
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_rotational_symmetry.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_rotational_symmetry.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_screen_deepConsensus.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_screen_deepConsensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_screen_deeplearning.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_screen_deeplearning.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_screen_particles.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_screen_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_shift_particles.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_shift_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_shift_volume.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_shift_volume.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_solid_angles.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_solid_angles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_split_volume.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_deep_center_predict.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # **************************************************************************
 # *
-# * Authors:     Carlos Oscar Sorzano (coss@cnb.csic.es)
+# * Authors:     COS Sorzano, Erney Ramirez and Adrian Sansinena
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 2 of the License, or
 # * (at your option) any later version.
@@ -19,94 +19,140 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-"""
-Protocol to split a volume in two volumes based on a set of images
-"""
 
+from pyworkflow import VERSION_3_0
+from pyworkflow.protocol import STEPS_PARALLEL
+from pyworkflow.protocol.params import (PointerParam, StringParam, FloatParam,
+                                        IntParam, BooleanParam, GPU_LIST, EnumParam)
 from pyworkflow.protocol.constants import LEVEL_ADVANCED
-from pyworkflow.protocol.params import PointerParam, FloatParam, IntParam, StringParam
-from pyworkflow.utils.path import cleanPath
-from pyworkflow import BETA, UPDATED, NEW, PROD
-from pwem.protocols import ProtClassify3D
-from pwem.objects import Volume
+from pyworkflow.utils.path import moveFile, cleanPattern
+from pwem.protocols import ProtAlign2D
+from pwem.emlib.metadata import iterRows, getFirstRow
+import pwem.emlib.metadata as md
+from xmipp3.convert import createItemMatrix, setXmippAttributes, readSetOfParticles, writeSetOfParticles
+from pwem import ALIGN_PROJ
+from pwem import emlib
 from pwem.emlib.image import ImageHandler
-from xmipp3.convert import writeSetOfParticles
-
+import os
+import sys
+import numpy as np
+import math
+from shutil import copy
+from os import remove
+from os.path import exists, join
+import xmipp3
+from pyworkflow import BETA, UPDATED, NEW, PROD
 
-class XmippProtSplitvolume(ProtClassify3D):
-    """Split volume in two"""
-    _label = 'split volume'
+class XmippProtDeepCenterPredict(ProtAlign2D, xmipp3.XmippProtocol):
+    """Predict the center particles using deep learning.""" 
+    _label = 'deep center predict'
+    _lastUpdateVersion = VERSION_3_0
     _devStatus = BETA
 
+    _conda_env = 'xmipp_DLTK_v1.0'
+    _cond_predictAnglesTrue = 'predictAngles==True'
+    _cond_predictAnglesFalse = 'predictAngles==False'
+    _cond_trainedModelTrue = 'trainedModel==True'
+    _cond_trainedModelFalse = 'trainedModel==False'
+    _cond_needModel = '(trainedModel==True) or (predictAngles==True)'
+
     def __init__(self, **args):
-        ProtClassify3D.__init__(self, **args)
+        ProtAlign2D.__init__(self, **args)
 
-    #--------------------------- DEFINE param functions --------------------------------------------
+    # --------------------------- DEFINE param functions --------------------------------------------
     def _defineParams(self, form):
+
+        form.addHidden(GPU_LIST, StringParam, default='0',
+                       expertLevel=LEVEL_ADVANCED,
+                       label="Choose GPU IDs",
+                       help="GPU may have several cores. Set it to zero"
+                            " if you do not know what we are talking about."
+                            " First core index is 0, second 1 and so on.")
+
         form.addSection(label='Input')
-        
-        form.addParam('directionalClasses', PointerParam, label="Directional classes", important=True, 
-                      pointerClass='SetOfAverages', pointerCondition='hasAlignmentProj',
-                      help='Select a set of particles with angles. Preferrably the output of a run of directional classes')
-        form.addParam('symmetryGroup', StringParam, default='c1',
-                      label="Symmetry group", 
-                      help='See [[Xmipp Symmetry][http://www2.mrc-lmb.cam.ac.uk/Xmipp/index.php/Conventions_%26_File_formats#Symmetry]] page '
-                           'for a description of the symmetry format accepted by Xmipp') 
-        form.addParam('mask', PointerParam, label="Mask", pointerClass='VolumeMask', allowsNull=True,
-                      help='The mask values must be binary: 0 (remove these voxels) and 1 (let them pass).')
-        form.addParam('Nrec', IntParam, label="Number of reconstructions", default=5000, expertLevel=LEVEL_ADVANCED, 
-                      help="Number of random reconstructions to perform");
-        form.addParam('Nsamples', IntParam, label="Number of images/reconstruction", default=15, expertLevel=LEVEL_ADVANCED, 
-                      help="Number of images per reconstruction. Consider that reconstructions with symmetry c1 will be perfomed");
-        form.addParam('alpha', FloatParam, label="Confidence level", default=0.05, expertLevel=LEVEL_ADVANCED, 
-                      help="This parameter is alpha. Two volumes, one at alpha/2 and another one at 1-alpha/2, will be generated");
-    
-    #--------------------------- INSERT steps functions --------------------------------------------
+
+        form.addParam('inputImageSet', PointerParam, label="Input Image set",
+                      pointerClass='SetOfParticles',
+                      help='The set of particles to predict shift')
+
+        form.addParam('Xdim', IntParam, label="Size of the images for training", default=128)
+
+        form.addParam('inputModel', PointerParam, label="Model trained",
+                      pointerClass='XmippProtDeepCenter',
+                      help='The model to predict angles')
+
+        form.addSection(label='Consensus')
+
+        form.addParam('numModels', IntParam,
+                      label="Number of models trained", default=5)
+
+        form.addParam('tolerance', IntParam,
+                      label="Tolerance in pixels", default=3,
+                      help="Max difference between predictions and their mean value.")
+
+        form.addParam('maxModels', IntParam,
+                      label="Maximum number of models dropped per particle", default=0,
+                      help="If more models are dropped, the particle is discarded.")
+
+        form.addParallelSection(threads=1, mpi=1)
+
+    # --------------------------- INSERT steps functions --------------------------------------------
     def _insertAllSteps(self):
-        self._insertFunctionStep('convertInputStep',self.directionalClasses.getObjId())
-        self._insertFunctionStep('generateSplittedVolumes')
-        self._insertFunctionStep('createOutput')
-
-    #--------------------------- STEPS functions ---------------------------------------------------
-    def convertInputStep(self, inputParticlesId):
-        writeSetOfParticles(self.directionalClasses.get(),self._getExtraPath("directionalClasses.xmd"))
-
-    def createOutput(self):
-        inputParticles = self.directionalClasses.get()
-        Ts = inputParticles.getSamplingRate()
-        volumesSet = self._createSetOfVolumes()
-        volumesSet.setSamplingRate(Ts)
-        for i in range(2):
-            vol = Volume()
-            fnVol = self._getExtraPath("split_v%d.vol"%(i+1))
-            fnMrc = self._getExtraPath("split_v%d.mrc"%(i+1))
-            self.runJob("xmipp_image_convert","-i %s -o %s -t vol"%(fnVol,fnMrc), numberOfMpi=1)
-            self.runJob("xmipp_image_header","-i %s --sampling_rate %f"%(fnMrc, Ts), numberOfMpi=1)
-            cleanPath(fnVol)
-            vol.setLocation(1, fnMrc)
-            volumesSet.append(vol)
-        
-        self._defineOutputs(outputVolumes=volumesSet)
-        self._defineSourceRelation(inputParticles, volumesSet)
-        
-    def generateSplittedVolumes(self):
-        inputParticles = self.directionalClasses.get()
-        Xdim = inputParticles.getDimensions()[0]
-        fnMask = ""
-        if self.mask.hasValue():
-            fnMask = self._getExtraPath("mask.vol")
-            img=ImageHandler()
-            img.convert(self.mask.get(), fnMask)
-            self.runJob('xmipp_image_resize',"-i %s --dim %d"%(fnMask,Xdim),numberOfMpi=1)
-            self.runJob('xmipp_transform_threshold',"-i %s --select below 0.5 --substitute binarize"%fnMask,numberOfMpi=1)
-
-        args="-i %s --oroot %s --Nrec %d --Nsamples %d --sym %s --alpha %f"%\
-             (self._getExtraPath("directionalClasses.xmd"),self._getExtraPath("split"),self.Nrec.get(),self.Nsamples.get(),
-              self.symmetryGroup.get(), self.alpha.get())
-        if fnMask!="":
-            args+=" --mask binary_file %s"%fnMask
-        self.runJob("xmipp_classify_first_split",args)
+        self.predictImgsFn = self._getExtraPath('predict_input_imgs.xmd')
+
+        if self.useQueueForSteps() or self.useQueue():
+            myStr = os.environ["CUDA_VISIBLE_DEVICES"]
+        else:
+            myStr = self.gpuList.get()
+            os.environ["CUDA_VISIBLE_DEVICES"] = self.gpuList.get()
+        numGPU = myStr.split(',')
+
+        self._insertFunctionStep("convertStep")
+        self._insertFunctionStep("predict", numGPU[0])
+        self._insertFunctionStep('createOutputStep')
+
+    # --------------------------- STEPS functions ---------------------------------------------------
+    def convertStep(self):
+        writeSetOfParticles(self.inputImageSet.get(), self.predictImgsFn)
+        self.runJob("xmipp_image_resize",
+                    "-i %s -o %s --save_metadata_stack %s --fourier %d" %
+                    (self.predictImgsFn,
+                        self._getExtraPath('trainingResized.stk'),
+                        self._getExtraPath('trainingResized.xmd'),
+                        self.Xdim), numberOfMpi=self.numberOfThreads.get()*self.numberOfMpi.get())
+
+    def predict(self, gpuId):
+        self.modelAng = self.inputModel.get()
+        args = "%s %s %s %s %s %d %d %d" % (
+            self._getExtraPath("trainingResized.xmd"), gpuId, self._getPath(), self.predictImgsFn,
+            self.modelAng._getExtraPath("modelCenter"), self.numModels.get(), self.tolerance.get(),
+            self.maxModels.get())
+
+        self.runJob("xmipp_deep_center_predict", args, numberOfMpi=1, env=self.getCondaEnv())
+
+        remove(self._getExtraPath("trainingResized.xmd"))
+        remove(self._getExtraPath("trainingResized.stk"))
+
+    def createOutputStep(self):
+        imgFname = self._getPath('predict_results.xmd')
+        outputSet = self._createSetOfParticles()
+
+        readSetOfParticles(imgFname, outputSet)
+        outputSet.copyInfo(self.inputImageSet.get())
+        outputSet.setAlignmentProj()
+
+        self._defineOutputs(outputParticles=outputSet)
+        self._store(outputSet)
+        self._defineSourceRelation(self.inputImageSet.get(), outputSet)
+
+    # --------------------------- INFO functions --------------------------------
+    def _methods(self):
+        methods = []
+        if hasattr(self, 'outputParticles'):
+            methods.append("We learned a model to center particles from %i input images (%s)." \
+                % (self.inputSet.get().getSize(), self.getObjectTag('inputSet')))
+        return methods
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_structure_map.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_structure_map.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_structure_map_zernike3d.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_structure_map_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_subtract_projection.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_subtract_projection.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from pyworkflow.protocol.params import PointerParam, BooleanParam, IntParam, FloatParam, EnumParam
 from pyworkflow.protocol.constants import LEVEL_ADVANCED
 from pwem import emlib
 from pwem.protocols import EMProtocol
 from xmipp3.convert import writeSetOfParticles, readSetOfParticles
 from pyworkflow import BETA, UPDATED, NEW, PROD
 
+OUTPUT = "output_particles.xmd"
 
 class XmippProtSubtractProjectionBase(EMProtocol):
     """ Helper class that contains some Protocol utilities methods
     used by both  XmippProtSubtractProjection and XmippProtBoostParticles."""
     _devStatus = UPDATED
 
     # --------------------------- DEFINE param functions --------------------------------------------
@@ -75,15 +76,15 @@
         self._insertFunctionStep('createOutputStep')
 
     # --------------------------- STEPS functions --------------------------------------------
     def createOutputStep(self):
         inputSet = self.inputParticles.get()
         outputSet = self._createSetOfParticles()
         outputSet.copyInfo(inputSet)
-        readSetOfParticles(self._getExtraPath("output_particles.xmd"), outputSet,
+        readSetOfParticles(self._getExtraPath(OUTPUT), outputSet,
                            extraLabels=[emlib.MDL_SUBTRACTION_R2, emlib.MDL_SUBTRACTION_BETA0,
                                         emlib.MDL_SUBTRACTION_BETA1])
         self._defineOutputs(outputParticles=outputSet)
         self._defineSourceRelation(inputSet, outputSet)
 
 
 class XmippProtSubtractProjection(XmippProtSubtractProjectionBase):
@@ -97,14 +98,16 @@
         XmippProtSubtractProjectionBase._defineParams(form)
         form.addParam('mask', PointerParam, pointerClass='VolumeMask', label='Mask ', allowsNull=True,
                       help='Specify a 3D mask for the region of the input volume that you want to keep or subtract, '
                            'avoiding masks with 1s in background. If no mask is given, the subtraction is performed in'
                            ' whole images.')
         form.addParam('subtract', EnumParam, default=0, choices=["Keep", "Subtract"], display=EnumParam.DISPLAY_HLIST,
                       label="Mask contains the part to ")
+        form.addParallelSection(threads=0, mpi=4)
+
     # --------------------------- INSERT steps functions --------------------------------------------
     def _insertSubSteps(self):
         self._insertFunctionStep('convertStep')
         self._insertFunctionStep('subtractionStep')
 
     # --------------------------- STEPS functions --------------------------------------------
     def convertStep(self):
@@ -112,21 +115,25 @@
 
     def subtractionStep(self):
         vol = self.vol.get().clone()
         fnVol = vol.getFileName()
         if fnVol.endswith('.mrc'):
             fnVol += ':mrc'
         args = '-i %s --ref %s -o %s --sampling %f --max_resolution %f --padding %f ' \
-               '--sigma %d --limit_freq %d --cirmaskrad %d --save %s' % \
-               (self._getExtraPath(self.INPUT_PARTICLES), fnVol, self._getExtraPath("output_particles"),
+               '--sigma %d --limit_freq %d --cirmaskrad %d --save %s --oroot %s' % \
+               (self._getExtraPath(self.INPUT_PARTICLES), fnVol, self._getExtraPath(OUTPUT),
                 vol.getSamplingRate(), self.resol.get(), self.pad.get(), self.sigma.get(),
-                int(self.limit_freq.get()), self.cirmaskrad.get(), self._getExtraPath())
+                int(self.limit_freq.get()), self.cirmaskrad.get(), self._getExtraPath(),
+                self._getExtraPath("subtracted_part"))
         mask = self.mask.get()
+        fnMask = mask.getFileName()
+        if fnMask.endswith('.mrc'):
+            fnMask += ':mrc'
         if mask is not None:
-            args += ' --mask %s' % mask.getFileName()
+            args += ' --mask %s' % fnMask
         if self.nonNegative.get():
             args += ' --nonNegative'
         if self.subtract.get():
             args += ' --subtract'
         self.runJob("xmipp_subtract_projection", args)
 
     # --------------------------- INFO functions --------------------------------------------
@@ -174,14 +181,15 @@
 
     _label = 'boost particles'
     INPUT_PARTICLES = "input_particles.xmd"
 
     # --------------------------- DEFINE param functions --------------------------------------------
     def _defineParams(self, form):
         XmippProtSubtractProjectionBase._defineParams(form)
+        form.addParallelSection(threads=0, mpi=4)
 
     # --------------------------- INSERT steps functions --------------------------------------------
     def _insertSubSteps(self):
         self._insertFunctionStep('convertStep')
         self._insertFunctionStep('boostingStep')
 
     # --------------------------- STEPS functions --------------------------------------------
@@ -190,18 +198,18 @@
 
     def boostingStep(self):
         vol = self.vol.get().clone()
         fnVol = vol.getFileName()
         if fnVol.endswith('.mrc'):
             fnVol += ':mrc'
         args = '-i %s --ref %s -o %s --sampling %f --max_resolution %f --padding %f --sigma %d --limit_freq %d ' \
-               '--cirmaskrad %d --boost --save %s'\
-               % (self._getExtraPath(self.INPUT_PARTICLES), fnVol, self._getExtraPath("output_particles"),
+               '--cirmaskrad %d --boost --save %s --oroot %s'\
+               % (self._getExtraPath(self.INPUT_PARTICLES), fnVol, self._getExtraPath(OUTPUT),
                   vol.getSamplingRate(), self.resol.get(), self.pad.get(), self.sigma.get(), int(self.limit_freq.get()),
-                  self.cirmaskrad.get(), self._getExtraPath())
+                  self.cirmaskrad.get(), self._getExtraPath(), self._getExtraPath("subtracted_part"))
 
         if self.nonNegative.get():
             args += ' --nonNegative'
         self.runJob("xmipp_subtract_projection", args)
 
     # --------------------------- INFO functions --------------------------------------------
     def _validate(self):
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_tilt_analysis.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_tilt_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,22 +238,14 @@
             self._updateOutputSet('discardedMicrographs', micSet_discarded, streamMode)
 
         if self.finished:  # Unlock createOutputStep if finished all jobs
             outputStep = self._getFirstJoinStep()
             if outputStep and outputStep.isWaiting():
                 outputStep.setStatus(cons.STATUS_NEW)
 
-    def _closeOutputSet(self):
-        if self.hasAttribute('outputMicrographs'):
-            self.outputMicrographs.close()
-            self.outputMicrographs.setStreamState(Set.STREAM_CLOSED)
-        if self.hasAttribute('discardedMicrographs'):
-            self.discardedMicrographs.close()
-            self.discardedMicrographs.setStreamState(Set.STREAM_CLOSED)
-
     def _insertNewMicrographSteps(self, insertedDict, inputMics):
         """ Insert steps to process new micrographs (from streaming)
         Params:
             insertedDict: contains already processed micrographs
             inputMics: input mics set to be check
         """
         deps = []
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_trigger_data.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_trigger_data.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_validate_fscq.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_validate_fscq.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_validate_nontilt.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_validate_nontilt.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_validate_overfitting.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_validate_overfitting.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_volume_adjust_sub.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_volume_adjust_sub.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_volume_deform_zernike3d.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_volume_deform_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_volume_local_sharpening.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_volume_local_sharpening.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_volume_strain.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_volume_strain.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_write_testC.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_write_testC.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols/protocol_write_testP.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols/protocol_write_testP.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/protocols.conf` & `scipion-em-xmipp-23.7.0.0/xmipp3/protocols.conf`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [PROTOCOLS]
 Protocols SPA = [
 	{"tag": "section", "text": "Movies", "openItem": "False", "children": [
 		{"tag": "protocol", "value": "XmippProtFlexAlign", "text": "default"},
 		{"tag": "protocol", "value": "XmippProtOFAlignment", "text": "default"},
 		{"tag": "protocol", "value": "XmippProtMovieMaxShift", "text": "default"},
 		{"tag": "protocol", "value": "XmippProtSplitFrames", "text": "default"}	,
-		{"tag": "protocol", "value": "XmippProtMovieGain", "text": "default"}
+		{"tag": "protocol", "value": "XmippProtMovieGain", "text": "default"},
+		{"tag": "protocol", "value": "XmippProtMovieDoseAnalysis", "text": "default"}
 	]},
 	{"tag": "section", "text": "Micrographs", "openItem": "False", "children": [
 		{"tag": "protocol_group", "text": "Preprocess", "openItem": "False", "children": [
 		    {"tag": "protocol", "value": "XmippProtPreprocessMicrographs", "text": "default"},
 		    {"tag": "protocol", "value": "XmippProtTiltAnalysis", "text": "default"}
 		]},
 		{"tag": "protocol_group", "text": "CTF estimation", "openItem": "False", "children": [
             {"tag": "protocol", "value": "XmippProtCTFMicrographs", "text": "default"},
             {"tag": "protocol", "value": "XmippProtCTFConsensus", "text": "default"}
         ]}
 	]},
 	{"tag": "section", "text": "Particles", "children": [
 		{"tag": "protocol_group", "text": "Picking", "openItem": "False", "children": [
-		{"tag": "protocol", "value": "XmippProtParticleBoxsize",   "text": "default"},
 		{"tag": "protocol", "value": "XmippProtParticlePicking",   "text": "default"},
 		{"tag": "protocol", "value": "XmippParticlePickingAutomatic",   "text": "default"},
 		{"tag": "protocol", "value": "XmippProtScreenDeepConsensus",   "text": "default"},
 		{"tag": "protocol", "value": "XmippProtDeepMicrographScreen",   "text": "default"},
 		{"tag": "protocol", "value": "XmippProtAssignmentTiltPair",   "text": "default"},		
 		{"tag": "protocol", "value": "XmippProtConsensusPicking",   "text": "default"},
 		{"tag": "protocol", "value": "XmippProtPickNoise",   "text": "default"},
@@ -65,16 +65,15 @@
 			{"tag": "protocol", "value": "XmippProtCL2D",   "text": "default"},			
 			{"tag": "protocol", "value": "XmippProtCoreAnalysis",   "text": "default"},
 			{"tag": "protocol", "value": "XmippProtGpuCrrCL2D",   "text": "default"},
 			{"tag": "protocol", "value": "XmippProtStrGpuCrrCL2D",   "text": "default"},
 			{"tag": "protocol", "value": "XmippProtStrGpuCrrSimple",   "text": "default"},
 			{"tag": "section", "text": "more", "openItem": "False", "children": [
 				{"tag": "protocol", "value": "XmippProtML2D", "text": "default"},
-				{"tag": "protocol", "value": "XmippProtKerdensom", "text": "default"},
-				{"tag": "protocol", "value": "XmippProtRotSpectra", "text": "default"}				
+				{"tag": "protocol", "value": "XmippProtKerdensom", "text": "default"}
 			]}
 		]}
 	]},
 	{"tag": "section", "text": "3D", "children": [
 	{"tag": "protocol_group", "text": "Initial volume", "openItem": "False", "children": [
 	{"tag": "protocol", "value": "XmippProtRansac",  "text": "default"},
 	{"tag": "protocol", "value": "XmippProtReconstructSignificant",  "text": "default"},
@@ -128,14 +127,15 @@
 		{"tag": "protocol", "value": "XmippProtAngularGraphConsistency", "text": "default"},
 		{"tag": "protocol", "value": "XmippProtValidateOverfitting",    "text": "default"}
 	]},
 	{"tag": "section", "text": "Resolution", "openItem": "False", "children": [
 		{"tag": "protocol", "value": "XmippProtMonoRes",   "text": "default"},
 		{"tag": "protocol", "value": "XmippProtDeepRes",   "text": "default"},		
 		{"tag": "protocol", "value": "XmippProtResolution3D",  "text": "default"},
+		{"tag": "protocol", "value": "XmippProtFSO",  "text": "default"},
 		{"tag": "protocol", "value": "XmippProtMultipleFSCs",  "text": "default"},
 		{"tag": "protocol", "value": "XmippProtMonoDir",  "text": "default"},
         {"tag": "protocol", "value": "XmippProtMonoTomo", "text": "default"}
 
 	]},
 	{"tag": "section", "text": "more", "openItem": "False", "children": [
 	{"tag": "protocol", "value": "XmippProtCombinePdb", "text": "default"},
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_convert_xmipp.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_convert_xmipp.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_angular_graph_consistency.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_angular_graph_consistency.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_apply_transformation_matrix.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_apply_transformation_matrix.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_compare_angles.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_compare_angles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_consensus_classes3D.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_consensus_classes3D.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_ctf_consensus.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_ctf_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_deep_denoising.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_deep_denoising.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_extract_asymmetric_unit.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_extract_asymmetric_unit.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_monodir.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_monodir.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_multiple_fsc.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_multiple_fsc.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_multireference_alignability.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_multireference_alignability.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_reconstruct_fourier.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_reconstruct_fourier.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_screen_deepConsensus.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_screen_deepConsensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_simulate_ctf.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_highres.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# ***************************************************************************
+# **************************************************************************
 # *
-# * Authors:     Carlos Oscar Sanchez Sorzano (coss@cnb.csic.es)
-# *              David Herreros Calero (dherreros@cnb.csic.es)
+# * Authors:    Carlos Oscar Sorzano (coss@cnb.csic.es)
+# *
+# * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 2 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
@@ -16,81 +17,89 @@
 # * You should have received a copy of the GNU General Public License
 # * along with this program; if not, write to the Free Software
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
-# ***************************************************************************
+# *
+# **************************************************************************
+
+from pyworkflow.tests import BaseTest, DataSet, setupTestProject
 
-import os
+from pwem.protocols import (ProtImportVolumes, ProtImportParticles, ProtSubSet,
+                            exists)
 
-from pyworkflow.tests import BaseTest, DataSet
-import pyworkflow.tests as tests
+from pwem import emlib
+from xmipp3.protocols import XmippProtReconstructHighRes
 
-import pyworkflow.utils as pwutils
 
-from pwem.protocols import ProtImportVolumes
-from xmipp3.protocols import XmippProtSimulateCTF, XmippProtCreateGallery
+class TestHighres(BaseTest):
+    @classmethod
+    def runImportVolume(cls, pattern, samplingRate):
+        """ Run an Import volumes protocol. """
+        cls.protImport = cls.newProtocol(ProtImportVolumes,
+                                         filesPath=pattern,
+                                         samplingRate=samplingRate
+                                         )
+        cls.launchProtocol(cls.protImport)
+        return cls.protImport
 
+    @classmethod
+    def runImportParticles(cls):
+        """ Import Particles.
+        """
+        args = {'importFrom': ProtImportParticles.IMPORT_FROM_SCIPION,
+                'sqliteFile': cls.particles,
+                'amplitudConstrast': 0.1,
+                'sphericalAberration': 2.0,
+                'voltage': 200,
+                'samplingRate': 0.99,
+                'haveDataBeenPhaseFlipped': True
+                }
+
+        # Id's should be set increasing from 1 if ### is not in the 
+        # pattern
+        protImport = cls.newProtocol(ProtImportParticles, **args)
+        protImport.setObjLabel('import particles')
+        cls.launchProtocol(protImport)
+        return protImport
 
-class TestXmippProtSimulateCTF(BaseTest):
-    """ Testing CTF simulation
-    """
     @classmethod
     def setUpClass(cls):
-        tests.setupTestProject(cls)
-        cls.dataset = DataSet.getDataSet('relion_tutorial')
-        cls.volume = cls.dataset.getFile(os.path.join('volumes', 'reference_masked.vol'))
-
-    def runImportVolume(self, pattern, sampling):
-        """ Run an Import volume protocol. """
-        protImport = self.newProtocol(ProtImportVolumes,
-                                     filesPath=pattern,
-                                     samplingRate=sampling,
-                                     objLabel='relion_tutorial volume ' + pwutils.removeBaseExt(pattern))
-        self.launchProtocol(protImport)
-        if protImport.outputVolume is None:
-            raise Exception('Import of volume: %s, failed. outputVolume is None.' % pattern)
-        return protImport.outputVolume
-
-    def runCreateGallery(self, volume):
-        protCreateGallery = self.newProtocol(XmippProtCreateGallery,
-                                             inputVolume=volume,
-                                             objLabel='Imported Volume Projections')
-        self.launchProtocol(protCreateGallery)
-        if protCreateGallery.outputReprojections is None:
-            raise Exception('Create Gallery faile: no output produced')
-        return protCreateGallery.outputReprojections
-
-    def runSimulateCTF(self, projections, defocus0=5000, defocusF=25000):
-        protSimulateCTF = self.newProtocol(XmippProtSimulateCTF,
-                                           inputParticles=projections,
-                                           Defocus0=defocus0,
-                                           DefocusF=defocusF,
-                                           objLabel='Projections with CTF - [%.2f, %.2f]' % (defocus0, defocusF))
-
-        self.launchProtocol(protSimulateCTF)
-        return protSimulateCTF.outputParticles
-
-    def testSimulateCTF(self):
-        importedVolume = self.runImportVolume(self.volume, 1)
-        projectionsGallery = self.runCreateGallery(importedVolume)
-
-        # Check default defoci values
-        projectionsCTFDefault = self.runSimulateCTF(projectionsGallery)
-        self.assertTrue(projectionsCTFDefault,
-                        "There was a problem with particles output")
-        self.assertEqual(projectionsCTFDefault.getSize(),1647,
-                        "There was a problem with particles output")
-        self.assertEqual(projectionsCTFDefault.getXDim(),60,
-                        "Unexpected particle size in output particles")
-        self.assertEqual(projectionsCTFDefault.getSamplingRate(),1,
-                        "Unexpected sampling rate in output particles")
-        for projection in projectionsCTFDefault.iterItems():
-            defocusU = projection.getCTF().getDefocusU()
-            defocusV = projection.getCTF().getDefocusV()
-            self.assertEqual(defocusU,defocusV,'DefocusU and DeofcusV are not equal but they should be')
-            self.assertGreaterEqual(defocusU,5000, 'DefocusU and DefocusV values are outside the specified range:'
-                                    '[%f, %f]' % (5000, 25000))
-            self.assertLessEqual(defocusU,25000, 'DefocusU and DefocusV values are outside the specified range:'
-                                    '[%f, %f]' % (5000, 25000))
+        setupTestProject(cls)
+
+        # Data
+        cls.dataset = DataSet.getDataSet('10010')
+        cls.initialVolume = cls.dataset.getFile('initialVolume')
+        cls.particles = cls.dataset.getFile('particles')
+
+        cls.protImportVol = cls.runImportVolume(cls.initialVolume, 4.95)
+        cls.protImportParts = cls.runImportParticles()
+
+    def test(self):
+        subset = self.newProtocol(ProtSubSet,
+                                  inputFullSet=self.protImportParts.outputParticles,
+                                  chooseAtRandom=True,
+                                  nElements=400)
+        self.launchProtocol(subset)
+
+        highres = self.newProtocol(XmippProtReconstructHighRes,
+                                   inputParticles=subset.outputParticles,
+                                   inputVolumes=self.protImportVol.outputVolume,
+                                   particleRadius=180,
+                                   symmetryGroup="i1",
+                                   nextResolutionCriterion=0.143,
+                                   alignmentMethod=XmippProtReconstructHighRes.AUTOMATIC_ALIGNMENT,
+                                   maximumTargetResolution="15 10 7",
+                                   numberOfMpi=8)
+        self.launchProtocol(highres)
+        self.assertIsNotNone(highres.outputParticles,
+                             "There was a problem with Highres")
+
+        fnResolution = highres._getExtraPath("Iter005/iterInfo.xmd")
+        if not exists(fnResolution):
+            self.assertTrue(False, fnResolution + " does not exist")
+        else:
+            md = emlib.MetaData("resolution@" + fnResolution)
+            R = md.getValue(emlib.MDL_RESOLUTION_FREQREAL, md.firstObject())
+            self.assertTrue(R < 10, "Resolution is not below 10A")
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_validate_fscq.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_validate_fscq.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocol_validate_overfitting.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_validate_overfitting.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_add_noise.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_add_noise.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_continuousflex.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_continuousflex.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,36 @@
 from pwem.protocols import ProtImportPdb
 from pwem.tests.workflows import TestWorkflow
 from pyworkflow.tests import setupTestProject, DataSet
 from continuousflex.protocols import (FlexProtNMA, FlexProtSynthesizeSubtomo, FlexProtSynthesizeImages, NMA_CUTOFF_ABS,
                                       FlexProtAlignmentNMA, FlexProtSubtomogramAveraging)
 from continuousflex.protocols.protocol_subtomograms_synthesize import MODE_RELATION_3CLUSTERS
 
+files_dictionary = {'pdb': 'pdb/AK.pdb', 'particles': 'particles/img.stk', 'vol': 'volumes/AK_LP10.vol',
+                    'precomputed_atomic': 'gold/images_WS_atoms.xmd',
+                    'precomputed_pseudoatomic': 'gold/images_WS_pseudoatoms.xmd',
+                    'small_stk': 'test_alignment_10images/particles/smallstack_img.stk',
+                    'subtomograms':'HEMNMA_3D/subtomograms/*.vol',
+                    'precomputed_HEMNMA3D_atoms':'HEMNMA_3D/gold/precomputed_atomic.xmd',
+                    'precomputed_HEMNMA3D_pseudo':'HEMNMA_3D/gold/precomputed_pseudo.xmd',
+
+                    'charmm_prm':'genesis/par_all36_prot.prm',
+                    'charmm_top':'genesis/top_all36_prot.rtf',
+                    '1ake_pdb':'genesis/1ake.pdb',
+                    '1ake_vol':'genesis/1ake.mrc',
+                    '4ake_pdb':'genesis/4ake.pdb',
+                    '4ake_aa_pdb':'genesis/4ake_aa.pdb',
+                    '4ake_aa_psf':'genesis/4ake_aa.psf',
+                    '4ake_ca_pdb':'genesis/4ake_ca.pdb',
+                    '4ake_ca_top':'genesis/4ake_ca.top',
+                    }
+DataSet(name='nma_V2.0', folder='nma_V2.0', files=files_dictionary,
+        url='https://raw.githubusercontent.com/continuousflex-org/testdata-continuousflex/main')
+
+
 
 class TestContinuousFlexBasics(TestWorkflow):
     """ Test protocol for HEMNMA, HEMNMA-3D, StructMap, TomoFlow and STA backend functions. """
     @classmethod
     def setUpClass(cls):
         # Create a new project
         setupTestProject(cls)
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_deepVolPostprocessing.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_deepVolPostprocessing.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_deepres.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_deepres.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_fso.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_fso.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_gpuCorr_classifier.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_gpuCorr_classifier.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_gpuCorr_fullStreaming.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_gpuCorr_fullStreaming.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_gpuCorr_semiStreaming.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_gpuCorr_semiStreaming.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_highres.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_metaprotocol_golden_highres.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # **************************************************************************
 # *
-# * Authors:    Carlos Oscar Sorzano (coss@cnb.csic.es)
+# * Authors:    Amaya Jimenez Moreno (ajimenez@cnb.csic.es)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 2 of the License, or
 # * (at your option) any later version.
@@ -21,23 +21,19 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 from pyworkflow.tests import BaseTest, DataSet, setupTestProject
+from pwem.protocols import (ProtImportVolumes, ProtImportParticles, exists)
+from xmipp3.protocols import XmippMetaProtGoldenHighRes
 
-from pwem.protocols import (ProtImportVolumes, ProtImportParticles, ProtSubSet,
-                            exists)
 
-from pwem import emlib
-from xmipp3.protocols import XmippProtReconstructHighRes
-
-
-class TestHighres(BaseTest):
+class TestGoldenHighres(BaseTest):
     @classmethod
     def runImportVolume(cls, pattern, samplingRate):
         """ Run an Import volumes protocol. """
         cls.protImport = cls.newProtocol(ProtImportVolumes,
                                          filesPath=pattern,
                                          samplingRate=samplingRate
                                          )
@@ -73,33 +69,28 @@
         cls.initialVolume = cls.dataset.getFile('initialVolume')
         cls.particles = cls.dataset.getFile('particles')
 
         cls.protImportVol = cls.runImportVolume(cls.initialVolume, 4.95)
         cls.protImportParts = cls.runImportParticles()
 
     def test(self):
-        subset = self.newProtocol(ProtSubSet,
-                                  inputFullSet=self.protImportParts.outputParticles,
-                                  chooseAtRandom=True,
-                                  nElements=400)
-        self.launchProtocol(subset)
-
-        highres = self.newProtocol(XmippProtReconstructHighRes,
-                                   inputParticles=subset.outputParticles,
+        goldenHighres = self.newProtocol(XmippMetaProtGoldenHighRes,
+                                   inputParticles=self.protImportParts.outputParticles,
                                    inputVolumes=self.protImportVol.outputVolume,
                                    particleRadius=180,
                                    symmetryGroup="i1",
-                                   nextResolutionCriterion=0.143,
-                                   alignmentMethod=XmippProtReconstructHighRes.AUTOMATIC_ALIGNMENT,
-                                   maximumTargetResolution="15 10 7",
+                                   discardParticles=True,
                                    numberOfMpi=8)
-        self.launchProtocol(highres)
-        self.assertIsNotNone(highres.outputParticles,
-                             "There was a problem with Highres")
+        self.launchProtocol(goldenHighres)
+        self.assertIsNotNone(goldenHighres.outputParticlesLocal1,
+                             "There was a problem with Golden Highres")
 
-        fnResolution = highres._getExtraPath("Iter005/iterInfo.xmd")
+        fnResolution = goldenHighres._getExtraPath('fnFSCs.txt')
         if not exists(fnResolution):
             self.assertTrue(False, fnResolution + " does not exist")
         else:
-            md = emlib.MetaData("resolution@" + fnResolution)
-            R = md.getValue(emlib.MDL_RESOLUTION_FREQREAL, md.firstObject())
-            self.assertTrue(R < 10, "Resolution is not below 10A")
+            count = len(open(fnResolution).readlines())
+            count = count - 10
+            result = 'outputParticlesLocal%d' % (count)
+            o = getattr(goldenHighres, result, None)
+            locals()[result] = o
+            self.assertIsNotNone(o, "Output: %s is None" % result)
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_local_defocus.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_local_defocus.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,16 @@
         protSimulateCTF = self.newProtocol(XmippProtSimulateCTF)
         protSimulateCTF.inputParticles.set(self.protCreateGallery.outputReprojections)
         self.launchProtocol(protSimulateCTF)
         self.assertIsNotNone(protSimulateCTF.outputParticles, "There was a problem with CTF simulation")
 
         protEstimateLocalDefocus = self.newProtocol(XmippProtLocalCTF,
                                                     inputSet=protSimulateCTF.outputParticles,
-                                                    inputVolume=self.protCreatePhantom.outputVolume)
+                                                    inputVolume=self.protCreatePhantom.outputVolume,
+                                                    sameDefocus=True)
         self.launchProtocol(protEstimateLocalDefocus)
         self.assertIsNotNone(protEstimateLocalDefocus.outputParticles.getFiles(),
                              "There was a problem with local CTF estimation")
         self.assertEqual(protEstimateLocalDefocus.outputParticles.getDim(), (40, 40, 181),
                          "There was a problem with size of set of particles")
         self.assertEqual(protEstimateLocalDefocus.outputParticles.getFirstItem().getSamplingRate(), 4,
                          "There was a problem with the sampling rate value of output particles")
@@ -66,27 +67,29 @@
 
 
 class TestXmippLocalDefocusEstimationConsensus(TestXmippLocalDefocusEstimation):
     """ Testing local defocus estimation consensus """
 
     def testXmippLocalDefocusConsensus(self):
         protSimulateCTF2 = self.newProtocol(XmippProtSimulateCTF,
-                                            inputParticles=self.protCreateGallery.outputReprojections)
+                                            inputParticles=self.protCreateGallery.outputReprojections,
+                                            astig=True)
         self.launchProtocol(protSimulateCTF2)
         self.assertIsNotNone(protSimulateCTF2.outputParticles, "There was a problem with second CTF simulation")
 
         protEstimateLocalDefocus2 = self.newProtocol(XmippProtLocalCTF,
                                                      inputSet=protSimulateCTF2.outputParticles,
                                                      inputVolume=self.protCreatePhantom.outputVolume)
         self.launchProtocol(protEstimateLocalDefocus2)
         self.assertIsNotNone(protEstimateLocalDefocus2.outputParticles.getFiles(),
                              "There was a problem with second CTF estimation")
 
         protSimulateCTF3 = self.newProtocol(XmippProtSimulateCTF,
-                                            inputParticles=self.protCreateGallery.outputReprojections)
+                                            inputParticles=self.protCreateGallery.outputReprojections,
+                                            astig=True)
         self.launchProtocol(protSimulateCTF3)
         self.assertIsNotNone(protSimulateCTF3.outputParticles, "There was a problem with third CTF simulation")
 
         protEstimateLocalDefocus3 = self.newProtocol(XmippProtLocalCTF,
                                                      inputSet=protSimulateCTF3.outputParticles,
                                                      inputVolume=self.protCreatePhantom.outputVolume)
         self.launchProtocol(protEstimateLocalDefocus3)
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_localdeblur.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_localdeblur.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_metaprotocol_golden_highres.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocol_deep_center_predict.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # **************************************************************************
 # *
-# * Authors:    Amaya Jimenez Moreno (ajimenez@cnb.csic.es)
+# * Authors:    Adrian Sansinena Rodriguez  (adrian.sansinena@cnb.csic.es)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 2 of the License, or
 # * (at your option) any later version.
@@ -21,76 +21,75 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 from pyworkflow.tests import BaseTest, DataSet, setupTestProject
-from pwem.protocols import (ProtImportVolumes, ProtImportParticles, exists)
-from xmipp3.protocols import XmippMetaProtGoldenHighRes
 
+from pwem.protocols import (ProtImportParticles, ProtSubSet,
+                            exists)
+
+from pwem import emlib
+from xmipp3.protocols import XmippProtDeepCenterPredict, XmippProtDeepCenter
 
-class TestGoldenHighres(BaseTest):
-    @classmethod
-    def runImportVolume(cls, pattern, samplingRate):
-        """ Run an Import volumes protocol. """
-        cls.protImport = cls.newProtocol(ProtImportVolumes,
-                                         filesPath=pattern,
-                                         samplingRate=samplingRate
-                                         )
-        cls.launchProtocol(cls.protImport)
-        return cls.protImport
 
+class TestDeepCenterPredict(BaseTest):
     @classmethod
     def runImportParticles(cls):
         """ Import Particles.
         """
         args = {'importFrom': ProtImportParticles.IMPORT_FROM_SCIPION,
                 'sqliteFile': cls.particles,
                 'amplitudConstrast': 0.1,
                 'sphericalAberration': 2.0,
                 'voltage': 200,
                 'samplingRate': 0.99,
                 'haveDataBeenPhaseFlipped': True
                 }
 
-        # Id's should be set increasing from 1 if ### is not in the 
-        # pattern
         protImport = cls.newProtocol(ProtImportParticles, **args)
         protImport.setObjLabel('import particles')
         cls.launchProtocol(protImport)
         return protImport
 
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
 
         # Data
         cls.dataset = DataSet.getDataSet('10010')
-        cls.initialVolume = cls.dataset.getFile('initialVolume')
         cls.particles = cls.dataset.getFile('particles')
 
-        cls.protImportVol = cls.runImportVolume(cls.initialVolume, 4.95)
         cls.protImportParts = cls.runImportParticles()
 
     def test(self):
-        goldenHighres = self.newProtocol(XmippMetaProtGoldenHighRes,
-                                   inputParticles=self.protImportParts.outputParticles,
-                                   inputVolumes=self.protImportVol.outputVolume,
-                                   particleRadius=180,
-                                   symmetryGroup="i1",
-                                   discardParticles=True,
-                                   numberOfMpi=8)
-        self.launchProtocol(goldenHighres)
-        self.assertIsNotNone(goldenHighres.outputParticlesLocal1,
-                             "There was a problem with Golden Highres")
-
-        fnResolution = goldenHighres._getExtraPath('fnFSCs.txt')
-        if not exists(fnResolution):
-            self.assertTrue(False, fnResolution + " does not exist")
-        else:
-            count = len(open(fnResolution).readlines())
-            count = count - 10
-            result = 'outputParticlesLocal%d' % (count)
-            o = getattr(goldenHighres, result, None)
-            locals()[result] = o
-            self.assertIsNotNone(o, "Output: %s is None" % result)
+        subset = self.newProtocol(ProtSubSet,
+                                  inputFullSet=self.protImportParts.outputParticles,
+                                  chooseAtRandom=True,
+                                  nElements=400)
+        self.launchProtocol(subset)
+
+        deepCenter = self.newProtocol(XmippProtDeepCenter,
+                                   inputTrainSet=subset.outputParticles,
+                                   Xdim=128,
+                                   modelPretrain=False,
+                                   numCenModels=5,
+                                   numEpochs_cen=1,
+                                   batchSize=32,
+                                   learningRate=0.001,
+                                   sigma=8,
+                                   patience=5)
+        self.launchProtocol(deepCenter)
+
+        deepCenterPredict = self.newProtocol(XmippProtDeepCenterPredict,
+                                      inputImageSet=subset.outputParticles,
+                                      Xdim=128,
+                                      inputModel=deepCenter,
+                                      numModels=5,
+                                      tolerance=2,
+                                      maxModels=1)
+        self.launchProtocol(deepCenterPredict)
+
+        self.assertIsNotNone(deepCenterPredict.outputParticles,
+                             "There was a problem with Deep Center Predict")
+
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_mixed_movies.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_mixed_movies.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_monores.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_monores.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_realignment_classes.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_realignment_classes.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_solid_angles.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_solid_angles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_xmipp_2d.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_xmipp_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1137,41 +1137,14 @@
                          inputAlignFirstPartTransMat[2, 3]]  # Z translation
 
         self.assertFalse(all(v == 0 for v in inTranslation))
         self.assertFalse(all(v == 0 for v in outTranslation))
         [self.assertAlmostEqual(inT * scale, outT) for inT, outT in zip(inTranslation, outTranslation)]
 
 
-class TestXmippRotSpectra(TestXmippBase):
-    """This class check if the protocol to calculate the rotational spectra from particles in Xmipp works properly."""
-    @classmethod
-    def setUpClass(cls):
-        setupTestProject(cls)
-        TestXmippBase.setData('mda')
-        cls.protImport = cls.runImportParticles(cls.particlesFn, 3.5)
-        cls.align2D = cls.runCL2DAlign(cls.protImport.outputParticles)
-         
-    def test_rotSpectra(self):
-        print("Run Rotational Spectra")
-        xmippProtRotSpectra = self.newProtocol(XmippProtRotSpectra, SomXdim=2, SomYdim=2)
-        xmippProtRotSpectra.inputParticles.set(self.align2D.outputParticles)
-        self.launchProtocol(xmippProtRotSpectra)        
-        self.assertIsNotNone(xmippProtRotSpectra.outputClasses, "There was a problem with Rotational Spectra")
-
-    def test_rotSpectraMask(self):
-        print("Run Rotational Spectra with Mask")
-        protMask = self.runCreateMask(3.5, 100)
-        xmippProtRotSpectra = self.newProtocol(XmippProtRotSpectra, useMask=True, SomXdim=2, SomYdim=2)
-        xmippProtRotSpectra.inputParticles.set(self.align2D.outputParticles)
-        xmippProtRotSpectra.useMask.set(True)
-        xmippProtRotSpectra.Mask.set(protMask.outputMask)
-        self.launchProtocol(xmippProtRotSpectra)
-        self.assertIsNotNone(xmippProtRotSpectra.outputClasses, "There was a problem with Rotational Spectra")
-
-
 class TestXmippKerdensom(TestXmippBase):
     """This class check if the protocol to calculate the kerdensom from particles in Xmipp works properly."""
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         TestXmippBase.setData('mda')
         cls.protImport = cls.runImportParticles(cls.particlesFn, 3.5)
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_xmipp_3d.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_xmipp_3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,27 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
+# General imports
+import os.path, shutil
+
+# Scipion em imports
+from pwem.convert import Ccp4Header
 from pwem.protocols import (ProtImportVolumes, ProtImportMask,
                             ProtImportParticles, ProtImportAverages,
-                            ProtImportPdb, ProtSubSet)
-from xmipp3.protocols.protocol_align_volume_and_particles import AlignVolPartOutputs
-
-try:
-    from itertools import izip
-except ImportError:
-    izip = zip
-
+                            ProtImportPdb, ProtSubSet, ProtImportSetOfAtomStructs)
 from pyworkflow.utils import greenStr, magentaStr
 from pyworkflow.tests import *
+
+# Plugin imports
+from xmipp3.protocols.protocol_align_volume_and_particles import AlignVolPartOutputs
 from xmipp3.base import *
 from xmipp3.convert import *
 from xmipp3.constants import *
 from xmipp3.protocols import *
 from xmipp3.protocols import (XmippFilterHelper as xfh,
                               XmippResizeHelper as xrh,
                               OP_COLUNM, OP_DOTPRODUCT, OP_MULTIPLY,
@@ -65,14 +66,16 @@
 MSG_WRONG_SIZE = "There was a problem with the size of the output "
 MSG_WRONG_DIM = "There was a problem with the dimensions of the output "
 MSG_WRONG_MASK = "There was a problem with create mask from volume"
 MSG_WRONG_ALIGNMENT = "There was a problem with the alignment of the output "
 MSG_WRONG_SHIFT = "There was a problem with output shift "
 MSG_WRONG_GALLERY = "There was a problem with the gallery creation"
 MSG_WRONG_ROTATION = "There was a problem with the rotation"
+MSG_WRONG_RECONSTRUCTION = "There was a problem with the reconstruction"
+MSG_WRONG_MERGER = "There was a problem with the merger of the "
 MSG_WRONG_IMPORT = "There was a problem with the import of "
 MSG_WRONG_PROTOCOL = "There was a problem with the protocol: "
 MSG_WRONG_MAP = "There was a problem with the map creation"
 
 class TestXmippBase(BaseTest):
     """ Some utility functions to import volumes that are used in several tests."""
 
@@ -1028,15 +1031,14 @@
                                          tilt0=70,
                                          tiltF=110)
         protRotSym.inputVolume.set(protImportVol.outputVolume)
         self.launchProtocol(protRotSym)
         self.assertIsNotNone(protRotSym.outputVolume,
                              "There was a problem with Rotational Symmetry")
 
-
 class TestXmippProjMatching(TestXmippBase):
 
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         cls.dataset = DataSet.getDataSet('relion_tutorial')
         cls.vol = cls.dataset.getFile('volume')
@@ -1049,44 +1051,43 @@
                                  sqliteFile=self.dataset.getFile('import/case2/particles.sqlite'),
                                  magnification=50000,
                                  samplingRate=7.08,
                                  haveDataBeenPhaseFlipped=True
                                  )
         self.launchProtocol(protImportParts)
         self.assertIsNotNone(protImportParts.getFiles(), "There was a problem with the import")
-        
+
         print("Get a Subset of particles")
         protSubset = self.newProtocol(ProtSubSet,
                                          objLabel='100 Particles',
                                          chooseAtRandom=True,
                                          nElements=100)
         protSubset.inputFullSet.set(protImportParts.outputParticles)
         self.launchProtocol(protSubset)
-        
+
         print("Import Volume")
         protImportVol = self.newProtocol(ProtImportVolumes,
                                          objLabel='Volume',
                                          filesPath=self.vol,
                                          samplingRate=7.08)
         self.launchProtocol(protImportVol)
         self.assertIsNotNone(protImportVol.getFiles(), "There was a problem with the import")
-        
+
         print("Run Projection Matching")
         protProjMatch = self.newProtocol(XmippProtProjMatch,
                                          ctfGroupMaxDiff=0.00001,
                                          mpiJobSize=10,
                                          numberOfIterations=2,
                                          numberOfThreads=2,
                                          numberOfMpi=3)
         protProjMatch.inputParticles.set(protSubset.outputParticles)
         protProjMatch.input3DReferences.set(protImportVol.outputVolume)
         self.launchProtocol(protProjMatch)
         self.assertIsNotNone(protProjMatch.outputVolume, "There was a problem with Projection Matching")
 
-
 class TestPdbImport(TestXmippBase):
     
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         cls.dataset = DataSet.getDataSet('nma')
         cls.pdb = cls.dataset.getFile('pdb')
@@ -1105,60 +1106,96 @@
                                        pdbFile=self.pdb)
         self.launchProtocol(protConvert)
         self.assertIsNotNone(protConvert.outputPdb.getFileName(), 
                              "There was a problem with the import")
 
 
 class TestXmippPdbConvert(TestXmippBase):
-    
     @classmethod
     def setUpClass(cls):
+        """ This function prepares the project before instantiating and running any protocol. """
         setupTestProject(cls)
         cls.dataset = DataSet.getDataSet('nma')
         cls.pdb = cls.dataset.getFile('pdb')
     
-    def testXmippPdbConvertFromDb(self):
-        print("Run convert a pdb from database")
-        protConvert = self.newProtocol(XmippProtConvertPdb, pdbId="3j3i", sampling=4, setSize=True,
-                                       size_z=100, size_y=100, size_x=100)
-        self.launchProtocol(protConvert)
-        self.assertIsNotNone(protConvert.outputVolume.getFileName(), "There was a problem with the conversion")
-        self.assertAlmostEqual(protConvert.outputVolume.getSamplingRate(), protConvert.sampling.get(), places=1,
-                               msg=(MSG_WRONG_SAMPLING, "volume"))
-        self.assertAlmostEqual(protConvert.outputVolume.getDim()[0], protConvert.size_z.get(), places=1,
-                               msg=(MSG_WRONG_SIZE, "volume"))
-        
-    def testXmippPdbConvertFromObj(self):
+    def test1XmippSinglePdb(self):
+        """ This function runs a test with a single pdb as input. """
         print("Run convert a pdb from import")
+
+        # Creating and launching import protocol to obtain input pdb
         protImport = self.newProtocol(ProtImportPdb, 
                                       inputPdbData=ProtImportPdb.IMPORT_FROM_FILES, 
                                       pdbFile=self.pdb)
         self.launchProtocol(protImport)
         self.assertIsNotNone(protImport.outputPdb.getFileName(), "There was a problem with the import")
         
+        # Creating and launching convert to pdb protocol
         protConvert = self.newProtocol(XmippProtConvertPdb, 
-                                       inputPdbData=XmippProtConvertPdb.IMPORT_OBJ, 
-                                       sampling=3, setSize=True, size_z=20, size_y=20, size_x=20)
+                                       numberOfMpi=1, sampling=3, setSize=True, size_z=20, size_y=20, size_x=20)
         protConvert.pdbObj.set(protImport.outputPdb)
         self.launchProtocol(protConvert)
-        self.assertIsNotNone(protConvert.outputVolume.getFileName(), "There was a problem with the conversion")
-        self.assertAlmostEqual(protConvert.outputVolume.getSamplingRate(), protConvert.sampling.get(), places=1,
+
+        # Obtaining output and analyzing results
+        volume = getattr(protConvert, protConvert.OUTPUT_NAME1, None)
+        volumeFn = volume.getFileName()
+        self.assertTrue(volumeFn.endswith(".mrc"), "Output volume form converting a pdb is not an mrc")
+        ccp4header = Ccp4Header(volumeFn, readHeader=True)
+        headerSr = ccp4header.getSampling()[0]
+        self.assertAlmostEquals(volume.getSamplingRate(), headerSr, "%s header for sampling rate is wrong." % volumeFn)
+
+        self.assertAlmostEqual(volume.getSamplingRate(), protConvert.sampling.get(), places=1,
                                msg=(MSG_WRONG_SAMPLING, "volume"))
-        self.assertAlmostEqual(protConvert.outputVolume.getDim()[0], protConvert.size_z.get(), places=1,
+        self.assertAlmostEqual(volume.getDim()[0], protConvert.size_z.get(), places=1,
                                msg=(MSG_WRONG_SIZE, "volume"))
 
-    def testXmippPdbConvertFromFn(self):
-        print("Run convert a pdb from file")
-        protConvert = self.newProtocol(XmippProtConvertPdb,inputPdbData=2, pdbFile=self.pdb, sampling=2, setSize=False)
+    def test2XmippPdbSet(self):
+        """ This function runs a test with a set of pdbs as input. """
+        print("Run convert a set of pdbs")
+
+        # Defining data path
+        dataPath = os.path.dirname(self.pdb)
+
+        # Obtaining list of pdb files inside folder
+        files = os.listdir(dataPath)
+        pdbFiles = [pdbFile for pdbFile in files if pdbFile.endswith('.pdb')]
+
+        # If there is only one .pdb file, duplicate it so we can have a set with at least two atom structures
+        tmpFiles = []
+        if len(pdbFiles) < 2:
+            newFile = pdbFiles[0].replace('.pdb', '_tmp.pdb')
+            shutil.copyfile(os.path.join(dataPath, pdbFiles[0]), os.path.join(dataPath, newFile))
+            tmpFiles.append(newFile)
+
+        # Creating and launching import protocol to obtain input pdbs
+        protImport = self.newProtocol(ProtImportSetOfAtomStructs,
+                                      inputPdbData=ProtImportSetOfAtomStructs.IMPORT_FROM_FILES,
+                                      filesPath=dataPath)
+        self.launchProtocol(protImport)
+        self.assertIsNotNone(protImport.outputAtomStructs.getFirstItem().getFileName(), "There was a problem with the import")
+
+        # Creating and launching convert to pdb protocol
+        protConvert = self.newProtocol(XmippProtConvertPdb, numberOfMpi=1, numberOfThreads=2, sampling=3, size=20)
+        protConvert.pdbObj.set(protImport.outputAtomStructs)
         self.launchProtocol(protConvert)
-        self.assertIsNotNone(protConvert.outputVolume.getFileName(), "There was a problem with the conversion")
-        self.assertAlmostEqual(protConvert.outputVolume.getSamplingRate(), protConvert.sampling.get(), places=1,
-                               msg=(MSG_WRONG_SAMPLING, "volume"))
-        self.assertAlmostEqual(protConvert.outputVolume.getDim()[0], 48, places=1, msg=(MSG_WRONG_SIZE, "volume"))
 
+        # Deleting tmp files if there were any
+        for tmpFile in tmpFiles:
+            os.remove(os.path.join(dataPath, tmpFile))
+
+        # Obtaining output and analyzing results
+        volumes = getattr(protConvert, protConvert.OUTPUT_NAME2, None)
+        volumeFn = volumes.getFirstItem().getFileName()
+        self.assertTrue(volumeFn.endswith(".mrc"), "Output volume form converting a pdb is not an mrc")
+        ccp4header = Ccp4Header(volumeFn, readHeader=True)
+        headerSr = ccp4header.getSampling()[0]
+        self.assertAlmostEquals(volumes.getSamplingRate(), headerSr, "%s header for sampling rate is wrong." % volumeFn)
+        self.assertAlmostEqual(volumes.getSamplingRate(), protConvert.sampling.get(), places=1,
+                               msg=(MSG_WRONG_SAMPLING, "volumes"))
+        self.assertAlmostEqual(volumes.getDim()[0], protConvert.size.get(), places=1,
+                               msg=(MSG_WRONG_SIZE, "volumes"))
 
 class TestXmippValidateNonTilt(TestXmippBase):
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         cls.dataset = DataSet.getDataSet('relion_tutorial')
         cls.vol = cls.dataset.getFile('volume')
@@ -1510,28 +1547,19 @@
         protCreateMaskKeep = self.newProtocol(XmippProtCreateMask3D,
                                               inputVolume=protCreatePhantom1item.outputVolume,
                                               threshold=0.1)
         self.launchProtocol(protCreateMaskKeep)
         self.assertIsNotNone(protCreateMaskKeep.getFiles(),
                              "There was a problem with the 3D mask of the 1 item phantom")
 
-        # Subtraction of particles - reference volume with and without mask
-        protSubtractProj = self.newProtocol(XmippProtSubtractProjection,
-                                            inputParticles=protCreateGallery.outputReprojections,
-                                            vol=protCreatePhantom1item.outputVolume)
-        self.launchProtocol(protSubtractProj)
-        self.assertIsNotNone(protSubtractProj.outputParticles,
-                             "There was a problem with projection subtraction")
-        self.assertEqual(protSubtractProj.outputParticles.getSamplingRate(), 1.0, (MSG_WRONG_SAMPLING, "particles"))
-        self.assertEqual(protSubtractProj.outputParticles.getFirstItem().getDim(), (80, 80, 1),
-                         (MSG_WRONG_DIM, "particles"))
-        self.assertEqual(protSubtractProj.outputParticles.getSize(), 181, (MSG_WRONG_SIZE, "particles"))
+        # Subtraction of particles - reference volume with mask
         protSubtractProjMask = self.newProtocol(XmippProtSubtractProjection,
                                                 inputParticles=protCreateGallery.outputReprojections,
                                                 vol=protCreatePhantom2items.outputVolume,
+                                                subtract=1,
                                                 mask=protCreateMaskKeep.outputMask)
         self.launchProtocol(protSubtractProjMask)
         self.assertIsNotNone(protSubtractProjMask.outputParticles,
                              "There was a problem with projection subtraction with mask")
         self.assertEqual(protSubtractProjMask.outputParticles.getSamplingRate(), 1.0, (MSG_WRONG_SAMPLING, "particles"))
         self.assertEqual(protSubtractProjMask.outputParticles.getFirstItem().getDim(), (80, 80, 1),
                          (MSG_WRONG_DIM, "particles"))
@@ -1541,15 +1569,17 @@
         protSimulateCTF = self.newProtocol(XmippProtSimulateCTF,
                                            inputParticles=protCreateGallery.outputReprojections)
         self.launchProtocol(protSimulateCTF)
         self.assertIsNotNone(protSimulateCTF.outputParticles,
                              "There was a problem with CTF simulation")
         protSubtractProjCTF = self.newProtocol(XmippProtSubtractProjection,
                                                inputParticles=protSimulateCTF.outputParticles,
-                                               vol=protCreatePhantom1item.outputVolume)
+                                               vol=protCreatePhantom1item.outputVolume,
+                                               subtract=1,
+                                               mask=protCreateMaskKeep.outputMask)
         self.launchProtocol(protSubtractProjCTF)
         self.assertIsNotNone(protSubtractProjCTF.outputParticles,
                              "There was a problem with projection subtraction CTF")
         self.assertEqual(protSubtractProjCTF.outputParticles.getSamplingRate(), 1.0, (MSG_WRONG_SAMPLING, "particles"))
         self.assertEqual(protSubtractProjCTF.outputParticles.getFirstItem().getDim(), (80, 80, 1),
                          (MSG_WRONG_DIM, "particles"))
         self.assertEqual(protSubtractProjCTF.outputParticles.getSize(), 181, (MSG_WRONG_SIZE, "particles"))
@@ -1557,15 +1587,17 @@
                                         input=protCreateGallery.outputReprojections,
                                         gaussianStd=15.0)
         self.launchProtocol(protAddNoise)
         self.assertIsNotNone(protAddNoise.outputParticles,
                              "There was a problem with add noise protocol")
         protSubtractProjNoise = self.newProtocol(XmippProtSubtractProjection,
                                                  inputParticles=protAddNoise.outputParticles,
-                                                 vol=protCreatePhantom1item.outputVolume)
+                                                 vol=protCreatePhantom1item.outputVolume,
+                                                 subtract=1,
+                                                 mask=protCreateMaskKeep.outputMask)
         self.launchProtocol(protSubtractProjNoise)
         self.assertIsNotNone(protSubtractProjNoise.outputParticles,
                              "There was a problem with projection subtraction with noise")
         self.assertEqual(protSubtractProjNoise.outputParticles.getSamplingRate(), 1.0, (MSG_WRONG_SAMPLING, "particles"))
         self.assertEqual(protSubtractProjNoise.outputParticles.getFirstItem().getDim(), (80, 80, 1),
                          (MSG_WRONG_DIM, "particles"))
         self.assertEqual(protSubtractProjNoise.outputParticles.getSize(), 181, (MSG_WRONG_SIZE, "particles"))
@@ -1573,15 +1605,17 @@
                                            input=protSimulateCTF.outputParticles,
                                            gaussianStd=15.0)
         self.launchProtocol(protAddNoiseCTF)
         self.assertIsNotNone(protAddNoiseCTF.outputParticles,
                              "There was a problem with add noise to ctf particles protocol")
         protSubtractProjNoiseCTF = self.newProtocol(XmippProtSubtractProjection,
                                                     inputParticles=protAddNoiseCTF.outputParticles,
-                                                    vol=protCreatePhantom1item.outputVolume)
+                                                    vol=protCreatePhantom1item.outputVolume,
+                                                    subtract=1,
+                                                    mask=protCreateMaskKeep.outputMask)
         self.launchProtocol(protSubtractProjNoiseCTF)
         self.assertIsNotNone(protSubtractProjNoiseCTF.outputParticles,
                              "There was a problem with projection subtraction with noise and CTF")
         self.assertEqual(protSubtractProjNoiseCTF.outputParticles.getSamplingRate(), 1.0, (MSG_WRONG_SAMPLING, "particles"))
         self.assertEqual(protSubtractProjNoiseCTF.outputParticles.getFirstItem().getDim(), (80, 80, 1),
                          (MSG_WRONG_DIM, "particles"))
         self.assertEqual(protSubtractProjNoiseCTF.outputParticles.getSize(), 181, (MSG_WRONG_SIZE, "particles"))
@@ -1613,25 +1647,28 @@
         self.assertIsNotNone(protCreateMaskKeepOver.getFiles(),
                              "There was a problem with the 3D mask of the 1 item overlap phantom")
 
         # Perform subtraction of overlapping particles with and without mask, noise and CTF
         protSubtractProjOver = self.newProtocol(XmippProtSubtractProjection,
                                                 inputParticles=protCreateGalleryOver.outputReprojections,
                                                 vol=protCreatePhantom2Over.outputVolume,
-                                                mask=protCreateMaskKeepOver.outputMask)
+                                                mask=protCreateMaskKeepOver.outputMask,
+                                                subtract=1)
         self.launchProtocol(protSubtractProjOver)
         self.assertIsNotNone(protSubtractProjOver.outputParticles,
                              "There was a problem with projection subtraction with overlap")
         self.assertEqual(protSubtractProjOver.outputParticles.getSamplingRate(), 1.0, (MSG_WRONG_SAMPLING, "particles"))
         self.assertEqual(protSubtractProjOver.outputParticles.getFirstItem().getDim(), (80, 80, 1),
                          (MSG_WRONG_DIM, "particles"))
         self.assertEqual(protSubtractProjOver.outputParticles.getSize(), 1647, (MSG_WRONG_SIZE, "particles"))
         protSubtractProjOverNoMask = self.newProtocol(XmippProtSubtractProjection,
                                                       inputParticles=protCreateGalleryOver.outputReprojections,
-                                                      vol=protCreatePhantom1Over.outputVolume)
+                                                      vol=protCreatePhantom1Over.outputVolume,
+                                                      mask=protCreateMaskKeepOver.outputMask,
+                                                      subtract=1)
         self.launchProtocol(protSubtractProjOverNoMask)
         self.assertIsNotNone(protSubtractProjOverNoMask.outputParticles,
                              "There was a problem with projection subtraction with overlap")
         self.assertEqual(protSubtractProjOverNoMask.outputParticles.getSamplingRate(), 1.0, (MSG_WRONG_SAMPLING, "particles"))
         self.assertEqual(protSubtractProjOverNoMask.outputParticles.getFirstItem().getDim(), (80, 80, 1),
                          (MSG_WRONG_DIM, "particles"))
         self.assertEqual(protSubtractProjOverNoMask.outputParticles.getSize(), 1647, (MSG_WRONG_SIZE, "particles"))
@@ -1644,15 +1681,17 @@
                                                input=protSimulateCTFOver.outputParticles,
                                                gaussianStd=15.0)
         self.launchProtocol(protAddNoiseCTFOver)
         self.assertIsNotNone(protAddNoiseCTFOver.outputParticles,
                              "There was a problem with add noise to ctf overlap particles protocol")
         protSubtractProjNoiseCTFOver = self.newProtocol(XmippProtSubtractProjection,
                                                         inputParticles=protAddNoiseCTFOver.outputParticles,
-                                                        vol=protCreatePhantom1Over.outputVolume)
+                                                        vol=protCreatePhantom1Over.outputVolume,
+                                                        mask=protCreateMaskKeepOver.outputMask,
+                                                        subtract=1)
         self.launchProtocol(protSubtractProjNoiseCTFOver)
         self.assertIsNotNone(protSubtractProjNoiseCTFOver.outputParticles,
                              "There was a problem with projection subtraction with noise and CTF overlap")
         self.assertEqual(protSubtractProjNoiseCTFOver.outputParticles.getSamplingRate(), 1.0, (MSG_WRONG_SAMPLING, "particles"))
         self.assertEqual(protSubtractProjNoiseCTFOver.outputParticles.getFirstItem().getDim(), (80, 80, 1),
                          (MSG_WRONG_DIM, "particles"))
         self.assertEqual(protSubtractProjNoiseCTFOver.outputParticles.getSize(), 1647, (MSG_WRONG_SIZE, "particles"))
@@ -2527,14 +2566,56 @@
         self.assertEqual(protRotateVolume2.deg.get(), 90, "The degree of rotation is wrong")
         self.assertEqual(protRotateVolume2.outputVolume.getDim(), protCreatePhantomReference.outputVolume.getDim(),
                          (MSG_WRONG_DIM, "phantom (initially rotated)"))
         self.assertEqual(protRotateVolume2.outputVolume.getSamplingRate(),
                          protCreatePhantomReference.outputVolume.getSamplingRate(),
                          (MSG_WRONG_SAMPLING, "rotated phantom"))
 
+class TestXmippReconstructSignificant(TestXmippBase):
+    """This class checks if the protocol reconstruct significant in Xmipp works properly."""
+    @classmethod
+    def setUpClass(cls):
+        setupTestProject(cls)
+
+    def testXmippReconstructSignificant(self):
+        # Create input data: phantom with one cylinder
+        protCreatePhantom1 = self.newProtocol(XmippProtPhantom,
+                                               desc='80 80 80 0\ncyl + 5 0 0 0 5 5 10 0 0 0',
+                                               sampling=1.0)
+        self.launchProtocol(protCreatePhantom1)
+        self.assertIsNotNone(protCreatePhantom1.getFiles(),
+                             "There was a problem with the phantom creation")
+        # Create particles from the first phantom
+        protCreateGallery = self.newProtocol(XmippProtCreateGallery,
+                                             inputVolume=protCreatePhantom1.outputVolume,
+                                             rotStep=15.0,
+                                             tiltStep=90.0)
+        self.launchProtocol(protCreateGallery)
+        self.assertIsNotNone(protCreateGallery.getFiles(),
+                             MSG_WRONG_GALLERY)
+        # Reconstruct significant (default values)
+        protReconstructSignificant = self.newProtocol(XmippProtReconstructSignificant,
+                                                      inputSet=protCreateGallery.outputReprojections)
+        self.launchProtocol(protReconstructSignificant)
+        self.assertIsNotNone(protReconstructSignificant.getFiles(),
+                             MSG_WRONG_RECONSTRUCTION)
+        self.assertIsNotNone(protReconstructSignificant.outputVolume,
+                             (MSG_WRONG_RECONSTRUCTION, " of the final volume"))
+        # Reconstruct significant (default values) with a reference volume
+        protReconstructSignificant2 = self.newProtocol(XmippProtReconstructSignificant,
+                                                       inputSet=protCreateGallery.outputReprojections,
+                                                       thereisRefVolume=True,
+                                                       refVolume=protCreatePhantom1.outputVolume)
+        self.launchProtocol(protReconstructSignificant2)
+        self.assertIsNotNone(protReconstructSignificant2.getFiles(),
+                             MSG_WRONG_RECONSTRUCTION)
+        self.assertIsNotNone(protReconstructSignificant2.outputVolume,
+                             (MSG_WRONG_RECONSTRUCTION, " of the final volume"))
+
+
 class TestXmippDeepHand(TestXmippBase):
     """This class checks if the protocol deep hand in Xmipp works properly."""
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         cls.dataset = DataSet.getDataSet(db_general)
         cls.vol1 = cls.dataset.getFile(helix)
@@ -2565,15 +2646,15 @@
         # Check if the thresholdAlpha and thresholdHand match the default values
         self.assertEqual(protDeepHand.thresholdAlpha.get(), 0.7, "There was a problem with the thresholdAlpha value")
         self.assertEqual(protDeepHand.thresholdHand.get(), 0.6, "There was a problem with the thresholdHand value")
         # Check if the dimension of the volume does not vary
         self.assertEqual(protDeepHand.outputVol.getDim(), protImportVol.outputVolume.getDim(),
                          (MSG_WRONG_DIM, "volume"))
         # Check if the hand value is right
-        self.assertAlmostEquals(protDeepHand.outputHand.get(), 0.380511, 6,"There was a problem with the hand value")
+        self.assertAlmostEquals(protDeepHand.outputHand.get(), 0.3805, 4,"There was a problem with the hand value")
         # Check if the flip is right
         self.assertTrue(protDeepHand.outputHand.get()<protDeepHand.thresholdHand.get(), "There was a problem with the flip")
 
 class TestXmippResolutionBfactor(TestXmippBase):
     """This class checks if the protocol resolution b factor in Xmipp works properly."""
     @classmethod
     def setUpClass(cls):
@@ -2630,15 +2711,14 @@
         print("Protocol local resolution/local bfactor")
         protbfactorResolution = self.newProtocol(XmippProtbfactorResolution,
                                                  pdbfile=protImportPdb.outputPdb,
                                                  localResolutionMap=protCreateMap.resolution_Volume,
                                                  fscResolution=8.35)
         self.launchProtocol(protbfactorResolution)
 
-
 if __name__ == "__main__":
     if len(sys.argv) > 1:
         className = sys.argv[1]
         cls = globals().get(className, None)
         if cls:
             suite = unittest.TestLoader().loadTestsFromTestCase(cls)
             unittest.TextTestRunner(verbosity=2).run(suite)
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_xmipp_mics.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_xmipp_mics.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,38 +286,14 @@
         ctfModel = protCTF.outputCTF.getFirstItem()
         self.assertAlmostEquals(ctfModel.getDefocusU(),23928.4, delta=500)
         self.assertAlmostEquals(ctfModel.getDefocusV(),23535.2, delta=500)
         self.assertAlmostEquals(ctfModel.getDefocusAngle(), 60.0, delta=20)
         sampling = ctfModel.getMicrograph().getSamplingRate()
         self.assertAlmostEquals(sampling, 2.474, delta=0.001)
 
-class TestXmippBoxsize(TestXmippBase):
-    """This class check if the protocol to determine the BoxSize in Xmipp works properly."""
-    @classmethod
-    def setUpClass(cls):
-        setupTestProject(cls)
-        TestXmippBase.setData()
-        fileName = DataSet.getDataSet('relion_tutorial').getFile('allMics')
-        cls.protImport = cls.runImportMicrograph(fileName,
-                                                 samplingRate=3.54,
-                                                 voltage=300,
-                                                 sphericalAberration=2,
-                                                 scannedPixelSize=None,
-                                                 magnification=56000)
-    def test1(self):
-        #TODO: CHECK IF THE PREDICTIONS ON MIC MATCH THE PREDICTIONS ON DOWNSAMPLED MICS
-        # Estimate CTF on the downsampled micrographs
-        print("Estimating boxsize...")
-        protCTF = XmippProtParticleBoxsize()
-        protCTF.inputMicrographs.set(self.protImport.outputMicrographs)
-        self.proj.launchProtocol(protCTF, wait=True)
-        self.assertIsNotNone(protCTF.boxsize, "Boxsize has not been produced.")
-        self.assertAlmostEquals(protCTF.boxsize.get(), 50, delta=20,
-                                msg='Wrong estimated boxsize.')
-
 
 class TestXmippAutomaticPicking(TestXmippBase):
     """This class check if the protocol to pick the micrographs automatically in Xmipp works properly."""
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         TestXmippBase.setData()
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_xmipp_movie_resize.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_xmipp_movie_resize.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_xmipp_movies.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_xmipp_movies.py`

 * *Files 3% similar despite different names*

```diff
@@ -788,7 +788,85 @@
         protDoMic = self.doFilter(self.alignedMovMics, rejType, label, mxMo=5)
         self._checkMaxShiftFiltering(protDoMic, label, hasMic=True, results=[True, True])
 
         protDoMic = self.doFilter(self.alignedMovDwMics, rejType, label)
         self._checkMaxShiftFiltering(protDoMic, label, hasMic=True,
                                      hasDw=True, results=[True, True])
 
+
+class TestMovieDoseAnalysis(BaseTest):
+
+    @classmethod
+    def setData(cls):
+        setupTestProject(cls)
+        cls.ds = DataSet.getDataSet('relion30_tutorial')
+
+    @classmethod
+    def runImportMovies(cls):
+        protImport = cls.newProtocol(
+            ProtImportMovies,
+            filesPath=cls.ds.getFile('Movies/'),
+            filesPattern='*.tiff',
+            samplingRateMode=0,
+            samplingRate=0.885,
+            magnification=50000,
+            scannedPixelSize=7.0,
+            voltage=200,
+            sphericalAberration=1.4,
+            doseInitial=0.0,
+            dosePerFrame=1.277,
+            gainFile=cls.ds.getFile("Movies/gain.mrc")
+        )
+        protImport.setObjLabel('import 24 movies')
+        protImport.setObjComment('Relion 3 tutorial movies:\n\n'
+                                 'Microscope Jeol Cryo-ARM 200\n'
+                                 'Data courtesy of Takyuki Kato in the Namba '
+                                 'group\n(Osaka University, Japan)')
+        return cls.launchProtocol(protImport)
+
+
+    @classmethod
+    def setUpClass(cls):
+        setupTestProject(cls)
+        cls.setData()
+        cls.protImport = cls.runImportMovies()
+
+    # ------- Tests ---------------------------------------
+    def testDoseAnalysisAssert(self):
+        """ This must create two sets of movies.
+        """
+        label = 'Dose Analysis Assert'
+        protPoisson = self.newProtocol(XmippProtMovieDoseAnalysis,
+                                       objLabel=label,
+                                       n_samples=10,
+                                       movieStep=4
+                                       )
+        protPoisson.inputMovies.set(self.protImport.outputMovies)
+        self.launchProtocol(protPoisson)
+
+        self.assertIsNotNone(getattr(protPoisson, 'outputMoviesDiscarded', None),
+                          "outputMoviesDiscarded were not created. "
+                          "Bad filtering in test.")
+
+        self.assertIsNotNone(getattr(protPoisson, 'outputMovies', None),
+                             "outputMovies were not created. "
+                             "Bad filtering in test.")
+
+    def testDoseAnalysisFiltering(self):
+        """ This must discard movies by dose analysis.
+        """
+        label = 'Dose Analysis Filter'
+        protPoisson = self.newProtocol(XmippProtMovieDoseAnalysis,
+                                       objLabel=label,
+                                       n_samples=24,
+                                       movieStep=4
+                                       )
+        protPoisson.inputMovies.set(self.protImport.outputMovies)
+        self.launchProtocol(protPoisson)
+
+        sizeAccepted = protPoisson.outputMovies.getSize()
+        self.assertEqual(sizeAccepted, 19, 'Number of accepted movies must be 19 and its '
+                                           '%d' % sizeAccepted)
+
+        sizeDiscarded = protPoisson.outputMoviesDiscarded.getSize()
+        self.assertEqual(sizeDiscarded, 5, 'Number of accepted movies must be 5 and its '
+                                            '%d' % sizeDiscarded)
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/tests/test_protocols_zernike3d.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/tests/test_protocols_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/utils.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/__init__.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 from .viewer import XmippViewer
 from .plotter import XmippPlotter
 
+from .viewer_angular_resolution_alignment import XmippProtAngResAlignViewer
 from .viewer_cl2d import XmippCL2DViewer
 from .viewer_ctf_consensus import XmippCTFConsensusViewer
 from .viewer_deep_consensus import XmippDeepConsensusViewer
 from .viewer_deep_micrograph_cleaner import XmippDeepMicrographViewer
 from .viewer_ml2d import XmippML2DViewer
 #from .viewer_mltomo import XmippMLTomoViewer
 from .viewer_movie_alignment import XmippMovieAlignViewer, XmippMovieMaxShiftViewer
@@ -44,27 +45,27 @@
 from .viewer_validate_nontilt import XmippValidateNonTiltViewer
 from .viewer_validate_fscq import XmippProtValFitViewer
 from .viewer_split_volume import XmippViewerSplitVolume
 from .viewer_validate_overfitting import XmippValidateOverfittingViewer
 from .viewer_volume_strain import XmippVolumeStrainViewer
 from .viewer_reconstruct_highres import XmippReconstructHighResViewer
 from .viewer_solid_angles import SolidAnglesViewer
-from .viewer_consensus_classes3D import XmippConsensusClasses3DViewer
-from .viewer_classes3D import XmippClasses3DViewer
+from .viewer_consensus_classes import XmippConsensusClassesViewer
 from .viewer_extract_asymmetric_unit import viewerXmippProtExtractUnit
 from .viewer_deepEMHancer import viewerXmippProtDeepVolPostProc
 from .viewer_local_sharpening import viewerXmippProtLocSharp
 from .viewer_volume_subtraction import XmippProtVolSubtractionViewer
 from .viewer_volume_consensus import XmippVolumeConsensusViewer
+from .viewer_dose_analysis import XmippMovieDoseAnalysisViewer
 
 #from .viewer_combine_pdb import XmippProtCombinePdbViewer
 
 from .viewer_projmatch import XmippProjMatchViewer
 
 from .viewer_volume_deform_zernike3d import XmippVolumeDeformZernike3DViewer
 from .viewer_structure_map import XmippProtStructureMapViewer
 from .viewer_pdb_deform_zernike3d import XmippPDBDeformViewer
 from .viewer_metaprotocol_golden_highres import XmippMetaprotocolGoldenHighResViewer
 
 # TODO: Import from continuousflex the modules needed to create clusters (soft dependency)
 from .viewer_analyze_local_ctf import XmippAnalyzeLocalCTFViewer
-from .viewer_subtract_projection import XmippSubtractProjectionViewer
+from .viewer_subtract_projection import XmippSubtractProjectionViewer
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/plotter.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/plotter.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,24 +37,23 @@
 from xmipp3.protocols import XmippProtCompareAngles
 from xmipp3.protocols import XmippProtConsensusLocalCTF
 from xmipp3.protocols import XmippProtExtractParticles
 from xmipp3.protocols import XmippProtExtractParticlesPairs
 from xmipp3.protocols import XmippProtKerdensom
 from xmipp3.protocols import XmippParticlePickingAutomatic
 from xmipp3.protocols import XmippProtParticlePickingPairs
-from xmipp3.protocols import XmippProtRotSpectra
+#from xmipp3.protocols import XmippProtRotSpectra
 from xmipp3.protocols import XmippProtScreenParticles
 from xmipp3.protocols import XmippProtCTFMicrographs
 from xmipp3.protocols import XmippProtValidateNonTilt
 from xmipp3.protocols import XmippProtMultiRefAlignability
 from xmipp3.protocols import XmippProtAngularGraphConsistency
 from xmipp3.protocols import XmippProtAssignmentTiltPair
 from xmipp3.protocols import XmippProtMovieGain
 from xmipp3.protocols import XmippProtDeepDenoising
-from xmipp3.protocols import XmippProtParticleBoxsize
 from .plotter import XmippPlotter
 from xmipp3.protocols import XmippProtTiltAnalysis
 from pwem.viewers.viewers_data import MicrographsView
 
 
 class XmippViewer(DataViewer):
     """ Wrapper to visualize different type of objects
@@ -66,24 +65,22 @@
                 XmippProtCompareAngles,
                 XmippProtConsensusLocalCTF,
                 XmippParticlePickingAutomatic,
                 XmippProtExtractParticles,
                 XmippProtExtractParticlesPairs,
                 XmippProtKerdensom,
                 XmippProtParticlePickingPairs,
-                XmippProtRotSpectra,
                 XmippProtScreenParticles,
                 XmippProtCTFMicrographs,
                 XmippProtValidateNonTilt,
                 XmippProtAssignmentTiltPair,
                 XmippProtMultiRefAlignability,
                 XmippProtAngularGraphConsistency,
                 XmippProtMovieGain,
                 XmippProtDeepDenoising,
-                XmippProtParticleBoxsize,
                 XmippProtTiltAnalysis
                 ]
 
     def __createTemporaryCtfs(self, obj, setOfMics):
         pwutils.cleanPath(obj._getPath("ctfs_temporary.sqlite"))
         self.protocol._createFilenameTemplates()
         ctfSet = self.protocol._createSetOfCTF("_temporary")
@@ -183,23 +180,14 @@
             #                                     samplingInterval=60,
             #                                     monitorTime=300,
             #                                     stddevValue=0.04,
             #                                     ratio1Value=1.15,
             #                                     ratio2Value=4.5)
             # self._views.append(MovieGainMonitorPlotter(movieGainMonitor))
 
-        elif issubclass(cls, XmippProtRotSpectra):
-            self._visualize(obj.outputClasses,
-                            viewParams={'columns': obj.SomXdim.get(),
-                                        RENDER: ' spectraPlot._filename average._filename',
-                                        ZOOM: 30,
-                                        VISIBLE: 'enabled id _size average._filename '
-                                                 'spectraPlot._filename',
-                                        'labels': 'id _size',
-                                        SORT_BY: 'id'})
 
         elif issubclass(cls, XmippProtKerdensom):
             self._visualize(obj.outputClasses, viewParams={'columns': obj.SomXdim.get(),
                                                            'render': 'average._filename '
                                                                      '_representative._filename',
                                                            'labels': '_size',
                                                            'sortby': 'id'})
@@ -285,40 +273,14 @@
                 writeSetOfMicrographs(micSet, micsfn)
                 inTmpFolder = True
 
             posDir = obj._getExtraPath()
             memory = showj.getJvmMaxMemory()
             launchSupervisedPickerGUI(micsfn, posDir, obj, mode='review',
                                       memory=memory, inTmpFolder=inTmpFolder)
-
-        elif issubclass(cls, XmippProtParticleBoxsize):
-            """ Launching a Coordinates viewer with only one coord in the center
-                with the estimated boxsize.
-            """
-            micSet = obj.inputMicrographs.get()
-
-            coordsFn = self._getExtraPath(micSet.getName()+'_coords_to_view.sqlite')
-            if not os.path.exists(coordsFn):
-                # Just creating the coords once
-                coordsSet = SetOfCoordinates(filename=coordsFn)
-                coordsSet.setBoxSize(obj.boxsize)
-                for mic in micSet:
-                    coord = Coordinate()
-                    coord.setMicrograph(mic)
-                    coord.setPosition(mic.getXDim()/2, mic.getYDim()/2)
-                    coordsSet.append(coord)
-                coordsSet.write()
-            else:
-                coordsSet = SetOfCoordinates(filename=coordsFn)
-                coordsSet.loadAllProperties()
-
-            coordsSet.setMicrographs(micSet)
-            coordsSet.setName(micSet.getName())
-            self._visualize(coordsSet)
-
          # We need this case to happens before the ProtParticlePicking one
         elif issubclass(cls, XmippProtAssignmentTiltPair):
             if obj.getOutputsSize() >= 1:
                 coordsSet = obj.getCoordsTiltPair()
                 self._visualize(coordsSet)
 
         elif issubclass(cls, XmippProtValidateNonTilt):
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_analyze_local_ctf.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_analyze_local_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_cl2d.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_cl2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_classes3D.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_eliminate_empty_images.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # **************************************************************************
 # *
-# * Authors:     J.M. De la Rosa Trevin (jmdelarosa@cnb.csic.es)
+# * Authors:     Roberto Marabini (roberto@cnb.csic.es)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 2 of the License, or
 # * (at your option) any later version.
@@ -20,142 +20,155 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-"""
-This module implement the wrappers aroung Xmipp CL2D protocol
-visualization program.
-"""
-from pyworkflow.gui import IconButton, Icon
-from pyworkflow.gui.form import FormWindow
-from pyworkflow.viewer import (ProtocolViewer, DESKTOP_TKINTER, WEB_DJANGO)
-from pyworkflow.protocol.params import StringParam, LabelParam, IntParam
-
-from xmipp3.protocols.protocol_consensus_classes3D import XmippProtConsensusClasses3D
-from pwem.objects import Class3D
-
-import pickle
-import matplotlib.pyplot as plt
-
-FILE_OBJECTIVE_FDATA = 'ObjectiveFData.pkl'
-FILE_CLUSTERINGS = 'clusterings.pkl'
-FILE_ELBOWCLUSTERS = 'elbowclusters.pkl'
+from pyworkflow.protocol.params import IntParam, LabelParam
+from pyworkflow.viewer import DESKTOP_TKINTER, WEB_DJANGO, ProtocolViewer
+from pwem.viewers import EmPlotter, ObjectView, ClassesView
+from pwem.viewers.showj import MODE, MODE_MD, ORDER, VISIBLE, RENDER, SORT_BY
+
+from xmipp3.protocols.protocol_eliminate_empty_images import \
+    XmippProtEliminateEmptyClasses, XmippProtEliminateEmptyParticles
 
 
-class XmippClasses3DViewer(ProtocolViewer):
-    """ Visualization of results from the consensus classes 3D protocol
+class XmippEliminateEmptyViewer(ProtocolViewer):
+    """ This protocol computes the maximum resolution up to which two
+     CTF estimations would be ``equivalent'', defining ``equivalent'' as having
+      a wave aberration function shift smaller than 90 degrees
     """
-    _label = 'viewer classes 3D'
-    _targets = [XmippProtConsensusClasses3D]
+    _label = 'viewer Eliminate empty images'
     _environments = [DESKTOP_TKINTER, WEB_DJANGO]
-
-    def __init__(self, **kwargs):
-        ProtocolViewer.__init__(self, **kwargs)
-        self.nclusters, self.objFValues = self.getObjectiveFData()
-        self._elbowIdx = self.getElbowIndex()
-        self._allClusterings = self.getClusterings()
-
-    def getObjectiveFData(self):
-        loadPath = self.protocol._getExtraPath(FILE_OBJECTIVE_FDATA)
-        with open(loadPath, 'rb') as f:
-            self._ObjFData = pickle.load(f)
-        return self._ObjFData
-
-    def getClusterings(self):
-        loadPath = self.protocol._getExtraPath(FILE_CLUSTERINGS)
-        with open(loadPath, 'rb') as f:
-            self._allClusterings = pickle.load(f)
-        return self._allClusterings
-
-    def getElbowIndex(self):
-        loadPath = self.protocol._getExtraPath(FILE_ELBOWCLUSTERS)
-        with open(loadPath, 'rb') as f:
-            self.elbowIndex = pickle.load(f)
-        return self.elbowIndex
+    _targets = [XmippProtEliminateEmptyParticles,
+                XmippProtEliminateEmptyClasses]
 
     def _defineParams(self, form):
+        isClassType = isinstance(self.protocol, XmippProtEliminateEmptyClasses)
+        self.imagesType = ('Averages' if isClassType else 'Particles')
         form.addSection(label='Visualization')
-        form.addParam('displayObjectiveFunction', LabelParam,
-                      label='Visualize Objective Function',
-                      help='Open a GUI to visualize the objective function for each number of clusters ')
-        form.addParam('chooseNumberOfClusters', IntParam, default=-1,
-                      label='Number of Clusters',
-                      help='Choose the final number of clusters in the consensus clustering. Press the eye')
-
-        #TODO: set an apply button to change the number of clusters instead of using the eye
-        '''command = self._chooseNumberOfClusters()
-        btn = IconButton(self.getWindow(), "Apply", Icon.ACTION_CONTINUE, command=command)
-        btn.config(relief="flat", activebackground=None, compound='left',
-                   fg='black', overrelief="raised")
-        btn.bind('<Button-1>')
-        btn.grid(row=2, column=2, sticky='nw')'''
-
+        form.addParam('visualizeIms', LabelParam,
+                       label="Visualize passed %s" % self.imagesType)
+        form.addParam('visualizeImsDiscarded', LabelParam,
+                        label="Visualize discarded %s" % self.imagesType)
+
+        if not isClassType:
+            form.addParam('justSpace', LabelParam, label="")
+            form.addParam('visualizeHistogram', IntParam, default=100,
+                          label="Visualize Histogram (Bin size)",
+                          help="Histogram of the emptiness score.")
 
     def _getVisualizeDict(self):
-        return {'chooseNumberOfClusters': self._chooseNumberOfClusters,
-                'displayObjectiveFunction': self._visualizeObjectiveFunction}
+        return {
+                 'visualizeIms': self._visualizeIms,
+                 'visualizeImsDiscarded': self._visualizeImsDiscarded,
+                 'visualizeHistogram': self._visualizeHistogram
+                }
+
+    def _visualizeImages(self, outputName):
+        views = []
+        prot = self.protocol
+        if hasattr(prot, outputName):
+            ouputFn = getattr(prot, outputName).getFileName()
+            ouputId = getattr(prot, outputName).strId()
+            labels = ('id enabled _index _filename _xmipp_scoreEmptiness '
+                      '_xmipp_scoreByVariance _xmipp_zScore '
+                      '_xmipp_cumulativeSSNR _sampling '
+                      '_ctfModel._defocusU _ctfModel._defocusV '
+                      '_ctfModel._defocusAngle _transform._matrix')
+            if 'Classes' in outputName:
+                views.append(ClassesView(self._project, ouputId, ouputFn))
+            else:
+                views.append(ObjectView(self._project, ouputId, ouputFn,
+                                        viewParams={ORDER: labels,
+                                        VISIBLE: labels,
+                                        SORT_BY: '_xmipp_scoreEmptiness desc',
+                                        MODE: MODE_MD,
+                                        RENDER: '_filename'}))
+        else:
+            appendStr = ', yet.' if prot.isActive() else '.'
+            self.infoMessage('%s does not have %s%s'
+                             % (prot.getObjLabel(), outputName,
+                                appendStr),
+                             title='Info message').show()
+        return views
+
+    def _visualizeIms(self, e=None):
+        return self._visualizeImages(outputName="output%s" % self.imagesType)
+
+    def _visualizeImsDiscarded(self, e=None):
+        return self._visualizeImages(outputName="eliminated%s" % self.imagesType)
 
-    def _visualizeObjectiveFunction(self, e=None):
-        nclusters, ob_values = self.nclusters, self.objFValues
-        elbowIdx = self._elbowIdx
-
-        plt.plot(nclusters, ob_values)
-        plt.scatter([nclusters[elbowIdx]], [ob_values[elbowIdx]], color='green')
-        plt.xlabel('Number of clusters')
-        plt.ylabel('Objective values')
-        plt.title('Objective values for each number of clusters')
-        plt.show()
-
-    def _chooseNumberOfClusters(self, e=None):
-        views=[]
-        nclusters = self.nclusters
-        elbow_nclust = nclusters[self._elbowIdx]
-
-        nclust = self.chooseNumberOfClusters.get()
-        if nclust == -1:
-            nclust = elbow_nclust
-        elif nclust > max(nclusters):
-            nclust = max(nclusters)
-
-        scipion_clustering = self.buildSetOfClasses(nclust)
-        self.protocol._defineOutputs(outputClasses=scipion_clustering)
-        for item in self.protocol.inputMultiClasses:
-            self.protocol._defineSourceRelation(item, scipion_clustering)
+    def _visualizeHistogram(self, e=None):
+        views = []
+        numberOfBins = self.visualizeHistogram.get()
+        goodScores = []
+        badScores = []
+        if hasattr(self.protocol, "outputParticles"):
+            goodScores += [part._xmipp_scoreEmptiness.get() for part in
+                           self.protocol.outputParticles]
+
+        if hasattr(self.protocol, "eliminatedParticles"):
+            badScores += [part._xmipp_scoreEmptiness.get() for part in
+                          self.protocol.eliminatedParticles]
+
+        plotter = EmPlotter()
+        plotter.createSubPlot("Emptiness Score", "Emptiness Score (a.u.)",
+                              "# of Particles")
+
+        values = [goodScores, badScores]
+        labels = ["Passed particles", "Discarded particles"]
+        colors = ['green', 'red']
+
+        plotMultiHistogram(values, colors, labels, numberOfBins, plotter, views)
 
-        #TODO: esto es un objeto SetOfClasses3D pero no sabemos como lanzar un viewer con el sin tener el protocolo
-        #views.append(ObjectView(self._project, self.protocol.strId()))
         return views
 
-    def buildSetOfClasses(self, nclust):
-        '''From a list of clusterings, nclust index it and that clustering
-        is converted into a scipion setOfClasses'''
-        clustIdx = self.nclusters.index(nclust)
-        clustering = self._allClusterings[clustIdx]
-
-        inputParticles = self.protocol.inputMultiClasses[0].get().getImages()
-        outputClasses = self.protocol._createSetOfClasses3D(inputParticles)
-        for classItem in clustering:
-            numOfPart = classItem[0]
-            partIds = classItem[1]
-            setRepId = classItem[2]
-            clsRepId = classItem[3]
-
-            setRep = self.protocol.inputMultiClasses[setRepId].get()
-            clRep = setRep[clsRepId]
-
-            newClass = Class3D()
-            # newClass.copyInfo(clRep)
-            newClass.setAcquisition(clRep.getAcquisition())
-            newClass.setRepresentative(clRep.getRepresentative())
-
-            outputClasses.append(newClass)
-
-            enabledClass = outputClasses[newClass.getObjId()]
-            enabledClass.enableAppend()
-            for itemId in partIds:
-                enabledClass.append(inputParticles[itemId])
-            outputClasses.update(enabledClass)
 
-        return outputClasses
+def plotMultiHistogram(valuesList, colors=None, legend=None, numOfBins=100,
+                       plotter=None, views=None, includeEmpties=False):
+    """ Values list must be a n-list of list,
+        where n is the number of the subhistograms to plot.
+        Multiple histograms will be plot in the same chart
+        If no views is passed, a new list-views will be returned with the hist.
+        If no plotter is passed, a new generic one will be created.
+    """
+
+    if not all([isinstance(x, list) for x in valuesList]):
+        print("Not all items in values list are lists. Returning...")
+        return
+
+    if colors is None:
+        from matplotlib import colors
+        from random import shuffle
+        colors = colors.cnames.keys()
+        shuffle(colors)
+
+
+    if any([len(x) for x in valuesList]):
+        if plotter is None:
+            plotter = EmPlotter()
+            plotter.createSubPlot("Histogram", "Score", "# of Items")
+
+        w1 = None
+        finalLegend = []
+        for idx, values in enumerate(valuesList):
+            if values or includeEmpties:
+                if w1 is None:
+                    w1 = (max(values) - min(values)) / numOfBins
+                else:
+                    numOfBins = int((max(values) - min(values)) / w1)
+
+                plotter.plotHist(values, nbins=numOfBins, color=colors[idx])
+                if legend:
+                    finalLegend.append(legend[idx])
+
+        if finalLegend:
+            plotter.legend(labels=finalLegend)
+
+        if views is None:
+            views = [plotter]
+        else:
+            views.append(plotter)
+
+        return views
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_ctf_consensus.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_ctf_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_deepEMHancer.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_deepEMHancer.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_deep_consensus.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_deep_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_deep_micrograph_cleaner.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_deep_micrograph_cleaner.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_extract_asymmetric_unit.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_extract_asymmetric_unit.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_local_sharpening.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_local_sharpening.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_metaprotocol_golden_highres.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_metaprotocol_golden_highres.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,19 +27,18 @@
 from glob import glob
 from os.path import exists, join
 
 from pyworkflow.protocol.params import EnumParam, NumericRangeParam, LabelParam, \
     IntParam, FloatParam
 from pyworkflow.protocol.constants import LEVEL_ADVANCED
 from pyworkflow.viewer import DESKTOP_TKINTER, WEB_DJANGO, ProtocolViewer
-from pwem.viewers import ObjectView, DataView, ChimeraClientView
+from pwem.viewers import ObjectView, DataView
 import pwem.viewers.showj as showj
+from pwem import emlib
 
-from xmippLib import (MDL_SAMPLINGRATE, MDL_ANGLE_ROT, MDL_ANGLE_TILT,
-                      MDL_RESOLUTION_FREQ, MDL_RESOLUTION_FRC, MetaData)
 from xmipp3.protocols.protocol_metaprotocol_golden_highres import \
     XmippMetaProtGoldenHighRes
 from .plotter import XmippPlotter
 
 class XmippMetaprotocolGoldenHighResViewer(ProtocolViewer):
     """ Visualize the output of protocol reconstruct highres """
     _label = 'viewer golden highres'
@@ -119,17 +118,17 @@
         a.grid(True)
         views = []
         views.append(xplotter)
         return views
 
 
     def _plotFSC(self, ab, fnFSC):
-        md = MetaData(fnFSC)
-        resolution_inv = [md.getValue(MDL_RESOLUTION_FREQ, f) for f in md]
-        frc = [md.getValue(MDL_RESOLUTION_FRC, f) for f in md]
+        md = emlib.MetaData(fnFSC)
+        resolution_inv = [md.getValue(emlib.MDL_RESOLUTION_FREQ, f) for f in md]
+        frc = [md.getValue(emlib.MDL_RESOLUTION_FRC, f) for f in md]
         # self.maxFrc = max(frc)
         self.minInv.append(min(resolution_inv))
         self.maxInv.append(max(resolution_inv))
         ab.plot(resolution_inv, frc)
         ab.xaxis.set_major_formatter(self._plotFormatter)
         ab.set_ylim([-0.1, 1.1])
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_ml2d.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_ml2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_movie_alignment.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_movie_alignment.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_normalize_strain.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_normalize_strain.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_pdb_deform_zernike3d.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_pdb_deform_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_projmatch.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_projmatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,26 +28,27 @@
 """
 This module implement the wrappers aroung Xmipp ML2D protocol
 visualization program.
 """
 
 from pyworkflow.protocol.executor import StepExecutor
 from pyworkflow.viewer import ProtocolViewer, DESKTOP_TKINTER, WEB_DJANGO
-from pwem.viewers import (DataView, EmPlotter, showj, ChimeraClientView,
+from pwem.viewers import (DataView, EmPlotter, showj,
                           ChimeraView, ObjectView, ChimeraAngDist)
 import pwem.objects as emobj
 from pyworkflow.utils import createUniqueFileName, cleanPattern, cleanPath
 from pyworkflow.protocol.constants import LEVEL_ADVANCED
 from pyworkflow.protocol.params import (LabelParam, IntParam, FloatParam,
                                         StringParam, EnumParam,
                                         NumericRangeParam, BooleanParam)
 import pyworkflow.utils as pwutils
+
 from xmipp3.convert import *
 from xmipp3.viewers.plotter import XmippPlotter
-from xmipp3.protocols import XmippProtProjMatch
+from ..protocols.protocol_projmatch import XmippProtProjMatch
 
 
 ITER_LAST = 0
 ITER_SELECTION = 1
 
 ANGDIST_2DPLOT = 0
 ANGDIST_CHIMERA = 1
@@ -319,16 +320,15 @@
                 vol = os.path.relpath(volFn, self.protocol._getExtraPath())
                 f.write("open %s\n" % vol)
             f.write('tile\n')
             f.close()
             view = ChimeraView(cmdFile)
         else:
             
-            #view = CommandView('xmipp_chimera_client --input "%s" --mode projector 256 &' % volumes[0])
-            view = ChimeraClientView(volumes[0], showProjection=True)
+            view = ChimeraView(volumes[0])
         
         return [view]
     
     def _showVolumes(self, volumes):
         if self.displayVolWith == VOLUME_CHIMERA:
             return self._showVolumesChimera(volumes)
         elif self.displayVolWith == VOLUME_SLICES:
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_ransac.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_ransac.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_reconstruct_highres.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_reconstruct_highres.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_resolution3d.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_resolution3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_resolution_bfactor.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_resolution_bfactor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_resolution_deepres.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_resolution_deepres.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_resolution_directional.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_resolution_directional.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_resolution_fso.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_resolution_fso.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,35 +319,45 @@
         a.axes.hlines(hthresholds, xx[0], xx[-1], colors='k', linestyles='dashed')
         a.axes.grid(True)
         textstr = ''
 
         res_01, okToPlot_01 = self.interpolRes(0.1, xx, yy)
         res_05, okToPlot_05 = self.interpolRes(0.5, xx, yy)
         res_09, okToPlot_09 = self.interpolRes(0.9, xx, yy)
-        
+
+        textstr = ''
+
         if okToPlot_09:
-           if self.protocol.halfVolumesFile:
-              sampling = self.protocol.inputHalves.get().getSamplingRate()
-           else:
-              sampling = self.protocol.half1.get().getSamplingRate()
+           textstr += str(0.9) + ' --> ' + str("{:.2f}".format(res_09)) + 'A\n'
+        if okToPlot_05:
+           textstr += str(0.5) + ' --> ' + str("{:.2f}".format(res_05)) + 'A\n'
+        if okToPlot_01:
+           textstr += str(0.1) + ' --> ' + str("{:.2f}".format(res_01)) + 'A'
+
+        props = dict(boxstyle='round', facecolor='white')
+        a.axes.text(0.0, 0.0, textstr, fontsize=12, ha="left", va="bottom", bbox=props)
+        
+        if self.protocol.halfVolumesFile:
+           sampling = self.protocol.inputHalves.get().getSamplingRate()
+        else:
+           sampling = self.protocol.half1.get().getSamplingRate()
+
+        if okToPlot_09 and okToPlot_01:
            t = round((2*sampling/(res_01))*len(yyBingham)) + 3
            if t<len(yyBingham):
               for component in range(t, len(yyBingham)-1):
                  yyBingham[component] = 0
            a.axes.plot(xx, yyBingham, 'r--')
         else:
            a.axes.plot(xx, yyBingham, 'r--')
 
-        if (okToPlot_01 and okToPlot_05 and okToPlot_09):
-            textstr = str(0.9) + ' --> ' + str("{:.2f}".format(res_09)) + 'A\n' + str(0.5) + ' --> ' + str(
-                "{:.2f}".format(res_05)) + 'A\n' + str(0.1) + ' --> ' + str("{:.2f}".format(res_01)) + 'A'
-            a.axes.axvspan(1.0 / res_09, 1.0 / res_01, alpha=0.3, color='green')
+        if not okToPlot_01:
+           res_01 = 2*sampling
 
-            props = dict(boxstyle='round', facecolor='white')
-            a.axes.text(0.0, 0.0, textstr, fontsize=12, ha="left", va="bottom", bbox=props)
+        a.axes.axvspan(1.0 / res_09, 1.0 / res_01, alpha=0.3, color='green')
 
         return plt.show()
 
     def _prepareDataForPlot(self, md, mdLabelX, mdLabelY):
         """ plot metadata columns mdLabelX and mdLabelY
             if nbins is in args then and histogram over y data is made
         """
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_solid_angles.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_solid_angles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_split_volume.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_split_volume.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_structure_map.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_structure_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,18 @@
             if not os.path.exists(file):
                 return [self.errorMessage('The necessary metadata was not produced\n'
                                           'Execute again the protocol\n',
                                           title='Missing result file')]
 
         self.coordinates = (np.loadtxt(file) for file in fnOutput)
         self.coordinates = np.vstack(self.coordinates)
-        labels = [str(idp) for idp in range(1, self.coordinates.shape[0] + 1)]
+        labels = [v.getObjLabel() for v in self.protocol.inputVolumes.get()]
+        if '' in labels:
+                labels = [str(idp) for idp in
+                          range(1, self.coordinates.shape[0] + 1)]
         if os.path.isfile(self._getExtraPath('weigths.txt')):
             weights = np.loadtxt(self._getExtraPath('weigths.txt'))
         else:
             weights = None
         plot = projectionPlot(self.coordinates, labels, weights)
         plot.initializePlot()
         return plot
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_subtract_projection.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_subtract_projection.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_swarm.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_swarm.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_validate_fscq.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_validate_fscq.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_validate_nontilt.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_validate_nontilt.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_validate_overfitting.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_validate_overfitting.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_volume_consensus.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_volume_consensus.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_volume_deform_zernike3d.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_volume_deform_zernike3d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_volume_strain.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_volume_strain.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/viewers/viewer_volume_subtraction.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/viewers/viewer_volume_subtraction.py`

 * *Files identical despite different names*

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/wizards.py` & `scipion-em-xmipp-23.7.0.0/xmipp3/wizards.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 from pwem.wizards.wizard import EmWizard
 from pyworkflow.wizard import Wizard
 from xmipp3.viewers import XmippMonoResViewer, XmippResDeepResViewer, XmippProtFSOViewer
 
 from .protocols.protocol_cl2d import IMAGES_PER_CLASS
 
 from .protocols import (
-    XmippProtCTFMicrographs, XmippProtProjMatch, XmippProtPreprocessParticles,
+    XmippProtCTFMicrographs, XmippProtPreprocessParticles, XmippProtProjMatch,
     XmippProtPreprocessMicrographs, XmippProtPreprocessVolumes,
     XmippProtExtractParticles, XmippProtExtractParticlesPairs, XmippProtPickingRemoveDuplicates,
     XmippProtFilterParticles, XmippProtFilterVolumes, XmippProtMaskParticles,
     XmippProtMaskVolumes, XmippProtAlignVolume, XmippProtCL2D,
     XmippProtHelicalParameters, XmippProtConsensusPicking, XmippProtMonoRes,
-    XmippProtRotSpectra, XmippProtReconstructHighRes, XmippProtExtractUnit,
+    XmippProtReconstructHighRes, XmippProtExtractUnit,
     XmippProtShiftParticles, XmippProtVolumeDeformZernike3D, XmippProtStructureMapZernike3D,
     XmippProtSubtractProjection, XmippProtBoostParticles)
 
 
 #===============================================================================
 # DOWNSAMPLING
 #===============================================================================
@@ -153,15 +153,18 @@
 # CONSENSUS RADIUS
 #===============================================================================
 class XmippParticleConsensusRadiusWizard(Wizard):
     _targets = [(XmippProtConsensusPicking, ['consensusRadius'])]
 
     def _getRadius(self, protocol):
         if protocol.inputCoordinates.hasValue():
-            boxSize=protocol.inputCoordinates[0].get().getBoxSize()
+            if protocol.inputCoordinates.get() == None:  # Protocol=XmippProtConsensusPicking => inputCoordinates=list
+                boxSize = protocol.inputCoordinates[0].get().getBoxSize()
+            else:  # Protocol=XmippProtPickingRemoveDuplicates => inputCoordinates=setOfCoordinates
+                boxSize = protocol.inputCoordinates.get().getBoxSize()
             radius = int(boxSize*0.1)
             if radius<10:
                 radius=10
         else:
             radius = 10
         return radius
 
@@ -216,16 +219,15 @@
         params = self._getParameters(form.protocol)
         _value = params['value']
         _label = params['label']
         ParticleMaskRadiusWizard.show(self, form, _value, _label, UNIT_PIXEL)
 
 
 class XmippParticleMaskRadiiWizard(ParticlesMaskRadiiWizard):
-    _targets = [(XmippProtMaskParticles, ['innerRadius', 'outerRadius']),
-                (XmippProtRotSpectra, ['spectraInnerRadius', 'spectraOuterRadius'])]
+    _targets = [(XmippProtMaskParticles, ['innerRadius', 'outerRadius'])]
 
     def _getParameters(self, protocol):
 
         label, value = self._getInputProtocol(self._targets, protocol)
 
         protParams = {}
         protParams['input']= protocol.inputParticles
@@ -309,29 +311,30 @@
     def _getParameters(self, protocol):
         protParams = {}
         protParams['input']= protocol.inputVolume
         protParams['label']= 'cylinderInnerRadius'
         protParams['value']= protocol.cylinderInnerRadius.get()
         return protParams
 
-
 class XmippVolumeMaskRadiusProjMWizard(XmippVolumeMaskRadiusWizard):
     _targets = [(XmippProtProjMatch, ['maskRadius'])]
 
     def _getParameters(self, protocol):
 
         label, value = self._getInputProtocol(self._targets, protocol)
 
         protParams = {}
         protParams['input']= protocol.input3DReferences
         protParams['label']= label
         protParams['value']= value
         return protParams
 
 
+
+
 class XmippVolumeRadiiWizard(VolumeMaskRadiiWizard):
     _targets = [(XmippProtMaskVolumes, ['innerRadius', 'outerRadius']),
                (XmippProtExtractUnit, ['innerRadius', 'outerRadius'])]
 
     def _getParameters(self, protocol):
 
         label, value = self._getInputProtocol(self._targets, protocol)
@@ -348,14 +351,15 @@
 
     def show(self, form):
         params = self._getParameters(form.protocol)
         _value = params['value']
         _label = params['label']
         VolumeMaskRadiiWizard.show(self, form, _value, _label, UNIT_PIXEL)
 
+
 class XmippVolumeRadiiProjMWizard(XmippVolumeRadiiWizard):
     _targets = [(XmippProtProjMatch, ['innerRadius', 'outerRadius'])]
 
     def _getParameters(self, protocol):
 
         label, value = self._getInputProtocol(self._targets, protocol)
         # Convert values to integer (From NumericListParam they come as string)
```

### Comparing `scipion-em-xmipp-23.3.0.3/xmipp3/xmipp_logo.png` & `scipion-em-xmipp-23.7.0.0/xmipp3/xmipp_logo.png`

 * *Files identical despite different names*

