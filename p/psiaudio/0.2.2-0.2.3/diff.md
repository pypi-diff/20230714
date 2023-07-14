# Comparing `tmp/psiaudio-0.2.2.tar.gz` & `tmp/psiaudio-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psiaudio-0.2.2.tar", last modified: Fri Mar 24 22:27:22 2023, max compression
+gzip compressed data, was "psiaudio-0.2.3.tar", last modified: Fri Jul 14 17:46:31 2023, max compression
```

## Comparing `psiaudio-0.2.2.tar` & `psiaudio-0.2.3.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 22:27:22.870916 psiaudio-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 22:27:22.858917 psiaudio-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 22:27:22.858917 psiaudio-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-03-24 22:27:13.000000 psiaudio-0.2.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-03-24 22:27:13.000000 psiaudio-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 22:27:13.000000 psiaudio-0.2.2/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-24 22:27:13.000000 psiaudio-0.2.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-24 22:27:13.000000 psiaudio-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-24 22:27:22.866917 psiaudio-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-24 22:27:13.000000 psiaudio-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 22:27:22.858917 psiaudio-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-24 22:27:13.000000 psiaudio-0.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-24 22:27:13.000000 psiaudio-0.2.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-24 22:27:13.000000 psiaudio-0.2.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 22:27:22.858917 psiaudio-0.2.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 22:27:22.862917 psiaudio-0.2.2/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-24 22:27:13.000000 psiaudio-0.2.2/docs/source/api/psiaudio.calibration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-24 22:27:13.000000 psiaudio-0.2.2/docs/source/api/psiaudio.pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-24 22:27:13.000000 psiaudio-0.2.2/docs/source/api/psiaudio.queue.rst
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-24 22:27:13.000000 psiaudio-0.2.2/docs/source/api/psiaudio.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-24 22:27:13.000000 psiaudio-0.2.2/docs/source/api/psiaudio.stim.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-24 22:27:13.000000 psiaudio-0.2.2/docs/source/api/psiaudio.util.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-03-24 22:27:13.000000 psiaudio-0.2.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-24 22:27:13.000000 psiaudio-0.2.2/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 22:27:22.862917 psiaudio-0.2.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 22:27:22.862917 psiaudio-0.2.2/examples/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-24 22:27:13.000000 psiaudio-0.2.2/examples/gallery/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-03-24 22:27:13.000000 psiaudio-0.2.2/examples/gallery/bandlimited-click.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-03-24 22:27:13.000000 psiaudio-0.2.2/examples/gallery/calibration-basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-03-24 22:27:13.000000 psiaudio-0.2.2/examples/gallery/chirp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-03-24 22:27:13.000000 psiaudio-0.2.2/examples/gallery/notch-noise-abr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-03-24 22:27:13.000000 psiaudio-0.2.2/examples/gallery/queue-introduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-03-24 22:27:13.000000 psiaudio-0.2.2/examples/gallery/queueing-wav-files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-03-24 22:27:13.000000 psiaudio-0.2.2/examples/gallery/repeat-chirp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-03-24 22:27:13.000000 psiaudio-0.2.2/examples/gallery/stimulus-generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-03-24 22:27:13.000000 psiaudio-0.2.2/examples/gallery/tone-complex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-24 22:27:13.000000 psiaudio-0.2.2/examples/gallery/tone-pips.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-03-24 22:27:13.000000 psiaudio-0.2.2/examples/play-wav-files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 22:27:22.866917 psiaudio-0.2.2/examples/wav-files/
--rwxr-xr-x   0 runner    (1001) docker     (123)   352844 2023-03-24 22:27:13.000000 psiaudio-0.2.2/examples/wav-files/00cat172_rec1_geese_excerpt1.wav
--rwxr-xr-x   0 runner    (1001) docker     (123)   352844 2023-03-24 22:27:13.000000 psiaudio-0.2.2/examples/wav-files/00cat221_rec1_laughing_excerpt1.wav
--rwxr-xr-x   0 runner    (1001) docker     (123)   352844 2023-03-24 22:27:13.000000 psiaudio-0.2.2/examples/wav-files/00cat28_rec1_bigband_bbc-big-band_american-patrol_0sec_excerpt1.wav
--rwxr-xr-x   0 runner    (1001) docker     (123)   352844 2023-03-24 22:27:13.000000 psiaudio-0.2.2/examples/wav-files/00cat78_rec1_chimes_in_the_wind_excerpt1.wav
--rwxr-xr-x   0 runner    (1001) docker     (123)   352844 2023-03-24 22:27:13.000000 psiaudio-0.2.2/examples/wav-files/00cat83_rec1_cicadas_excerpt1.wav
--rwxr-xr-x   0 runner    (1001) docker     (123)   352844 2023-03-24 22:27:13.000000 psiaudio-0.2.2/examples/wav-files/00cat92_rec1_country_song_excerpt1.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 22:27:22.866917 psiaudio-0.2.2/psiaudio/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-24 22:27:13.000000 psiaudio-0.2.2/psiaudio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-03-24 22:27:13.000000 psiaudio-0.2.2/psiaudio/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-03-24 22:27:13.000000 psiaudio-0.2.2/psiaudio/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    43335 2023-03-24 22:27:13.000000 psiaudio-0.2.2/psiaudio/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-03-24 22:27:13.000000 psiaudio-0.2.2/psiaudio/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    18823 2023-03-24 22:27:13.000000 psiaudio-0.2.2/psiaudio/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 22:27:22.866917 psiaudio-0.2.2/psiaudio/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 22:27:13.000000 psiaudio-0.2.2/psiaudio/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   142772 2023-03-24 22:27:13.000000 psiaudio-0.2.2/psiaudio/resources/starship_cal.csv
--rw-r--r--   0 runner    (1001) docker     (123)    45633 2023-03-24 22:27:13.000000 psiaudio-0.2.2/psiaudio/stim.py
--rw-r--r--   0 runner    (1001) docker     (123)    35478 2023-03-24 22:27:13.000000 psiaudio-0.2.2/psiaudio/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-24 22:27:22.000000 psiaudio-0.2.2/psiaudio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 22:27:22.866917 psiaudio-0.2.2/psiaudio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-24 22:27:22.000000 psiaudio-0.2.2/psiaudio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-03-24 22:27:22.000000 psiaudio-0.2.2/psiaudio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 22:27:22.000000 psiaudio-0.2.2/psiaudio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-24 22:27:22.000000 psiaudio-0.2.2/psiaudio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-24 22:27:22.000000 psiaudio-0.2.2/psiaudio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-03-24 22:27:13.000000 psiaudio-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-24 22:27:13.000000 psiaudio-0.2.2/release.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 22:27:22.870916 psiaudio-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 22:27:22.866917 psiaudio-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-03-24 22:27:13.000000 psiaudio-0.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-03-24 22:27:13.000000 psiaudio-0.2.2/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    27785 2023-03-24 22:27:13.000000 psiaudio-0.2.2/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    19018 2023-03-24 22:27:13.000000 psiaudio-0.2.2/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-03-24 22:27:13.000000 psiaudio-0.2.2/tests/test_signal_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14153 2023-03-24 22:27:13.000000 psiaudio-0.2.2/tests/test_stim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-24 22:27:13.000000 psiaudio-0.2.2/tests/test_stim_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-03-24 22:27:13.000000 psiaudio-0.2.2/tests/test_stim_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-03-24 22:27:13.000000 psiaudio-0.2.2/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:46:31.492068 psiaudio-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:46:31.480068 psiaudio-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:46:31.484068 psiaudio-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-14 17:46:17.000000 psiaudio-0.2.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-14 17:46:17.000000 psiaudio-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 17:46:17.000000 psiaudio-0.2.3/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-14 17:46:17.000000 psiaudio-0.2.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-14 17:46:17.000000 psiaudio-0.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-14 17:46:31.492068 psiaudio-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-14 17:46:17.000000 psiaudio-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:46:31.484068 psiaudio-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-14 17:46:17.000000 psiaudio-0.2.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-14 17:46:17.000000 psiaudio-0.2.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-14 17:46:17.000000 psiaudio-0.2.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:46:31.484068 psiaudio-0.2.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:46:31.484068 psiaudio-0.2.3/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-14 17:46:17.000000 psiaudio-0.2.3/docs/source/api/psiaudio.calibration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-14 17:46:17.000000 psiaudio-0.2.3/docs/source/api/psiaudio.pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-14 17:46:17.000000 psiaudio-0.2.3/docs/source/api/psiaudio.queue.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-14 17:46:17.000000 psiaudio-0.2.3/docs/source/api/psiaudio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-14 17:46:17.000000 psiaudio-0.2.3/docs/source/api/psiaudio.stim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-14 17:46:17.000000 psiaudio-0.2.3/docs/source/api/psiaudio.util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-14 17:46:17.000000 psiaudio-0.2.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-14 17:46:17.000000 psiaudio-0.2.3/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:46:31.484068 psiaudio-0.2.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:46:31.488068 psiaudio-0.2.3/examples/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-14 17:46:17.000000 psiaudio-0.2.3/examples/gallery/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-14 17:46:17.000000 psiaudio-0.2.3/examples/gallery/bandlimited-click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-07-14 17:46:17.000000 psiaudio-0.2.3/examples/gallery/calibration-basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-14 17:46:17.000000 psiaudio-0.2.3/examples/gallery/chirp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-14 17:46:17.000000 psiaudio-0.2.3/examples/gallery/notch-noise-abr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-14 17:46:17.000000 psiaudio-0.2.3/examples/gallery/queue-introduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-07-14 17:46:17.000000 psiaudio-0.2.3/examples/gallery/queueing-wav-files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-14 17:46:17.000000 psiaudio-0.2.3/examples/gallery/repeat-chirp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-14 17:46:17.000000 psiaudio-0.2.3/examples/gallery/stimulus-generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-14 17:46:17.000000 psiaudio-0.2.3/examples/gallery/tone-complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-14 17:46:17.000000 psiaudio-0.2.3/examples/gallery/tone-pips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-14 17:46:17.000000 psiaudio-0.2.3/examples/play-wav-files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:46:31.488068 psiaudio-0.2.3/examples/wav-files/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   352844 2023-07-14 17:46:17.000000 psiaudio-0.2.3/examples/wav-files/00cat172_rec1_geese_excerpt1.wav
+-rwxr-xr-x   0 runner    (1001) docker     (123)   352844 2023-07-14 17:46:17.000000 psiaudio-0.2.3/examples/wav-files/00cat221_rec1_laughing_excerpt1.wav
+-rwxr-xr-x   0 runner    (1001) docker     (123)   352844 2023-07-14 17:46:17.000000 psiaudio-0.2.3/examples/wav-files/00cat28_rec1_bigband_bbc-big-band_american-patrol_0sec_excerpt1.wav
+-rwxr-xr-x   0 runner    (1001) docker     (123)   352844 2023-07-14 17:46:17.000000 psiaudio-0.2.3/examples/wav-files/00cat78_rec1_chimes_in_the_wind_excerpt1.wav
+-rwxr-xr-x   0 runner    (1001) docker     (123)   352844 2023-07-14 17:46:17.000000 psiaudio-0.2.3/examples/wav-files/00cat83_rec1_cicadas_excerpt1.wav
+-rwxr-xr-x   0 runner    (1001) docker     (123)   352844 2023-07-14 17:46:17.000000 psiaudio-0.2.3/examples/wav-files/00cat92_rec1_country_song_excerpt1.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:46:31.492068 psiaudio-0.2.3/psiaudio/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-14 17:46:17.000000 psiaudio-0.2.3/psiaudio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-14 17:46:17.000000 psiaudio-0.2.3/psiaudio/audiograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-07-14 17:46:17.000000 psiaudio-0.2.3/psiaudio/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-07-14 17:46:17.000000 psiaudio-0.2.3/psiaudio/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44238 2023-07-14 17:46:17.000000 psiaudio-0.2.3/psiaudio/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-07-14 17:46:17.000000 psiaudio-0.2.3/psiaudio/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18981 2023-07-14 17:46:17.000000 psiaudio-0.2.3/psiaudio/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:46:31.492068 psiaudio-0.2.3/psiaudio/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:46:17.000000 psiaudio-0.2.3/psiaudio/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   142772 2023-07-14 17:46:17.000000 psiaudio-0.2.3/psiaudio/resources/starship_cal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    48979 2023-07-14 17:46:17.000000 psiaudio-0.2.3/psiaudio/stim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35478 2023-07-14 17:46:17.000000 psiaudio-0.2.3/psiaudio/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 17:46:31.000000 psiaudio-0.2.3/psiaudio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:46:31.492068 psiaudio-0.2.3/psiaudio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-14 17:46:31.000000 psiaudio-0.2.3/psiaudio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-14 17:46:31.000000 psiaudio-0.2.3/psiaudio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:46:31.000000 psiaudio-0.2.3/psiaudio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-14 17:46:31.000000 psiaudio-0.2.3/psiaudio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 17:46:31.000000 psiaudio-0.2.3/psiaudio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-14 17:46:17.000000 psiaudio-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-14 17:46:17.000000 psiaudio-0.2.3/release.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:46:31.492068 psiaudio-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:46:31.492068 psiaudio-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-14 17:46:17.000000 psiaudio-0.2.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-14 17:46:17.000000 psiaudio-0.2.3/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27785 2023-07-14 17:46:17.000000 psiaudio-0.2.3/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19018 2023-07-14 17:46:17.000000 psiaudio-0.2.3/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-07-14 17:46:17.000000 psiaudio-0.2.3/tests/test_signal_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14153 2023-07-14 17:46:17.000000 psiaudio-0.2.3/tests/test_stim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-14 17:46:17.000000 psiaudio-0.2.3/tests/test_stim_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-14 17:46:17.000000 psiaudio-0.2.3/tests/test_stim_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-07-14 17:46:17.000000 psiaudio-0.2.3/tests/test_util.py
```

### Comparing `psiaudio-0.2.2/.github/workflows/publish-to-pypi.yml` & `psiaudio-0.2.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/.gitignore` & `psiaudio-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/.readthedocs.yaml` & `psiaudio-0.2.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/LICENSE.txt` & `psiaudio-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/PKG-INFO` & `psiaudio-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psiaudio
-Version: 0.2.2
+Version: 0.2.3
 Summary: Audio tools supporting psiexperiment
 Author-email: Brad Buran <bburan@alum.mit.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 Maintainer-email: Brad Buran <bburan@alum.mit.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: examples
 Provides-Extra: docs
```

### Comparing `psiaudio-0.2.2/README.md` & `psiaudio-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/docs/Makefile` & `psiaudio-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/docs/make.bat` & `psiaudio-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/docs/source/conf.py` & `psiaudio-0.2.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/examples/gallery/bandlimited-click.py` & `psiaudio-0.2.3/examples/gallery/bandlimited-click.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/examples/gallery/calibration-basics.py` & `psiaudio-0.2.3/examples/gallery/calibration-basics.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/examples/gallery/chirp.py` & `psiaudio-0.2.3/examples/gallery/chirp.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/examples/gallery/notch-noise-abr.py` & `psiaudio-0.2.3/examples/gallery/notch-noise-abr.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/examples/gallery/queue-introduction.py` & `psiaudio-0.2.3/examples/gallery/queue-introduction.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/examples/gallery/queueing-wav-files.py` & `psiaudio-0.2.3/examples/gallery/queueing-wav-files.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/examples/gallery/repeat-chirp.py` & `psiaudio-0.2.3/examples/gallery/repeat-chirp.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/examples/gallery/stimulus-generation.py` & `psiaudio-0.2.3/examples/gallery/stimulus-generation.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/examples/gallery/tone-complex.py` & `psiaudio-0.2.3/examples/gallery/tone-complex.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/examples/gallery/tone-pips.py` & `psiaudio-0.2.3/examples/gallery/tone-pips.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/examples/play-wav-files.py` & `psiaudio-0.2.3/examples/play-wav-files.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/examples/wav-files/00cat172_rec1_geese_excerpt1.wav` & `psiaudio-0.2.3/examples/wav-files/00cat172_rec1_geese_excerpt1.wav`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/examples/wav-files/00cat221_rec1_laughing_excerpt1.wav` & `psiaudio-0.2.3/examples/wav-files/00cat221_rec1_laughing_excerpt1.wav`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/examples/wav-files/00cat28_rec1_bigband_bbc-big-band_american-patrol_0sec_excerpt1.wav` & `psiaudio-0.2.3/examples/wav-files/00cat28_rec1_bigband_bbc-big-band_american-patrol_0sec_excerpt1.wav`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/examples/wav-files/00cat78_rec1_chimes_in_the_wind_excerpt1.wav` & `psiaudio-0.2.3/examples/wav-files/00cat78_rec1_chimes_in_the_wind_excerpt1.wav`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/examples/wav-files/00cat83_rec1_cicadas_excerpt1.wav` & `psiaudio-0.2.3/examples/wav-files/00cat83_rec1_cicadas_excerpt1.wav`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/examples/wav-files/00cat92_rec1_country_song_excerpt1.wav` & `psiaudio-0.2.3/examples/wav-files/00cat92_rec1_country_song_excerpt1.wav`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/psiaudio/__init__.py` & `psiaudio-0.2.3/psiaudio/__init__.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/psiaudio/buffer.py` & `psiaudio-0.2.3/psiaudio/buffer.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/psiaudio/calibration.py` & `psiaudio-0.2.3/psiaudio/calibration.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/psiaudio/pipeline.py` & `psiaudio-0.2.3/psiaudio/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 log = logging.getLogger(__name__)
 
 from collections import deque
 from copy import copy
+from threading import Event
 
 import numpy as np
 import pandas as pd
 from scipy import signal
 
 from . import util
 
@@ -609,15 +610,15 @@
                 target(data)
                 break
 
 
 @coroutine
 def extract_epochs(fs, queue, epoch_size, target, buffer_size=0,
                    empty_queue_cb=None, removed_queue=None, prestim_time=0,
-                   poststim_time=0):
+                   poststim_time=0, source_complete=None):
     '''
     Coroutine to facilitate extracting epochs from an incoming stream of data
 
 
     Parameters
     ----------
     fs : float
@@ -650,14 +651,19 @@
         `queue`). If the epoch has not been fully captured yet, this epoch will
         be removed from the list of epochs to capture.
     prestim_time : float
         Additional time to capture before the specified epoch start.
     poststim_time : float
         Additional time to capture beyond the specified epoch size (or
         `duration`).
+    source_complete : {None, Event}
+        If None, assume that once there are no more epochs to extract and call
+        the empty_queue_cb notification. If an Event, the empty_queue_cb
+        notification will be fired once the Event is set and there are no more
+        epochs to extract.
     '''
     # The variable `tlb` tracks the number of samples that have been acquired
     # and reflects the lower bound of `data`. For example, if we have acquired
     # 300,000 samples, then the next chunk of data received from (yield) will
     # start at sample 300,000 (remember that Python is zero-based indexing, so
     # the first sample has an index of 0).
     tlb = 0
@@ -677,14 +683,23 @@
     buffer_samples = round(buffer_size * fs)
 
     # Since we may capture very short, rapidly occurring epochs (at, say,
     # 80 per second), I find it best to accumulate as many epochs as possible before
     # calling the next target. This list will maintain the accumulated set.
     epochs = []
 
+    # Create dummy event and auto-set it to generate old behavior (where we
+    # call the queue_complete_cb as soon as we have no more epochs to capture).
+    # The problem with this old behavior si that if there is a long interval in
+    # between stimuli, the next epoch may not be generated until all pending
+    # epochs have been captured.
+    if source_complete is None:
+        source_complete = Event()
+        source_complete.set()
+
     # This is used for communicating events
     if removed_queue is None:
         removed_queue = deque()
 
     while True:
         # Wait for new data to become available
         data = (yield)
@@ -778,15 +793,18 @@
             oldest_samples = prior_samples[0]
             tub = oldest_samples[0] + oldest_samples[1].shape[-1]
             if tub < (tlb - buffer_samples):
                 prior_samples.pop(0)
             else:
                 break
 
-        if not (queue or epoch_coroutines) and empty_queue_cb:
+        if source_complete.is_set() \
+                and (len(queue) == 0) \
+                and (len(epoch_coroutines) == 0) \
+                and (empty_queue_cb is not None):
             # If queue and epoch coroutines are complete, call queue callback
             # once and only once.
             empty_queue_cb()
             empty_queue_cb = None
 
 
 @coroutine
```

### Comparing `psiaudio-0.2.2/psiaudio/plot.py` & `psiaudio-0.2.3/psiaudio/plot.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/psiaudio/queue.py` & `psiaudio-0.2.3/psiaudio/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         self._samples = 0
 
         # Callbacks to trigger for the specified event.
         self._notifiers = {
             'added': [],
             'removed': [],
             'decrement': [],
+            'empty': [],
         }
 
         # Is stimulus generation paused?
         self._paused = False
 
         # Is queue complete?
         self._empty = False
@@ -72,14 +73,17 @@
         # Start time of queue relative to acquisition start.
         self._t0 = 0
 
         # Tracks waveforms generated by queue. This is used in the event we
         # need to pause stimulus generation.
         self._generated = []
 
+    def clone(self):
+        return copy.deepcopy(self)
+
     @property
     def fs(self):
         return self._fs
 
     def get_ts(self):
         return self._samples / self._fs
 
@@ -102,15 +106,16 @@
         Perhaps we should drop rewind_samples and make it set_time with no
         requirement that the new time be related to the old time in any
         particular way.
         '''
         # Reset the samples
         new_sample = int(round((t - self._t0) * self._fs))
         if check and (new_sample > self._samples):
-            raise ValueError(f'Cannot rewind past last sample generated. Requested {t:.3f}s, last sample was {self.get_ts():.3f}s.')
+            raise ValueError(f'Cannot rewind past last sample generated. ' \
+                             'Requested {t:.3f}s, last sample was {self.get_ts():.3f}s.')
         self._samples = new_sample
         log.debug('Rewound queue samples back to %d', self._samples)
 
     def pause(self, t=None):
         log.debug('Pausing queue')
         self._paused = True
         if t is not None:
@@ -398,14 +403,15 @@
         while samples > 0:
             try:
                 waveform = self._pop_buffer(samples, decrement)
             except QueueEmptyError:
                 log.info('Queue is empty')
                 waveform = np.zeros(samples)
                 self._empty = True
+                self._notify('empty', {})
             samples -= len(waveform)
             self._samples += len(waveform)
             waveforms.append(waveform)
         waveform = np.concatenate(waveforms, axis=-1)
         log.trace('Generated %d samples', len(waveform))
         return waveform
```

### Comparing `psiaudio-0.2.2/psiaudio/resources/starship_cal.csv` & `psiaudio-0.2.3/psiaudio/resources/starship_cal.csv`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/psiaudio/stim.py` & `psiaudio-0.2.3/psiaudio/stim.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 log = logging.getLogger(__name__)
 
 from functools import partial
 import itertools
 from pathlib import Path
 
 import numpy as np
+import pandas as pd
 from scipy import signal
 from scipy.io import wavfile
 
+from . import audiograms
 from . import util
 from . import queue
 
 
 def fast_cache(f):
     cache = {}
     kwd_marker = object()
@@ -21,14 +23,33 @@
         if key not in cache:
             cache[key] = f(*args, **kw)
         return cache[key]
     return wrapper
 
 
 ################################################################################
+# Utilities
+################################################################################
+def apply_max_correction(sf, max_correction):
+    db = util.db(sf)
+    db_mean = np.mean(db)
+    db_min = db_mean - max_correction
+    db_max = db_mean + max_correction
+    return util.dbi(np.clip(db, db_min, db_max))
+
+
+def apply_audiogram_weighting(freq, sf, audiogram_weighting):
+    audiogram = pd.Series(getattr(audiograms, audiogram_weighting))
+    a_freq = audiogram.index.values
+    a_level = audiogram.values
+    a_level -= a_level.min()
+    return sf * np.interp(freq, a_freq, util.dbi(a_level))
+
+
+################################################################################
 # Base classes
 ################################################################################
 class Waveform:
 
     def reset(self):
         raise NotImplementedError
 
@@ -100,14 +121,17 @@
 
     def get_duration(self):
         return len(self.waveform)/self.fs
 
     def is_complete(self):
         return self.offset >= len(self.waveform)
 
+    def max_amplitude(self):
+        return np.abs(self.waveform).max()
+
 
 class Carrier(Waveform):
     '''
     A continuous waveform
     '''
 
     def get_duration(self):
@@ -174,14 +198,17 @@
         if lb >= 0:
             token[:lb] = 0
         if ub > 0:
             token[ub:] = 0
         self.offset += samples
         return token
 
+    def max_amplitude(self):
+        return self.input_factory.max_amplitude()
+
 
 ################################################################################
 # Gated envelopes
 ################################################################################
 @fast_cache
 def envelope(window, fs, duration, rise_time=None, offset=0, start_time=0,
              samples='auto'):
@@ -386,14 +413,17 @@
     def __init__(self, fs, depth, fm, duty_cycle, calibration, input_factory):
         vars(self).update(locals())
 
     def env(self, samples):
         return square_wave(self.fs, self.offset, samples, self.depth, self.fm,
                            self.duty_cycle)
 
+    def max_amplitude(self):
+        return self.input_factory.max_amplitude()
+
 
 ################################################################################
 # Broadband noise
 ################################################################################
 class BroadbandNoiseFactory(Carrier):
     '''
     Factory for generating continuous bandlimited noise
@@ -557,31 +587,68 @@
 class BandlimitedFIRNoiseFactory(Carrier):
     '''
     Factory for generating continuous shaped noise using FIR filters.
 
     This is similar to shaped noise, but with simpler inputs if all you want is
     bandlimited noise (i.e., no requirement to generate the dictionary of
     gains).
+
+    Parameters
+    ----------
+    fs : float
+        Sampling rate of stimuli
+    fl : float
+        Lower frequency of noise band
+    fh : float
+        Upper frequency of noise band
+    level : float
+        Noise level
+    ntaps : int
+        Number of taps to use for FIR filter. The default generally works well.
+    window : string
+        Any valid window name offered by scipy. This is passed to firwin2.
+    polarity : int
+        Can be used to invert the polarity
+    seed : {None, int}
+        Set the seed if you want to generate frozen, reproducible noise.
+    max_correction : float
+        Maximum amount to adjust noise when equalizing based on speaker
+        calibration. Over-correcting the noise may lead to some very large
+        amplitudes and limit the range of possible stimulus levels. If noise is
+        not equalized, this setting is ignored.
+    equalize : bool
+        Equalize the noise based on the calibration to generate spectrally flat
+        noise?
+    calibration : instance of psiaudio.calibration.BaseCalibration
+        Used to generate the appropriate noise amplitude (and equalize the
+        noise if requested).
     '''
     def __init__(self, fs, fl, fh, level, ntaps=1001, window='hann',
-                 polarity=1, seed=None, equalize=False, calibration=None):
+                 polarity=1, seed=None, max_correction=np.inf, equalize=False,
+                 calibration=None, audiogram_weighting=None):
         vars(self).update(locals())
 
         if calibration is None:
             raise NotImplemented
 
         # Calculate the gains for the shaped noise
         if equalize:
             freq = np.arange(fl, fh + 1)
             sf = calibration.get_sf(freq, level)
         else:
             freq = np.array([fl, fh])
             sf = calibration.get_mean_sf(fl, fh, level)
             sf = np.full_like(freq, fill_value=sf)
 
+        if max_correction is not None and equalize:
+            sf = apply_max_correction(sf, max_correction)
+
+        if audiogram_weighting is not None:
+            sf = apply_audiogram_weighting(freq, sf, audiogram_weighting)
+
         freq = np.concatenate(([0, fl / 1.1], freq, [fh * 1.1, fs / 2]))
         sf = np.pad(sf, 2)
 
         self.taps = signal.firwin2(ntaps, freq=freq, gain=sf, window=window, fs=fs)
         self.initial_zi = signal.lfilter_zi(self.taps, [1])
 
         # The RMS value of noise drawn from a uniform distribution is
@@ -846,14 +913,19 @@
         # rather than cache the result.
         waveform = tone(self.fs, self.frequency, self.level, self.phase,
                         self.polarity, calibration=self.calibration,
                         offset=self.offset, samples=samples)
         self.offset += samples
         return waveform
 
+    def max_amplitude(self):
+        rms = self.level if self.calibration is None \
+            else self.calibration.get_sf(self.frequency, self.level)
+        return rms * np.sqrt(2) * 1.1
+
 
 ################################################################################
 # SAMTone
 ################################################################################
 def sam_tone(fs, fc, fm, level, depth=1, phase=0, polarity=1, calibration=None,
              samples='auto', offset=0, duration=None, eq_power=True,
              equalize=True):
@@ -926,14 +998,19 @@
             depth=self.depth, phase=self.phase, polarity=self.polarity,
             eq_power=self.eq_power, equalize=self.equalize,
             calibration=self.calibration, offset=self.offset, samples=samples
         )
         self.offset += samples
         return waveform
 
+    def max_amplitude(self):
+        rms = self.level if self.calibration is None \
+            else self.calibration.get_sf(self.fc, self.level)
+        return rms * np.sqrt(2) * 1.1 * 3
+
 
 ################################################################################
 # Silence
 ################################################################################
 class SilenceFactory(Carrier):
     '''
     Generate silence
@@ -1021,15 +1098,16 @@
     return result.ravel()
 
 
 ################################################################################
 # Chirp
 ################################################################################
 def chirp(fs, start_frequency, end_frequency, duration, level,
-          calibration=None, window='boxcar', equalize=False):
+          calibration=None, window='boxcar', equalize=False,
+          max_correction=np.inf, audiogram_weighting=None):
     '''
     Notes
     -----
     Windowing algorithm was implemented as described in Neumann et al., 1994 to
     enable implementation of the Hann windowed chirp in the middel ear acoustic
     reflex assay described by Valero et al., 2016.
     '''
@@ -1054,35 +1132,39 @@
         sf = level
     else:
         if not equalize:
             sf = calibration.get_mean_sf(start_frequency, end_frequency, level)
         else:
             sf = calibration.get_sf(ifreq, level)
 
+    if max_correction is not None and equalize:
+        sf = apply_max_correction(sf, max_correction)
+
+    if audiogram_weighting is not None:
+        sf = apply_audiogram_weighting(ifreq, sf, audiogram_weighting)
+
     # We need to normalize the window so that it has a RMS of 1. Then, we
     # multiply by the square root of 2 since we are using the sin function
     # (e.g. Vpeak = np.sqrt(2) * Vrms). Finally, multiply by the scaling factor
     # that gives us our desired level.
     w /= util.rms(w)
     return np.sqrt(2) * sf * w * np.sin(2 * np.pi * phase)
 
 
 class ChirpFactory(FixedWaveform):
 
     def __init__(self, fs, start_frequency, end_frequency, duration, level,
-                 calibration, window='boxcar', equalize=False):
+                 calibration, window='boxcar', equalize=False,
+                 max_correction=np.inf, audiogram_weighting=None):
         kwargs = locals()
         kwargs.pop('self')
         vars(self).update(kwargs)
         self.waveform = chirp(**kwargs)
         self.reset()
 
-    def max_amplitude(self):
-        return np.abs(self.waveform).max()
-
 
 ################################################################################
 # Click
 ################################################################################
 class ClickFactory(FixedWaveform):
 
     def __init__(self, fs, duration, level, polarity, calibration):
@@ -1093,58 +1175,67 @@
         self.reset()
 
 
 ################################################################################
 # Bandlimited Click
 ################################################################################
 def bandlimited_click(fs, flb, fub, window=0.1, level=1, calibration=None,
-                      equalize=False):
+                      equalize=False, max_correction=np.inf,
+                      audiogram_weighting=None):
     '''
     Generate bandlimited click.
 
     Parameters
     ----------
 
     The click waveform will be symmetric around the center of the window.
     '''
-
     n_window = int(round(window * fs))
     n = int(round(fs))
     freq = np.fft.rfftfreq(n, d=1/fs)
+    log.error(freq)
     psd = np.zeros_like(freq)
     m = (freq >= flb) & (freq < fub)
-    psd[m] = 1
+    #psd[m] = 1
 
     if calibration is None:
-        if equalize:
-            raise ValueError('Cannot equalize signal without calibration')
         sf = level
     else:
-        if not equalize:
-            sf = calibration.get_sf(freq[m], level)
-            psd[m] = psd[m] * sf / sf.mean()
-        else:
-            sf = calibration.get_sf(freq[m], level)
+        band_level = util.band_to_spectrum_level(level, m.sum())
+        sf = calibration.get_sf(freq[m], band_level)
+
+    if max_correction is not None and equalize:
+        sf = apply_max_correction(sf, max_correction)
+
+    if audiogram_weighting is not None:
+        sf = apply_audiogram_weighting(freq[m], sf, audiogram_weighting)
+
+    #if equalize:
+    #    psd[m] = psd[m] * sf / sf.mean()
+    psd[m] = sf
 
     sf = util.dbi(util.db(sf).mean())
 
     csd = psd * np.exp(-1j * freq * 2 * np.pi * 0.5)
     waveform = util.csd_to_signal(csd)
-    waveform = waveform / waveform.ptp() * sf
+    #waveform = waveform / waveform.ptp() * sf
     lb = int(round(n / 2 - n_window / 2))
     waveform = waveform[lb:lb+n_window]
     return waveform
 
 
 class BandlimitedClickFactory(FixedWaveform):
 
-    def __init__(self, fs, flb, fub, window, level, calibration):
-        vars(self).update(locals())
-        self.waveform = bandlimited_click(fs, flb, fub, window, level=level,
-                                          calibration=calibration)
+    def __init__(self, fs, flb, fub, window, level, calibration=None,
+                 equalize=False, max_correction=np.inf,
+                 audiogram_weighting=None):
+        kwargs = locals()
+        kwargs.pop('self')
+        vars(self).update(kwargs)
+        self.waveform = bandlimited_click(**kwargs)
         self.reset()
 
 
 ################################################################################
 # Wavfiles
 ################################################################################
 @fast_cache
```

### Comparing `psiaudio-0.2.2/psiaudio/util.py` & `psiaudio-0.2.3/psiaudio/util.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/psiaudio.egg-info/PKG-INFO` & `psiaudio-0.2.3/psiaudio.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psiaudio
-Version: 0.2.2
+Version: 0.2.3
 Summary: Audio tools supporting psiexperiment
 Author-email: Brad Buran <bburan@alum.mit.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 Maintainer-email: Brad Buran <bburan@alum.mit.edu>, "Buran Consulting, LLC" <info@bradburan.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: examples
 Provides-Extra: docs
```

### Comparing `psiaudio-0.2.2/psiaudio.egg-info/SOURCES.txt` & `psiaudio-0.2.3/psiaudio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 examples/wav-files/00cat172_rec1_geese_excerpt1.wav
 examples/wav-files/00cat221_rec1_laughing_excerpt1.wav
 examples/wav-files/00cat28_rec1_bigband_bbc-big-band_american-patrol_0sec_excerpt1.wav
 examples/wav-files/00cat78_rec1_chimes_in_the_wind_excerpt1.wav
 examples/wav-files/00cat83_rec1_cicadas_excerpt1.wav
 examples/wav-files/00cat92_rec1_country_song_excerpt1.wav
 psiaudio/__init__.py
+psiaudio/audiograms.py
 psiaudio/buffer.py
 psiaudio/calibration.py
 psiaudio/pipeline.py
 psiaudio/plot.py
 psiaudio/queue.py
 psiaudio/stim.py
 psiaudio/util.py
```

### Comparing `psiaudio-0.2.2/pyproject.toml` & `psiaudio-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/release.md` & `psiaudio-0.2.3/release.md`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/tests/conftest.py` & `psiaudio-0.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/tests/test_calibration.py` & `psiaudio-0.2.3/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/tests/test_pipeline.py` & `psiaudio-0.2.3/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/tests/test_queue.py` & `psiaudio-0.2.3/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/tests/test_signal_buffer.py` & `psiaudio-0.2.3/tests/test_signal_buffer.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/tests/test_stim.py` & `psiaudio-0.2.3/tests/test_stim.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/tests/test_stim_factory.py` & `psiaudio-0.2.3/tests/test_stim_factory.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/tests/test_stim_noise.py` & `psiaudio-0.2.3/tests/test_stim_noise.py`

 * *Files identical despite different names*

### Comparing `psiaudio-0.2.2/tests/test_util.py` & `psiaudio-0.2.3/tests/test_util.py`

 * *Files identical despite different names*

