# Comparing `tmp/weewx-5.0.0b8.tar.gz` & `tmp/weewx-5.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weewx-5.0.0b8.tar", max compression
+gzip compressed data, was "weewx-5.0.0b9.tar", max compression
```

## Comparing `weewx-5.0.0b8.tar` & `weewx-5.0.0b9.tar`

### file list

```diff
@@ -1,512 +1,512 @@
--rw-r--r--   0        0        0    32472 2023-05-30 12:01:49.265499 weewx-5.0.0b8/LICENSE.txt
--rw-r--r--   0        0        0     3725 2023-07-11 14:40:18.430439 weewx-5.0.0b8/README.md
--rw-r--r--   0        0        0      230 2023-05-30 12:01:49.265499 weewx-5.0.0b8/bin/schemas/__init__.py
--rw-r--r--   0        0        0     3448 2023-05-30 12:01:49.269499 weewx-5.0.0b8/bin/schemas/wview.py
--rw-r--r--   0        0        0     5953 2023-05-30 12:01:49.269499 weewx-5.0.0b8/bin/schemas/wview_extended.py
--rw-r--r--   0        0        0     2105 2023-05-30 12:01:49.269499 weewx-5.0.0b8/bin/schemas/wview_small.py
--rwxr-xr-x   0        0        0    52292 2023-07-11 14:40:18.430439 weewx-5.0.0b8/bin/wee_database.py
--rwxr-xr-x   0        0        0    16172 2023-07-11 14:40:18.430439 weewx-5.0.0b8/bin/wee_debug.py
--rwxr-xr-x   0        0        0     2187 2023-07-11 14:40:18.430439 weewx-5.0.0b8/bin/wee_device.py
--rwxr-xr-x   0        0        0    38911 2023-07-11 14:40:18.430439 weewx-5.0.0b8/bin/wee_import.py
--rwxr-xr-x   0        0        0     5630 2023-07-11 14:40:18.430439 weewx-5.0.0b8/bin/wee_reports.py
--rw-r--r--   0        0        0        0 2023-07-11 19:25:45.005305 weewx-5.0.0b8/bin/wee_resources/__init__.py
--rw-r--r--   0        0        0      306 2023-05-30 12:01:49.269499 weewx-5.0.0b8/bin/wee_resources/bin/user/__init__.py
--rw-r--r--   0        0        0      324 2023-07-11 16:35:41.678500 weewx-5.0.0b8/bin/wee_resources/bin/user/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      398 2023-07-11 16:35:41.678500 weewx-5.0.0b8/bin/wee_resources/bin/user/__pycache__/extensions.cpython-37.pyc
--rw-r--r--   0        0        0      541 2023-05-30 12:01:49.269499 weewx-5.0.0b8/bin/wee_resources/bin/user/extensions.py
--rw-r--r--   0        0        0    33399 2023-07-11 16:33:27.114872 weewx-5.0.0b8/bin/wee_resources/docs/404.html
--rw-r--r--   0        0        0     1870 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/images/favicon.png
--rw-r--r--   0        0        0   113489 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/bundle.b4d07000.min.js
--rw-r--r--   0        0        0   954781 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/bundle.b4d07000.min.js.map
--rw-r--r--   0        0        0    17074 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-r--r--   0        0        0     4654 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.da.min.js
--rw-r--r--   0        0        0     6119 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.de.min.js
--rw-r--r--   0        0        0     6208 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.du.min.js
--rw-r--r--   0        0        0    11499 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.es.min.js
--rw-r--r--   0        0        0     9342 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-r--r--   0        0        0    10669 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-r--r--   0        0        0     3383 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hi.min.js
--rw-r--r--   0        0        0     9437 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-r--r--   0        0        0     1264 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hy.min.js
--rw-r--r--   0        0        0    11232 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.it.min.js
--rw-r--r--   0        0        0     2313 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-r--r--   0        0        0       36 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-r--r--   0        0        0     3494 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.kn.min.js
--rw-r--r--   0        0        0     7972 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ko.min.js
--rw-r--r--   0        0        0      817 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-r--r--   0        0        0     6026 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-r--r--   0        0        0     4754 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.no.min.js
--rw-r--r--   0        0        0    10171 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-r--r--   0        0        0    10958 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-r--r--   0        0        0    10331 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-r--r--   0        0        0     4901 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sa.min.js
--rw-r--r--   0        0        0     3647 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-r--r--   0        0        0     4523 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-r--r--   0        0        0     2406 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ta.min.js
--rw-r--r--   0        0        0     2330 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.te.min.js
--rw-r--r--   0        0        0     1031 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.th.min.js
--rw-r--r--   0        0        0    15009 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-r--r--   0        0        0      784 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-r--r--   0        0        0     2158 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.zh.min.js
--rw-r--r--   0        0        0    22878 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/tinyseg.js
--rw-r--r--   0        0        0   677463 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/wordcut.js
--rw-r--r--   0        0        0    38916 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/workers/search.208ed371.min.js
--rw-r--r--   0        0        0   209901 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/workers/search.208ed371.min.js.map
--rw-r--r--   0        0        0   113455 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/stylesheets/main.85bb2934.min.css
--rw-r--r--   0        0        0    38958 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/stylesheets/main.85bb2934.min.css.map
--rw-r--r--   0        0        0    12227 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/stylesheets/palette.a6bdf11c.min.css
--rw-r--r--   0        0        0     3628 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/assets/stylesheets/palette.a6bdf11c.min.css.map
--rw-r--r--   0        0        0   195549 2023-07-11 16:33:27.158872 weewx-5.0.0b8/bin/wee_resources/docs/changes/index.html
--rw-r--r--   0        0        0    36103 2023-07-11 16:33:27.158872 weewx-5.0.0b8/bin/wee_resources/docs/copyright/index.html
--rw-r--r--   0        0        0      565 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/css/tocbot-4.12.0.css
--rw-r--r--   0        0        0      565 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/css/tocbot-4.3.1.css
--rw-r--r--   0        0        0    12148 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/css/weewx_ui.css
--rw-r--r--   0        0        0    63176 2023-07-11 16:33:27.238871 weewx-5.0.0b8/bin/wee_resources/docs/custom/appendix/index.html
--rw-r--r--   0        0        0   141313 2023-07-11 16:33:27.274871 weewx-5.0.0b8/bin/wee_resources/docs/custom/cheetah/index.html
--rw-r--r--   0        0        0    72909 2023-07-11 16:33:27.290871 weewx-5.0.0b8/bin/wee_resources/docs/custom/custom-reports/index.html
--rw-r--r--   0        0        0    60588 2023-07-11 16:33:27.298871 weewx-5.0.0b8/bin/wee_resources/docs/custom/database/index.html
--rw-r--r--   0        0        0    35129 2023-07-11 16:33:27.302871 weewx-5.0.0b8/bin/wee_resources/docs/custom/derived/index.html
--rw-r--r--   0        0        0    49424 2023-07-11 16:33:27.306871 weewx-5.0.0b8/bin/wee_resources/docs/custom/drivers/index.html
--rw-r--r--   0        0        0    40791 2023-07-11 16:33:27.310871 weewx-5.0.0b8/bin/wee_resources/docs/custom/extensions/index.html
--rw-r--r--   0        0        0    62049 2023-07-11 16:33:27.318871 weewx-5.0.0b8/bin/wee_resources/docs/custom/image-generator/index.html
--rw-r--r--   0        0        0    71330 2023-07-11 16:33:27.226872 weewx-5.0.0b8/bin/wee_resources/docs/custom/index.html
--rw-r--r--   0        0        0    65342 2023-07-11 16:33:27.334871 weewx-5.0.0b8/bin/wee_resources/docs/custom/localization/index.html
--rw-r--r--   0        0        0    48294 2023-07-11 16:33:27.338871 weewx-5.0.0b8/bin/wee_resources/docs/custom/multiple-bindings/index.html
--rw-r--r--   0        0        0   120067 2023-07-11 16:33:27.362871 weewx-5.0.0b8/bin/wee_resources/docs/custom/report-options/index.html
--rw-r--r--   0        0        0    51431 2023-07-11 16:33:27.366871 weewx-5.0.0b8/bin/wee_resources/docs/custom/report-scheduling/index.html
--rw-r--r--   0        0        0    83864 2023-07-11 16:33:27.390871 weewx-5.0.0b8/bin/wee_resources/docs/custom/service-engine/index.html
--rw-r--r--   0        0        0    46163 2023-07-11 16:33:27.398871 weewx-5.0.0b8/bin/wee_resources/docs/custom/units/index.html
--rw-r--r--   0        0        0    71514 2023-07-11 16:33:27.170872 weewx-5.0.0b8/bin/wee_resources/docs/devnotes/index.html
--rw-r--r--   0        0        0     2747 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/examples/tag.htm
--rw-r--r--   0        0        0    41207 2023-07-11 16:33:27.402871 weewx-5.0.0b8/bin/wee_resources/docs/hardware/acurite/index.html
--rw-r--r--   0        0        0    62276 2023-07-11 16:33:27.410871 weewx-5.0.0b8/bin/wee_resources/docs/hardware/cc3000/index.html
--rw-r--r--   0        0        0    56883 2023-07-11 16:33:27.426871 weewx-5.0.0b8/bin/wee_resources/docs/hardware/drivers/index.html
--rw-r--r--   0        0        0    48895 2023-07-11 16:33:27.430871 weewx-5.0.0b8/bin/wee_resources/docs/hardware/fousb/index.html
--rw-r--r--   0        0        0    47564 2023-07-11 16:33:27.438871 weewx-5.0.0b8/bin/wee_resources/docs/hardware/te923/index.html
--rw-r--r--   0        0        0    39191 2023-07-11 16:33:27.442871 weewx-5.0.0b8/bin/wee_resources/docs/hardware/ultimeter/index.html
--rw-r--r--   0        0        0    69436 2023-07-11 16:33:27.454871 weewx-5.0.0b8/bin/wee_resources/docs/hardware/vantage/index.html
--rw-r--r--   0        0        0    43746 2023-07-11 16:33:27.458871 weewx-5.0.0b8/bin/wee_resources/docs/hardware/wmr100/index.html
--rw-r--r--   0        0        0    43859 2023-07-11 16:33:27.466871 weewx-5.0.0b8/bin/wee_resources/docs/hardware/wmr300/index.html
--rw-r--r--   0        0        0    43390 2023-07-11 16:33:27.470871 weewx-5.0.0b8/bin/wee_resources/docs/hardware/wmr9x8/index.html
--rw-r--r--   0        0        0    38474 2023-07-11 16:33:27.474871 weewx-5.0.0b8/bin/wee_resources/docs/hardware/ws1/index.html
--rw-r--r--   0        0        0    45261 2023-07-11 16:33:27.478871 weewx-5.0.0b8/bin/wee_resources/docs/hardware/ws23xx/index.html
--rw-r--r--   0        0        0    50877 2023-07-11 16:33:27.482871 weewx-5.0.0b8/bin/wee_resources/docs/hardware/ws28xx/index.html
--rw-r--r--   0        0        0    54196 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/antialias.gif
--rw-r--r--   0        0        0     3145 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/day-gap-not-shown.png
--rw-r--r--   0        0        0     3269 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/day-gap-showing.png
--rw-r--r--   0        0        0     7579 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/daycompare.png
--rw-r--r--   0        0        0     8705 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/daytemp_with_avg.png
--rw-r--r--   0        0        0     7803 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/dayvaporp.png
--rw-r--r--   0        0        0     7663 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/daywindvec.png
--rw-r--r--   0        0        0     1026 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/favicon.png
--rw-r--r--   0        0        0    38406 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/ferrites.jpg
--rw-r--r--   0        0        0     3638 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/funky_degree.png
--rw-r--r--   0        0        0    19123 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/image_parts.png
--rw-r--r--   0        0        0    86388 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/image_parts.xcf
--rw-r--r--   0        0        0     2136 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/logo-apple.png
--rw-r--r--   0        0        0     4734 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/logo-centos.png
--rw-r--r--   0        0        0    14541 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/logo-debian.png
--rw-r--r--   0        0        0    24662 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/logo-fedora.png
--rw-r--r--   0        0        0    12046 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/logo-linux.png
--rw-r--r--   0        0        0    27245 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/logo-mint.png
--rw-r--r--   0        0        0    15980 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/logo-opensuse.png
--rw-r--r--   0        0        0    14374 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/logo-pypi.svg
--rw-r--r--   0        0        0     1192 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/logo-redhat.png
--rw-r--r--   0        0        0     3926 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/logo-rpi.png
--rw-r--r--   0        0        0     7877 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/logo-suse.png
--rw-r--r--   0        0        0    13954 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/logo-ubuntu.png
--rw-r--r--   0        0        0    12208 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/logo-weewx.png
--rw-r--r--   0        0        0    35496 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/pipeline.png
--rw-r--r--   0        0        0     6709 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/sample_monthrain.png
--rw-r--r--   0        0        0    10107 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/sample_monthtempdew.png
--rw-r--r--   0        0        0    10649 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/weekgustoverlay.png
--rw-r--r--   0        0        0     8468 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/weektempdew.png
--rw-r--r--   0        0        0     6602 2023-07-11 16:33:27.014872 weewx-5.0.0b8/bin/wee_resources/docs/images/yeardiff.png
--rw-r--r--   0        0        0     7286 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/images/yearhilow.png
--rw-r--r--   0        0        0    39824 2023-07-11 16:33:27.130872 weewx-5.0.0b8/bin/wee_resources/docs/index.html
--rw-r--r--   0        0        0    32611 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/js/cash.js
--rw-r--r--   0        0        0    14828 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/js/cash.min.js
--rw-r--r--   0        0        0    11422 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/js/tocbot-4.12.0.js
--rw-r--r--   0        0        0    11422 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/js/tocbot-4.12.0.min.js
--rw-r--r--   0        0        0     8892 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/js/tocbot-4.3.1.min.js
--rw-r--r--   0        0        0     4640 2023-07-11 16:33:27.018872 weewx-5.0.0b8/bin/wee_resources/docs/js/weewx.js
--rw-r--r--   0        0        0    44267 2023-07-11 16:33:27.486871 weewx-5.0.0b8/bin/wee_resources/docs/quickstarts/debian/index.html
--rw-r--r--   0        0        0    45484 2023-07-11 16:33:27.494871 weewx-5.0.0b8/bin/wee_resources/docs/quickstarts/git/index.html
--rw-r--r--   0        0        0    35086 2023-07-11 16:33:27.482871 weewx-5.0.0b8/bin/wee_resources/docs/quickstarts/index.html
--rw-r--r--   0        0        0    61417 2023-07-11 16:33:27.514871 weewx-5.0.0b8/bin/wee_resources/docs/quickstarts/pip/index.html
--rw-r--r--   0        0        0    43066 2023-07-11 16:33:27.518871 weewx-5.0.0b8/bin/wee_resources/docs/quickstarts/redhat/index.html
--rw-r--r--   0        0        0    42005 2023-07-11 16:33:27.522871 weewx-5.0.0b8/bin/wee_resources/docs/quickstarts/suse/index.html
--rw-r--r--   0        0        0  1044277 2023-07-11 16:33:27.698871 weewx-5.0.0b8/bin/wee_resources/docs/search/search_index.json
--rw-r--r--   0        0        0    12774 2023-07-11 16:33:27.114872 weewx-5.0.0b8/bin/wee_resources/docs/sitemap.xml
--rw-r--r--   0        0        0      754 2023-07-11 16:33:27.114872 weewx-5.0.0b8/bin/wee_resources/docs/sitemap.xml.gz
--rw-r--r--   0        0        0    95541 2023-07-11 16:33:27.194872 weewx-5.0.0b8/bin/wee_resources/docs/sle/index.html
--rw-r--r--   0        0        0    38273 2023-07-11 16:33:27.530871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/backing-up-weewx/index.html
--rw-r--r--   0        0        0    35047 2023-07-11 16:33:27.526871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/index.html
--rw-r--r--   0        0        0    41306 2023-07-11 16:33:27.530871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/installing-weewx/index.html
--rw-r--r--   0        0        0    39555 2023-07-11 16:33:27.538871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/mysql-mariadb-config/index.html
--rw-r--r--   0        0        0    38605 2023-07-11 16:33:27.538871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/running-weewx/index.html
--rw-r--r--   0        0        0    38636 2023-07-11 16:33:27.542871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/system-requirements/index.html
--rw-r--r--   0        0        0    41715 2023-07-11 16:33:27.558871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/troubleshooting/hardware/index.html
--rw-r--r--   0        0        0    35174 2023-07-11 16:33:27.554871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/troubleshooting/index.html
--rw-r--r--   0        0        0    42231 2023-07-11 16:33:27.562871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/troubleshooting/meteo/index.html
--rw-r--r--   0        0        0    62769 2023-07-11 16:33:27.570871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/troubleshooting/software/index.html
--rw-r--r--   0        0        0    42047 2023-07-11 16:33:27.546871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/webserver-integration/index.html
--rw-r--r--   0        0        0    39125 2023-07-11 16:33:27.578871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/data-bindings/index.html
--rw-r--r--   0        0        0    38632 2023-07-11 16:33:27.582871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/databases/index.html
--rw-r--r--   0        0        0    42056 2023-07-11 16:33:27.582871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/databasetypes/index.html
--rw-r--r--   0        0        0    42685 2023-07-11 16:33:27.590871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/engine/index.html
--rw-r--r--   0        0        0    39653 2023-07-11 16:33:27.590871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/general/index.html
--rw-r--r--   0        0        0    37931 2023-07-11 16:33:27.574871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/index.html
--rw-r--r--   0        0        0    84345 2023-07-11 16:33:27.602871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/stations-config/index.html
--rw-r--r--   0        0        0    40458 2023-07-11 16:33:27.606871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/stdarchive/index.html
--rw-r--r--   0        0        0    36995 2023-07-11 16:33:27.610871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/stdcalibrate-config/index.html
--rw-r--r--   0        0        0    37580 2023-07-11 16:33:27.614871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/stdconvert-config/index.html
--rw-r--r--   0        0        0    37788 2023-07-11 16:33:27.614871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/stdqc-config/index.html
--rw-r--r--   0        0        0    60403 2023-07-11 16:33:27.622871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/stdreport-config/index.html
--rw-r--r--   0        0        0    70521 2023-07-11 16:33:27.630871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/stdrestful-config/index.html
--rw-r--r--   0        0        0    35969 2023-07-11 16:33:27.634871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/stdtimesynch/index.html
--rw-r--r--   0        0        0    57058 2023-07-11 16:33:27.642871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/stdwxcalculate-config/index.html
--rw-r--r--   0        0        0    42899 2023-07-11 16:33:27.554871 weewx-5.0.0b8/bin/wee_resources/docs/usersguide/where/index.html
--rw-r--r--   0        0        0    57483 2023-07-11 16:33:27.646870 weewx-5.0.0b8/bin/wee_resources/docs/utilities/wee_database/index.html
--rw-r--r--   0        0        0    46261 2023-07-11 16:33:27.650870 weewx-5.0.0b8/bin/wee_resources/docs/utilities/wee_debug/index.html
--rw-r--r--   0        0        0    36546 2023-07-11 16:33:27.654871 weewx-5.0.0b8/bin/wee_resources/docs/utilities/wee_device/index.html
--rw-r--r--   0        0        0   254864 2023-07-11 16:33:27.670870 weewx-5.0.0b8/bin/wee_resources/docs/utilities/wee_import/index.html
--rw-r--r--   0        0        0    38858 2023-07-11 16:33:27.674871 weewx-5.0.0b8/bin/wee_resources/docs/utilities/wee_reports/index.html
--rw-r--r--   0        0        0    55279 2023-07-11 16:33:27.682870 weewx-5.0.0b8/bin/wee_resources/docs/utilities/weectl-database/index.html
--rw-r--r--   0        0        0    45743 2023-07-11 16:33:27.686870 weewx-5.0.0b8/bin/wee_resources/docs/utilities/weectl-extension/index.html
--rw-r--r--   0        0        0    57489 2023-07-11 16:33:27.690870 weewx-5.0.0b8/bin/wee_resources/docs/utilities/weectl-station/index.html
--rw-r--r--   0        0        0    35764 2023-07-11 16:33:27.694870 weewx-5.0.0b8/bin/wee_resources/docs/utilities/weewxd/index.html
--rw-r--r--   0        0        0   150794 2023-07-11 16:33:27.214872 weewx-5.0.0b8/bin/wee_resources/docs/versions/index.html
--rw-r--r--   0        0        0     3097 2023-06-26 17:07:40.352703 weewx-5.0.0b8/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-37.pyc
--rw-r--r--   0        0        0    10729 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/alarm.py
--rw-r--r--   0        0        0      179 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/basic/changelog
--rw-r--r--   0        0        0     1563 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/basic/install.py
--rw-r--r--   0        0        0     1243 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/basic/readme.md
--rw-r--r--   0        0        0     1510 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/examples/basic/skins/basic/basic.css
--rw-r--r--   0        0        0     6451 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/examples/basic/skins/basic/current.inc
--rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/examples/basic/skins/basic/favicon.ico
--rw-r--r--   0        0        0    11292 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/examples/basic/skins/basic/hilo.inc
--rw-r--r--   0        0        0     1665 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/basic/skins/basic/index.html.tmpl
--rw-r--r--   0        0        0     2216 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/examples/basic/skins/basic/lang/en.conf
--rw-r--r--   0        0        0     2408 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/examples/basic/skins/basic/lang/fr.conf
--rw-r--r--   0        0        0     3173 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/examples/basic/skins/basic/skin.conf
--rw-r--r--   0        0        0     2080 2023-07-11 16:37:41.554096 weewx-5.0.0b8/bin/wee_resources/examples/colorize/__pycache__/colorize_1.cpython-37.pyc
--rw-r--r--   0        0        0     2255 2023-07-11 16:37:41.574095 weewx-5.0.0b8/bin/wee_resources/examples/colorize/__pycache__/colorize_2.cpython-37.pyc
--rw-r--r--   0        0        0     3290 2023-07-11 16:37:41.574095 weewx-5.0.0b8/bin/wee_resources/examples/colorize/__pycache__/colorize_3.cpython-37.pyc
--rw-r--r--   0        0        0     2128 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/colorize/colorize_1.py
--rw-r--r--   0        0        0     2617 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/colorize/colorize_2.py
--rw-r--r--   0        0        0     4001 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/colorize/colorize_3.py
--rw-r--r--   0        0        0     4180 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/fileparse/bin/user/fileparse.py
--rw-r--r--   0        0        0      269 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/fileparse/changelog
--rw-r--r--   0        0        0      835 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/fileparse/install.py
--rw-r--r--   0        0        0     2086 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/fileparse/readme.md
--rw-r--r--   0        0        0    10792 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/lowBattery.py
--rw-r--r--   0        0        0     1108 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/examples/mem.py
--rw-r--r--   0        0        0     5986 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/pmon/bin/user/pmon.py
--rw-r--r--   0        0        0      341 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/pmon/changelog
--rw-r--r--   0        0        0     1511 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/pmon/install.py
--rw-r--r--   0        0        0     2628 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/pmon/readme.md
--rw-r--r--   0        0        0      507 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/pmon/skins/pmon/index.html.tmpl
--rw-r--r--   0        0        0     1234 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/examples/pmon/skins/pmon/skin.conf
--rw-r--r--   0        0        0     4334 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/tests/test_vaporpressure.py
--rw-r--r--   0        0        0     4285 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/examples/vaporpressure.py
--rw-r--r--   0        0        0     3034 2023-07-11 16:37:41.586095 weewx-5.0.0b8/bin/wee_resources/examples/xstats/bin/user/__pycache__/xstats.cpython-37.pyc
--rw-r--r--   0        0        0     5662 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/xstats/bin/user/xstats.py
--rw-r--r--   0        0        0      146 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/xstats/changelog
--rw-r--r--   0        0        0      850 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/xstats/install.py
--rw-r--r--   0        0        0     2923 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/xstats/readme.txt
--rw-r--r--   0        0        0     2138 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/xstats/skins/xstats/index.html.tmpl
--rw-r--r--   0        0        0      591 2023-07-11 14:40:18.482441 weewx-5.0.0b8/bin/wee_resources/examples/xstats/skins/xstats/skin.conf
--rw-r--r--   0        0        0      676 2023-07-11 19:25:19.905464 weewx-5.0.0b8/bin/wee_resources/skins/Ftp/skin.conf
--rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/skins/Mobile/favicon.ico
--rw-r--r--   0        0        0     2573 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/skins/Mobile/index.html.tmpl
--rw-r--r--   0        0        0     1021 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/skins/Mobile/lang/de.conf
--rw-r--r--   0        0        0     1000 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/skins/Mobile/lang/en.conf
--rw-r--r--   0        0        0     1101 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/skins/Mobile/lang/nl.conf
--rw-r--r--   0        0        0     2940 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/skins/Mobile/lang/no.conf
--rw-r--r--   0        0        0      671 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/skins/Mobile/mobile.css
--rw-r--r--   0        0        0     5171 2023-07-11 19:25:19.909464 weewx-5.0.0b8/bin/wee_resources/skins/Mobile/skin.conf
--rw-r--r--   0        0        0      760 2023-07-11 19:25:19.913464 weewx-5.0.0b8/bin/wee_resources/skins/Rsync/skin.conf
--rw-r--r--   0        0        0     2667 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y-%m.txt.tmpl
--rw-r--r--   0        0        0     5460 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y.txt.tmpl
--rw-r--r--   0        0        0     1482 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/about.inc
--rw-r--r--   0        0        0      674 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/analytics.inc
--rw-r--r--   0        0        0     1137 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/celestial.html.tmpl
--rw-r--r--   0        0        0     6214 2023-07-11 14:40:18.486441 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/celestial.inc
--rw-r--r--   0        0        0     1291 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/current.inc
--rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/favicon.ico
--rw-r--r--   0        0        0   172876 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/font/Kanit-Bold.ttf
--rw-r--r--   0        0        0   169744 2023-05-30 12:01:49.289499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/font/Kanit-Regular.ttf
--rw-r--r--   0        0        0     4383 2023-07-11 14:40:18.486441 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/font/OFL.txt
--rw-r--r--   0        0        0   224592 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/font/OpenSans-Bold.ttf
--rw-r--r--   0        0        0   217360 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/font/OpenSans-Regular.ttf
--rw-r--r--   0        0        0    20248 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/font/OpenSans.woff
--rw-r--r--   0        0        0    10352 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/font/OpenSans.woff2
--rw-r--r--   0        0        0     4348 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/font/license.txt
--rw-r--r--   0        0        0     4360 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/hilo.inc
--rw-r--r--   0        0        0      858 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/identifier.inc
--rw-r--r--   0        0        0     2787 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/index.html.tmpl
--rw-r--r--   0        0        0     9216 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/cn.conf
--rw-r--r--   0        0        0     9844 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/cz.conf
--rw-r--r--   0        0        0     9745 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/de.conf
--rw-r--r--   0        0        0     9459 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/en.conf
--rw-r--r--   0        0        0    10702 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/es.conf
--rw-r--r--   0        0        0    10673 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/fr.conf
--rw-r--r--   0        0        0    11838 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/gr.conf
--rw-r--r--   0        0        0     9947 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/it.conf
--rw-r--r--   0        0        0     9548 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/nl.conf
--rw-r--r--   0        0        0    10705 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/no.conf
--rw-r--r--   0        0        0    15356 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/th.conf
--rw-r--r--   0        0        0      920 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/map.inc
--rw-r--r--   0        0        0      572 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/radar.inc
--rw-r--r--   0        0        0     4373 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/rss.xml.tmpl
--rw-r--r--   0        0        0      642 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/satellite.inc
--rw-r--r--   0        0        0     5406 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/seasons.css
--rw-r--r--   0        0        0     6404 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/seasons.js
--rw-r--r--   0        0        0     3947 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/sensors.inc
--rw-r--r--   0        0        0    27402 2023-07-11 19:25:19.917464 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/skin.conf
--rw-r--r--   0        0        0     1294 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/statistics.html.tmpl
--rw-r--r--   0        0        0     3971 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/statistics.inc
--rw-r--r--   0        0        0     2771 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/sunmoon.inc
--rw-r--r--   0        0        0      987 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/tabular.html.tmpl
--rw-r--r--   0        0        0     2450 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/telemetry.html.tmpl
--rw-r--r--   0        0        0     1115 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Seasons/titlebar.inc
--rw-r--r--   0        0        0     1804 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/barometer.html.tmpl
--rw-r--r--   0        0        0      143 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/custom.js
--rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/favicon.ico
--rw-r--r--   0        0        0     1043 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/humidity.html.tmpl
--rw-r--r--   0        0        0     4846 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x1.png
--rw-r--r--   0        0        0     7142 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x2.png
--rw-r--r--   0        0        0     4421 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x1.png
--rw-r--r--   0        0        0     6095 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x2.png
--rw-r--r--   0        0        0     2457 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/index.html.tmpl
--rw-r--r--   0        0        0     1639 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/lang/de.conf
--rw-r--r--   0        0        0     1554 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/lang/en.conf
--rw-r--r--   0        0        0     1594 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/lang/nl.conf
--rw-r--r--   0        0        0     3530 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/lang/no.conf
--rw-r--r--   0        0        0     1502 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/rain.html.tmpl
--rw-r--r--   0        0        0     7806 2023-07-11 19:25:19.921464 weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/skin.conf
--rw-r--r--   0        0        0     1588 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/temp.html.tmpl
--rw-r--r--   0        0        0     1681 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/wind.html.tmpl
--rw-r--r--   0        0        0     2591 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y-%m.txt.tmpl
--rw-r--r--   0        0        0     5364 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y.txt.tmpl
--rw-r--r--   0        0        0     8546 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/RSS/weewx_rss.xml.tmpl
--rw-r--r--   0        0        0       76 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/backgrounds/band.gif
--rw-r--r--   0        0        0     2593 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/backgrounds/butterfly.jpg
--rw-r--r--   0        0        0     1508 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/backgrounds/drops.gif
--rw-r--r--   0        0        0     1386 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/backgrounds/flower.jpg
--rw-r--r--   0        0        0     2277 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/backgrounds/leaf.jpg
--rw-r--r--   0        0        0     8609 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/backgrounds/night.gif
--rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.293499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/favicon.ico
--rw-r--r--   0        0        0   313856 2023-07-11 14:40:18.486441 weewx-5.0.0b8/bin/wee_resources/skins/Standard/font/DejaVuSansMono-Bold.ttf
--rw-r--r--   0        0        0    20739 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/index.html.tmpl
--rw-r--r--   0        0        0     9390 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/lang/de.conf
--rw-r--r--   0        0        0     9264 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/lang/en.conf
--rw-r--r--   0        0        0     9765 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/lang/fr.conf
--rw-r--r--   0        0        0     9356 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/lang/nl.conf
--rw-r--r--   0        0        0    10875 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/lang/no.conf
--rw-r--r--   0        0        0    15140 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/month.html.tmpl
--rw-r--r--   0        0        0    16429 2023-07-11 19:25:19.921464 weewx-5.0.0b8/bin/wee_resources/skins/Standard/skin.conf
--rw-r--r--   0        0        0     1456 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/barometer.html.tmpl
--rw-r--r--   0        0        0      143 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/custom.js
--rw-r--r--   0        0        0     1012 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/humidity.html.tmpl
--rw-r--r--   0        0        0     4846 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x1.png
--rw-r--r--   0        0        0     7142 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x2.png
--rw-r--r--   0        0        0     4421 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x1.png
--rw-r--r--   0        0        0     6095 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x2.png
--rw-r--r--   0        0        0     1918 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/index.html.tmpl
--rw-r--r--   0        0        0     1000 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/radar.html.tmpl
--rw-r--r--   0        0        0     1394 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/rain.html.tmpl
--rw-r--r--   0        0        0     1441 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/temp_outside.html.tmpl
--rw-r--r--   0        0        0     1508 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/wind.html.tmpl
--rw-r--r--   0        0        0    15057 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/week.html.tmpl
--rw-r--r--   0        0        0     3533 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/weewx.css
--rw-r--r--   0        0        0     9990 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/skins/Standard/year.html.tmpl
--rw-r--r--   0        0        0      154 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/apache/conf-available/weewx.conf
--rw-r--r--   0        0        0      167 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/apache/conf.d/weewx.conf
--rw-r--r--   0        0        0      136 2023-07-11 14:40:18.486441 weewx-5.0.0b8/bin/wee_resources/util/default/weewx
--rwxr-xr-x   0        0        0     8897 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/i18n/i18n-report
--rw-r--r--   0        0        0     9052 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/import/csv-example.conf
--rw-r--r--   0        0        0     8250 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/import/cumulus-example.conf
--rw-r--r--   0        0        0    14923 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/import/wd-example.conf
--rw-r--r--   0        0        0     7100 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/import/weathercat-example.conf
--rw-r--r--   0        0        0     6202 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/import/wu-example.conf
--rwxr-xr-x   0        0        0     6057 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/init.d/weewx-multi
--rwxr-xr-x   0        0        0      862 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/init.d/weewx.bsd
--rwxr-xr-x   0        0        0     5111 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/init.d/weewx.debian
--rw-r--r--   0        0        0      647 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/init.d/weewx.freebsd
--rwxr-xr-x   0        0        0     8372 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/init.d/weewx.lsb
--rwxr-xr-x   0        0        0     1659 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/init.d/weewx.redhat
--rwxr-xr-x   0        0        0     4856 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/init.d/weewx.suse
--rw-r--r--   0        0        0      914 2023-07-11 14:40:18.490441 weewx-5.0.0b8/bin/wee_resources/util/launchd/com.weewx.weewxd.plist
--rw-r--r--   0        0        0     1800 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/logrotate.d/weewx
--rw-r--r--   0        0        0       83 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/logwatch/conf/logfiles/weewx.conf
--rw-r--r--   0        0        0       32 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/logwatch/conf/services/weewx.conf
--rwxr-xr-x   0        0        0    54942 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/logwatch/scripts/services/weewx
--rw-r--r--   0        0        0       82 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/newsyslog.d/weewx.conf
--rw-r--r--   0        0        0     2219 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/rsyslog.d/weewx.conf
--rwxr-xr-x   0        0        0      319 2023-07-11 14:40:18.490441 weewx-5.0.0b8/bin/wee_resources/util/scripts/wee_database
--rwxr-xr-x   0        0        0      316 2023-07-11 14:40:18.490441 weewx-5.0.0b8/bin/wee_resources/util/scripts/wee_debug
--rwxr-xr-x   0        0        0      317 2023-07-11 14:40:18.490441 weewx-5.0.0b8/bin/wee_resources/util/scripts/wee_device
--rwxr-xr-x   0        0        0      317 2023-07-11 14:40:18.490441 weewx-5.0.0b8/bin/wee_resources/util/scripts/wee_import
--rwxr-xr-x   0        0        0      318 2023-07-11 14:40:18.490441 weewx-5.0.0b8/bin/wee_resources/util/scripts/wee_reports
--rwxr-xr-x   0        0        0      313 2023-07-11 14:40:18.490441 weewx-5.0.0b8/bin/wee_resources/util/scripts/weectl
--rwxr-xr-x   0        0        0      313 2023-07-11 14:40:18.490441 weewx-5.0.0b8/bin/wee_resources/util/scripts/weewxd
--rw-r--r--   0        0        0     2564 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/solaris/weewx-smf.xml
--rw-r--r--   0        0        0      526 2023-07-11 14:40:18.490441 weewx-5.0.0b8/bin/wee_resources/util/systemd/weewx.service
--rw-r--r--   0        0        0       34 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/tmpfiles.d/weewx.conf
--rw-r--r--   0        0        0      149 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/udev/rules.d/acurite.rules
--rw-r--r--   0        0        0      135 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/udev/rules.d/cc3000.rules
--rw-r--r--   0        0        0      153 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/udev/rules.d/fousb.rules
--rw-r--r--   0        0        0      147 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/udev/rules.d/te923.rules
--rw-r--r--   0        0        0      624 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/udev/rules.d/vantage.rules
--rw-r--r--   0        0        0     1560 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/udev/rules.d/weewx.rules
--rw-r--r--   0        0        0      158 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/udev/rules.d/wmr100.rules
--rw-r--r--   0        0        0      158 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/udev/rules.d/wmr300.rules
--rw-r--r--   0        0        0      152 2023-05-30 12:01:49.297499 weewx-5.0.0b8/bin/wee_resources/util/udev/rules.d/ws28xx.rules
--rw-r--r--   0        0        0    18375 2023-07-11 19:25:19.905464 weewx-5.0.0b8/bin/wee_resources/weewx.conf
--rw-r--r--   0        0        0    25898 2023-07-11 14:40:18.430439 weewx-5.0.0b8/bin/weecfg/__init__.py
--rw-r--r--   0        0        0    26461 2023-07-11 14:40:18.430439 weewx-5.0.0b8/bin/weecfg/database.py
--rw-r--r--   0        0        0    24020 2023-07-11 14:40:18.430439 weewx-5.0.0b8/bin/weecfg/extension.py
--rw-r--r--   0        0        0    33889 2023-07-11 19:17:56.536474 weewx-5.0.0b8/bin/weecfg/station_config.py
--rw-r--r--   0        0        0    45364 2023-07-11 14:40:18.430439 weewx-5.0.0b8/bin/weecfg/update_config.py
--rwxr-xr-x   0        0        0     1473 2023-07-11 14:40:18.430439 weewx-5.0.0b8/bin/weectl.py
--rw-r--r--   0        0        0     2475 2023-07-11 14:40:18.430439 weewx-5.0.0b8/bin/weectllib/__init__.py
--rw-r--r--   0        0        0    20988 2023-07-11 14:40:18.430439 weewx-5.0.0b8/bin/weectllib/database_cmd.py
--rw-r--r--   0        0        0    29103 2023-07-11 14:40:18.430439 weewx-5.0.0b8/bin/weectllib/db_actions.py
--rw-r--r--   0        0        0     6856 2023-07-11 14:40:18.430439 weewx-5.0.0b8/bin/weectllib/extension_cmd.py
--rw-r--r--   0        0        0    16486 2023-07-11 14:40:18.430439 weewx-5.0.0b8/bin/weectllib/station_cmd.py
--rw-r--r--   0        0        0     4538 2023-05-30 12:01:49.269499 weewx-5.0.0b8/bin/weedb/NOTES.md
--rw-r--r--   0        0        0     6717 2023-07-11 14:40:18.430439 weewx-5.0.0b8/bin/weedb/__init__.py
--rw-r--r--   0        0        0    11213 2023-07-11 14:40:18.434439 weewx-5.0.0b8/bin/weedb/mysql.py
--rw-r--r--   0        0        0    11161 2023-07-11 14:40:18.434439 weewx-5.0.0b8/bin/weedb/sqlite.py
--rw-r--r--   0        0        0      255 2023-05-30 12:01:49.269499 weewx-5.0.0b8/bin/weeimport/__init__.py
--rw-r--r--   0        0        0    11110 2023-05-30 12:01:49.269499 weewx-5.0.0b8/bin/weeimport/csvimport.py
--rw-r--r--   0        0        0    20265 2023-05-30 12:01:49.269499 weewx-5.0.0b8/bin/weeimport/cumulusimport.py
--rw-r--r--   0        0        0    35701 2023-05-30 12:01:49.269499 weewx-5.0.0b8/bin/weeimport/wdimport.py
--rw-r--r--   0        0        0    18225 2023-07-11 14:40:18.434439 weewx-5.0.0b8/bin/weeimport/weathercatimport.py
--rw-r--r--   0        0        0    69526 2023-07-11 14:40:18.434439 weewx-5.0.0b8/bin/weeimport/weeimport.py
--rw-r--r--   0        0        0    17222 2023-07-11 14:40:18.434439 weewx-5.0.0b8/bin/weeimport/wuimport.py
--rw-r--r--   0        0        0      367 2023-05-30 12:01:49.273499 weewx-5.0.0b8/bin/weeplot/__init__.py
--rw-r--r--   0        0        0    33267 2023-07-11 14:40:18.434439 weewx-5.0.0b8/bin/weeplot/genplot.py
--rw-r--r--   0        0        0    25533 2023-07-11 14:40:18.434439 weewx-5.0.0b8/bin/weeplot/utilities.py
--rw-r--r--   0        0        0     1633 2023-05-30 12:01:49.273499 weewx-5.0.0b8/bin/weeutil/Moon.py
--rw-r--r--   0        0        0    18296 2023-05-30 12:01:49.273499 weewx-5.0.0b8/bin/weeutil/Sun.py
--rw-r--r--   0        0        0      142 2023-05-30 12:01:49.273499 weewx-5.0.0b8/bin/weeutil/__init__.py
--rw-r--r--   0        0        0     9408 2023-07-11 14:40:18.434439 weewx-5.0.0b8/bin/weeutil/config.py
--rw-r--r--   0        0        0    12986 2023-07-11 14:40:18.434439 weewx-5.0.0b8/bin/weeutil/ftpupload.py
--rw-r--r--   0        0        0     3150 2023-07-11 14:40:18.438439 weewx-5.0.0b8/bin/weeutil/log.py
--rw-r--r--   0        0        0     5896 2023-07-11 14:40:18.438439 weewx-5.0.0b8/bin/weeutil/logger.py
--rw-r--r--   0        0        0     6593 2023-05-30 12:01:49.273499 weewx-5.0.0b8/bin/weeutil/rsyncupload.py
--rw-r--r--   0        0        0     2224 2023-05-30 12:01:49.273499 weewx-5.0.0b8/bin/weeutil/timediff.py
--rw-r--r--   0        0        0    65551 2023-07-11 14:40:18.438439 weewx-5.0.0b8/bin/weeutil/weeutil.py
--rw-r--r--   0        0        0     5929 2023-07-11 19:25:19.925464 weewx-5.0.0b8/bin/weewx/__init__.py
--rw-r--r--   0        0        0    26063 2023-07-11 14:40:18.442440 weewx-5.0.0b8/bin/weewx/accum.py
--rw-r--r--   0        0        0    25229 2023-07-11 14:40:18.442440 weewx-5.0.0b8/bin/weewx/almanac.py
--rw-r--r--   0        0        0    33390 2023-07-11 14:40:18.442440 weewx-5.0.0b8/bin/weewx/cheetahgenerator.py
--rw-r--r--   0        0        0     3393 2023-05-30 12:01:49.273499 weewx-5.0.0b8/bin/weewx/crc16.py
--rw-r--r--   0        0        0     2888 2023-07-11 14:40:18.442440 weewx-5.0.0b8/bin/weewx/daemon.py
--rw-r--r--   0        0        0    11955 2023-07-11 14:40:18.442440 weewx-5.0.0b8/bin/weewx/defaults.py
--rw-r--r--   0        0        0     5148 2023-07-11 14:40:18.442440 weewx-5.0.0b8/bin/weewx/drivers/__init__.py
--rw-r--r--   0        0        0    38987 2023-05-30 12:01:49.273499 weewx-5.0.0b8/bin/weewx/drivers/acurite.py
--rw-r--r--   0        0        0    64005 2023-07-11 14:40:18.442440 weewx-5.0.0b8/bin/weewx/drivers/cc3000.py
--rw-r--r--   0        0        0    78592 2023-07-11 14:40:18.442440 weewx-5.0.0b8/bin/weewx/drivers/fousb.py
--rw-r--r--   0        0        0    14931 2023-05-30 12:01:49.273499 weewx-5.0.0b8/bin/weewx/drivers/simulator.py
--rw-r--r--   0        0        0    99881 2023-05-30 12:01:49.273499 weewx-5.0.0b8/bin/weewx/drivers/te923.py
--rw-r--r--   0        0        0    15797 2023-05-30 12:01:49.273499 weewx-5.0.0b8/bin/weewx/drivers/ultimeter.py
--rw-r--r--   0        0        0   139883 2023-07-11 14:40:18.446440 weewx-5.0.0b8/bin/weewx/drivers/vantage.py
--rw-r--r--   0        0        0    17795 2023-05-30 12:01:49.273499 weewx-5.0.0b8/bin/weewx/drivers/wmr100.py
--rw-r--r--   0        0        0    72747 2023-05-30 12:01:49.273499 weewx-5.0.0b8/bin/weewx/drivers/wmr300.py
--rw-r--r--   0        0        0    29536 2023-07-11 14:40:18.446440 weewx-5.0.0b8/bin/weewx/drivers/wmr9x8.py
--rw-r--r--   0        0        0    18843 2023-07-11 14:40:18.446440 weewx-5.0.0b8/bin/weewx/drivers/ws1.py
--rw-r--r--   0        0        0    79489 2023-07-11 14:40:18.450440 weewx-5.0.0b8/bin/weewx/drivers/ws23xx.py
--rw-r--r--   0        0        0   173578 2023-05-30 12:01:49.277499 weewx-5.0.0b8/bin/weewx/drivers/ws28xx.py
--rw-r--r--   0        0        0    37475 2023-07-11 14:40:18.450440 weewx-5.0.0b8/bin/weewx/engine.py
--rw-r--r--   0        0        0      276 2023-05-30 12:01:49.277499 weewx-5.0.0b8/bin/weewx/filegenerator.py
--rw-r--r--   0        0        0    18278 2023-07-11 14:40:18.450440 weewx-5.0.0b8/bin/weewx/imagegenerator.py
--rw-r--r--   0        0        0    73115 2023-07-11 14:40:18.458440 weewx-5.0.0b8/bin/weewx/manager.py
--rw-r--r--   0        0        0     3187 2023-05-30 12:01:49.277499 weewx-5.0.0b8/bin/weewx/qc.py
--rw-r--r--   0        0        0    37780 2023-07-11 14:40:18.458440 weewx-5.0.0b8/bin/weewx/reportengine.py
--rw-r--r--   0        0        0    79730 2023-07-11 14:40:18.462440 weewx-5.0.0b8/bin/weewx/restx.py
--rw-r--r--   0        0        0     7207 2023-05-30 12:01:49.277499 weewx-5.0.0b8/bin/weewx/station.py
--rw-r--r--   0        0        0    31917 2023-07-11 14:49:15.562347 weewx-5.0.0b8/bin/weewx/tags.py
--rw-r--r--   0        0        0    71594 2023-07-11 14:40:18.466440 weewx-5.0.0b8/bin/weewx/units.py
--rw-r--r--   0        0        0    25248 2023-05-30 12:01:49.281499 weewx-5.0.0b8/bin/weewx/uwxutils.py
--rw-r--r--   0        0        0      246 2023-05-30 12:01:49.281499 weewx-5.0.0b8/bin/weewx/wxengine.py
--rw-r--r--   0        0        0    30034 2023-05-30 12:01:49.281499 weewx-5.0.0b8/bin/weewx/wxformulas.py
--rw-r--r--   0        0        0      367 2023-05-30 12:01:49.281499 weewx-5.0.0b8/bin/weewx/wxmanager.py
--rw-r--r--   0        0        0     7270 2023-05-30 12:01:49.281499 weewx-5.0.0b8/bin/weewx/wxservices.py
--rw-r--r--   0        0        0    34353 2023-07-11 14:40:18.466440 weewx-5.0.0b8/bin/weewx/wxxtypes.py
--rw-r--r--   0        0        0    55988 2023-07-11 14:40:18.470440 weewx-5.0.0b8/bin/weewx/xtypes.py
--rwxr-xr-x   0        0        0     9648 2023-07-11 14:40:18.470440 weewx-5.0.0b8/bin/weewxd.py
--rw-r--r--   0        0        0    12175 2023-07-11 14:40:18.482441 weewx-5.0.0b8/pkg/changelog.el
--rw-r--r--   0        0        0    12070 2023-07-11 14:40:18.482441 weewx-5.0.0b8/pkg/changelog.suse
--rw-r--r--   0        0        0     2731 2023-05-30 12:01:49.289499 weewx-5.0.0b8/pkg/debian/README
--rw-r--r--   0        0        0    21471 2023-07-11 14:40:18.482441 weewx-5.0.0b8/pkg/debian/changelog
--rw-r--r--   0        0        0        3 2023-07-11 14:40:18.482441 weewx-5.0.0b8/pkg/debian/compat
--rw-r--r--   0        0        0       36 2023-05-30 12:01:49.289499 weewx-5.0.0b8/pkg/debian/conffiles
--rwxr-xr-x   0        0        0     3398 2023-07-11 14:40:18.482441 weewx-5.0.0b8/pkg/debian/config
--rw-r--r--   0        0        0      724 2023-07-11 14:40:18.482441 weewx-5.0.0b8/pkg/debian/control
--rw-r--r--   0        0        0      926 2023-07-11 14:40:18.482441 weewx-5.0.0b8/pkg/debian/copyright
--rwxr-xr-x   0        0        0     8937 2023-07-11 14:40:18.482441 weewx-5.0.0b8/pkg/debian/postinst
--rwxr-xr-x   0        0        0      906 2023-05-30 12:01:49.289499 weewx-5.0.0b8/pkg/debian/postrm
--rwxr-xr-x   0        0        0      410 2023-05-30 12:01:49.289499 weewx-5.0.0b8/pkg/debian/preinst
--rwxr-xr-x   0        0        0      693 2023-07-11 14:40:18.486441 weewx-5.0.0b8/pkg/debian/prerm
--rwxr-xr-x   0        0        0     2985 2023-07-11 14:40:18.486441 weewx-5.0.0b8/pkg/debian/rules
--rw-r--r--   0        0        0       12 2023-05-30 12:01:49.289499 weewx-5.0.0b8/pkg/debian/source/format
--rw-r--r--   0        0        0     5501 2023-07-11 14:40:18.486441 weewx-5.0.0b8/pkg/debian/templates
--rw-r--r--   0        0        0     1708 2023-07-11 14:40:18.486441 weewx-5.0.0b8/pkg/index-apt.html
--rw-r--r--   0        0        0     1728 2023-05-30 12:01:49.289499 weewx-5.0.0b8/pkg/index-suse.html
--rw-r--r--   0        0        0     1714 2023-05-30 12:01:49.289499 weewx-5.0.0b8/pkg/index-yum.html
--rwxr-xr-x   0        0        0     9874 2023-05-30 12:01:49.289499 weewx-5.0.0b8/pkg/mkchangelog.pl
--rw-r--r--   0        0        0       79 2023-05-30 12:01:49.289499 weewx-5.0.0b8/pkg/weewx-el8.repo
--rw-r--r--   0        0        0       57 2023-05-30 12:01:49.289499 weewx-5.0.0b8/pkg/weewx-python2.list
--rw-r--r--   0        0        0       56 2023-05-30 12:01:49.289499 weewx-5.0.0b8/pkg/weewx-python3.list
--rw-r--r--   0        0        0       83 2023-05-30 12:01:49.289499 weewx-5.0.0b8/pkg/weewx-suse12.repo
--rw-r--r--   0        0        0       83 2023-05-30 12:01:49.289499 weewx-5.0.0b8/pkg/weewx-suse15.repo
--rw-r--r--   0        0        0     2201 2023-05-30 12:01:49.289499 weewx-5.0.0b8/pkg/weewx.smf
--rw-r--r--   0        0        0     7144 2023-07-11 14:40:18.486441 weewx-5.0.0b8/pkg/weewx.spec.in
--rw-r--r--   0        0        0     2829 2023-07-11 19:25:14.745497 weewx-5.0.0b8/pyproject.toml
--rw-r--r--   0        0        0      154 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/apache/conf-available/weewx.conf
--rw-r--r--   0        0        0      167 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/apache/conf.d/weewx.conf
--rw-r--r--   0        0        0      136 2023-07-11 14:40:18.486441 weewx-5.0.0b8/util/default/weewx
--rwxr-xr-x   0        0        0     8897 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/i18n/i18n-report
--rw-r--r--   0        0        0     9052 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/import/csv-example.conf
--rw-r--r--   0        0        0     8250 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/import/cumulus-example.conf
--rw-r--r--   0        0        0    14923 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/import/wd-example.conf
--rw-r--r--   0        0        0     7100 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/import/weathercat-example.conf
--rw-r--r--   0        0        0     6202 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/import/wu-example.conf
--rwxr-xr-x   0        0        0     6057 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/init.d/weewx-multi
--rwxr-xr-x   0        0        0      862 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/init.d/weewx.bsd
--rwxr-xr-x   0        0        0     5111 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/init.d/weewx.debian
--rw-r--r--   0        0        0      647 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/init.d/weewx.freebsd
--rwxr-xr-x   0        0        0     8372 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/init.d/weewx.lsb
--rwxr-xr-x   0        0        0     1659 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/init.d/weewx.redhat
--rwxr-xr-x   0        0        0     4856 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/init.d/weewx.suse
--rw-r--r--   0        0        0      914 2023-07-11 14:40:18.490441 weewx-5.0.0b8/util/launchd/com.weewx.weewxd.plist
--rw-r--r--   0        0        0     1800 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/logrotate.d/weewx
--rw-r--r--   0        0        0       83 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/logwatch/conf/logfiles/weewx.conf
--rw-r--r--   0        0        0       32 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/logwatch/conf/services/weewx.conf
--rwxr-xr-x   0        0        0    54942 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/logwatch/scripts/services/weewx
--rw-r--r--   0        0        0       82 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/newsyslog.d/weewx.conf
--rw-r--r--   0        0        0     2219 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/rsyslog.d/weewx.conf
--rwxr-xr-x   0        0        0      319 2023-07-11 14:40:18.490441 weewx-5.0.0b8/util/scripts/wee_database
--rwxr-xr-x   0        0        0      316 2023-07-11 14:40:18.490441 weewx-5.0.0b8/util/scripts/wee_debug
--rwxr-xr-x   0        0        0      317 2023-07-11 14:40:18.490441 weewx-5.0.0b8/util/scripts/wee_device
--rwxr-xr-x   0        0        0      317 2023-07-11 14:40:18.490441 weewx-5.0.0b8/util/scripts/wee_import
--rwxr-xr-x   0        0        0      318 2023-07-11 14:40:18.490441 weewx-5.0.0b8/util/scripts/wee_reports
--rwxr-xr-x   0        0        0      313 2023-07-11 14:40:18.490441 weewx-5.0.0b8/util/scripts/weectl
--rwxr-xr-x   0        0        0      313 2023-07-11 14:40:18.490441 weewx-5.0.0b8/util/scripts/weewxd
--rw-r--r--   0        0        0     2564 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/solaris/weewx-smf.xml
--rw-r--r--   0        0        0      526 2023-07-11 14:40:18.490441 weewx-5.0.0b8/util/systemd/weewx.service
--rw-r--r--   0        0        0       34 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/tmpfiles.d/weewx.conf
--rw-r--r--   0        0        0      149 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/udev/rules.d/acurite.rules
--rw-r--r--   0        0        0      135 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/udev/rules.d/cc3000.rules
--rw-r--r--   0        0        0      153 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/udev/rules.d/fousb.rules
--rw-r--r--   0        0        0      147 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/udev/rules.d/te923.rules
--rw-r--r--   0        0        0      624 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/udev/rules.d/vantage.rules
--rw-r--r--   0        0        0     1560 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/udev/rules.d/weewx.rules
--rw-r--r--   0        0        0      158 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/udev/rules.d/wmr100.rules
--rw-r--r--   0        0        0      158 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/udev/rules.d/wmr300.rules
--rw-r--r--   0        0        0      152 2023-05-30 12:01:49.297499 weewx-5.0.0b8/util/udev/rules.d/ws28xx.rules
--rw-r--r--   0        0        0     5491 1970-01-01 00:00:00.000000 weewx-5.0.0b8/PKG-INFO
+-rw-r--r--   0        0        0    32472 2023-05-30 12:01:49.265499 weewx-5.0.0b9/LICENSE.txt
+-rw-r--r--   0        0        0     3725 2023-07-11 14:40:18.430439 weewx-5.0.0b9/README.md
+-rw-r--r--   0        0        0      230 2023-05-30 12:01:49.265499 weewx-5.0.0b9/bin/schemas/__init__.py
+-rw-r--r--   0        0        0     3448 2023-05-30 12:01:49.269499 weewx-5.0.0b9/bin/schemas/wview.py
+-rw-r--r--   0        0        0     5953 2023-05-30 12:01:49.269499 weewx-5.0.0b9/bin/schemas/wview_extended.py
+-rw-r--r--   0        0        0     2105 2023-05-30 12:01:49.269499 weewx-5.0.0b9/bin/schemas/wview_small.py
+-rwxr-xr-x   0        0        0    52292 2023-07-11 14:40:18.430439 weewx-5.0.0b9/bin/wee_database.py
+-rwxr-xr-x   0        0        0    16172 2023-07-11 14:40:18.430439 weewx-5.0.0b9/bin/wee_debug.py
+-rwxr-xr-x   0        0        0     2187 2023-07-11 14:40:18.430439 weewx-5.0.0b9/bin/wee_device.py
+-rwxr-xr-x   0        0        0    38911 2023-07-11 14:40:18.430439 weewx-5.0.0b9/bin/wee_import.py
+-rwxr-xr-x   0        0        0     5630 2023-07-11 14:40:18.430439 weewx-5.0.0b9/bin/wee_reports.py
+-rw-r--r--   0        0        0        0 2023-07-14 13:27:06.598670 weewx-5.0.0b9/bin/wee_resources/__init__.py
+-rw-r--r--   0        0        0      306 2023-05-30 12:01:49.269499 weewx-5.0.0b9/bin/wee_resources/bin/user/__init__.py
+-rw-r--r--   0        0        0      324 2023-07-12 13:58:45.913592 weewx-5.0.0b9/bin/wee_resources/bin/user/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      398 2023-07-12 13:58:45.913592 weewx-5.0.0b9/bin/wee_resources/bin/user/__pycache__/extensions.cpython-37.pyc
+-rw-r--r--   0        0        0      541 2023-05-30 12:01:49.269499 weewx-5.0.0b9/bin/wee_resources/bin/user/extensions.py
+-rw-r--r--   0        0        0    33399 2023-07-14 13:24:24.909767 weewx-5.0.0b9/bin/wee_resources/docs/404.html
+-rw-r--r--   0        0        0     1870 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0   113489 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/bundle.b4d07000.min.js
+-rw-r--r--   0        0        0   954781 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/bundle.b4d07000.min.js.map
+-rw-r--r--   0        0        0    17074 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0        0        0     4654 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0        0        0     6119 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0        0        0     6208 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0        0        0    11499 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0        0        0     9342 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0        0        0    10669 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0        0        0     3383 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0        0        0     9437 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0        0        0     1264 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hy.min.js
+-rw-r--r--   0        0        0    11232 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0        0        0     2313 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0        0        0       36 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0        0        0     3494 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.kn.min.js
+-rw-r--r--   0        0        0     7972 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0        0        0      817 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0        0        0     6026 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0        0        0     4754 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0        0        0    10171 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0        0        0    10958 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0        0        0    10331 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0        0        0     4901 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sa.min.js
+-rw-r--r--   0        0        0     3647 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0        0        0     4523 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0        0        0     2406 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0        0        0     2330 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.te.min.js
+-rw-r--r--   0        0        0     1031 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0        0        0    15009 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0        0        0      784 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0        0        0     2158 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0        0        0    22878 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0        0        0   677463 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/wordcut.js
+-rw-r--r--   0        0        0    38916 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/workers/search.208ed371.min.js
+-rw-r--r--   0        0        0   209901 2023-07-14 13:24:24.817766 weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/workers/search.208ed371.min.js.map
+-rw-r--r--   0        0        0   113455 2023-07-14 13:24:24.817766 weewx-5.0.0b9/bin/wee_resources/docs/assets/stylesheets/main.85bb2934.min.css
+-rw-r--r--   0        0        0    38958 2023-07-14 13:24:24.817766 weewx-5.0.0b9/bin/wee_resources/docs/assets/stylesheets/main.85bb2934.min.css.map
+-rw-r--r--   0        0        0    12227 2023-07-14 13:24:24.817766 weewx-5.0.0b9/bin/wee_resources/docs/assets/stylesheets/palette.a6bdf11c.min.css
+-rw-r--r--   0        0        0     3628 2023-07-14 13:24:24.817766 weewx-5.0.0b9/bin/wee_resources/docs/assets/stylesheets/palette.a6bdf11c.min.css.map
+-rw-r--r--   0        0        0   195652 2023-07-14 13:24:24.953767 weewx-5.0.0b9/bin/wee_resources/docs/changes/index.html
+-rw-r--r--   0        0        0    36103 2023-07-14 13:24:24.957767 weewx-5.0.0b9/bin/wee_resources/docs/copyright/index.html
+-rw-r--r--   0        0        0      565 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/css/tocbot-4.12.0.css
+-rw-r--r--   0        0        0      565 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/css/tocbot-4.3.1.css
+-rw-r--r--   0        0        0    12148 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/css/weewx_ui.css
+-rw-r--r--   0        0        0    63176 2023-07-14 13:24:25.037768 weewx-5.0.0b9/bin/wee_resources/docs/custom/appendix/index.html
+-rw-r--r--   0        0        0   142794 2023-07-14 13:24:25.073768 weewx-5.0.0b9/bin/wee_resources/docs/custom/cheetah/index.html
+-rw-r--r--   0        0        0    72909 2023-07-14 13:24:25.089768 weewx-5.0.0b9/bin/wee_resources/docs/custom/custom-reports/index.html
+-rw-r--r--   0        0        0    60588 2023-07-14 13:24:25.097768 weewx-5.0.0b9/bin/wee_resources/docs/custom/database/index.html
+-rw-r--r--   0        0        0    35129 2023-07-14 13:24:25.097768 weewx-5.0.0b9/bin/wee_resources/docs/custom/derived/index.html
+-rw-r--r--   0        0        0    49424 2023-07-14 13:24:25.101768 weewx-5.0.0b9/bin/wee_resources/docs/custom/drivers/index.html
+-rw-r--r--   0        0        0    40791 2023-07-14 13:24:25.105769 weewx-5.0.0b9/bin/wee_resources/docs/custom/extensions/index.html
+-rw-r--r--   0        0        0    62049 2023-07-14 13:24:25.117769 weewx-5.0.0b9/bin/wee_resources/docs/custom/image-generator/index.html
+-rw-r--r--   0        0        0    71330 2023-07-14 13:24:25.021768 weewx-5.0.0b9/bin/wee_resources/docs/custom/index.html
+-rw-r--r--   0        0        0    65342 2023-07-14 13:24:25.129769 weewx-5.0.0b9/bin/wee_resources/docs/custom/localization/index.html
+-rw-r--r--   0        0        0    48294 2023-07-14 13:24:25.137769 weewx-5.0.0b9/bin/wee_resources/docs/custom/multiple-bindings/index.html
+-rw-r--r--   0        0        0   120067 2023-07-14 13:24:25.157769 weewx-5.0.0b9/bin/wee_resources/docs/custom/report-options/index.html
+-rw-r--r--   0        0        0    51431 2023-07-14 13:24:25.165769 weewx-5.0.0b9/bin/wee_resources/docs/custom/report-scheduling/index.html
+-rw-r--r--   0        0        0    83864 2023-07-14 13:24:25.189769 weewx-5.0.0b9/bin/wee_resources/docs/custom/service-engine/index.html
+-rw-r--r--   0        0        0    46163 2023-07-14 13:24:25.193769 weewx-5.0.0b9/bin/wee_resources/docs/custom/units/index.html
+-rw-r--r--   0        0        0    71514 2023-07-14 13:24:24.965767 weewx-5.0.0b9/bin/wee_resources/docs/devnotes/index.html
+-rw-r--r--   0        0        0     2747 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/examples/tag.htm
+-rw-r--r--   0        0        0    41207 2023-07-14 13:24:25.201769 weewx-5.0.0b9/bin/wee_resources/docs/hardware/acurite/index.html
+-rw-r--r--   0        0        0    62276 2023-07-14 13:24:25.209769 weewx-5.0.0b9/bin/wee_resources/docs/hardware/cc3000/index.html
+-rw-r--r--   0        0        0    56883 2023-07-14 13:24:25.225769 weewx-5.0.0b9/bin/wee_resources/docs/hardware/drivers/index.html
+-rw-r--r--   0        0        0    48895 2023-07-14 13:24:25.229769 weewx-5.0.0b9/bin/wee_resources/docs/hardware/fousb/index.html
+-rw-r--r--   0        0        0    47564 2023-07-14 13:24:25.237769 weewx-5.0.0b9/bin/wee_resources/docs/hardware/te923/index.html
+-rw-r--r--   0        0        0    39191 2023-07-14 13:24:25.241770 weewx-5.0.0b9/bin/wee_resources/docs/hardware/ultimeter/index.html
+-rw-r--r--   0        0        0    69436 2023-07-14 13:24:25.253770 weewx-5.0.0b9/bin/wee_resources/docs/hardware/vantage/index.html
+-rw-r--r--   0        0        0    43746 2023-07-14 13:24:25.257770 weewx-5.0.0b9/bin/wee_resources/docs/hardware/wmr100/index.html
+-rw-r--r--   0        0        0    43859 2023-07-14 13:24:25.265770 weewx-5.0.0b9/bin/wee_resources/docs/hardware/wmr300/index.html
+-rw-r--r--   0        0        0    43390 2023-07-14 13:24:25.269770 weewx-5.0.0b9/bin/wee_resources/docs/hardware/wmr9x8/index.html
+-rw-r--r--   0        0        0    38474 2023-07-14 13:24:25.273770 weewx-5.0.0b9/bin/wee_resources/docs/hardware/ws1/index.html
+-rw-r--r--   0        0        0    45261 2023-07-14 13:24:25.277770 weewx-5.0.0b9/bin/wee_resources/docs/hardware/ws23xx/index.html
+-rw-r--r--   0        0        0    50877 2023-07-14 13:24:25.281770 weewx-5.0.0b9/bin/wee_resources/docs/hardware/ws28xx/index.html
+-rw-r--r--   0        0        0    54196 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/images/antialias.gif
+-rw-r--r--   0        0        0     3145 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/images/day-gap-not-shown.png
+-rw-r--r--   0        0        0     3269 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/images/day-gap-showing.png
+-rw-r--r--   0        0        0     7579 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/images/daycompare.png
+-rw-r--r--   0        0        0     8705 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/images/daytemp_with_avg.png
+-rw-r--r--   0        0        0     7803 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/images/dayvaporp.png
+-rw-r--r--   0        0        0     7663 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/images/daywindvec.png
+-rw-r--r--   0        0        0     1026 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/images/favicon.png
+-rw-r--r--   0        0        0    38406 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/images/ferrites.jpg
+-rw-r--r--   0        0        0     3638 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/images/funky_degree.png
+-rw-r--r--   0        0        0    19123 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/images/image_parts.png
+-rw-r--r--   0        0        0    86388 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/images/image_parts.xcf
+-rw-r--r--   0        0        0     2136 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/images/logo-apple.png
+-rw-r--r--   0        0        0     4734 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/images/logo-centos.png
+-rw-r--r--   0        0        0    14541 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/images/logo-debian.png
+-rw-r--r--   0        0        0    24662 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/images/logo-fedora.png
+-rw-r--r--   0        0        0    12046 2023-07-14 13:24:24.809766 weewx-5.0.0b9/bin/wee_resources/docs/images/logo-linux.png
+-rw-r--r--   0        0        0    27245 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/images/logo-mint.png
+-rw-r--r--   0        0        0    15980 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/images/logo-opensuse.png
+-rw-r--r--   0        0        0    14374 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/images/logo-pypi.svg
+-rw-r--r--   0        0        0     1192 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/images/logo-redhat.png
+-rw-r--r--   0        0        0     3926 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/images/logo-rpi.png
+-rw-r--r--   0        0        0     7877 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/images/logo-suse.png
+-rw-r--r--   0        0        0    13954 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/images/logo-ubuntu.png
+-rw-r--r--   0        0        0    12208 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/images/logo-weewx.png
+-rw-r--r--   0        0        0    35496 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/images/pipeline.png
+-rw-r--r--   0        0        0     6709 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/images/sample_monthrain.png
+-rw-r--r--   0        0        0    10107 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/images/sample_monthtempdew.png
+-rw-r--r--   0        0        0    10649 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/images/weekgustoverlay.png
+-rw-r--r--   0        0        0     8468 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/images/weektempdew.png
+-rw-r--r--   0        0        0     6602 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/images/yeardiff.png
+-rw-r--r--   0        0        0     7286 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/images/yearhilow.png
+-rw-r--r--   0        0        0    39824 2023-07-14 13:24:24.929767 weewx-5.0.0b9/bin/wee_resources/docs/index.html
+-rw-r--r--   0        0        0    32611 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/js/cash.js
+-rw-r--r--   0        0        0    14828 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/js/cash.min.js
+-rw-r--r--   0        0        0    11422 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/js/tocbot-4.12.0.js
+-rw-r--r--   0        0        0    11422 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/js/tocbot-4.12.0.min.js
+-rw-r--r--   0        0        0     8892 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/js/tocbot-4.3.1.min.js
+-rw-r--r--   0        0        0     4640 2023-07-14 13:24:24.813766 weewx-5.0.0b9/bin/wee_resources/docs/js/weewx.js
+-rw-r--r--   0        0        0    44267 2023-07-14 13:24:25.289770 weewx-5.0.0b9/bin/wee_resources/docs/quickstarts/debian/index.html
+-rw-r--r--   0        0        0    45484 2023-07-14 13:24:25.293770 weewx-5.0.0b9/bin/wee_resources/docs/quickstarts/git/index.html
+-rw-r--r--   0        0        0    35086 2023-07-14 13:24:25.281770 weewx-5.0.0b9/bin/wee_resources/docs/quickstarts/index.html
+-rw-r--r--   0        0        0    61417 2023-07-14 13:24:25.313770 weewx-5.0.0b9/bin/wee_resources/docs/quickstarts/pip/index.html
+-rw-r--r--   0        0        0    43066 2023-07-14 13:24:25.317770 weewx-5.0.0b9/bin/wee_resources/docs/quickstarts/redhat/index.html
+-rw-r--r--   0        0        0    42005 2023-07-14 13:24:25.325770 weewx-5.0.0b9/bin/wee_resources/docs/quickstarts/suse/index.html
+-rw-r--r--   0        0        0  1041665 2023-07-14 13:24:25.501772 weewx-5.0.0b9/bin/wee_resources/docs/search/search_index.json
+-rw-r--r--   0        0        0    12774 2023-07-14 13:24:24.909767 weewx-5.0.0b9/bin/wee_resources/docs/sitemap.xml
+-rw-r--r--   0        0        0      755 2023-07-14 13:24:24.909767 weewx-5.0.0b9/bin/wee_resources/docs/sitemap.xml.gz
+-rw-r--r--   0        0        0    95541 2023-07-14 13:24:24.989768 weewx-5.0.0b9/bin/wee_resources/docs/sle/index.html
+-rw-r--r--   0        0        0    38273 2023-07-14 13:24:25.329770 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/backing-up-weewx/index.html
+-rw-r--r--   0        0        0    35047 2023-07-14 13:24:25.325770 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/index.html
+-rw-r--r--   0        0        0    41306 2023-07-14 13:24:25.333770 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/installing-weewx/index.html
+-rw-r--r--   0        0        0    39555 2023-07-14 13:24:25.337770 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/mysql-mariadb-config/index.html
+-rw-r--r--   0        0        0    38605 2023-07-14 13:24:25.341770 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/running-weewx/index.html
+-rw-r--r--   0        0        0    38636 2023-07-14 13:24:25.341770 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/system-requirements/index.html
+-rw-r--r--   0        0        0    41715 2023-07-14 13:24:25.361770 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/troubleshooting/hardware/index.html
+-rw-r--r--   0        0        0    35174 2023-07-14 13:24:25.357771 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/troubleshooting/index.html
+-rw-r--r--   0        0        0    42231 2023-07-14 13:24:25.361770 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/troubleshooting/meteo/index.html
+-rw-r--r--   0        0        0    62769 2023-07-14 13:24:25.369771 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/troubleshooting/software/index.html
+-rw-r--r--   0        0        0    42047 2023-07-14 13:24:25.345770 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/webserver-integration/index.html
+-rw-r--r--   0        0        0    39125 2023-07-14 13:24:25.377771 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/data-bindings/index.html
+-rw-r--r--   0        0        0    38632 2023-07-14 13:24:25.381771 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/databases/index.html
+-rw-r--r--   0        0        0    42056 2023-07-14 13:24:25.385771 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/databasetypes/index.html
+-rw-r--r--   0        0        0    42685 2023-07-14 13:24:25.389771 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/engine/index.html
+-rw-r--r--   0        0        0    39653 2023-07-14 13:24:25.389771 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/general/index.html
+-rw-r--r--   0        0        0    37931 2023-07-14 13:24:25.373771 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/index.html
+-rw-r--r--   0        0        0    84345 2023-07-14 13:24:25.405771 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/stations-config/index.html
+-rw-r--r--   0        0        0    40458 2023-07-14 13:24:25.405771 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/stdarchive/index.html
+-rw-r--r--   0        0        0    36995 2023-07-14 13:24:25.409771 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/stdcalibrate-config/index.html
+-rw-r--r--   0        0        0    37580 2023-07-14 13:24:25.413771 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/stdconvert-config/index.html
+-rw-r--r--   0        0        0    37788 2023-07-14 13:24:25.413771 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/stdqc-config/index.html
+-rw-r--r--   0        0        0    60403 2023-07-14 13:24:25.421771 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/stdreport-config/index.html
+-rw-r--r--   0        0        0    70521 2023-07-14 13:24:25.429771 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/stdrestful-config/index.html
+-rw-r--r--   0        0        0    35969 2023-07-14 13:24:25.433771 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/stdtimesynch/index.html
+-rw-r--r--   0        0        0    57058 2023-07-14 13:24:25.441771 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/stdwxcalculate-config/index.html
+-rw-r--r--   0        0        0    42899 2023-07-14 13:24:25.353770 weewx-5.0.0b9/bin/wee_resources/docs/usersguide/where/index.html
+-rw-r--r--   0        0        0    57483 2023-07-14 13:24:25.449771 weewx-5.0.0b9/bin/wee_resources/docs/utilities/wee_database/index.html
+-rw-r--r--   0        0        0    46261 2023-07-14 13:24:25.453771 weewx-5.0.0b9/bin/wee_resources/docs/utilities/wee_debug/index.html
+-rw-r--r--   0        0        0    36546 2023-07-14 13:24:25.457771 weewx-5.0.0b9/bin/wee_resources/docs/utilities/wee_device/index.html
+-rw-r--r--   0        0        0   254864 2023-07-14 13:24:25.477771 weewx-5.0.0b9/bin/wee_resources/docs/utilities/wee_import/index.html
+-rw-r--r--   0        0        0    38858 2023-07-14 13:24:25.477771 weewx-5.0.0b9/bin/wee_resources/docs/utilities/wee_reports/index.html
+-rw-r--r--   0        0        0    55279 2023-07-14 13:24:25.485772 weewx-5.0.0b9/bin/wee_resources/docs/utilities/weectl-database/index.html
+-rw-r--r--   0        0        0    45743 2023-07-14 13:24:25.489771 weewx-5.0.0b9/bin/wee_resources/docs/utilities/weectl-extension/index.html
+-rw-r--r--   0        0        0    56490 2023-07-14 13:24:25.497772 weewx-5.0.0b9/bin/wee_resources/docs/utilities/weectl-station/index.html
+-rw-r--r--   0        0        0    35764 2023-07-14 13:24:25.497772 weewx-5.0.0b9/bin/wee_resources/docs/utilities/weewxd/index.html
+-rw-r--r--   0        0        0   150794 2023-07-14 13:24:25.013768 weewx-5.0.0b9/bin/wee_resources/docs/versions/index.html
+-rw-r--r--   0        0        0     3097 2023-06-26 17:07:40.352703 weewx-5.0.0b9/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-37.pyc
+-rw-r--r--   0        0        0    10729 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/alarm.py
+-rw-r--r--   0        0        0      179 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/basic/changelog
+-rw-r--r--   0        0        0     1563 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/basic/install.py
+-rw-r--r--   0        0        0     1243 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/basic/readme.md
+-rw-r--r--   0        0        0     1510 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/examples/basic/skins/basic/basic.css
+-rw-r--r--   0        0        0     6451 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/examples/basic/skins/basic/current.inc
+-rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/examples/basic/skins/basic/favicon.ico
+-rw-r--r--   0        0        0    11292 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/examples/basic/skins/basic/hilo.inc
+-rw-r--r--   0        0        0     1665 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/basic/skins/basic/index.html.tmpl
+-rw-r--r--   0        0        0     2216 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/examples/basic/skins/basic/lang/en.conf
+-rw-r--r--   0        0        0     2408 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/examples/basic/skins/basic/lang/fr.conf
+-rw-r--r--   0        0        0     3173 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/examples/basic/skins/basic/skin.conf
+-rw-r--r--   0        0        0     2080 2023-07-13 00:27:45.768250 weewx-5.0.0b9/bin/wee_resources/examples/colorize/__pycache__/colorize_1.cpython-37.pyc
+-rw-r--r--   0        0        0     2255 2023-07-13 00:27:45.788250 weewx-5.0.0b9/bin/wee_resources/examples/colorize/__pycache__/colorize_2.cpython-37.pyc
+-rw-r--r--   0        0        0     3290 2023-07-13 00:27:45.788250 weewx-5.0.0b9/bin/wee_resources/examples/colorize/__pycache__/colorize_3.cpython-37.pyc
+-rw-r--r--   0        0        0     2128 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/colorize/colorize_1.py
+-rw-r--r--   0        0        0     2617 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/colorize/colorize_2.py
+-rw-r--r--   0        0        0     4001 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/colorize/colorize_3.py
+-rw-r--r--   0        0        0     4180 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/fileparse/bin/user/fileparse.py
+-rw-r--r--   0        0        0      269 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/fileparse/changelog
+-rw-r--r--   0        0        0      835 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/fileparse/install.py
+-rw-r--r--   0        0        0     2086 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/fileparse/readme.md
+-rw-r--r--   0        0        0    10792 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/lowBattery.py
+-rw-r--r--   0        0        0     1108 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/examples/mem.py
+-rw-r--r--   0        0        0     5986 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/pmon/bin/user/pmon.py
+-rw-r--r--   0        0        0      341 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/pmon/changelog
+-rw-r--r--   0        0        0     1511 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/pmon/install.py
+-rw-r--r--   0        0        0     2628 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/pmon/readme.md
+-rw-r--r--   0        0        0      507 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/pmon/skins/pmon/index.html.tmpl
+-rw-r--r--   0        0        0     1234 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/examples/pmon/skins/pmon/skin.conf
+-rw-r--r--   0        0        0     4334 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/tests/test_vaporpressure.py
+-rw-r--r--   0        0        0     4285 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/examples/vaporpressure.py
+-rw-r--r--   0        0        0     3034 2023-07-13 00:27:45.796250 weewx-5.0.0b9/bin/wee_resources/examples/xstats/bin/user/__pycache__/xstats.cpython-37.pyc
+-rw-r--r--   0        0        0     5662 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/xstats/bin/user/xstats.py
+-rw-r--r--   0        0        0      146 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/xstats/changelog
+-rw-r--r--   0        0        0      850 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/xstats/install.py
+-rw-r--r--   0        0        0     2923 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/xstats/readme.txt
+-rw-r--r--   0        0        0     2138 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/xstats/skins/xstats/index.html.tmpl
+-rw-r--r--   0        0        0      591 2023-07-11 14:40:18.482441 weewx-5.0.0b9/bin/wee_resources/examples/xstats/skins/xstats/skin.conf
+-rw-r--r--   0        0        0      676 2023-07-14 13:25:46.914307 weewx-5.0.0b9/bin/wee_resources/skins/Ftp/skin.conf
+-rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/skins/Mobile/favicon.ico
+-rw-r--r--   0        0        0     2573 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/skins/Mobile/index.html.tmpl
+-rw-r--r--   0        0        0     1021 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/skins/Mobile/lang/de.conf
+-rw-r--r--   0        0        0     1000 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/skins/Mobile/lang/en.conf
+-rw-r--r--   0        0        0     1101 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/skins/Mobile/lang/nl.conf
+-rw-r--r--   0        0        0     2940 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/skins/Mobile/lang/no.conf
+-rw-r--r--   0        0        0      671 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/skins/Mobile/mobile.css
+-rw-r--r--   0        0        0     5171 2023-07-14 13:25:46.918307 weewx-5.0.0b9/bin/wee_resources/skins/Mobile/skin.conf
+-rw-r--r--   0        0        0      760 2023-07-14 13:25:46.922307 weewx-5.0.0b9/bin/wee_resources/skins/Rsync/skin.conf
+-rw-r--r--   0        0        0     2667 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y-%m.txt.tmpl
+-rw-r--r--   0        0        0     5460 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y.txt.tmpl
+-rw-r--r--   0        0        0     1482 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/about.inc
+-rw-r--r--   0        0        0      674 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/analytics.inc
+-rw-r--r--   0        0        0     1137 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/celestial.html.tmpl
+-rw-r--r--   0        0        0     6214 2023-07-11 14:40:18.486441 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/celestial.inc
+-rw-r--r--   0        0        0     1291 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/current.inc
+-rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/favicon.ico
+-rw-r--r--   0        0        0   172876 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/font/Kanit-Bold.ttf
+-rw-r--r--   0        0        0   169744 2023-05-30 12:01:49.289499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/font/Kanit-Regular.ttf
+-rw-r--r--   0        0        0     4383 2023-07-11 14:40:18.486441 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/font/OFL.txt
+-rw-r--r--   0        0        0   224592 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/font/OpenSans-Bold.ttf
+-rw-r--r--   0        0        0   217360 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/font/OpenSans-Regular.ttf
+-rw-r--r--   0        0        0    20248 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/font/OpenSans.woff
+-rw-r--r--   0        0        0    10352 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/font/OpenSans.woff2
+-rw-r--r--   0        0        0     4348 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/font/license.txt
+-rw-r--r--   0        0        0     4360 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/hilo.inc
+-rw-r--r--   0        0        0      858 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/identifier.inc
+-rw-r--r--   0        0        0     2787 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/index.html.tmpl
+-rw-r--r--   0        0        0     9216 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/cn.conf
+-rw-r--r--   0        0        0     9844 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/cz.conf
+-rw-r--r--   0        0        0     9745 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/de.conf
+-rw-r--r--   0        0        0     9459 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/en.conf
+-rw-r--r--   0        0        0    10702 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/es.conf
+-rw-r--r--   0        0        0    10673 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/fr.conf
+-rw-r--r--   0        0        0    11838 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/gr.conf
+-rw-r--r--   0        0        0     9947 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/it.conf
+-rw-r--r--   0        0        0     9548 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/nl.conf
+-rw-r--r--   0        0        0    10705 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/no.conf
+-rw-r--r--   0        0        0    15356 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/th.conf
+-rw-r--r--   0        0        0      920 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/map.inc
+-rw-r--r--   0        0        0      572 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/radar.inc
+-rw-r--r--   0        0        0     4373 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/rss.xml.tmpl
+-rw-r--r--   0        0        0      642 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/satellite.inc
+-rw-r--r--   0        0        0     5406 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/seasons.css
+-rw-r--r--   0        0        0     6404 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/seasons.js
+-rw-r--r--   0        0        0     3947 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/sensors.inc
+-rw-r--r--   0        0        0    27402 2023-07-14 13:25:46.926307 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/skin.conf
+-rw-r--r--   0        0        0     1294 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/statistics.html.tmpl
+-rw-r--r--   0        0        0     3971 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/statistics.inc
+-rw-r--r--   0        0        0     2771 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/sunmoon.inc
+-rw-r--r--   0        0        0      987 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/tabular.html.tmpl
+-rw-r--r--   0        0        0     2450 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/telemetry.html.tmpl
+-rw-r--r--   0        0        0     1115 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Seasons/titlebar.inc
+-rw-r--r--   0        0        0     1804 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/barometer.html.tmpl
+-rw-r--r--   0        0        0      143 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/custom.js
+-rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/favicon.ico
+-rw-r--r--   0        0        0     1043 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/humidity.html.tmpl
+-rw-r--r--   0        0        0     4846 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x1.png
+-rw-r--r--   0        0        0     7142 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x2.png
+-rw-r--r--   0        0        0     4421 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x1.png
+-rw-r--r--   0        0        0     6095 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x2.png
+-rw-r--r--   0        0        0     2457 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/index.html.tmpl
+-rw-r--r--   0        0        0     1639 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/lang/de.conf
+-rw-r--r--   0        0        0     1554 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/lang/en.conf
+-rw-r--r--   0        0        0     1594 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/lang/nl.conf
+-rw-r--r--   0        0        0     3530 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/lang/no.conf
+-rw-r--r--   0        0        0     1502 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/rain.html.tmpl
+-rw-r--r--   0        0        0     7806 2023-07-14 13:25:46.926307 weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/skin.conf
+-rw-r--r--   0        0        0     1588 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/temp.html.tmpl
+-rw-r--r--   0        0        0     1681 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/wind.html.tmpl
+-rw-r--r--   0        0        0     2591 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y-%m.txt.tmpl
+-rw-r--r--   0        0        0     5364 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y.txt.tmpl
+-rw-r--r--   0        0        0     8546 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/RSS/weewx_rss.xml.tmpl
+-rw-r--r--   0        0        0       76 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/backgrounds/band.gif
+-rw-r--r--   0        0        0     2593 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/backgrounds/butterfly.jpg
+-rw-r--r--   0        0        0     1508 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/backgrounds/drops.gif
+-rw-r--r--   0        0        0     1386 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/backgrounds/flower.jpg
+-rw-r--r--   0        0        0     2277 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/backgrounds/leaf.jpg
+-rw-r--r--   0        0        0     8609 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/backgrounds/night.gif
+-rw-r--r--   0        0        0     1150 2023-05-30 12:01:49.293499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/favicon.ico
+-rw-r--r--   0        0        0   313856 2023-07-11 14:40:18.486441 weewx-5.0.0b9/bin/wee_resources/skins/Standard/font/DejaVuSansMono-Bold.ttf
+-rw-r--r--   0        0        0    20739 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/index.html.tmpl
+-rw-r--r--   0        0        0     9390 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/lang/de.conf
+-rw-r--r--   0        0        0     9264 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/lang/en.conf
+-rw-r--r--   0        0        0     9765 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/lang/fr.conf
+-rw-r--r--   0        0        0     9356 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/lang/nl.conf
+-rw-r--r--   0        0        0    10875 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/lang/no.conf
+-rw-r--r--   0        0        0    15140 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/month.html.tmpl
+-rw-r--r--   0        0        0    16429 2023-07-14 13:25:46.930307 weewx-5.0.0b9/bin/wee_resources/skins/Standard/skin.conf
+-rw-r--r--   0        0        0     1456 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/barometer.html.tmpl
+-rw-r--r--   0        0        0      143 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/custom.js
+-rw-r--r--   0        0        0     1012 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/humidity.html.tmpl
+-rw-r--r--   0        0        0     4846 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x1.png
+-rw-r--r--   0        0        0     7142 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x2.png
+-rw-r--r--   0        0        0     4421 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x1.png
+-rw-r--r--   0        0        0     6095 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x2.png
+-rw-r--r--   0        0        0     1918 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/index.html.tmpl
+-rw-r--r--   0        0        0     1000 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/radar.html.tmpl
+-rw-r--r--   0        0        0     1394 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/rain.html.tmpl
+-rw-r--r--   0        0        0     1441 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/temp_outside.html.tmpl
+-rw-r--r--   0        0        0     1508 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/wind.html.tmpl
+-rw-r--r--   0        0        0    15057 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/week.html.tmpl
+-rw-r--r--   0        0        0     3533 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/weewx.css
+-rw-r--r--   0        0        0     9990 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/skins/Standard/year.html.tmpl
+-rw-r--r--   0        0        0      154 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/apache/conf-available/weewx.conf
+-rw-r--r--   0        0        0      167 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/apache/conf.d/weewx.conf
+-rw-r--r--   0        0        0      136 2023-07-11 14:40:18.486441 weewx-5.0.0b9/bin/wee_resources/util/default/weewx
+-rwxr-xr-x   0        0        0     8897 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/i18n/i18n-report
+-rw-r--r--   0        0        0     9052 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/import/csv-example.conf
+-rw-r--r--   0        0        0     8250 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/import/cumulus-example.conf
+-rw-r--r--   0        0        0    14923 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/import/wd-example.conf
+-rw-r--r--   0        0        0     7100 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/import/weathercat-example.conf
+-rw-r--r--   0        0        0     6202 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/import/wu-example.conf
+-rwxr-xr-x   0        0        0     6057 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/init.d/weewx-multi
+-rwxr-xr-x   0        0        0      862 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/init.d/weewx.bsd
+-rwxr-xr-x   0        0        0     5111 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/init.d/weewx.debian
+-rw-r--r--   0        0        0      647 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/init.d/weewx.freebsd
+-rwxr-xr-x   0        0        0     8372 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/init.d/weewx.lsb
+-rwxr-xr-x   0        0        0     1659 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/init.d/weewx.redhat
+-rwxr-xr-x   0        0        0     4856 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/init.d/weewx.suse
+-rw-r--r--   0        0        0      914 2023-07-11 14:40:18.490441 weewx-5.0.0b9/bin/wee_resources/util/launchd/com.weewx.weewxd.plist
+-rw-r--r--   0        0        0     1800 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/logrotate.d/weewx
+-rw-r--r--   0        0        0       83 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/logwatch/conf/logfiles/weewx.conf
+-rw-r--r--   0        0        0       32 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/logwatch/conf/services/weewx.conf
+-rwxr-xr-x   0        0        0    54942 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/logwatch/scripts/services/weewx
+-rw-r--r--   0        0        0       82 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/newsyslog.d/weewx.conf
+-rw-r--r--   0        0        0     2219 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/rsyslog.d/weewx.conf
+-rwxr-xr-x   0        0        0      319 2023-07-11 14:40:18.490441 weewx-5.0.0b9/bin/wee_resources/util/scripts/wee_database
+-rwxr-xr-x   0        0        0      316 2023-07-11 14:40:18.490441 weewx-5.0.0b9/bin/wee_resources/util/scripts/wee_debug
+-rwxr-xr-x   0        0        0      317 2023-07-11 14:40:18.490441 weewx-5.0.0b9/bin/wee_resources/util/scripts/wee_device
+-rwxr-xr-x   0        0        0      317 2023-07-11 14:40:18.490441 weewx-5.0.0b9/bin/wee_resources/util/scripts/wee_import
+-rwxr-xr-x   0        0        0      318 2023-07-11 14:40:18.490441 weewx-5.0.0b9/bin/wee_resources/util/scripts/wee_reports
+-rwxr-xr-x   0        0        0      313 2023-07-11 14:40:18.490441 weewx-5.0.0b9/bin/wee_resources/util/scripts/weectl
+-rwxr-xr-x   0        0        0      313 2023-07-11 14:40:18.490441 weewx-5.0.0b9/bin/wee_resources/util/scripts/weewxd
+-rw-r--r--   0        0        0     2564 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/solaris/weewx-smf.xml
+-rw-r--r--   0        0        0      526 2023-07-11 14:40:18.490441 weewx-5.0.0b9/bin/wee_resources/util/systemd/weewx.service
+-rw-r--r--   0        0        0       34 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/tmpfiles.d/weewx.conf
+-rw-r--r--   0        0        0      149 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/udev/rules.d/acurite.rules
+-rw-r--r--   0        0        0      135 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/udev/rules.d/cc3000.rules
+-rw-r--r--   0        0        0      153 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/udev/rules.d/fousb.rules
+-rw-r--r--   0        0        0      147 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/udev/rules.d/te923.rules
+-rw-r--r--   0        0        0      624 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/udev/rules.d/vantage.rules
+-rw-r--r--   0        0        0     1560 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/udev/rules.d/weewx.rules
+-rw-r--r--   0        0        0      158 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/udev/rules.d/wmr100.rules
+-rw-r--r--   0        0        0      158 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/udev/rules.d/wmr300.rules
+-rw-r--r--   0        0        0      152 2023-05-30 12:01:49.297499 weewx-5.0.0b9/bin/wee_resources/util/udev/rules.d/ws28xx.rules
+-rw-r--r--   0        0        0    18375 2023-07-14 13:25:46.906307 weewx-5.0.0b9/bin/wee_resources/weewx.conf
+-rw-r--r--   0        0        0    25898 2023-07-11 14:40:18.430439 weewx-5.0.0b9/bin/weecfg/__init__.py
+-rw-r--r--   0        0        0    26461 2023-07-11 14:40:18.430439 weewx-5.0.0b9/bin/weecfg/database.py
+-rw-r--r--   0        0        0    24020 2023-07-11 14:40:18.430439 weewx-5.0.0b9/bin/weecfg/extension.py
+-rw-r--r--   0        0        0    33867 2023-07-14 12:13:49.722273 weewx-5.0.0b9/bin/weecfg/station_config.py
+-rw-r--r--   0        0        0    45364 2023-07-11 14:40:18.430439 weewx-5.0.0b9/bin/weecfg/update_config.py
+-rwxr-xr-x   0        0        0     1473 2023-07-11 14:40:18.430439 weewx-5.0.0b9/bin/weectl.py
+-rw-r--r--   0        0        0     2475 2023-07-11 14:40:18.430439 weewx-5.0.0b9/bin/weectllib/__init__.py
+-rw-r--r--   0        0        0    20988 2023-07-11 14:40:18.430439 weewx-5.0.0b9/bin/weectllib/database_cmd.py
+-rw-r--r--   0        0        0    29103 2023-07-11 14:40:18.430439 weewx-5.0.0b9/bin/weectllib/db_actions.py
+-rw-r--r--   0        0        0     6856 2023-07-11 14:40:18.430439 weewx-5.0.0b9/bin/weectllib/extension_cmd.py
+-rw-r--r--   0        0        0    16486 2023-07-11 21:02:09.629978 weewx-5.0.0b9/bin/weectllib/station_cmd.py
+-rw-r--r--   0        0        0     4538 2023-05-30 12:01:49.269499 weewx-5.0.0b9/bin/weedb/NOTES.md
+-rw-r--r--   0        0        0     6717 2023-07-11 14:40:18.430439 weewx-5.0.0b9/bin/weedb/__init__.py
+-rw-r--r--   0        0        0    11213 2023-07-11 14:40:18.434439 weewx-5.0.0b9/bin/weedb/mysql.py
+-rw-r--r--   0        0        0    11161 2023-07-11 14:40:18.434439 weewx-5.0.0b9/bin/weedb/sqlite.py
+-rw-r--r--   0        0        0      255 2023-05-30 12:01:49.269499 weewx-5.0.0b9/bin/weeimport/__init__.py
+-rw-r--r--   0        0        0    11110 2023-05-30 12:01:49.269499 weewx-5.0.0b9/bin/weeimport/csvimport.py
+-rw-r--r--   0        0        0    20265 2023-05-30 12:01:49.269499 weewx-5.0.0b9/bin/weeimport/cumulusimport.py
+-rw-r--r--   0        0        0    35701 2023-05-30 12:01:49.269499 weewx-5.0.0b9/bin/weeimport/wdimport.py
+-rw-r--r--   0        0        0    18225 2023-07-11 14:40:18.434439 weewx-5.0.0b9/bin/weeimport/weathercatimport.py
+-rw-r--r--   0        0        0    69526 2023-07-11 14:40:18.434439 weewx-5.0.0b9/bin/weeimport/weeimport.py
+-rw-r--r--   0        0        0    17222 2023-07-11 14:40:18.434439 weewx-5.0.0b9/bin/weeimport/wuimport.py
+-rw-r--r--   0        0        0      367 2023-05-30 12:01:49.273499 weewx-5.0.0b9/bin/weeplot/__init__.py
+-rw-r--r--   0        0        0    33267 2023-07-11 14:40:18.434439 weewx-5.0.0b9/bin/weeplot/genplot.py
+-rw-r--r--   0        0        0    25533 2023-07-11 14:40:18.434439 weewx-5.0.0b9/bin/weeplot/utilities.py
+-rw-r--r--   0        0        0     1633 2023-05-30 12:01:49.273499 weewx-5.0.0b9/bin/weeutil/Moon.py
+-rw-r--r--   0        0        0    18296 2023-05-30 12:01:49.273499 weewx-5.0.0b9/bin/weeutil/Sun.py
+-rw-r--r--   0        0        0      142 2023-05-30 12:01:49.273499 weewx-5.0.0b9/bin/weeutil/__init__.py
+-rw-r--r--   0        0        0     9408 2023-07-11 14:40:18.434439 weewx-5.0.0b9/bin/weeutil/config.py
+-rw-r--r--   0        0        0    12986 2023-07-11 14:40:18.434439 weewx-5.0.0b9/bin/weeutil/ftpupload.py
+-rw-r--r--   0        0        0     3150 2023-07-11 14:40:18.438439 weewx-5.0.0b9/bin/weeutil/log.py
+-rw-r--r--   0        0        0     5896 2023-07-11 14:40:18.438439 weewx-5.0.0b9/bin/weeutil/logger.py
+-rw-r--r--   0        0        0     6593 2023-05-30 12:01:49.273499 weewx-5.0.0b9/bin/weeutil/rsyncupload.py
+-rw-r--r--   0        0        0     2224 2023-05-30 12:01:49.273499 weewx-5.0.0b9/bin/weeutil/timediff.py
+-rw-r--r--   0        0        0    65551 2023-07-11 14:40:18.438439 weewx-5.0.0b9/bin/weeutil/weeutil.py
+-rw-r--r--   0        0        0     5929 2023-07-14 13:25:46.934307 weewx-5.0.0b9/bin/weewx/__init__.py
+-rw-r--r--   0        0        0    25878 2023-07-13 13:57:57.742680 weewx-5.0.0b9/bin/weewx/accum.py
+-rw-r--r--   0        0        0    25445 2023-07-11 23:34:10.145179 weewx-5.0.0b9/bin/weewx/almanac.py
+-rw-r--r--   0        0        0    33390 2023-07-11 14:40:18.442440 weewx-5.0.0b9/bin/weewx/cheetahgenerator.py
+-rw-r--r--   0        0        0     3393 2023-05-30 12:01:49.273499 weewx-5.0.0b9/bin/weewx/crc16.py
+-rw-r--r--   0        0        0     2888 2023-07-11 14:40:18.442440 weewx-5.0.0b9/bin/weewx/daemon.py
+-rw-r--r--   0        0        0    11955 2023-07-11 14:40:18.442440 weewx-5.0.0b9/bin/weewx/defaults.py
+-rw-r--r--   0        0        0     5148 2023-07-11 14:40:18.442440 weewx-5.0.0b9/bin/weewx/drivers/__init__.py
+-rw-r--r--   0        0        0    38987 2023-05-30 12:01:49.273499 weewx-5.0.0b9/bin/weewx/drivers/acurite.py
+-rw-r--r--   0        0        0    64005 2023-07-11 14:40:18.442440 weewx-5.0.0b9/bin/weewx/drivers/cc3000.py
+-rw-r--r--   0        0        0    78592 2023-07-11 14:40:18.442440 weewx-5.0.0b9/bin/weewx/drivers/fousb.py
+-rw-r--r--   0        0        0    14931 2023-05-30 12:01:49.273499 weewx-5.0.0b9/bin/weewx/drivers/simulator.py
+-rw-r--r--   0        0        0    99881 2023-05-30 12:01:49.273499 weewx-5.0.0b9/bin/weewx/drivers/te923.py
+-rw-r--r--   0        0        0    15797 2023-05-30 12:01:49.273499 weewx-5.0.0b9/bin/weewx/drivers/ultimeter.py
+-rw-r--r--   0        0        0   139883 2023-07-11 14:40:18.446440 weewx-5.0.0b9/bin/weewx/drivers/vantage.py
+-rw-r--r--   0        0        0    17795 2023-05-30 12:01:49.273499 weewx-5.0.0b9/bin/weewx/drivers/wmr100.py
+-rw-r--r--   0        0        0    72747 2023-05-30 12:01:49.273499 weewx-5.0.0b9/bin/weewx/drivers/wmr300.py
+-rw-r--r--   0        0        0    29536 2023-07-11 14:40:18.446440 weewx-5.0.0b9/bin/weewx/drivers/wmr9x8.py
+-rw-r--r--   0        0        0    18843 2023-07-11 14:40:18.446440 weewx-5.0.0b9/bin/weewx/drivers/ws1.py
+-rw-r--r--   0        0        0    79489 2023-07-11 14:40:18.450440 weewx-5.0.0b9/bin/weewx/drivers/ws23xx.py
+-rw-r--r--   0        0        0   173578 2023-05-30 12:01:49.277499 weewx-5.0.0b9/bin/weewx/drivers/ws28xx.py
+-rw-r--r--   0        0        0    37475 2023-07-11 14:40:18.450440 weewx-5.0.0b9/bin/weewx/engine.py
+-rw-r--r--   0        0        0      276 2023-05-30 12:01:49.277499 weewx-5.0.0b9/bin/weewx/filegenerator.py
+-rw-r--r--   0        0        0    18278 2023-07-11 14:40:18.450440 weewx-5.0.0b9/bin/weewx/imagegenerator.py
+-rw-r--r--   0        0        0    73115 2023-07-11 14:40:18.458440 weewx-5.0.0b9/bin/weewx/manager.py
+-rw-r--r--   0        0        0     3187 2023-05-30 12:01:49.277499 weewx-5.0.0b9/bin/weewx/qc.py
+-rw-r--r--   0        0        0    37780 2023-07-11 14:40:18.458440 weewx-5.0.0b9/bin/weewx/reportengine.py
+-rw-r--r--   0        0        0    79730 2023-07-11 14:40:18.462440 weewx-5.0.0b9/bin/weewx/restx.py
+-rw-r--r--   0        0        0     7207 2023-05-30 12:01:49.277499 weewx-5.0.0b9/bin/weewx/station.py
+-rw-r--r--   0        0        0    32125 2023-07-11 19:31:11.123304 weewx-5.0.0b9/bin/weewx/tags.py
+-rw-r--r--   0        0        0    71594 2023-07-11 14:40:18.466440 weewx-5.0.0b9/bin/weewx/units.py
+-rw-r--r--   0        0        0    25248 2023-05-30 12:01:49.281499 weewx-5.0.0b9/bin/weewx/uwxutils.py
+-rw-r--r--   0        0        0      246 2023-05-30 12:01:49.281499 weewx-5.0.0b9/bin/weewx/wxengine.py
+-rw-r--r--   0        0        0    30034 2023-05-30 12:01:49.281499 weewx-5.0.0b9/bin/weewx/wxformulas.py
+-rw-r--r--   0        0        0      367 2023-05-30 12:01:49.281499 weewx-5.0.0b9/bin/weewx/wxmanager.py
+-rw-r--r--   0        0        0     7270 2023-05-30 12:01:49.281499 weewx-5.0.0b9/bin/weewx/wxservices.py
+-rw-r--r--   0        0        0    34353 2023-07-11 14:40:18.466440 weewx-5.0.0b9/bin/weewx/wxxtypes.py
+-rw-r--r--   0        0        0    55988 2023-07-11 14:40:18.470440 weewx-5.0.0b9/bin/weewx/xtypes.py
+-rwxr-xr-x   0        0        0     9648 2023-07-11 14:40:18.470440 weewx-5.0.0b9/bin/weewxd.py
+-rw-r--r--   0        0        0    12175 2023-07-11 14:40:18.482441 weewx-5.0.0b9/pkg/changelog.el
+-rw-r--r--   0        0        0    12070 2023-07-11 14:40:18.482441 weewx-5.0.0b9/pkg/changelog.suse
+-rw-r--r--   0        0        0     2731 2023-05-30 12:01:49.289499 weewx-5.0.0b9/pkg/debian/README
+-rw-r--r--   0        0        0    21625 2023-07-14 13:25:50.606327 weewx-5.0.0b9/pkg/debian/changelog
+-rw-r--r--   0        0        0        3 2023-07-11 14:40:18.482441 weewx-5.0.0b9/pkg/debian/compat
+-rw-r--r--   0        0        0       36 2023-05-30 12:01:49.289499 weewx-5.0.0b9/pkg/debian/conffiles
+-rwxr-xr-x   0        0        0     3398 2023-07-11 14:40:18.482441 weewx-5.0.0b9/pkg/debian/config
+-rw-r--r--   0        0        0      724 2023-07-11 14:40:18.482441 weewx-5.0.0b9/pkg/debian/control
+-rw-r--r--   0        0        0      926 2023-07-11 14:40:18.482441 weewx-5.0.0b9/pkg/debian/copyright
+-rwxr-xr-x   0        0        0     8937 2023-07-11 14:40:18.482441 weewx-5.0.0b9/pkg/debian/postinst
+-rwxr-xr-x   0        0        0      906 2023-05-30 12:01:49.289499 weewx-5.0.0b9/pkg/debian/postrm
+-rwxr-xr-x   0        0        0      410 2023-05-30 12:01:49.289499 weewx-5.0.0b9/pkg/debian/preinst
+-rwxr-xr-x   0        0        0      693 2023-07-11 14:40:18.486441 weewx-5.0.0b9/pkg/debian/prerm
+-rwxr-xr-x   0        0        0     2985 2023-07-11 14:40:18.486441 weewx-5.0.0b9/pkg/debian/rules
+-rw-r--r--   0        0        0       12 2023-05-30 12:01:49.289499 weewx-5.0.0b9/pkg/debian/source/format
+-rw-r--r--   0        0        0     5501 2023-07-11 14:40:18.486441 weewx-5.0.0b9/pkg/debian/templates
+-rw-r--r--   0        0        0     1708 2023-07-11 14:40:18.486441 weewx-5.0.0b9/pkg/index-apt.html
+-rw-r--r--   0        0        0     1728 2023-05-30 12:01:49.289499 weewx-5.0.0b9/pkg/index-suse.html
+-rw-r--r--   0        0        0     1714 2023-05-30 12:01:49.289499 weewx-5.0.0b9/pkg/index-yum.html
+-rwxr-xr-x   0        0        0     9874 2023-05-30 12:01:49.289499 weewx-5.0.0b9/pkg/mkchangelog.pl
+-rw-r--r--   0        0        0       79 2023-05-30 12:01:49.289499 weewx-5.0.0b9/pkg/weewx-el8.repo
+-rw-r--r--   0        0        0       57 2023-05-30 12:01:49.289499 weewx-5.0.0b9/pkg/weewx-python2.list
+-rw-r--r--   0        0        0       56 2023-05-30 12:01:49.289499 weewx-5.0.0b9/pkg/weewx-python3.list
+-rw-r--r--   0        0        0       83 2023-05-30 12:01:49.289499 weewx-5.0.0b9/pkg/weewx-suse12.repo
+-rw-r--r--   0        0        0       83 2023-05-30 12:01:49.289499 weewx-5.0.0b9/pkg/weewx-suse15.repo
+-rw-r--r--   0        0        0     2201 2023-05-30 12:01:49.289499 weewx-5.0.0b9/pkg/weewx.smf
+-rw-r--r--   0        0        0     7144 2023-07-11 14:40:18.486441 weewx-5.0.0b9/pkg/weewx.spec.in
+-rw-r--r--   0        0        0     2829 2023-07-14 13:25:44.190292 weewx-5.0.0b9/pyproject.toml
+-rw-r--r--   0        0        0      154 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/apache/conf-available/weewx.conf
+-rw-r--r--   0        0        0      167 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/apache/conf.d/weewx.conf
+-rw-r--r--   0        0        0      136 2023-07-11 14:40:18.486441 weewx-5.0.0b9/util/default/weewx
+-rwxr-xr-x   0        0        0     8897 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/i18n/i18n-report
+-rw-r--r--   0        0        0     9052 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/import/csv-example.conf
+-rw-r--r--   0        0        0     8250 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/import/cumulus-example.conf
+-rw-r--r--   0        0        0    14923 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/import/wd-example.conf
+-rw-r--r--   0        0        0     7100 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/import/weathercat-example.conf
+-rw-r--r--   0        0        0     6202 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/import/wu-example.conf
+-rwxr-xr-x   0        0        0     6057 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/init.d/weewx-multi
+-rwxr-xr-x   0        0        0      862 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/init.d/weewx.bsd
+-rwxr-xr-x   0        0        0     5111 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/init.d/weewx.debian
+-rw-r--r--   0        0        0      647 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/init.d/weewx.freebsd
+-rwxr-xr-x   0        0        0     8372 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/init.d/weewx.lsb
+-rwxr-xr-x   0        0        0     1659 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/init.d/weewx.redhat
+-rwxr-xr-x   0        0        0     4856 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/init.d/weewx.suse
+-rw-r--r--   0        0        0      914 2023-07-11 14:40:18.490441 weewx-5.0.0b9/util/launchd/com.weewx.weewxd.plist
+-rw-r--r--   0        0        0     1800 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/logrotate.d/weewx
+-rw-r--r--   0        0        0       83 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/logwatch/conf/logfiles/weewx.conf
+-rw-r--r--   0        0        0       32 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/logwatch/conf/services/weewx.conf
+-rwxr-xr-x   0        0        0    54942 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/logwatch/scripts/services/weewx
+-rw-r--r--   0        0        0       82 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/newsyslog.d/weewx.conf
+-rw-r--r--   0        0        0     2219 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/rsyslog.d/weewx.conf
+-rwxr-xr-x   0        0        0      319 2023-07-11 14:40:18.490441 weewx-5.0.0b9/util/scripts/wee_database
+-rwxr-xr-x   0        0        0      316 2023-07-11 14:40:18.490441 weewx-5.0.0b9/util/scripts/wee_debug
+-rwxr-xr-x   0        0        0      317 2023-07-11 14:40:18.490441 weewx-5.0.0b9/util/scripts/wee_device
+-rwxr-xr-x   0        0        0      317 2023-07-11 14:40:18.490441 weewx-5.0.0b9/util/scripts/wee_import
+-rwxr-xr-x   0        0        0      318 2023-07-11 14:40:18.490441 weewx-5.0.0b9/util/scripts/wee_reports
+-rwxr-xr-x   0        0        0      313 2023-07-11 14:40:18.490441 weewx-5.0.0b9/util/scripts/weectl
+-rwxr-xr-x   0        0        0      313 2023-07-11 14:40:18.490441 weewx-5.0.0b9/util/scripts/weewxd
+-rw-r--r--   0        0        0     2564 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/solaris/weewx-smf.xml
+-rw-r--r--   0        0        0      526 2023-07-11 14:40:18.490441 weewx-5.0.0b9/util/systemd/weewx.service
+-rw-r--r--   0        0        0       34 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/tmpfiles.d/weewx.conf
+-rw-r--r--   0        0        0      149 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/udev/rules.d/acurite.rules
+-rw-r--r--   0        0        0      135 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/udev/rules.d/cc3000.rules
+-rw-r--r--   0        0        0      153 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/udev/rules.d/fousb.rules
+-rw-r--r--   0        0        0      147 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/udev/rules.d/te923.rules
+-rw-r--r--   0        0        0      624 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/udev/rules.d/vantage.rules
+-rw-r--r--   0        0        0     1560 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/udev/rules.d/weewx.rules
+-rw-r--r--   0        0        0      158 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/udev/rules.d/wmr100.rules
+-rw-r--r--   0        0        0      158 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/udev/rules.d/wmr300.rules
+-rw-r--r--   0        0        0      152 2023-05-30 12:01:49.297499 weewx-5.0.0b9/util/udev/rules.d/ws28xx.rules
+-rw-r--r--   0        0        0     5491 1970-01-01 00:00:00.000000 weewx-5.0.0b9/PKG-INFO
```

### Comparing `weewx-5.0.0b8/LICENSE.txt` & `weewx-5.0.0b9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/README.md` & `weewx-5.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/schemas/wview.py` & `weewx-5.0.0b9/bin/schemas/wview.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/schemas/wview_extended.py` & `weewx-5.0.0b9/bin/schemas/wview_extended.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/schemas/wview_small.py` & `weewx-5.0.0b9/bin/schemas/wview_small.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_database.py` & `weewx-5.0.0b9/bin/wee_database.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_debug.py` & `weewx-5.0.0b9/bin/wee_debug.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_device.py` & `weewx-5.0.0b9/bin/wee_device.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_import.py` & `weewx-5.0.0b9/bin/wee_import.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_reports.py` & `weewx-5.0.0b9/bin/wee_reports.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/bin/user/extensions.py` & `weewx-5.0.0b9/bin/wee_resources/bin/user/extensions.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/404.html` & `weewx-5.0.0b9/bin/wee_resources/docs/404.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/images/favicon.png` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/bundle.b4d07000.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/bundle.b4d07000.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/bundle.b4d07000.min.js.map` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/bundle.b4d07000.min.js.map`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ar.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.da.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.de.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.du.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.es.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fi.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fr.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hi.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hi.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hu.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hy.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.hy.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.it.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ja.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.kn.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.kn.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ko.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ko.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.multi.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.nl.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.no.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.pt.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ro.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ru.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sa.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sa.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sv.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ta.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.ta.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.te.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.te.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.th.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.th.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.tr.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.vi.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.zh.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/min/lunr.zh.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/tinyseg.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/lunr/wordcut.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/lunr/wordcut.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/workers/search.208ed371.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/workers/search.208ed371.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/javascripts/workers/search.208ed371.min.js.map` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/javascripts/workers/search.208ed371.min.js.map`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/stylesheets/main.85bb2934.min.css` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/stylesheets/main.85bb2934.min.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/stylesheets/main.85bb2934.min.css.map` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/stylesheets/main.85bb2934.min.css.map`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/stylesheets/palette.a6bdf11c.min.css` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/stylesheets/palette.a6bdf11c.min.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/assets/stylesheets/palette.a6bdf11c.min.css.map` & `weewx-5.0.0b9/bin/wee_resources/docs/assets/stylesheets/palette.a6bdf11c.min.css.map`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/changes/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/changes/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -3238,14 +3238,16 @@
 padded 3 digits. E.g., <code>005°</code> instead of <code>5°</code>. </p>
 <p>Most almanac properties are now returned as <code>ValueHelpers</code>, so they will
 obey local formatting conventions (in particular, decimal separators). To
 avoid breaking old skins, these properties now have new names. For example,
 use <code>$almanac.venus.altitude</code> instead of <code>$almanac.venus.alt</code>. </p>
 <p>Fix problem that prevented database from getting hit when calculating 
 <code>pressure</code>. Fixes issue #875.</p>
+<p>Fix problem that caused crashes with <code>firstlast</code> accumulator type.
+Fixes issue #876.</p>
 <h3 id="4102-02222023">4.10.2 02/22/2023<a class="headerlink" href="#4102-02222023" title="Permanent link">&para;</a></h3>
 <p>Removed errant "f-string" in <code>imagegenerator.py</code>.</p>
 <p>Added missing <code>.long_form</code> to <code>celestial.inc</code> that would cause total daylight
 to be given in seconds, instead of long form.</p>
 <p>Fix problem that a <code>None</code> value in <code>long_form()</code> would raise an exception.
 PR #843. Thanks to user Karen!</p>
 <p>The module <code>user.extensions</code> is now imported into <code>wee_reports</code>. Thanks to
```

#### html2text {}

```diff
@@ -365,14 +365,16 @@
 padded 3 digits. E.g., 005Â° instead of 5Â°.
 Most almanac properties are now returned as ValueHelpers, so they will obey
 local formatting conventions (in particular, decimal separators). To avoid
 breaking old skins, these properties now have new names. For example, use
 $almanac.venus.altitude instead of $almanac.venus.alt.
 Fix problem that prevented database from getting hit when calculating pressure.
 Fixes issue #875.
+Fix problem that caused crashes with firstlast accumulator type. Fixes issue
+#876.
 **** 4.10.2 02/22/2023¶ ****
 Removed errant "f-string" in imagegenerator.py.
 Added missing .long_form to celestial.inc that would cause total daylight to be
 given in seconds, instead of long form.
 Fix problem that a None value in long_form() would raise an exception. PR #843.
 Thanks to user Karen!
 The module user.extensions is now imported into wee_reports. Thanks to user
```

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/copyright/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/copyright/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/css/tocbot-4.12.0.css` & `weewx-5.0.0b9/bin/wee_resources/docs/css/tocbot-4.12.0.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/css/tocbot-4.3.1.css` & `weewx-5.0.0b9/bin/wee_resources/docs/css/tocbot-4.3.1.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/css/weewx_ui.css` & `weewx-5.0.0b9/bin/wee_resources/docs/css/weewx_ui.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/custom/appendix/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/custom/appendix/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/custom/cheetah/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/custom/cheetah/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -3689,29 +3689,29 @@
     [[Geographical]]
         &quot;Altitude&quot; = &quot;ระดับความสูง&quot;    # As in height above sea level
     [[Astronomical]]
         &quot;Altitude&quot; = &quot;อัลติจูด&quot;         # As in angle above the horizon
     ...
 </code></pre></div>
 <h2 id="almanac">Almanac<a class="headerlink" href="#almanac" title="Permanent link">&para;</a></h2>
-<p>If module <a href="https://rhodesmill.org/pyephem">pyephem</a> has been installed, then WeeWX can generate extensive almanac information for the Sun, Moon, Venus, Mars, Jupiter, and other heavenly bodies, including their rise, transit and set times, as well as their azimuth and altitude. Other information is also available.</p>
+<p>If module <a href="https://rhodesmill.org/pyephem"><code>ephem</code></a> has been installed, then WeeWX can generate extensive almanac information for the Sun, Moon, Venus, Mars, Jupiter, and other heavenly bodies, including their rise, transit and set times, as well as their azimuth and altitude. Other information is also available.</p>
 <p>Here is an example template:</p>
 <div class="highlight"><pre><span></span><code>Current time is $current.dateTime
 #if $almanac.hasExtras
     Sunrise, transit, sunset: $almanac.sun.rise $almanac.sun.transit $almanac.sun.set
     Moonrise, transit, moonset: $almanac.moon.rise $almanac.moon.transit $almanac.moon.set
     Mars rise, transit, set: $almanac.mars.rise $almanac.mars.transit $almanac.mars.set
     Azimuth, altitude of Mars: $almanac.mars.azimuth $almanac.mars.altitude
     Next new, full moon: $almanac.next_new_moon; $almanac.next_full_moon
     Next summer, winter solstice: $almanac.next_summer_solstice; $almanac.next_winter_solstice
 #else
     Sunrise, sunset: $almanac.sunrise $almanac.sunset
 #end if
 </code></pre></div>
-<p>If pyephem is installed this would result in:</p>
+<p>If <code>ephem</code> is installed this would result in:</p>
 <div class="example_output">
 Current time is 03-Sep-2010 11:00
     Sunrise, transit, sunset: 06:29 13:05 19:40
     Moonrise, transit, moonset: 00:29 08:37 16:39
     Mars rise, transit, set: 10:12 15:38 21:04
     Azimuth, altitude of Mars: 111° 08°
     Next new, full moon: 08-Sep-2010 03:29; 23-Sep-2010 02:17
@@ -3804,15 +3804,15 @@
 <h3 id="heavenly-bodies">Heavenly bodies<a class="headerlink" href="#heavenly-bodies" title="Permanent link">&para;</a></h3>
 <p>The second category does require a heavenly body. This covers queries such as, "When does Jupiter rise?" or, "When does the sun transit?" Examples are</p>
 <div class="highlight"><pre><span></span><code>$almanac.jupiter.rise
 </code></pre></div>
 <p>or</p>
 <div class="highlight"><pre><span></span><code>$almanac.sun.transit
 </code></pre></div>
-<p>To accurately calculate these times, WeeWX automatically uses the present temperature and pressure to calculate refraction effects. However, you can override these values, which will be necessary if you wish to match the almanac times published by the Naval Observatory <a href="https://rhodesmill.org/pyephem/rise-set.html">as explained in the pyephem documentation</a>. For example, to match the sunrise time as published by the Observatory, instead of</p>
+<p>To accurately calculate these times, WeeWX automatically uses the present temperature and pressure to calculate refraction effects. However, you can override these values, which will be necessary if you wish to match the almanac times published by the Naval Observatory <a href="https://rhodesmill.org/pyephem/rise-set.html">as explained in the PyEphem documentation</a>. For example, to match the sunrise time as published by the Observatory, instead of</p>
 <div class="highlight"><pre><span></span><code>$almanac.sun.rise
 </code></pre></div>
 <p>use</p>
 <div class="highlight"><pre><span></span><code>$almanac(pressure=0, horizon=-34.0/60.0).sun.rise
 </code></pre></div>
 <p>By setting pressure to zero we are bypassing the refraction calculations
 and manually setting the horizon to be 34 arcminutes lower than the
@@ -3834,74 +3834,129 @@
 </code></pre></div>
 <p>As you can see, many other properties can be overridden besides pressure
 and the horizon angle.</p>
 <p>PyEphem offers an extensive list of objects that can be used for the
 <em><code>heavenly_body</code></em> tag. All the planets and many stars are in the
 list.</p>
 <p>The possible values for the <em><code>attribute</code></em> tag are listed in the
-following table:</p>
+following table, along with the corresponding name used in the PyEphem documentation.</p>
 <table class="indent" style="width: 80%">
-    <caption>Attributes that can be used with heavenly bodies
-    </caption>
-    <tbody class="code">
-    <tr>
+    <caption>Attributes that can be used with heavenly bodies</caption>
+    <tbody>
+    <tr class="first_row">
+        <td>WeeWX name</td>
+        <td>PyEphem name</td>
+    </tr>
+    <tr class="code">
         <td>azimuth</td>
+        <td>az</td>
+    </tr>
+    <tr class="code">
         <td>altitude</td>
+        <td>alt</td>
     </tr>
-    <tr>
+    <tr class="code">
         <td>astro_ra</td>
+        <td>a_ra</td>
+    </tr>
+    <tr class="code">
         <td>astro_dec</td>
+        <td>a_dec</td>
     </tr>
-    <tr>
+    <tr class="code">
         <td>geo_ra</td>
+        <td>g_ra</td>
+    </tr>
+    <tr class="code">
         <td>topo_ra</td>
+        <td>ra</td>
     </tr>
-    <tr>
+    <tr class="code">
         <td>geo_dec</td>
+        <td>g_dec</td>
+    </tr>
+    <tr class="code">
         <td>topo_dec</td>
+        <td>dec</td>
     </tr>
-    <tr>
+    <tr class="code">
+        <td>elongation</td>
         <td>elong</td>
+    </tr>
+    <tr class="code">
+        <td>radius_size</td>
         <td>radius</td>
     </tr>
-    <tr>
+    <tr class="code">
+        <td>hlongitude</td>
         <td>hlon</td>
+    </tr>
+    <tr class="code">
+        <td>hlatitude</td>
         <td>hlat</td>
     </tr>
-    <tr>
+    <tr class="code">
+        <td>sublatitude</td>
         <td>sublat</td>
-        <td>sublong</td>
     </tr>
-    <tr>
+    <tr class="code">
+        <td>sublongitude</td>
+        <td>sublon</td>
+    </tr>
+    <tr class="code">
+        <td>next_rising</td>
         <td>next_rising</td>
+    </tr>
+    <tr class="code">
+        <td>next_setting</td>
         <td>next_setting</td>
     </tr>
-    <tr>
+    <tr class="code">
+        <td>next_transit</td>
         <td>next_transit</td>
+    </tr>
+    <tr class="code">
+        <td>next_antitransit</td>
         <td>next_antitransit</td>
     </tr>
-    <tr>
+    <tr class="code">
         <td>previous_rising</td>
+        <td>previous_rising</td>
+    </tr>
+    <tr class="code">
+        <td>previous_setting</td>
         <td>previous_setting</td>
     </tr>
-    <tr>
+    <tr class="code">
+        <td>previous_transit</td>
         <td>previous_transit</td>
+    </tr>
+    <tr class="code">
+        <td>previous_antitransit</td>
         <td>previous_antitransit</td>
     </tr>
-    <tr>
+    <tr class="code">
         <td>rise</td>
+        <td>next_rising</td>
+    </tr>
+    <tr class="code">
         <td>set</td>
+        <td>next_setting</td>
     </tr>
-    <tr>
+    <tr class="code">
         <td>transit</td>
-        <td>visible</td>
+        <td>next_transit</td>
+    </tr>
+    <tr>
+        <td class="code">visible</td>
+        <td>N/A</td>
     </tr>
     <tr>
-        <td>visible_change</td>
-        <td> </td>
+        <td class="code">visible_change</td>
+        <td>N/A</td>
     </tr>
     </tbody>
 </table>
 
 <div class="admonition note">
 <p class="admonition-title">Note</p>
 <p>The tags <code>topo_ra</code>, <code>astro__ra</code> and <code>geo_ra</code> return values in decimal degrees rather than customary values from 0 to 24 hours.</p>
@@ -3928,15 +3983,15 @@
 <li>
 <p>Put the following in the file <code>user/extensions.py</code>:</p>
 <div class="highlight"><pre><span></span><code>import ephem
 eros = ephem.readdb(&quot;433 Eros,e,10.8276,304.3222,178.8165,1.457940,0.5598795,0.22258902,71.2803,09/04.0/2017,2000,H11.16,0.46&quot;)
 ephem.Eros = eros
 </code></pre></div>
 <p>This does two things: it adds orbital information about <em>433 Eros</em>
-to the internal pyephem database, and it makes that data available
+to the internal PyEphem database, and it makes that data available
 under the name <code>Eros</code> (note the capital letter).</p>
 </li>
 <li>
 <p>You can then use <em>433 Eros</em> like any other body in your templates.
     For example, to display when it will rise above the horizon:</p>
 <div class="highlight"><pre><span></span><code>$almanac.eros.rise
 </code></pre></div>
```

#### html2text {}

```diff
@@ -1051,15 +1051,15 @@
         "Altitude" = "à¸£à¸°à¸à¸±à¸à¸à¸§à¸²à¸¡à¸ªà¸¹à¸"    # As in height
 above sea level
     [[Astronomical]]
         "Altitude" = "à¸­à¸±à¸¥à¸à¸´à¸à¸¹à¸"         # As in angle above the
 horizon
     ...
 ***** Almanac¶ *****
-If module pyephem has been installed, then WeeWX can generate extensive almanac
+If module ephem has been installed, then WeeWX can generate extensive almanac
 information for the Sun, Moon, Venus, Mars, Jupiter, and other heavenly bodies,
 including their rise, transit and set times, as well as their azimuth and
 altitude. Other information is also available.
 Here is an example template:
 Current time is $current.dateTime
 #if $almanac.hasExtras
     Sunrise, transit, sunset: $almanac.sun.rise $almanac.sun.transit
@@ -1071,15 +1071,15 @@
     Azimuth, altitude of Mars: $almanac.mars.azimuth $almanac.mars.altitude
     Next new, full moon: $almanac.next_new_moon; $almanac.next_full_moon
     Next summer, winter solstice: $almanac.next_summer_solstice;
 $almanac.next_winter_solstice
 #else
     Sunrise, sunset: $almanac.sunrise $almanac.sunset
 #end if
-If pyephem is installed this would result in:
+If ephem is installed this would result in:
 Current time is 03-Sep-2010 11:00 Sunrise, transit, sunset: 06:29 13:05 19:40
 Moonrise, transit, moonset: 00:29 08:37 16:39 Mars rise, transit, set: 10:12
 15:38 21:04 Azimuth, altitude of Mars: 111Â° 08Â° Next new, full moon: 08-Sep-
 2010 03:29; 23-Sep-2010 02:17 Next summer, winter solstice: 21-Jun-2011 10:16;
 21-Dec-2010 15:38
 Otherwise, a fallback of basic calculations is used, resulting in:
 Current time is 29-Mar-2011 09:20
@@ -1121,15 +1121,15 @@
 "When does Jupiter rise?" or, "When does the sun transit?" Examples are
 $almanac.jupiter.rise
 or
 $almanac.sun.transit
 To accurately calculate these times, WeeWX automatically uses the present
 temperature and pressure to calculate refraction effects. However, you can
 override these values, which will be necessary if you wish to match the almanac
-times published by the Naval Observatory as_explained_in_the_pyephem
+times published by the Naval Observatory as_explained_in_the_PyEphem
 documentation. For example, to match the sunrise time as published by the
 Observatory, instead of
 $almanac.sun.rise
 use
 $almanac(pressure=0, horizon=-34.0/60.0).sun.rise
 By setting pressure to zero we are bypassing the refraction calculations and
 manually setting the horizon to be 34 arcminutes lower than the normal horizon.
@@ -1146,31 +1146,46 @@
          horizon=horizon,              ## degrees
          temperature=temperature_C     ## degrees C
        ).heavenly_body(use_center=[01]).attribute
 As you can see, many other properties can be overridden besides pressure and
 the horizon angle.
 PyEphem offers an extensive list of objects that can be used for the
 heavenly_body tag. All the planets and many stars are in the list.
-The possible values for the attribute tag are listed in the following table:
-  Attributes that can be used with
-           heavenly bodies
-azimuth          altitude
-astro_ra         astro_dec
-geo_ra           topo_ra
-geo_dec          topo_dec
-elong            radius
-hlon             hlat
-sublat           sublong
-next_rising      next_setting
-next_transit     next_antitransit
-previous_rising  previous_setting
-previous_transit previous_antitransit
-rise             set
-transit          visible
-visible_change   Â 
+The possible values for the attribute tag are listed in the following table,
+along with the corresponding name used in the PyEphem documentation.
+Attributes that can be used with heavenly
+                 bodies
+WeeWX name           PyEphem name
+azimuth              az
+altitude             alt
+astro_ra             a_ra
+astro_dec            a_dec
+geo_ra               g_ra
+topo_ra              ra
+geo_dec              g_dec
+topo_dec             dec
+elongation           elong
+radius_size          radius
+hlongitude           hlon
+hlatitude            hlat
+sublatitude          sublat
+sublongitude         sublon
+next_rising          next_rising
+next_setting         next_setting
+next_transit         next_transit
+next_antitransit     next_antitransit
+previous_rising      previous_rising
+previous_setting     previous_setting
+previous_transit     previous_transit
+previous_antitransit previous_antitransit
+rise                 next_rising
+set                  next_setting
+transit              next_transit
+visible              N/A
+visible_change       N/A
 Note
 The tags topo_ra, astro__ra and geo_ra return values in decimal degrees rather
 than customary values from 0 to 24 hours.
 **** Functions¶ ****
 There is actually one function in this category: separation. It returns the
 angular separation between two heavenly bodies. For example, to calculate the
 angular separation between Venus and Mars you would use:
@@ -1186,15 +1201,15 @@
    1. Put the following in the file user/extensions.py:
       import ephem
       eros = ephem.readdb("433
       Eros,e,10.8276,304.3222,178.8165,1.457940,0.5598795,0.22258902,71.2803,09/
       04.0/2017,2000,H11.16,0.46")
       ephem.Eros = eros
       This does two things: it adds orbital information about 433 Eros to the
-      internal pyephem database, and it makes that data available under the
+      internal PyEphem database, and it makes that data available under the
       name Eros (note the capital letter).
    2. You can then use 433 Eros like any other body in your templates. For
       example, to display when it will rise above the horizon:
       $almanac.eros.rise
 ***** Wind¶ *****
 Wind deserves a few comments because it is stored in the database in two
 different ways: as a set of scalars, and as a vector of speed and direction.
```

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/custom/custom-reports/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/custom/custom-reports/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/custom/database/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/custom/database/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/custom/derived/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/custom/derived/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/custom/drivers/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/custom/drivers/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/custom/extensions/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/custom/extensions/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/custom/image-generator/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/custom/image-generator/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/custom/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/custom/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/custom/localization/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/custom/localization/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/custom/multiple-bindings/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/custom/multiple-bindings/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/custom/report-options/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/custom/report-options/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/custom/report-scheduling/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/custom/report-scheduling/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/custom/service-engine/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/custom/service-engine/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/custom/units/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/custom/units/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/devnotes/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/devnotes/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/examples/tag.htm` & `weewx-5.0.0b9/bin/wee_resources/docs/examples/tag.htm`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/hardware/acurite/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/hardware/acurite/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/hardware/cc3000/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/hardware/cc3000/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/hardware/drivers/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/hardware/drivers/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/hardware/fousb/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/hardware/fousb/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/hardware/te923/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/hardware/te923/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/hardware/ultimeter/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/hardware/ultimeter/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/hardware/vantage/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/hardware/vantage/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/hardware/wmr100/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/hardware/wmr100/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/hardware/wmr300/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/hardware/wmr300/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/hardware/wmr9x8/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/hardware/wmr9x8/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/hardware/ws1/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/hardware/ws1/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/hardware/ws23xx/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/hardware/ws23xx/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/hardware/ws28xx/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/hardware/ws28xx/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/antialias.gif` & `weewx-5.0.0b9/bin/wee_resources/docs/images/antialias.gif`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/day-gap-not-shown.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/day-gap-not-shown.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/day-gap-showing.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/day-gap-showing.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/daycompare.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/daycompare.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/daytemp_with_avg.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/daytemp_with_avg.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/dayvaporp.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/dayvaporp.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/daywindvec.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/daywindvec.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/favicon.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/ferrites.jpg` & `weewx-5.0.0b9/bin/wee_resources/docs/images/ferrites.jpg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/funky_degree.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/funky_degree.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/image_parts.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/image_parts.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/image_parts.xcf` & `weewx-5.0.0b9/bin/wee_resources/docs/images/image_parts.xcf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/logo-apple.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/logo-apple.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/logo-centos.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/logo-centos.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/logo-debian.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/logo-debian.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/logo-fedora.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/logo-fedora.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/logo-linux.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/logo-linux.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/logo-mint.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/logo-mint.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/logo-opensuse.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/logo-opensuse.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/logo-pypi.svg` & `weewx-5.0.0b9/bin/wee_resources/docs/images/logo-pypi.svg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/logo-redhat.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/logo-redhat.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/logo-rpi.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/logo-rpi.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/logo-suse.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/logo-suse.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/logo-ubuntu.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/logo-ubuntu.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/logo-weewx.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/logo-weewx.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/pipeline.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/pipeline.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/sample_monthrain.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/sample_monthrain.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/sample_monthtempdew.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/sample_monthtempdew.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/weekgustoverlay.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/weekgustoverlay.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/weektempdew.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/weektempdew.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/yeardiff.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/yeardiff.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/images/yearhilow.png` & `weewx-5.0.0b9/bin/wee_resources/docs/images/yearhilow.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/js/cash.js` & `weewx-5.0.0b9/bin/wee_resources/docs/js/cash.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/js/cash.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/js/cash.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/js/tocbot-4.12.0.js` & `weewx-5.0.0b9/bin/wee_resources/docs/js/tocbot-4.12.0.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/js/tocbot-4.12.0.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/js/tocbot-4.12.0.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/js/tocbot-4.3.1.min.js` & `weewx-5.0.0b9/bin/wee_resources/docs/js/tocbot-4.3.1.min.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/js/weewx.js` & `weewx-5.0.0b9/bin/wee_resources/docs/js/weewx.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/quickstarts/debian/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/quickstarts/debian/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/quickstarts/git/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/quickstarts/git/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/quickstarts/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/quickstarts/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/quickstarts/pip/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/quickstarts/pip/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/quickstarts/redhat/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/quickstarts/redhat/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/quickstarts/suse/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/quickstarts/suse/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/search/search_index.json` & `weewx-5.0.0b9/bin/wee_resources/docs/search/search_index.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9957113629209945%*

 * *Differences: {"'docs'": "{11: {'text': '<p>Python 2.7 is no longer supported. You must have Python 3.7 "*

 * *           '(introduced May 2018) or greater.</p> <p>WeeWX can now be installed using pip.</p> '*

 * *           '<p>With pip installs, user data is stored in <code>~/weewx-data</code> by default,  '*

 * *           'instead of <code>/home/weewx</code>. This allows pip installs to be done without root '*

 * *           'privileges. However, <code>/home/weewx</code> can still be used.</p> <p>The new '*

 * *           'utility <code>weect […]*

```diff
@@ -62,15 +62,15 @@
         {
             "location": "changes/#weewx-change-history",
             "text": "",
             "title": "WeeWX change history"
         },
         {
             "location": "changes/#500-mmddyyyy",
-            "text": "<p>Python 2.7 is no longer supported. You must have Python 3.7 (introduced May 2018) or greater.</p> <p>WeeWX can now be installed using pip.</p> <p>With pip installs, user data is stored in <code>~/weewx-data</code> by default,  instead of <code>/home/weewx</code>. This allows pip installs to be done without root privileges. However, <code>/home/weewx</code> can still be used.</p> <p>The new utility <code>weectl</code> is now used for configuring stations, extensions, and the databases. With time, it will probably take on other responsibilities.</p> <p>Package installs now use systemd instead of the old System V <code>/etc/init.d</code>.</p> <p>Removed all references to the deprecated package <code>distutils</code>, which is due to be removed in Python v3.12.</p> <p>Removed the utility <code>wunderfixer</code>. The Weather Underground seems to no longer allow posting past-dated records.</p> <p>Documentation now uses MkDocs.</p> <p>Logging handler <code>rotate</code> has been removed. Its need to access a privileged location <code>/var/log/</code> on start up would cause crashes, even if it was never used.</p> <p>MacOS now logs to <code>syslog</code> like any other system, rather than <code>rotate</code>.</p> <p>Method <code>ImageDraw.textsize()</code> and constant <code>ImageFont.LAYOUT_BASIC</code> were deprecated in Pillow 9.2 (1-Jul-2022), then removed in Pillow 10.0 (1-Jul-2023). Replaced them with alternatives.</p> <p>The Standard skin now uses the font <code>DejaVuSansMono-Bold</code> and includes a copy. Before, it had to rely on hardwired font paths, which were less reliable.</p> <p>If the uploaders get a response code of 429 (\"TOO MANY REQUESTS\"), they no longer bother trying again.</p> <p>Limit station registration to once a day, max.</p> <p>Station registration now uses HTTP POST, instead of HTTP GET.</p> <p>Station registration is delayed by a random length of time to avoid everyone hitting the server at the same time.</p> <p>Fix problem where aggregation of null wind directions returns 90\u00b0 instead of null. Fixes issue #849.</p> <p>Fix wrong station type for Vantage <code>wee_device --info</code> query.</p> <p>Add retransmit information for Vantage <code>wee_device --info</code> query.</p> <p>Fix problem when setting Vantage repeater. Fixes issue #863.</p> <p>Detect \"dash\" values for rain-related measurements on Vantage stations.</p> <p>Change aggregations <code>minsumtime</code> and <code>maxsumtime</code> to return start-of-day,  rather than the time of max rainfall during the day.</p> <p>Relax requirement that column <code>dateTime</code> be the first column in the database. Fixes issue #855.</p> <p>Fix bug when using Pillow v9.5.0. Fixes issue #862.</p> <p>Allow aggregation of xtypes that are not in the database schema. Fixes issue #864.</p> <p>Additional shorthand notations for aggregation and trend intervals. For example, '3h' for three hours.</p> <p>Accumulator <code>firstlast</code> no longer coerces values to a string. Thanks to user \"Karen\" for spotting this!</p> <p>Fixed problem that prevented the astrometric heliocentric longitude of a body from being calculated properly.</p> <p>Default format for azimuth properties (such as wind direction) is now zero padded 3 digits. E.g., <code>005\u00b0</code> instead of <code>5\u00b0</code>. </p> <p>Most almanac properties are now returned as <code>ValueHelpers</code>, so they will obey local formatting conventions (in particular, decimal separators). To avoid breaking old skins, these properties now have new names. For example, use <code>$almanac.venus.altitude</code> instead of <code>$almanac.venus.alt</code>. </p> <p>Fix problem that prevented database from getting hit when calculating  <code>pressure</code>. Fixes issue #875.</p>",
+            "text": "<p>Python 2.7 is no longer supported. You must have Python 3.7 (introduced May 2018) or greater.</p> <p>WeeWX can now be installed using pip.</p> <p>With pip installs, user data is stored in <code>~/weewx-data</code> by default,  instead of <code>/home/weewx</code>. This allows pip installs to be done without root privileges. However, <code>/home/weewx</code> can still be used.</p> <p>The new utility <code>weectl</code> is now used for configuring stations, extensions, and the databases. With time, it will probably take on other responsibilities.</p> <p>Package installs now use systemd instead of the old System V <code>/etc/init.d</code>.</p> <p>Removed all references to the deprecated package <code>distutils</code>, which is due to be removed in Python v3.12.</p> <p>Removed the utility <code>wunderfixer</code>. The Weather Underground seems to no longer allow posting past-dated records.</p> <p>Documentation now uses MkDocs.</p> <p>Logging handler <code>rotate</code> has been removed. Its need to access a privileged location <code>/var/log/</code> on start up would cause crashes, even if it was never used.</p> <p>MacOS now logs to <code>syslog</code> like any other system, rather than <code>rotate</code>.</p> <p>Method <code>ImageDraw.textsize()</code> and constant <code>ImageFont.LAYOUT_BASIC</code> were deprecated in Pillow 9.2 (1-Jul-2022), then removed in Pillow 10.0 (1-Jul-2023). Replaced them with alternatives.</p> <p>The Standard skin now uses the font <code>DejaVuSansMono-Bold</code> and includes a copy. Before, it had to rely on hardwired font paths, which were less reliable.</p> <p>If the uploaders get a response code of 429 (\"TOO MANY REQUESTS\"), they no longer bother trying again.</p> <p>Limit station registration to once a day, max.</p> <p>Station registration now uses HTTP POST, instead of HTTP GET.</p> <p>Station registration is delayed by a random length of time to avoid everyone hitting the server at the same time.</p> <p>Fix problem where aggregation of null wind directions returns 90\u00b0 instead of null. Fixes issue #849.</p> <p>Fix wrong station type for Vantage <code>wee_device --info</code> query.</p> <p>Add retransmit information for Vantage <code>wee_device --info</code> query.</p> <p>Fix problem when setting Vantage repeater. Fixes issue #863.</p> <p>Detect \"dash\" values for rain-related measurements on Vantage stations.</p> <p>Change aggregations <code>minsumtime</code> and <code>maxsumtime</code> to return start-of-day,  rather than the time of max rainfall during the day.</p> <p>Relax requirement that column <code>dateTime</code> be the first column in the database. Fixes issue #855.</p> <p>Fix bug when using Pillow v9.5.0. Fixes issue #862.</p> <p>Allow aggregation of xtypes that are not in the database schema. Fixes issue #864.</p> <p>Additional shorthand notations for aggregation and trend intervals. For example, '3h' for three hours.</p> <p>Accumulator <code>firstlast</code> no longer coerces values to a string. Thanks to user \"Karen\" for spotting this!</p> <p>Fixed problem that prevented the astrometric heliocentric longitude of a body from being calculated properly.</p> <p>Default format for azimuth properties (such as wind direction) is now zero padded 3 digits. E.g., <code>005\u00b0</code> instead of <code>5\u00b0</code>. </p> <p>Most almanac properties are now returned as <code>ValueHelpers</code>, so they will obey local formatting conventions (in particular, decimal separators). To avoid breaking old skins, these properties now have new names. For example, use <code>$almanac.venus.altitude</code> instead of <code>$almanac.venus.alt</code>. </p> <p>Fix problem that prevented database from getting hit when calculating  <code>pressure</code>. Fixes issue #875.</p> <p>Fix problem that caused crashes with <code>firstlast</code> accumulator type. Fixes issue #876.</p>",
             "title": "5.0.0 MM/DD/YYYY"
         },
         {
             "location": "changes/#4102-02222023",
             "text": "<p>Removed errant \"f-string\" in <code>imagegenerator.py</code>.</p> <p>Added missing <code>.long_form</code> to <code>celestial.inc</code> that would cause total daylight to be given in seconds, instead of long form.</p> <p>Fix problem that a <code>None</code> value in <code>long_form()</code> would raise an exception. PR #843. Thanks to user Karen!</p> <p>The module <code>user.extensions</code> is now imported into <code>wee_reports</code>. Thanks to user jocelynj! PR #842.</p> <p>Fix problem that prevented <code>wee_device --set-retransmit</code> from working on Vantage stations.</p> <p>Using a bad data binding with an aggregation tag no longer results in an exception. Instead, it shows the tag in the results. Related to PR #817.</p>",
             "title": "4.10.2 02/22/2023"
         },
@@ -1432,35 +1432,35 @@
         {
             "location": "custom/cheetah/#context-sensitive-lookups-pgettext",
             "text": "<p>A common problem is that the same string may have different translations, depending on its context. For example, in English, the word \"Altitude\" is used to mean both height above sea level, and the angle of a heavenly body from the horizon, but that's not necessarily true in other languages. For example, in Thai, \"\u0e23\u0e30\u0e14\u0e31\u0e1a\u0e04\u0e27\u0e32\u0e21\u0e2a\u0e39\u0e07\" is used to mean the former, \"\u0e2d\u0e31\u0e25\u0e15\u0e34\u0e08\u0e39\u0e14\" the latter. The function <code>pgettext()</code> (the \"p\" stands for particular) allows you to distinguish between the two. Its semantics are very similar to the GNU and Python versions of the function. Here's an example:</p> <pre><code>&lt;p&gt;$pgettext(\"Geographical\",\"Altitude\"): $station.altitude&lt;/p&gt;\n&lt;p&gt;$pgettext(\"Astronomical\",\"Altitude\"): $almanac.moon.alt&lt;/p&gt;\n</code></pre> <p>The <code>[Texts]</code> section of the language file should then contain a subsection for each context. For example, the Thai language file would include:</p> <p><code>th.conf</code></p> <pre><code>[Texts]\n    ...\n    [[Geographical]]\n        \"Altitude\" = \"\u0e23\u0e30\u0e14\u0e31\u0e1a\u0e04\u0e27\u0e32\u0e21\u0e2a\u0e39\u0e07\"    # As in height above sea level\n    [[Astronomical]]\n        \"Altitude\" = \"\u0e2d\u0e31\u0e25\u0e15\u0e34\u0e08\u0e39\u0e14\"         # As in angle above the horizon\n    ...\n</code></pre>",
             "title": "Context sensitive lookups: <code>$pgettext()</code>"
         },
         {
             "location": "custom/cheetah/#almanac",
-            "text": "<p>If module pyephem has been installed, then WeeWX can generate extensive almanac information for the Sun, Moon, Venus, Mars, Jupiter, and other heavenly bodies, including their rise, transit and set times, as well as their azimuth and altitude. Other information is also available.</p> <p>Here is an example template:</p> <pre><code>Current time is $current.dateTime\n#if $almanac.hasExtras\n    Sunrise, transit, sunset: $almanac.sun.rise $almanac.sun.transit $almanac.sun.set\n    Moonrise, transit, moonset: $almanac.moon.rise $almanac.moon.transit $almanac.moon.set\n    Mars rise, transit, set: $almanac.mars.rise $almanac.mars.transit $almanac.mars.set\n    Azimuth, altitude of Mars: $almanac.mars.azimuth $almanac.mars.altitude\n    Next new, full moon: $almanac.next_new_moon; $almanac.next_full_moon\n    Next summer, winter solstice: $almanac.next_summer_solstice; $almanac.next_winter_solstice\n#else\n    Sunrise, sunset: $almanac.sunrise $almanac.sunset\n#end if\n</code></pre> <p>If pyephem is installed this would result in:</p>  Current time is 03-Sep-2010 11:00     Sunrise, transit, sunset: 06:29 13:05 19:40     Moonrise, transit, moonset: 00:29 08:37 16:39     Mars rise, transit, set: 10:12 15:38 21:04     Azimuth, altitude of Mars: 111\u00b0 08\u00b0     Next new, full moon: 08-Sep-2010 03:29; 23-Sep-2010 02:17     Next summer, winter solstice: 21-Jun-2011 10:16; 21-Dec-2010 15:38  <p>Otherwise, a fallback of basic calculations is used, resulting in:</p>  Current time is 29-Mar-2011 09:20   Sunrise, sunset: 06:51 19:30  <p>As shown in the example, you can test whether this extended almanac information is available with the value <code>$almanac.hasExtras</code>.</p> <p>The almanac information falls into three categories:</p> <ul> <li>Calendar events</li> <li>Heavenly bodies</li> <li>Functions</li> </ul> <p>We will cover each of these separately.</p>",
+            "text": "<p>If module <code>ephem</code> has been installed, then WeeWX can generate extensive almanac information for the Sun, Moon, Venus, Mars, Jupiter, and other heavenly bodies, including their rise, transit and set times, as well as their azimuth and altitude. Other information is also available.</p> <p>Here is an example template:</p> <pre><code>Current time is $current.dateTime\n#if $almanac.hasExtras\n    Sunrise, transit, sunset: $almanac.sun.rise $almanac.sun.transit $almanac.sun.set\n    Moonrise, transit, moonset: $almanac.moon.rise $almanac.moon.transit $almanac.moon.set\n    Mars rise, transit, set: $almanac.mars.rise $almanac.mars.transit $almanac.mars.set\n    Azimuth, altitude of Mars: $almanac.mars.azimuth $almanac.mars.altitude\n    Next new, full moon: $almanac.next_new_moon; $almanac.next_full_moon\n    Next summer, winter solstice: $almanac.next_summer_solstice; $almanac.next_winter_solstice\n#else\n    Sunrise, sunset: $almanac.sunrise $almanac.sunset\n#end if\n</code></pre> <p>If <code>ephem</code> is installed this would result in:</p>  Current time is 03-Sep-2010 11:00     Sunrise, transit, sunset: 06:29 13:05 19:40     Moonrise, transit, moonset: 00:29 08:37 16:39     Mars rise, transit, set: 10:12 15:38 21:04     Azimuth, altitude of Mars: 111\u00b0 08\u00b0     Next new, full moon: 08-Sep-2010 03:29; 23-Sep-2010 02:17     Next summer, winter solstice: 21-Jun-2011 10:16; 21-Dec-2010 15:38  <p>Otherwise, a fallback of basic calculations is used, resulting in:</p>  Current time is 29-Mar-2011 09:20   Sunrise, sunset: 06:51 19:30  <p>As shown in the example, you can test whether this extended almanac information is available with the value <code>$almanac.hasExtras</code>.</p> <p>The almanac information falls into three categories:</p> <ul> <li>Calendar events</li> <li>Heavenly bodies</li> <li>Functions</li> </ul> <p>We will cover each of these separately.</p>",
             "title": "Almanac"
         },
         {
             "location": "custom/cheetah/#calendar-events",
             "text": "<p>\"Calendar events\" do not require a heavenly body. They cover things such as the time of the next solstice or next first quarter moon, or the sidereal time. The syntax is:</p> <pre><code>$almanac.next_solstice\n</code></pre> <p>or</p> <pre><code>$almanac.next_first_quarter_moon\n</code></pre> <p>or</p> <pre><code>$almanac.sidereal_angle\n</code></pre> <p>Here is a table of the information that falls into this category:</p> Calendar events previous_equinox next_equinox previous_solstice next_solstice previous_autumnal_equinox next_autumnal_equinox previous_vernal_equinox next_vernal_equinox previous_winter_solstice next_winter_solstice previous_summer_solstice next_summer_solstice previous_new_moon next_new_moon previous_first_quarter_moon next_first_quarter_moon previous_full_moon next_full_moon previous_last_quarter_moon next_last_quarter_moon sidereal_angle <p>Note</p> <p>The tag <code>$almanac.sidereal_angle</code> returns a value in decimal degrees rather than a more customary value from 0 to 24 hours.</p>",
             "title": "Calendar events"
         },
         {
             "location": "custom/cheetah/#heavenly-bodies",
-            "text": "<p>The second category does require a heavenly body. This covers queries such as, \"When does Jupiter rise?\" or, \"When does the sun transit?\" Examples are</p> <pre><code>$almanac.jupiter.rise\n</code></pre> <p>or</p> <pre><code>$almanac.sun.transit\n</code></pre> <p>To accurately calculate these times, WeeWX automatically uses the present temperature and pressure to calculate refraction effects. However, you can override these values, which will be necessary if you wish to match the almanac times published by the Naval Observatory as explained in the pyephem documentation. For example, to match the sunrise time as published by the Observatory, instead of</p> <pre><code>$almanac.sun.rise\n</code></pre> <p>use</p> <pre><code>$almanac(pressure=0, horizon=-34.0/60.0).sun.rise\n</code></pre> <p>By setting pressure to zero we are bypassing the refraction calculations and manually setting the horizon to be 34 arcminutes lower than the normal horizon. This is what the Navy uses.</p> <p>If you wish to calculate the start of civil twilight, you can set the horizon to -6 degrees, and also tell WeeWX to use the center of the sun (instead of the upper limb, which it normally uses) to do the calcuation:</p> <pre><code>$almanac(pressure=0, horizon=-6).sun(use_center=1).rise\n</code></pre> <p>The general syntax is:</p> <pre><code>$almanac(almanac_time=time,            ## Unix epoch time\n         lat=latitude, lon=longitude,  ## degrees\n         altitude=altitude,            ## meters\n         pressure=pressure,            ## mbars\n         horizon=horizon,              ## degrees\n         temperature=temperature_C     ## degrees C\n       ).heavenly_body(use_center=[01]).attribute\n</code></pre> <p>As you can see, many other properties can be overridden besides pressure and the horizon angle.</p> <p>PyEphem offers an extensive list of objects that can be used for the <code>heavenly_body</code> tag. All the planets and many stars are in the list.</p> <p>The possible values for the <code>attribute</code> tag are listed in the following table:</p> Attributes that can be used with heavenly bodies      azimuth altitude astro_ra astro_dec geo_ra topo_ra geo_dec topo_dec elong radius hlon hlat sublat sublong next_rising next_setting next_transit next_antitransit previous_rising previous_setting previous_transit previous_antitransit rise set transit visible visible_change <p>Note</p> <p>The tags <code>topo_ra</code>, <code>astro__ra</code> and <code>geo_ra</code> return values in decimal degrees rather than customary values from 0 to 24 hours.</p>",
+            "text": "<p>The second category does require a heavenly body. This covers queries such as, \"When does Jupiter rise?\" or, \"When does the sun transit?\" Examples are</p> <pre><code>$almanac.jupiter.rise\n</code></pre> <p>or</p> <pre><code>$almanac.sun.transit\n</code></pre> <p>To accurately calculate these times, WeeWX automatically uses the present temperature and pressure to calculate refraction effects. However, you can override these values, which will be necessary if you wish to match the almanac times published by the Naval Observatory as explained in the PyEphem documentation. For example, to match the sunrise time as published by the Observatory, instead of</p> <pre><code>$almanac.sun.rise\n</code></pre> <p>use</p> <pre><code>$almanac(pressure=0, horizon=-34.0/60.0).sun.rise\n</code></pre> <p>By setting pressure to zero we are bypassing the refraction calculations and manually setting the horizon to be 34 arcminutes lower than the normal horizon. This is what the Navy uses.</p> <p>If you wish to calculate the start of civil twilight, you can set the horizon to -6 degrees, and also tell WeeWX to use the center of the sun (instead of the upper limb, which it normally uses) to do the calcuation:</p> <pre><code>$almanac(pressure=0, horizon=-6).sun(use_center=1).rise\n</code></pre> <p>The general syntax is:</p> <pre><code>$almanac(almanac_time=time,            ## Unix epoch time\n         lat=latitude, lon=longitude,  ## degrees\n         altitude=altitude,            ## meters\n         pressure=pressure,            ## mbars\n         horizon=horizon,              ## degrees\n         temperature=temperature_C     ## degrees C\n       ).heavenly_body(use_center=[01]).attribute\n</code></pre> <p>As you can see, many other properties can be overridden besides pressure and the horizon angle.</p> <p>PyEphem offers an extensive list of objects that can be used for the <code>heavenly_body</code> tag. All the planets and many stars are in the list.</p> <p>The possible values for the <code>attribute</code> tag are listed in the following table, along with the corresponding name used in the PyEphem documentation.</p> Attributes that can be used with heavenly bodies WeeWX name PyEphem name azimuth az altitude alt astro_ra a_ra astro_dec a_dec geo_ra g_ra topo_ra ra geo_dec g_dec topo_dec dec elongation elong radius_size radius hlongitude hlon hlatitude hlat sublatitude sublat sublongitude sublon next_rising next_rising next_setting next_setting next_transit next_transit next_antitransit next_antitransit previous_rising previous_rising previous_setting previous_setting previous_transit previous_transit previous_antitransit previous_antitransit rise next_rising set next_setting transit next_transit visible N/A visible_change N/A <p>Note</p> <p>The tags <code>topo_ra</code>, <code>astro__ra</code> and <code>geo_ra</code> return values in decimal degrees rather than customary values from 0 to 24 hours.</p>",
             "title": "Heavenly bodies"
         },
         {
             "location": "custom/cheetah/#functions",
             "text": "<p>There is actually one function in this category: <code>separation</code>. It returns the angular separation between two heavenly bodies. For example, to calculate the angular separation between Venus and Mars you would use:</p> <pre><code>&lt;p&gt;The separation between Venus and Mars is\n      $almanac.separation(($almanac.venus.alt,$almanac.venus.az), ($almanac.mars.alt,$almanac.mars.az))&lt;/p&gt;\n</code></pre> <p>This would result in:</p>  The separation between Venus and Mars is 55:55:31.8",
             "title": "Functions"
         },
         {
             "location": "custom/cheetah/#adding-new-bodies-to-the-almanac",
-            "text": "<p>It is possible to extend the WeeWX almanac, adding new bodies that it was not previously aware of. For example, say we wanted to add 433 Eros, the first asteroid visited by a spacecraft. Here is the process:</p> <ol> <li> <p>Put the following in the file <code>user/extensions.py</code>:</p> <pre><code>import ephem\neros = ephem.readdb(\"433 Eros,e,10.8276,304.3222,178.8165,1.457940,0.5598795,0.22258902,71.2803,09/04.0/2017,2000,H11.16,0.46\")\nephem.Eros = eros\n</code></pre> <p>This does two things: it adds orbital information about 433 Eros to the internal pyephem database, and it makes that data available under the name <code>Eros</code> (note the capital letter).</p> </li> <li> <p>You can then use 433 Eros like any other body in your templates.     For example, to display when it will rise above the horizon:</p> <pre><code>$almanac.eros.rise\n</code></pre> </li> </ol>",
+            "text": "<p>It is possible to extend the WeeWX almanac, adding new bodies that it was not previously aware of. For example, say we wanted to add 433 Eros, the first asteroid visited by a spacecraft. Here is the process:</p> <ol> <li> <p>Put the following in the file <code>user/extensions.py</code>:</p> <pre><code>import ephem\neros = ephem.readdb(\"433 Eros,e,10.8276,304.3222,178.8165,1.457940,0.5598795,0.22258902,71.2803,09/04.0/2017,2000,H11.16,0.46\")\nephem.Eros = eros\n</code></pre> <p>This does two things: it adds orbital information about 433 Eros to the internal PyEphem database, and it makes that data available under the name <code>Eros</code> (note the capital letter).</p> </li> <li> <p>You can then use 433 Eros like any other body in your templates.     For example, to display when it will rise above the horizon:</p> <pre><code>$almanac.eros.rise\n</code></pre> </li> </ol>",
             "title": "Adding new bodies to the almanac"
         },
         {
             "location": "custom/cheetah/#wind",
             "text": "<p>Wind deserves a few comments because it is stored in the database in two different ways: as a set of scalars, and as a vector of speed and direction. Here are the four wind-related scalars stored in the main archive database:</p> Archive type Meaning Valid contexts windSpeed The average wind speed seen during the archive period.                       $current, $latest, $hour, $day, $week, $month, $year, $rainyear          windDir If software record generation is used, this is the vector average over the archive period. If             hardware record generation is used, the value is hardware dependent.          windGust The maximum (gust) wind speed seen during the archive period.          windGustDir The direction of the wind when the gust was observed. <p>Some wind aggregation types, notably <code>vecdir</code> and <code>vecavg</code>, require wind speed and direction. For these, WeeWX provides a composite observation type called <code>wind</code>. It is stored directly in the daily summaries, but synthesized for aggregations other than multiples of a day.</p> Daily summary type Meaning Valid contexts wind A vector composite of the wind. <code>$hour</code>, <code>$day</code>, <code>$week</code>, <code>$month</code>, <code>$year</code>, <code>$rainyear</code> <p>Any of these can be used in your tags. Here are some examples:</p> Tag Meaning $current.windSpeed The average wind speed over the most recent archive interval.          $current.windDir If software record generation is used, this is the vector average over the archive interval. If             hardware record generation is used, the value is hardware dependent.          $current.windGust The maximum wind speed (gust) over the most recent archive interval.          $current.windGustDir The direction of the gust. $day.windSpeed.avg$day.wind.avg The average wind speed since midnight. If the wind blows east at 5 m/s for 2 hours, then west at 5             m/s for 2 hours, the average wind speed is 5 m/s.          $day.wind.vecavg The vector average wind speed since midnight. If the wind blows east at 5 m/s for 2 hours,             then west at 5 m/s for 2 hours, the vector average wind speed is zero.          $day.wind.vecdir The direction of the vector averaged wind speed. If the wind blows northwest at 5 m/s for two hours,             then southwest at 5 m/s for two hours, the vector averaged direction is west.          $day.windGust.max$day.wind.max The maximum wind gust since midnight. $day.wind.gustdir The direction of the maximum wind gust. $day.windGust.maxtime$day.wind.maxtime The time of the maximum wind gust. $day.windSpeed.max The max average wind speed. The wind is averaged over each of the archive intervals. Then the             maximum of these values is taken. Note that this is not the same as the maximum wind gust.          $day.windDir.avg              Not a very useful quantity. This is the strict, arithmetic average of all the compass wind             directions. If the wind blows at 350\u00b0 for two hours then at 10\u00b0 for two hours,             then the scalar average wind direction will be 180\u00b0 \u2014 probably not what you             expect, nor want.",
             "title": "Wind"
         },
@@ -5142,126 +5142,151 @@
         {
             "location": "utilities/weectl-extension/#install-examples",
             "text": "<p>These examples illustrate how to use the extension installer.</p> <p>Do a dry run of installing an uploader for the Windy website, maximum verbosity:</p> <pre><code>% weectl extension install https://github.com/matthewwall/weewx-windy/archive/master.zip --dry-run --verbosity=3\nRequest to install 'https://github.com/matthewwall/weewx-windy/archive/master.zip'\nThis is a dry run. Nothing will actually be done.\nExtracting from zip archive /var/folders/xm/72q6zf8j71x8df2cqh0j9f6c0000gn/T/tmpuvuc_c0k\n  Request to install extension found in directory /var/folders/xm/72q6zf8j71x8df2cqh0j9f6c0000gn/T/tmpif_nj_0g/weewx-windy-master/\n  Found extension with name 'windy'\nCopying new files\n    Copying from '/var/folders/xm/72q6zf8j71x8df2cqh0j9f6c0000gn/T/tmpif_nj_0g/weewx-windy-master/bin/user/windy.py' to '/Users/Shared/weewx/bin/user/windy.py'\nCopied 0 files\n  Adding services to service lists\n    Added new service user.windy.Windy to restful_services\n  Adding sections to configuration file\n    Merged extension settings into configuration file\nSaving installer file to /Users/Shared/weewx/bin/user/installer/windy\nFinished installing extension windy from https://github.com/matthewwall/weewx-windy/archive/master.zip\nThis was a dry run. Nothing was actually done.\n</code></pre> <p>Do it for real, default verbosity:</p> <pre><code>% weectl extension install https://github.com/matthewwall/weewx-windy/archive/master.zip\nRequest to install 'https://github.com/matthewwall/weewx-windy/archive/master.zip'\nExtracting from zip archive /var/folders/xm/72q6zf8j71x8df2cqh0j9f6c0000gn/T/tmpk8ggl4qr\nSaving installer file to /Users/Shared/weewx/bin/user/installer/windy\nSaved configuration dictionary. Backup copy at /Users/Shared/weewx/weewx.conf.20230110152037\nFinished installing extension windy from https://github.com/matthewwall/weewx-windy/archive/master.zip\n</code></pre> <p>List the results:</p> <pre><code>% weectl extension list                                                                 \nExtension Name    Version   Description\nwindy             0.7       Upload weather data to Windy.\n</code></pre> <p>Uninstall the extension:</p> <pre><code>% weectl extension uninstall windy\nRequest to remove extension 'windy'\nFinished removing extension 'windy'\n</code></pre>",
             "title": "Examples"
         },
         {
             "location": "utilities/weectl-station/",
-            "text": "<p>Use the <code>weectl</code> subcommand <code>station</code> to manage the user data for a station, including its configuration file</p> <p>Specify <code>--help</code> to see the actions and options.</p> <p>In the documentation that follows,  the exact output will depend on your operating system and username. What is shown below is for Linux and user <code>tkeffer</code>.</p>",
+            "text": "<p>Use the <code>weectl</code> subcommand <code>station</code> to manage the user data for a station, including its configuration file.</p> <p>Specify <code>--help</code> to see the actions and options.</p> <p>In the documentation that follows,  the exact output will depend on your operating system and username. What is shown below is for Linux and user <code>tkeffer</code>.</p>",
             "title": "weectl station"
         },
         {
-            "location": "utilities/weectl-station/#create-a-new-user-data-aera",
-            "text": "<pre><code>weectl station create\n    [--dist-config=DIST-CONFIG-PATH]\n    [--driver=DRIVER]\n    [--location=LOCATION]\n    [--altitude=ALTITUDE,(foot|meter)]\n    [--latitude=LATITUDE] [--longitude=LONGITUDE]\n    [--register=(y,n) [--station-url=STATION_URL]]\n    [--units=(us|metricwx|metric)]\n    [--skin-root=SKIN_ROOT]\n    [--sqlite-root=SQLITE_ROOT]\n    [--html-root=HTML_ROOT]\n    [--user-root=USER_ROOT]\n    [--docs-root=DOCS_ROOT]\n    [--examples-root=EXAMPLES_ROOT]\n    [--no-prompt]\n    [--config=CONFIG-PATH]\n    [--dry-run]\n</code></pre> <p>This action will create a new area for user data. After the command completes, the area will include</p> <ul> <li>A configuration file, <code>weewx.conf</code>;</li> <li>Documentation;</li> <li>Examples;</li> <li>Utility files; and</li> <li>Skins.</li> </ul> <p><code>weectl station create</code> is typically used when installing using pip, or when you want to create multiple stations.</p>",
-            "title": "Create a new user data aera"
+            "location": "utilities/weectl-station/#create-a-new-user-data-area",
+            "text": "<pre><code>weectl station create\n    [--driver=DRIVER]\n    [--location=LOCATION]\n    [--altitude=ALTITUDE,(foot|meter)]\n    [--latitude=LATITUDE] [--longitude=LONGITUDE]\n    [--register=(y,n) [--station-url=STATION_URL]]\n    [--units=(us|metricwx|metric)]\n    [--skin-root=SKIN_ROOT]\n    [--sqlite-root=SQLITE_ROOT]\n    [--html-root=HTML_ROOT]\n    [--user-root=USER_ROOT]\n    [--docs-root=DOCS_ROOT]\n    [--examples-root=EXAMPLES_ROOT]\n    [--no-prompt]\n    [--config=CONFIG-PATH]\n    [--dist-config=DIST-CONFIG-PATH]\n    [--dry-run]\n</code></pre> <p>This action will create a new area for user data. After the command completes, the area will include</p> <ul> <li>A configuration file, <code>weewx.conf</code>;</li> <li>Documentation;</li> <li>Examples;</li> <li>Utility files; and</li> <li>Skins.</li> </ul> <p><code>weectl station create</code> is typically used when installing using pip, or when you want to create multiple stations.</p>",
+            "title": "Create a new user data area"
+        },
+        {
+            "location": "utilities/weectl-station/#create-user-data-with-prompting",
+            "text": "<p>If invoked without any options, <code>weectl station create</code> will prompt you for various settings, such as the type of hardware you are using, the station altitude and location, etc. This is what most users will want.</p>",
+            "title": "Create user data with prompting"
+        },
+        {
+            "location": "utilities/weectl-station/#create-user-data-without-prompting",
+            "text": "<p>A new user data area can be created without prompting by using option <code>--no-prompt</code>. This is most useful when creating a station with an automated script. For example,</p> <pre><code>weectl station create --no-prompt --driver=weewx.drivers.vantage \\\n    --altitude=\"400,foot\" --latitude=45.1 --longitude=-105.9 \\ \n    --location=\"My Special Station\"\n</code></pre> <p>will create a station with the indicated values. If a value is not specified, a default will be used.</p> <p>See the section Common options for details of the various options.</p>",
+            "title": "Create user data without prompting"
+        },
+        {
+            "location": "utilities/weectl-station/#reconfigure-an-existing-station",
+            "text": "<pre><code>weectl station reconfigure\n    [--driver=DRIVER]\n    [--location=LOCATION]\n    [--altitude=ALTITUDE,(foot|meter)]\n    [--latitude=LATITUDE] [--longitude=LONGITUDE]\n    [--register=(y,n) [--station-url=STATION_URL]]\n    [--units=(us|metricwx|metric)]\n    [--skin-root=SKIN_ROOT]\n    [--sqlite-root=SQLITE_ROOT]\n    [--html-root=HTML_ROOT]\n    [--no-backup]\n    [--no-prompt]\n    [--config=CONFIG-PATH] \n    [--dry-run]\n</code></pre> <p>This action will reconfigure the contents of an existing configuration file (generally named <code>weewx.conf</code>). </p> <p>It is often used for changing drivers.</p>",
+            "title": "Reconfigure an existing station"
+        },
+        {
+            "location": "utilities/weectl-station/#reconfigure-with-prompting",
+            "text": "<p>If invoked without the <code>--no-prompt</code> option, <code>weectl station reconfigure</code> will prompt you for new settings.</p>",
+            "title": "Reconfigure with prompting"
+        },
+        {
+            "location": "utilities/weectl-station/#reconfigure-without-prompting",
+            "text": "<p>If the option <code>--no-prompt</code> is specified, <code>weectl station reconfigure</code> will reconfigure the configuration file using whatever options you've specified on the command line.</p> <p>For example, to keep all settings, but change to the Vantage driver you would use</p> <pre><code>weectl station reconfigure --no-prompt --driver=weewx.drivers.vantage\n</code></pre>",
+            "title": "Reconfigure without prompting"
+        },
+        {
+            "location": "utilities/weectl-station/#upgrade-an-existing-station",
+            "text": "<pre><code>weectl station upgrade\n    [--docs-root=DOCS_ROOT]\n    [--examples-root=EXAMPLES_ROOT]\n    [--skin-root=SKIN_ROOT]\n    [--what (config|docs|examples|util|skins)...]\n    [--no-backup]\n    [--no-prompt]\n    [--config=CONFIG-PATH]\n    [--dist-config=DIST-CONFIG-PATH]]\n    [--dry-run]\n</code></pre> <p>If you installed using pip, then do an upgrade using pip, it will only upgrade the code base. It does not touch the user data area. Use this action to upgrade all or part of the user data area.</p> <p>It can also be useful for upgrading a package install. While these generally </p>",
+            "title": "Upgrade an existing station"
+        },
+        {
+            "location": "utilities/weectl-station/#-what",
+            "text": "<p>By default, <code>weectl station upgrade</code> will upgrade the configuration file, documentation, examples, and utility files. However, you can customize exactly what gets upgraded.</p> <p>Note</p> <p>The <code>--what</code> option does not take an equal sign (<code>=</code>). Just list the desired things to be upgraded, without commas between them.</p> <p>For example, to upgrade the configuration file and skins only, you would specify</p> <pre><code>weectl station upgrade --what config skins\n</code></pre>",
+            "title": "--what"
+        },
+        {
+            "location": "utilities/weectl-station/#common-options",
+            "text": "<p>In what follows, <code>WEEWX_ROOT</code> is the directory holding the configuration file. For a pip install, this is typically <code>~/weewx-data/</code>. For package installs, it is usually <code>/etc/weewx/</code>.</p>",
+            "title": "Common options"
         },
         {
             "location": "utilities/weectl-station/#-driverdriver",
-            "text": "<p>Which driver to use. Default is <code>simulator</code>.</p>",
+            "text": "<p>Which driver to use. Default is <code>weewx.drivers.simulator</code>.</p>",
             "title": "--driver=DRIVER"
         },
         {
             "location": "utilities/weectl-station/#-locationlocation",
-            "text": "<p>A description of your station, such as <code>--location=\"A small town in Rongovia\"</code></p>",
+            "text": "<p>A description of your station, such as <code>--location=\"A small town in Rongovia\"</code> Default is <code>WeeWX</code>.</p>",
             "title": "--location=LOCATION"
         },
         {
             "location": "utilities/weectl-station/#-altitudealtitude",
-            "text": "<p>The altitude of your station, along with the unit it is measured in. For example, <code>--altitude=50,meter</code>. Note that the unit is measured in the singular (<code>foot</code>, not <code>feet</code>).</p>",
+            "text": "<p>The altitude of your station, along with the unit it is measured in. For example, <code>--altitude=50,meter</code>. Note that the unit is measured in the singular (<code>foot</code>, not <code>feet</code>). Default is <code>\"0,foot\"</code>.</p>",
             "title": "--altitude=ALTITUDE"
         },
         {
             "location": "utilities/weectl-station/#-latitudelatitude",
-            "text": "<p>The station latitude in decimal degrees. Negative for the southern hemisphere.</p>",
+            "text": "<p>The station latitude in decimal degrees. Negative for the southern hemisphere. Default is <code>0</code>.</p>",
             "title": "--latitude=LATITUDE"
         },
         {
             "location": "utilities/weectl-station/#-longitudelongitude",
-            "text": "<p>The station longitude in decimal degrees. Negative for the western hemisphere.</p>",
+            "text": "<p>The station longitude in decimal degrees. Negative for the western hemisphere. Default is <code>0</code>.</p>",
             "title": "--longitude=LONGITUDE"
         },
         {
             "location": "utilities/weectl-station/#-registeryn",
-            "text": "<p>Whether to include the station in the WeeWX registry and map. If you set <code>--register</code>, you must also specify a unique URL for your station with option <code>--station-url</code>.</p>",
+            "text": "<p>Whether to include the station in the WeeWX registry and map. If you choose to register your station, you must also specify a unique URL for your station with option <code>--station-url</code>. Default is <code>n</code> (do not register).</p>",
             "title": "--register={y|n}"
         },
         {
             "location": "utilities/weectl-station/#-station-urlurl",
-            "text": "<p>A unique URL for your station.</p> <p>Example: <code>--station-url=https://www.wunderground.com/dashboard/pws/KNDPETE15</code>.</p>",
+            "text": "<p>A unique URL for your station.</p> <p>Example: <code>--station-url=https://www.wunderground.com/dashboard/pws/KNDPETE15</code>. No default.</p>",
             "title": "--station-url=URL"
         },
         {
             "location": "utilities/weectl-station/#-unitsunit_system",
-            "text": "<p>What units to use for your reports. Options are <code>us</code>, <code>metricwx</code>, or <code>metric</code>. See the Appendix Units for details.</p>",
+            "text": "<p>What units to use for your reports. Options are <code>us</code>, <code>metricwx</code>, or <code>metric</code>. See the Appendix Units for details. Default is <code>us</code>.</p>",
             "title": "--units=UNIT_SYSTEM"
         },
         {
-            "location": "utilities/weectl-station/#-no-prompt",
-            "text": "<p>Generally, the utility will prompt for values unless <code>--no-prompt</code> has been set. With <code>--no-prompt</code>, the values to be used are the default values, replaced with whatever options have been set on the command line. For example,</p> <pre><code>weectl station create --driver='weewx.drivers.vantage' --no-prompt\n</code></pre> <p>will cause the defaults to be used for all values except <code>--driver</code>, which will use the Vantage driver.</p>",
-            "title": "--no-prompt"
+            "location": "utilities/weectl-station/#-skin-rootskin_root",
+            "text": "<p>The location of the directory holding the skins relative to <code>WEEWX_ROOT</code>. Of course, like any other path, if the option starts with a slash (<code>/</code>), it becomes an absolute path. Default is <code>skins</code>.</p>",
+            "title": "--skin-root=SKIN_ROOT"
         },
         {
-            "location": "utilities/weectl-station/#-configfilename",
-            "text": "<p>Path to the configuration file to be created. The directory of the path will become the value for <code>WEEWX_ROOT</code> in the configuration file. Default is <code>~/weewx-data/weewx.conf</code>.</p>",
-            "title": "--config=FILENAME"
+            "location": "utilities/weectl-station/#-sqlite-rootsqlite_root",
+            "text": "<p>The location of the directory holding the SQLite database relative to <code>WEEWX_ROOT</code>. Of course, like any other path, if the option starts with a slash (<code>/</code>), it becomes an absolute path. Default is <code>skins</code>.</p>",
+            "title": "--sqlite-root=SQLITE_ROOT"
         },
         {
-            "location": "utilities/weectl-station/#-dry-run",
-            "text": "<p>With option <code>--dry-run</code> you can test what <code>weect station create</code> would do without actually doing it. It will print out the steps, but not actually write anything.</p>",
-            "title": "--dry-run"
+            "location": "utilities/weectl-station/#-html-roothtml_root",
+            "text": "<p>Where generated HTML files should be placed, relative to <code>WEEWX_ROOT</code>.  Of course, like any other path, if the option starts with a slash (<code>/</code>), it becomes an absolute path. Default is <code>public_html</code>.</p>",
+            "title": "--html-root=HTML_ROOT"
         },
         {
-            "location": "utilities/weectl-station/#root-options",
-            "text": "<p>\"Root options\" include</p> <p><code>--skin-root</code> <code>--sqlite-root</code> <code>--html-root</code> <code>--user-root</code> <code>--docs-root</code> <code>--examples-root</code></p> <p>All of these root options are relative to <code>WEEWX_ROOT</code>. Of course, like any other path, if the option starts with a slash (<code>/</code>), it becomes an absolute path. So, for example,</p> <pre><code>--html-root=/var/www/html\n</code></pre> <p>will cause HTML files to be put in the traditional system WWW directory <code>/var/www/html</code>.</p>",
-            "title": "root options"
+            "location": "utilities/weectl-station/#-user-rootuser_root",
+            "text": "<p>Where user extensions can be found, relative to <code>WEEWX_ROOT</code>. Of course, like any other path, if the option starts with a slash (<code>/</code>), it becomes an absolute path. Default is <code>bin/user</code>.</p>",
+            "title": "--user-root=USER_ROOT"
         },
         {
-            "location": "utilities/weectl-station/#weectl-station-reconfigure",
-            "text": "<p>This action will reconfigure the contents of the configuration file <code>weewx.conf</code>. Unless option <code>--no-prompt</code> has been specified, it will prompt you for each setting, using the previous settings as default values, and give you a chance to change them. </p> <p>Specify <code>--help</code> to see the options: <pre><code>weectl station reconfigure  --help\n</code></pre> <pre><code>usage: weectl station reconfigure [--config=CONFIG-PATH] \n                                  [--driver=DRIVER]\n                                  [--location=LOCATION]\n                                  [--altitude=ALTITUDE,{foot|meter}]\n                                  [--latitude=LATITUDE] [--longitude=LONGITUDE]\n                                  [--register={y,n} [--station-url=STATION_URL]]\n                                  [--units={us,metricwx,metric}]\n                                  [--skin-root=SKIN_ROOT]\n                                  [--sqlite-root=SQLITE_ROOT]\n                                  [--html-root=HTML_ROOT]\n                                  [--no-prompt]\n                                  [--no-backup]\n                                  [--dry-run]\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --config CONFIG-PATH  Path to configuration file. Default is\n                        \"/home/tkeffer/weewx-data/weewx.conf\"\n  --driver DRIVER       Driver to use. Default is \"weewx.drivers.simulator\".\n  --location LOCATION   A description of the station. This will be used for\n                        report titles. Default is \"WeeWX\".\n  --altitude ALTITUDE,{foot|meter}\n                        The station altitude in either feet or meters. For\n                        example, \"750,foot\" or \"320,meter\". Default is \"0,\n                        foot\".\n  --latitude LATITUDE   The station latitude in decimal degrees. Default is\n                        \"0.00\".\n  --longitude LONGITUDE\n                        The station longitude in decimal degrees. Default is\n                        \"0.00\".\n  --register {y,n}      Register this station in the weewx registry? Default\n                        is \"n\" (do not register).\n  --station-url STATION_URL\n                        Unique URL to be used if registering the station.\n                        Required if the station is to be registered.\n  --units {us,metricwx,metric}\n                        Set display units to us, metricwx, or metric. Default\n                        is \"us\".\n  --skin-root SKIN_ROOT\n                        Where to put the skins, relatve to WEEWX_ROOT. Default\n                        is \"skins\".\n  --sqlite-root SQLITE_ROOT\n                        Where to put the SQLite database, relative to\n                        WEEWX_ROOT. Default is \"archive\".\n  --html-root HTML_ROOT\n                        Where to put the generated HTML and images, relative\n                        to WEEWX_ROOT. Default is \"public_html\".\n  --no-prompt           Do not prompt. Use default values.\n  --no-backup           Do not backup the old configuration file.\n  --dry-run             Print what would happen, but do not actually do it.\n</code></pre></p>",
-            "title": "weectl station reconfigure"
+            "location": "utilities/weectl-station/#-docs-rootdocs_root",
+            "text": "<p>Where the WeeWX documentation can be found, relative to <code>WEEWX_ROOT</code>. Of course, like any other path, if the option starts with a slash (<code>/</code>), it becomes an absolute path. Default is <code>docs</code>.</p>",
+            "title": "--docs-root=DOCS_ROOT"
         },
         {
-            "location": "utilities/weectl-station/#-configfilename_1",
-            "text": "<p>Path to the configuration file to be updated. The directory of the path will become the value for <code>WEEWX_ROOT</code> in the configuration file. Default is <code>~/weewx-data/weewx.conf</code>.</p>",
-            "title": "--config=FILENAME"
-        },
-        {
-            "location": "utilities/weectl-station/#-no-prompt_1",
-            "text": "<p>When used with the <code>--no-prompt</code> option, <code>weectl station reconfigure</code> will modify specific parameters with no interaction. For example, this would set the station altitude to 35 feet:</p> <pre><code>weectl station reconfigure --altitude=35,foot --no-prompt\n</code></pre> <p>This would change the driver to a user-installed netatmo driver:</p> <pre><code>weectl station reconfigure --driver=user.netatmo --no-prompt\n</code></pre>",
-            "title": "--no-prompt"
-        },
-        {
-            "location": "utilities/weectl-station/#-dry-run_1",
-            "text": "<p>With option <code>--dry-run</code> you can test what <code>weect station create</code> would do without actually doing it. It will print out the steps, but not actually write anything.</p>",
-            "title": "--dry-run"
+            "location": "utilities/weectl-station/#-examples-rootexamples_root",
+            "text": "<p>Where the WeeWX examples can be found, relative to <code>WEEWX_ROOT</code>. Of course, like any other path, if the option starts with a slash (<code>/</code>), it becomes an absolute path. Default is <code>examples</code>.</p>",
+            "title": "--examples-root=EXAMPLES_ROOT"
         },
         {
             "location": "utilities/weectl-station/#-no-backup",
-            "text": "<p>Do not create a copy of the previous configuration file.</p> <p>Other options are as described in the <code>weectl station create</code> section.</p>",
+            "text": "<p>Generally, if <code>weectl station</code> changes your configuration file, it will save a timestamped version of your original configuration file. If you specify <code>--no-backup</code>, then it will not save a copy.</p>",
             "title": "--no-backup"
         },
         {
-            "location": "utilities/weectl-station/#weectl-station-upgrade",
-            "text": "<p>This action can upgrade the configuration file, documentation, examples, daemon utility files, and skins.  When you upgrade the WeeWX software, that process does not modify existing configurations or skins.  In most cases, the WeeWX developers will maintain backward-compatibility, so older configurations and skins will continue to work with new WeeWX updates. However, if you want to get new features, you might have to update your configurations or skins.  Use this utility to do that.</p> <p>Specify <code>--help</code> to see the options: <pre><code>weectl station upgrade --help\n</code></pre> <pre><code>usage: weectl station upgrade [--config=CONFIG-PATH]\n                              [--dist-config=DIST-CONFIG-PATH]]\n                              [--docs-root=DOCS_ROOT]\n                              [--examples-root=EXAMPLES_ROOT]\n                              [--skin-root=SKIN_ROOT]\n                              [--what [{config,docs,examples,util,skins} ... ]\n                              [--no-prompt]\n                              [--no-backup]\n                              [--dry-run]\n\nUpgrade an existing user data area, including any combination of the\nconfiguration file, docs, examples, daemon utility files, and skins. In what\nfollows, WEEWX_ROOT is the directory that contains the configuration\nfile. For example, if \"--config=/home/tkeffer/weewx-data/weewx.conf\", then\nWEEWX_ROOT will be \"/home/tkeffer/weewx-data\".\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --config CONFIG-PATH  Path to configuration file. Default is\n                        \"/home/tkeffer/weewx-data/weewx.conf\"\n  --dist-config DIST-CONFIG-PATH\n                        Use configuration file DIST-CONFIG-PATH as the new\n                        configuration file. Default is to retrieve it from\n                        package resources. The average user is unlikely to\n                        need this option.\n  --docs-root DOCS_ROOT\n                        Where to put the new documentation, relative to\n                        WEEWX_ROOT. Default is \"docs\".\n  --examples-root EXAMPLES_ROOT\n                        Where to put the new examples, relative to WEEWX_ROOT.\n                        Default is \"examples\".\n  --skin-root SKIN_ROOT\n                        Where to put the skins, relative to WEEWX_ROOT.\n                        Default is \"skins\".\n  --what {config,docs,examples,util,skins} [{config,docs,examples,util,skins} ...]\n                        What to upgrade. Default is to upgrade the\n                        configuration file, documentation, examples, and\n                        daemon utility files.\n  --no-prompt           Do not prompt. Use default values.\n  --no-backup           Do not backup the old configuration file.\n  --dry-run             Print what would happen, but do not actually do it.\n</code></pre></p>",
-            "title": "weectl station upgrade"
+            "location": "utilities/weectl-station/#-no-prompt",
+            "text": "<p>Generally, the utility will prompt for values unless <code>--no-prompt</code> has been set. With <code>--no-prompt</code>, the values to be used are the default values, replaced with whatever options have been set on the command line. For example,</p> <pre><code>weectl station create --driver='weewx.drivers.vantage' --no-prompt\n</code></pre> <p>will cause the defaults to be used for all values except <code>--driver</code>, which will use the Vantage driver.</p>",
+            "title": "--no-prompt"
         },
         {
-            "location": "utilities/weectl-station/#-configfilename_2",
-            "text": "<p>Path to the configuration file to be updated. The directory of the path will become the value for <code>WEEWX_ROOT</code> in the configuration file. Default is <code>~/weewx-data/weewx.conf</code>.</p>",
+            "location": "utilities/weectl-station/#-configfilename",
+            "text": "<p>Path to the configuration file to be created. The directory of the path will become the value for <code>WEEWX_ROOT</code> in the configuration file. Default is <code>~/weewx-data/weewx.conf</code>.</p>",
             "title": "--config=FILENAME"
         },
         {
-            "location": "utilities/weectl-station/#-what",
-            "text": "<p>By default, <code>weectl station upgrade</code> will upgrade the configuration file, documentation, examples, and daemon utility files. However, you can customize exactly what gets upgraded. </p> <p>Note</p> <p>The <code>--what</code> option does not take an equal sign (<code>=</code>). Just list the desired things to be upgraded, without commas between them.</p> <p>For example, to upgrade the configuration file and skins only, you would specify</p> <pre><code>weectl station upgrade --what config skins\n</code></pre>",
-            "title": "--what"
-        },
-        {
-            "location": "utilities/weectl-station/#root-options_1",
-            "text": "<p>\"Root options\" include</p> <p><code>--skin-root</code> <code>--docs-root</code> <code>--examples-root</code></p> <p>All of these root options are relative to <code>WEEWX_ROOT</code>. Of course, like any other path, if the option starts with a slash (<code>/</code>), it becomes an absolute path. So, for example,</p> <pre><code>--docs-root=/usr/local/doc/weewx\n</code></pre> <p>will cause documentation files to be put in <code>/usr/local/doc/weewx</code>.</p>",
-            "title": "root options"
+            "location": "utilities/weectl-station/#-dry-run",
+            "text": "<p>With option <code>--dry-run</code> you can test what <code>weect station</code> would do without actually doing it. It will print out the steps, but not actually write anything.</p>",
+            "title": "--dry-run"
         },
         {
             "location": "utilities/weewxd/",
             "text": "<p>The <code>weewxd</code> application is the heart of WeeWX.  It collects data from hardware, processes the data, archives the data, then generates reports from the data.</p> <p>It can be run directly, or in the background as a daemon.  When it is run directly, <code>weewxd</code> emits LOOP and ARCHIVE data to stdout.</p> <p>Specify <code>--help</code> to see how it is used: <pre><code>weewxd --help\n</code></pre> <pre><code>Usage: weewxd --help\n       weewxd --version\n       weewxd config_file [--daemon] [--pidfile=PIDFILE] \n                          [--exit]   [--loop-on-init]\n                          [--log-label=LABEL]\n\n  Entry point to the weewx weather program. Can be run directly, or as a daemon\n  by specifying the '--daemon' option.\n\nArguments:\n    config_file: The weewx configuration file to be used.\n\n\nOptions:\n  -h, --help            show this help message and exit\n  -d, --daemon          Run as a daemon\n  -p PIDFILE, --pidfile=PIDFILE\n                        Store the process ID in PIDFILE\n  -v, --version         Display version number then exit\n  -x, --exit            Exit on I/O and database errors instead of restarting\n  -r, --loop-on-init    Retry forever if device is not ready on startup\n  -n LABEL, --log-label=LABEL\n                        Label to use in syslog entries\n</code></pre></p>",
             "title": "weewxd"
         }
     ]
```

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/sitemap.xml` & `weewx-5.0.0b9/bin/wee_resources/docs/sitemap.xml`

 * *Files 8% similar despite different names*

#### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/sitemap.xml` & `weewx-5.0.0b9/bin/wee_resources/docs/sitemap.xml`

```diff
@@ -1,383 +1,383 @@
 <?xml version="1.0" encoding="utf-8"?>
 <urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
   <url>
     <loc>https://www.weewx.com/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/changes/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/copyright/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/devnotes/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/sle/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/versions/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/appendix/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/cheetah/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/custom-reports/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/database/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/derived/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/drivers/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/extensions/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/image-generator/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/localization/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/multiple-bindings/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/report-options/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/report-scheduling/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/service-engine/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/custom/units/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/hardware/acurite/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/hardware/cc3000/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/hardware/drivers/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/hardware/fousb/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/hardware/te923/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/hardware/ultimeter/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/hardware/vantage/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/hardware/wmr100/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/hardware/wmr300/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/hardware/wmr9x8/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/hardware/ws1/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/hardware/ws23xx/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/hardware/ws28xx/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/quickstarts/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/quickstarts/debian/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/quickstarts/git/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/quickstarts/pip/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/quickstarts/redhat/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/quickstarts/suse/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/backing-up-weewx/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/installing-weewx/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/mysql-mariadb-config/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/running-weewx/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/system-requirements/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/webserver-integration/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/where/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/troubleshooting/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/troubleshooting/hardware/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/troubleshooting/meteo/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/troubleshooting/software/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/data-bindings/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/databases/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/databasetypes/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/engine/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/general/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/stations-config/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/stdarchive/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/stdcalibrate-config/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/stdconvert-config/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/stdqc-config/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/stdreport-config/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/stdrestful-config/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/stdtimesynch/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/usersguide/weewx-config-file/stdwxcalculate-config/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/utilities/wee_database/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/utilities/wee_debug/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/utilities/wee_device/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/utilities/wee_import/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/utilities/wee_reports/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/utilities/weectl-database/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/utilities/weectl-extension/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/utilities/weectl-station/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://www.weewx.com/utilities/weewxd/</loc>
-    <lastmod>2023-07-11</lastmod>
+    <lastmod>2023-07-14</lastmod>
     <changefreq>daily</changefreq>
   </url>
 </urlset>
```

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/sle/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/sle/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/backing-up-weewx/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/backing-up-weewx/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/installing-weewx/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/installing-weewx/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/mysql-mariadb-config/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/mysql-mariadb-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/running-weewx/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/running-weewx/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/system-requirements/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/system-requirements/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/troubleshooting/hardware/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/troubleshooting/hardware/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/troubleshooting/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/troubleshooting/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/troubleshooting/meteo/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/troubleshooting/meteo/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/troubleshooting/software/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/troubleshooting/software/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/webserver-integration/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/webserver-integration/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/data-bindings/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/data-bindings/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/databases/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/databases/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/databasetypes/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/databasetypes/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/engine/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/engine/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/general/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/general/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/stations-config/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/stations-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/stdarchive/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/stdarchive/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/stdcalibrate-config/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/stdcalibrate-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/stdconvert-config/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/stdconvert-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/stdqc-config/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/stdqc-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/stdreport-config/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/stdreport-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/stdrestful-config/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/stdrestful-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/stdtimesynch/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/stdtimesynch/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/weewx-config-file/stdwxcalculate-config/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/weewx-config-file/stdwxcalculate-config/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/usersguide/where/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/usersguide/where/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/utilities/wee_database/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/utilities/wee_database/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/utilities/wee_debug/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/utilities/wee_debug/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/utilities/wee_device/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/utilities/wee_device/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/utilities/wee_import/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/utilities/wee_import/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/utilities/wee_reports/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/utilities/wee_reports/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/utilities/weectl-database/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/utilities/weectl-database/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/utilities/weectl-extension/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/utilities/weectl-extension/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/utilities/weectl-station/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/utilities/weectl-station/index.html`

 * *Files 13% similar despite different names*

```diff
@@ -1289,19 +1289,93 @@
     <label class="md-nav__title" for="__toc">
       <span class="md-nav__icon md-icon"></span>
       Table of contents
     </label>
     <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
       
         <li class="md-nav__item">
-  <a href="#create-a-new-user-data-aera" class="md-nav__link">
-    Create a new user data aera
+  <a href="#create-a-new-user-data-area" class="md-nav__link">
+    Create a new user data area
   </a>
   
-    <nav class="md-nav" aria-label="Create a new user data aera">
+    <nav class="md-nav" aria-label="Create a new user data area">
+      <ul class="md-nav__list">
+        
+          <li class="md-nav__item">
+  <a href="#create-user-data-with-prompting" class="md-nav__link">
+    Create user data with prompting
+  </a>
+  
+</li>
+        
+          <li class="md-nav__item">
+  <a href="#create-user-data-without-prompting" class="md-nav__link">
+    Create user data without prompting
+  </a>
+  
+</li>
+        
+      </ul>
+    </nav>
+  
+</li>
+      
+        <li class="md-nav__item">
+  <a href="#reconfigure-an-existing-station" class="md-nav__link">
+    Reconfigure an existing station
+  </a>
+  
+    <nav class="md-nav" aria-label="Reconfigure an existing station">
+      <ul class="md-nav__list">
+        
+          <li class="md-nav__item">
+  <a href="#reconfigure-with-prompting" class="md-nav__link">
+    Reconfigure with prompting
+  </a>
+  
+</li>
+        
+          <li class="md-nav__item">
+  <a href="#reconfigure-without-prompting" class="md-nav__link">
+    Reconfigure without prompting
+  </a>
+  
+</li>
+        
+      </ul>
+    </nav>
+  
+</li>
+      
+        <li class="md-nav__item">
+  <a href="#upgrade-an-existing-station" class="md-nav__link">
+    Upgrade an existing station
+  </a>
+  
+    <nav class="md-nav" aria-label="Upgrade an existing station">
+      <ul class="md-nav__list">
+        
+          <li class="md-nav__item">
+  <a href="#-what" class="md-nav__link">
+    --what
+  </a>
+  
+</li>
+        
+      </ul>
+    </nav>
+  
+</li>
+      
+        <li class="md-nav__item">
+  <a href="#common-options" class="md-nav__link">
+    Common options
+  </a>
+  
+    <nav class="md-nav" aria-label="Common options">
       <ul class="md-nav__list">
         
           <li class="md-nav__item">
   <a href="#-driverdriver" class="md-nav__link">
     --driver=DRIVER
   </a>
   
@@ -1353,112 +1427,79 @@
   <a href="#-unitsunit_system" class="md-nav__link">
     --units=UNIT_SYSTEM
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#-no-prompt" class="md-nav__link">
-    --no-prompt
+  <a href="#-skin-rootskin_root" class="md-nav__link">
+    --skin-root=SKIN_ROOT
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#-configfilename" class="md-nav__link">
-    --config=FILENAME
+  <a href="#-sqlite-rootsqlite_root" class="md-nav__link">
+    --sqlite-root=SQLITE_ROOT
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#-dry-run" class="md-nav__link">
-    --dry-run
+  <a href="#-html-roothtml_root" class="md-nav__link">
+    --html-root=HTML_ROOT
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#root-options" class="md-nav__link">
-    root options
+  <a href="#-user-rootuser_root" class="md-nav__link">
+    --user-root=USER_ROOT
   </a>
   
 </li>
         
-      </ul>
-    </nav>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#weectl-station-reconfigure" class="md-nav__link">
-    weectl station reconfigure
-  </a>
-  
-    <nav class="md-nav" aria-label="weectl station reconfigure">
-      <ul class="md-nav__list">
-        
           <li class="md-nav__item">
-  <a href="#-configfilename_1" class="md-nav__link">
-    --config=FILENAME
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#-no-prompt_1" class="md-nav__link">
-    --no-prompt
+  <a href="#-docs-rootdocs_root" class="md-nav__link">
+    --docs-root=DOCS_ROOT
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#-dry-run_1" class="md-nav__link">
-    --dry-run
+  <a href="#-examples-rootexamples_root" class="md-nav__link">
+    --examples-root=EXAMPLES_ROOT
   </a>
   
 </li>
         
           <li class="md-nav__item">
   <a href="#-no-backup" class="md-nav__link">
     --no-backup
   </a>
   
 </li>
         
-      </ul>
-    </nav>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#weectl-station-upgrade" class="md-nav__link">
-    weectl station upgrade
-  </a>
-  
-    <nav class="md-nav" aria-label="weectl station upgrade">
-      <ul class="md-nav__list">
-        
           <li class="md-nav__item">
-  <a href="#-configfilename_2" class="md-nav__link">
-    --config=FILENAME
+  <a href="#-no-prompt" class="md-nav__link">
+    --no-prompt
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#-what" class="md-nav__link">
-    --what
+  <a href="#-configfilename" class="md-nav__link">
+    --config=FILENAME
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#root-options_1" class="md-nav__link">
-    root options
+  <a href="#-dry-run" class="md-nav__link">
+    --dry-run
   </a>
   
 </li>
         
       </ul>
     </nav>
   
@@ -1897,19 +1938,93 @@
     <label class="md-nav__title" for="__toc">
       <span class="md-nav__icon md-icon"></span>
       Table of contents
     </label>
     <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
       
         <li class="md-nav__item">
-  <a href="#create-a-new-user-data-aera" class="md-nav__link">
-    Create a new user data aera
+  <a href="#create-a-new-user-data-area" class="md-nav__link">
+    Create a new user data area
+  </a>
+  
+    <nav class="md-nav" aria-label="Create a new user data area">
+      <ul class="md-nav__list">
+        
+          <li class="md-nav__item">
+  <a href="#create-user-data-with-prompting" class="md-nav__link">
+    Create user data with prompting
+  </a>
+  
+</li>
+        
+          <li class="md-nav__item">
+  <a href="#create-user-data-without-prompting" class="md-nav__link">
+    Create user data without prompting
+  </a>
+  
+</li>
+        
+      </ul>
+    </nav>
+  
+</li>
+      
+        <li class="md-nav__item">
+  <a href="#reconfigure-an-existing-station" class="md-nav__link">
+    Reconfigure an existing station
   </a>
   
-    <nav class="md-nav" aria-label="Create a new user data aera">
+    <nav class="md-nav" aria-label="Reconfigure an existing station">
+      <ul class="md-nav__list">
+        
+          <li class="md-nav__item">
+  <a href="#reconfigure-with-prompting" class="md-nav__link">
+    Reconfigure with prompting
+  </a>
+  
+</li>
+        
+          <li class="md-nav__item">
+  <a href="#reconfigure-without-prompting" class="md-nav__link">
+    Reconfigure without prompting
+  </a>
+  
+</li>
+        
+      </ul>
+    </nav>
+  
+</li>
+      
+        <li class="md-nav__item">
+  <a href="#upgrade-an-existing-station" class="md-nav__link">
+    Upgrade an existing station
+  </a>
+  
+    <nav class="md-nav" aria-label="Upgrade an existing station">
+      <ul class="md-nav__list">
+        
+          <li class="md-nav__item">
+  <a href="#-what" class="md-nav__link">
+    --what
+  </a>
+  
+</li>
+        
+      </ul>
+    </nav>
+  
+</li>
+      
+        <li class="md-nav__item">
+  <a href="#common-options" class="md-nav__link">
+    Common options
+  </a>
+  
+    <nav class="md-nav" aria-label="Common options">
       <ul class="md-nav__list">
         
           <li class="md-nav__item">
   <a href="#-driverdriver" class="md-nav__link">
     --driver=DRIVER
   </a>
   
@@ -1961,112 +2076,79 @@
   <a href="#-unitsunit_system" class="md-nav__link">
     --units=UNIT_SYSTEM
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#-no-prompt" class="md-nav__link">
-    --no-prompt
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#-configfilename" class="md-nav__link">
-    --config=FILENAME
+  <a href="#-skin-rootskin_root" class="md-nav__link">
+    --skin-root=SKIN_ROOT
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#-dry-run" class="md-nav__link">
-    --dry-run
+  <a href="#-sqlite-rootsqlite_root" class="md-nav__link">
+    --sqlite-root=SQLITE_ROOT
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#root-options" class="md-nav__link">
-    root options
+  <a href="#-html-roothtml_root" class="md-nav__link">
+    --html-root=HTML_ROOT
   </a>
   
 </li>
         
-      </ul>
-    </nav>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#weectl-station-reconfigure" class="md-nav__link">
-    weectl station reconfigure
-  </a>
-  
-    <nav class="md-nav" aria-label="weectl station reconfigure">
-      <ul class="md-nav__list">
-        
           <li class="md-nav__item">
-  <a href="#-configfilename_1" class="md-nav__link">
-    --config=FILENAME
+  <a href="#-user-rootuser_root" class="md-nav__link">
+    --user-root=USER_ROOT
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#-no-prompt_1" class="md-nav__link">
-    --no-prompt
+  <a href="#-docs-rootdocs_root" class="md-nav__link">
+    --docs-root=DOCS_ROOT
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#-dry-run_1" class="md-nav__link">
-    --dry-run
+  <a href="#-examples-rootexamples_root" class="md-nav__link">
+    --examples-root=EXAMPLES_ROOT
   </a>
   
 </li>
         
           <li class="md-nav__item">
   <a href="#-no-backup" class="md-nav__link">
     --no-backup
   </a>
   
 </li>
         
-      </ul>
-    </nav>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#weectl-station-upgrade" class="md-nav__link">
-    weectl station upgrade
-  </a>
-  
-    <nav class="md-nav" aria-label="weectl station upgrade">
-      <ul class="md-nav__list">
-        
           <li class="md-nav__item">
-  <a href="#-configfilename_2" class="md-nav__link">
-    --config=FILENAME
+  <a href="#-no-prompt" class="md-nav__link">
+    --no-prompt
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#-what" class="md-nav__link">
-    --what
+  <a href="#-configfilename" class="md-nav__link">
+    --config=FILENAME
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#root-options_1" class="md-nav__link">
-    root options
+  <a href="#-dry-run" class="md-nav__link">
+    --dry-run
   </a>
   
 </li>
         
       </ul>
     </nav>
   
@@ -2085,262 +2167,186 @@
               <article class="md-content__inner md-typeset">
                 
                   
 
 
 <h1 id="weectl-station">weectl station<a class="headerlink" href="#weectl-station" title="Permanent link">&para;</a></h1>
 <p>Use the <code>weectl</code> subcommand <code>station</code> to manage the user data for a
-station, including its configuration file</p>
+station, including its configuration file.</p>
 <p>Specify <code>--help</code> to see the actions and options.</p>
 <p>In the documentation that follows,  the exact output will depend on your
 operating system and username. What is shown below is for Linux and user
 <code>tkeffer</code>.</p>
-<h2 id="create-a-new-user-data-aera">Create a new user data aera<a class="headerlink" href="#create-a-new-user-data-aera" title="Permanent link">&para;</a></h2>
+<h2 id="create-a-new-user-data-area">Create a new user data area<a class="headerlink" href="#create-a-new-user-data-area" title="Permanent link">&para;</a></h2>
 <div class="highlight"><pre><span></span><code>weectl station create
-    [--dist-config=DIST-CONFIG-PATH]
     [--driver=DRIVER]
     [--location=LOCATION]
     [--altitude=ALTITUDE,(foot|meter)]
     [--latitude=LATITUDE] [--longitude=LONGITUDE]
     [--register=(y,n) [--station-url=STATION_URL]]
     [--units=(us|metricwx|metric)]
     [--skin-root=SKIN_ROOT]
     [--sqlite-root=SQLITE_ROOT]
     [--html-root=HTML_ROOT]
     [--user-root=USER_ROOT]
     [--docs-root=DOCS_ROOT]
     [--examples-root=EXAMPLES_ROOT]
     [--no-prompt]
     [--config=CONFIG-PATH]
+    [--dist-config=DIST-CONFIG-PATH]
     [--dry-run]
 </code></pre></div>
 <p>This action will create a new area for user data. After the command completes,
 the area will include</p>
 <ul>
 <li>A configuration file, <code>weewx.conf</code>;</li>
 <li>Documentation;</li>
 <li>Examples;</li>
 <li>Utility files; and</li>
 <li>Skins.</li>
 </ul>
 <p><code>weectl station create</code> is typically used when installing using pip, or when
 you want to create multiple stations.</p>
+<h3 id="create-user-data-with-prompting">Create user data with prompting<a class="headerlink" href="#create-user-data-with-prompting" title="Permanent link">&para;</a></h3>
+<p>If invoked without any options, <code>weectl station create</code> will prompt you for various settings,
+such as the type of hardware you are using, the station altitude and location, etc. This is what
+most users will want.</p>
+<h3 id="create-user-data-without-prompting">Create user data without prompting<a class="headerlink" href="#create-user-data-without-prompting" title="Permanent link">&para;</a></h3>
+<p>A new user data area can be created without prompting by using option <code>--no-prompt</code>. This
+is most useful when creating a station with an automated script. For
+example,</p>
+<div class="highlight"><pre><span></span><code>weectl station create --no-prompt --driver=weewx.drivers.vantage \
+    --altitude=&quot;400,foot&quot; --latitude=45.1 --longitude=-105.9 \ 
+    --location=&quot;My Special Station&quot;
+</code></pre></div>
+<p>will create a station with the indicated values. If a value is not specified, a default will
+be used.</p>
+<p>See the section <a href="#common-options"><em>Common options</em></a> for details of the various options.</p>
+<h2 id="reconfigure-an-existing-station">Reconfigure an existing station<a class="headerlink" href="#reconfigure-an-existing-station" title="Permanent link">&para;</a></h2>
+<div class="highlight"><pre><span></span><code>weectl station reconfigure
+    [--driver=DRIVER]
+    [--location=LOCATION]
+    [--altitude=ALTITUDE,(foot|meter)]
+    [--latitude=LATITUDE] [--longitude=LONGITUDE]
+    [--register=(y,n) [--station-url=STATION_URL]]
+    [--units=(us|metricwx|metric)]
+    [--skin-root=SKIN_ROOT]
+    [--sqlite-root=SQLITE_ROOT]
+    [--html-root=HTML_ROOT]
+    [--no-backup]
+    [--no-prompt]
+    [--config=CONFIG-PATH] 
+    [--dry-run]
+</code></pre></div>
+<p>This action will reconfigure the contents of an existing configuration file (generally named
+<code>weewx.conf</code>). </p>
+<p>It is often used for changing drivers.</p>
+<h3 id="reconfigure-with-prompting">Reconfigure with prompting<a class="headerlink" href="#reconfigure-with-prompting" title="Permanent link">&para;</a></h3>
+<p>If invoked without the <code>--no-prompt</code> option, <code>weectl station reconfigure</code> will prompt you for new
+settings.</p>
+<h3 id="reconfigure-without-prompting">Reconfigure without prompting<a class="headerlink" href="#reconfigure-without-prompting" title="Permanent link">&para;</a></h3>
+<p>If the option <code>--no-prompt</code> is specified, <code>weectl station reconfigure</code> will reconfigure the
+configuration file using whatever options you've specified on the command line.</p>
+<p>For example, to keep all settings, but change to the Vantage driver you would use</p>
+<div class="highlight"><pre><span></span><code>weectl station reconfigure --no-prompt --driver=weewx.drivers.vantage
+</code></pre></div>
+<h2 id="upgrade-an-existing-station">Upgrade an existing station<a class="headerlink" href="#upgrade-an-existing-station" title="Permanent link">&para;</a></h2>
+<div class="highlight"><pre><span></span><code>weectl station upgrade
+    [--docs-root=DOCS_ROOT]
+    [--examples-root=EXAMPLES_ROOT]
+    [--skin-root=SKIN_ROOT]
+    [--what (config|docs|examples|util|skins)...]
+    [--no-backup]
+    [--no-prompt]
+    [--config=CONFIG-PATH]
+    [--dist-config=DIST-CONFIG-PATH]]
+    [--dry-run]
+</code></pre></div>
+<p>If you installed using pip, then do an upgrade using pip, it will only upgrade the code base. It
+does not touch the user data area. Use this action to upgrade all or part of the user data area.</p>
+<p>It can also be useful for upgrading a package install. While these generally </p>
+<h3 id="-what">--what<a class="headerlink" href="#-what" title="Permanent link">&para;</a></h3>
+<p>By default, <code>weectl station upgrade</code> will upgrade the configuration file, documentation, examples,
+and utility files. However, you can customize exactly what gets upgraded.</p>
+<div class="admonition note">
+<p class="admonition-title">Note</p>
+<p>The <code>--what</code> option does not take an equal sign (<code>=</code>). Just list the
+desired things to be upgraded, without commas between them.</p>
+</div>
+<p>For example, to upgrade the configuration file and skins only, you would
+specify</p>
+<div class="highlight"><pre><span></span><code>weectl station upgrade --what config skins
+</code></pre></div>
+<h2 id="common-options">Common options<a class="headerlink" href="#common-options" title="Permanent link">&para;</a></h2>
+<p>In what follows, <code>WEEWX_ROOT</code> is the directory holding the configuration file. For a pip
+install, this is typically <code>~/weewx-data/</code>. For package installs, it is usually <code>/etc/weewx/</code>.</p>
 <h3 id="-driverdriver">--driver=DRIVER<a class="headerlink" href="#-driverdriver" title="Permanent link">&para;</a></h3>
-<p>Which driver to use. Default is <code>simulator</code>.</p>
+<p>Which driver to use. Default is <code>weewx.drivers.simulator</code>.</p>
 <h3 id="-locationlocation">--location=LOCATION<a class="headerlink" href="#-locationlocation" title="Permanent link">&para;</a></h3>
-<p>A description of your station, such as <code>--location="A small town in Rongovia"</code></p>
+<p>A description of your station, such as <code>--location="A small town in Rongovia"</code> Default
+is <code>WeeWX</code>.</p>
 <h3 id="-altitudealtitude">--altitude=ALTITUDE<a class="headerlink" href="#-altitudealtitude" title="Permanent link">&para;</a></h3>
 <p>The altitude of your station, along with the unit it is measured in. For
 example, <code>--altitude=50,meter</code>. Note that the unit is measured in the singular
-(<code>foot</code>, not <code>feet</code>).</p>
+(<code>foot</code>, not <code>feet</code>). Default is <code>"0,foot"</code>.</p>
 <h3 id="-latitudelatitude">--latitude=LATITUDE<a class="headerlink" href="#-latitudelatitude" title="Permanent link">&para;</a></h3>
-<p>The station latitude in decimal degrees. Negative for the southern hemisphere.</p>
+<p>The station latitude in decimal degrees. Negative for the southern hemisphere. Default is
+<code>0</code>.</p>
 <h3 id="-longitudelongitude">--longitude=LONGITUDE<a class="headerlink" href="#-longitudelongitude" title="Permanent link">&para;</a></h3>
-<p>The station longitude in decimal degrees. Negative for the western hemisphere.</p>
+<p>The station longitude in decimal degrees. Negative for the western hemisphere. Default is <code>0</code>.</p>
 <h3 id="-registeryn">--register={y|n}<a class="headerlink" href="#-registeryn" title="Permanent link">&para;</a></h3>
-<p>Whether to include the station in the WeeWX registry and
-<a href="https://weewx.com/stations.html">map</a>. If you set <code>--register</code>, you must also
-specify a unique URL for your station with option <code>--station-url</code>.</p>
+<p>Whether to include the station in the WeeWX registry and <a href="https://weewx.com/stations.html">map</a>. If
+you choose to register your station, you must also specify a unique URL for your station with
+option <code>--station-url</code>. Default is <code>n</code> (do not register).</p>
 <h3 id="-station-urlurl">--station-url=URL<a class="headerlink" href="#-station-urlurl" title="Permanent link">&para;</a></h3>
 <p>A unique URL for your station.</p>
-<p>Example: <code>--station-url=https://www.wunderground.com/dashboard/pws/KNDPETE15</code>.</p>
+<p>Example: <code>--station-url=https://www.wunderground.com/dashboard/pws/KNDPETE15</code>. No default.</p>
 <h3 id="-unitsunit_system">--units=UNIT_SYSTEM<a class="headerlink" href="#-unitsunit_system" title="Permanent link">&para;</a></h3>
 <p>What units to use for your reports. Options are <code>us</code>, <code>metricwx</code>, or <code>metric</code>.
-See the Appendix <a href="../../custom/appendix/#units"><em>Units</em></a> for details.</p>
+See the Appendix <a href="../../custom/appendix/#units"><em>Units</em></a> for details. Default is <code>us</code>.</p>
+<h3 id="-skin-rootskin_root">--skin-root=SKIN_ROOT<a class="headerlink" href="#-skin-rootskin_root" title="Permanent link">&para;</a></h3>
+<p>The location of the directory holding the skins <em>relative to <code>WEEWX_ROOT</code></em>. Of course, like any
+other path, if the option starts with a slash (<code>/</code>), it becomes an absolute path. Default is
+<code>skins</code>.</p>
+<h3 id="-sqlite-rootsqlite_root">--sqlite-root=SQLITE_ROOT<a class="headerlink" href="#-sqlite-rootsqlite_root" title="Permanent link">&para;</a></h3>
+<p>The location of the directory holding the SQLite database <em>relative to <code>WEEWX_ROOT</code></em>. Of course,
+like any other path, if the option starts with a slash (<code>/</code>), it becomes an absolute path. Default
+is <code>skins</code>.</p>
+<h3 id="-html-roothtml_root">--html-root=HTML_ROOT<a class="headerlink" href="#-html-roothtml_root" title="Permanent link">&para;</a></h3>
+<p>Where generated HTML files should be placed, <em>relative to <code>WEEWX_ROOT</code></em>.  Of course, like any other
+path, if the option starts with a slash (<code>/</code>), it becomes an absolute path. Default is
+<code>public_html</code>.</p>
+<h3 id="-user-rootuser_root">--user-root=USER_ROOT<a class="headerlink" href="#-user-rootuser_root" title="Permanent link">&para;</a></h3>
+<p>Where user extensions can be found, <em>relative to <code>WEEWX_ROOT</code></em>. Of course, like any other path, if
+the option starts with a slash (<code>/</code>), it becomes an absolute path. Default is <code>bin/user</code>.</p>
+<h3 id="-docs-rootdocs_root">--docs-root=DOCS_ROOT<a class="headerlink" href="#-docs-rootdocs_root" title="Permanent link">&para;</a></h3>
+<p>Where the WeeWX documentation can be found, <em>relative to <code>WEEWX_ROOT</code></em>. Of course, like any other
+path, if the option starts with a slash (<code>/</code>), it becomes an absolute path. Default is <code>docs</code>.</p>
+<h3 id="-examples-rootexamples_root">--examples-root=EXAMPLES_ROOT<a class="headerlink" href="#-examples-rootexamples_root" title="Permanent link">&para;</a></h3>
+<p>Where the WeeWX examples can be found, <em>relative to <code>WEEWX_ROOT</code></em>. Of course, like any other path,
+if the option starts with a slash (<code>/</code>), it becomes an absolute path. Default is <code>examples</code>.</p>
+<h3 id="-no-backup">--no-backup<a class="headerlink" href="#-no-backup" title="Permanent link">&para;</a></h3>
+<p>Generally, if <code>weectl station</code> changes your configuration file, it will save a timestamped version
+of your original configuration file. If you specify <code>--no-backup</code>, then it will not save a copy.</p>
 <h3 id="-no-prompt">--no-prompt<a class="headerlink" href="#-no-prompt" title="Permanent link">&para;</a></h3>
 <p>Generally, the utility will prompt for values unless <code>--no-prompt</code> has been
 set. With <code>--no-prompt</code>, the values to be used are the default values,
 replaced with whatever options have been set on the command line. For example,</p>
 <div class="highlight"><pre><span></span><code>weectl station create --driver=&#39;weewx.drivers.vantage&#39; --no-prompt
 </code></pre></div>
 <p>will cause the defaults to be used for all values except <code>--driver</code>, which will
 use the Vantage driver.</p>
 <h3 id="-configfilename">--config=FILENAME<a class="headerlink" href="#-configfilename" title="Permanent link">&para;</a></h3>
 <p>Path to the configuration file to be created. The directory of the path will
 become the value for <code>WEEWX_ROOT</code> in the configuration file. Default is
 <code>~/weewx-data/weewx.conf</code>.</p>
 <h3 id="-dry-run">--dry-run<a class="headerlink" href="#-dry-run" title="Permanent link">&para;</a></h3>
-<p>With option <code>--dry-run</code> you can test what <code>weect station create</code> would do
-without actually doing it. It will print out the steps, but not
-actually write anything.</p>
-<h3 id="root-options">root options<a class="headerlink" href="#root-options" title="Permanent link">&para;</a></h3>
-<p>"Root options" include</p>
-<p><code>--skin-root</code><br/>
-<code>--sqlite-root</code><br/>
-<code>--html-root</code><br/>
-<code>--user-root</code><br/>
-<code>--docs-root</code><br/>
-<code>--examples-root</code></p>
-<p>All of these root options are <em>relative to <code>WEEWX_ROOT</code></em>. Of course, like any
-other path, if the option starts with a slash (<code>/</code>), it becomes an absolute
-path. So, for example,</p>
-<div class="highlight"><pre><span></span><code>--html-root=/var/www/html
-</code></pre></div>
-<p>will cause HTML files to be put in the traditional system WWW directory
-<code>/var/www/html</code>.</p>
-<h2 id="weectl-station-reconfigure">weectl station reconfigure<a class="headerlink" href="#weectl-station-reconfigure" title="Permanent link">&para;</a></h2>
-<p>This action will reconfigure the contents of the configuration file
-<code>weewx.conf</code>. Unless option <code>--no-prompt</code> has been specified, it will prompt
-you for each setting, using the previous settings as default values, and give
-you a chance to change them. </p>
-<p>Specify <code>--help</code> to see the options:
-<div class="highlight"><pre><span></span><code>weectl station reconfigure  --help
-</code></pre></div>
-<div class="highlight"><pre><span></span><code>usage: weectl station reconfigure [--config=CONFIG-PATH] 
-                                  [--driver=DRIVER]
-                                  [--location=LOCATION]
-                                  [--altitude=ALTITUDE,{foot|meter}]
-                                  [--latitude=LATITUDE] [--longitude=LONGITUDE]
-                                  [--register={y,n} [--station-url=STATION_URL]]
-                                  [--units={us,metricwx,metric}]
-                                  [--skin-root=SKIN_ROOT]
-                                  [--sqlite-root=SQLITE_ROOT]
-                                  [--html-root=HTML_ROOT]
-                                  [--no-prompt]
-                                  [--no-backup]
-                                  [--dry-run]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --config CONFIG-PATH  Path to configuration file. Default is
-                        &quot;/home/tkeffer/weewx-data/weewx.conf&quot;
-  --driver DRIVER       Driver to use. Default is &quot;weewx.drivers.simulator&quot;.
-  --location LOCATION   A description of the station. This will be used for
-                        report titles. Default is &quot;WeeWX&quot;.
-  --altitude ALTITUDE,{foot|meter}
-                        The station altitude in either feet or meters. For
-                        example, &quot;750,foot&quot; or &quot;320,meter&quot;. Default is &quot;0,
-                        foot&quot;.
-  --latitude LATITUDE   The station latitude in decimal degrees. Default is
-                        &quot;0.00&quot;.
-  --longitude LONGITUDE
-                        The station longitude in decimal degrees. Default is
-                        &quot;0.00&quot;.
-  --register {y,n}      Register this station in the weewx registry? Default
-                        is &quot;n&quot; (do not register).
-  --station-url STATION_URL
-                        Unique URL to be used if registering the station.
-                        Required if the station is to be registered.
-  --units {us,metricwx,metric}
-                        Set display units to us, metricwx, or metric. Default
-                        is &quot;us&quot;.
-  --skin-root SKIN_ROOT
-                        Where to put the skins, relatve to WEEWX_ROOT. Default
-                        is &quot;skins&quot;.
-  --sqlite-root SQLITE_ROOT
-                        Where to put the SQLite database, relative to
-                        WEEWX_ROOT. Default is &quot;archive&quot;.
-  --html-root HTML_ROOT
-                        Where to put the generated HTML and images, relative
-                        to WEEWX_ROOT. Default is &quot;public_html&quot;.
-  --no-prompt           Do not prompt. Use default values.
-  --no-backup           Do not backup the old configuration file.
-  --dry-run             Print what would happen, but do not actually do it.
-</code></pre></div></p>
-<h3 id="-configfilename_1">--config=FILENAME<a class="headerlink" href="#-configfilename_1" title="Permanent link">&para;</a></h3>
-<p>Path to the configuration file to be updated. The directory of the path will
-become the value for <code>WEEWX_ROOT</code> in the configuration file. Default is
-<code>~/weewx-data/weewx.conf</code>.</p>
-<h3 id="-no-prompt_1">--no-prompt<a class="headerlink" href="#-no-prompt_1" title="Permanent link">&para;</a></h3>
-<p>When used with the <code>--no-prompt</code> option, <code>weectl station reconfigure</code> will
-modify specific parameters with no interaction. For example, this would set
-the station altitude to 35 feet:</p>
-<div class="highlight"><pre><span></span><code>weectl station reconfigure --altitude=35,foot --no-prompt
-</code></pre></div>
-<p>This would change the driver to a user-installed netatmo driver:</p>
-<div class="highlight"><pre><span></span><code>weectl station reconfigure --driver=user.netatmo --no-prompt
-</code></pre></div>
-<h3 id="-dry-run_1">--dry-run<a class="headerlink" href="#-dry-run_1" title="Permanent link">&para;</a></h3>
-<p>With option <code>--dry-run</code> you can test what <code>weect station create</code> would do
+<p>With option <code>--dry-run</code> you can test what <code>weect station</code> would do
 without actually doing it. It will print out the steps, but not
 actually write anything.</p>
-<h3 id="-no-backup">--no-backup<a class="headerlink" href="#-no-backup" title="Permanent link">&para;</a></h3>
-<p>Do not create a copy of the previous configuration file.</p>
-<p>Other options are as described in the <a href="#weectl-station-create"><code>weectl station create</code></a> section.</p>
-<h2 id="weectl-station-upgrade">weectl station upgrade<a class="headerlink" href="#weectl-station-upgrade" title="Permanent link">&para;</a></h2>
-<p>This action can upgrade the configuration file, documentation, examples,
-daemon utility files, and skins.  When you upgrade the WeeWX software, that
-process does not modify existing configurations or skins.  In most cases,
-the WeeWX developers will maintain backward-compatibility, so older
-configurations and skins will continue to work with new WeeWX updates.
-However, if you want to get new features, you might have to update your
-configurations or skins.  Use this utility to do that.</p>
-<p>Specify <code>--help</code> to see the options:
-<div class="highlight"><pre><span></span><code>weectl station upgrade --help
-</code></pre></div>
-<div class="highlight"><pre><span></span><code>usage: weectl station upgrade [--config=CONFIG-PATH]
-                              [--dist-config=DIST-CONFIG-PATH]]
-                              [--docs-root=DOCS_ROOT]
-                              [--examples-root=EXAMPLES_ROOT]
-                              [--skin-root=SKIN_ROOT]
-                              [--what [{config,docs,examples,util,skins} ... ]
-                              [--no-prompt]
-                              [--no-backup]
-                              [--dry-run]
-
-Upgrade an existing user data area, including any combination of the
-configuration file, docs, examples, daemon utility files, and skins. In what
-follows, WEEWX_ROOT is the directory that contains the configuration
-file. For example, if &quot;--config=/home/tkeffer/weewx-data/weewx.conf&quot;, then
-WEEWX_ROOT will be &quot;/home/tkeffer/weewx-data&quot;.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --config CONFIG-PATH  Path to configuration file. Default is
-                        &quot;/home/tkeffer/weewx-data/weewx.conf&quot;
-  --dist-config DIST-CONFIG-PATH
-                        Use configuration file DIST-CONFIG-PATH as the new
-                        configuration file. Default is to retrieve it from
-                        package resources. The average user is unlikely to
-                        need this option.
-  --docs-root DOCS_ROOT
-                        Where to put the new documentation, relative to
-                        WEEWX_ROOT. Default is &quot;docs&quot;.
-  --examples-root EXAMPLES_ROOT
-                        Where to put the new examples, relative to WEEWX_ROOT.
-                        Default is &quot;examples&quot;.
-  --skin-root SKIN_ROOT
-                        Where to put the skins, relative to WEEWX_ROOT.
-                        Default is &quot;skins&quot;.
-  --what {config,docs,examples,util,skins} [{config,docs,examples,util,skins} ...]
-                        What to upgrade. Default is to upgrade the
-                        configuration file, documentation, examples, and
-                        daemon utility files.
-  --no-prompt           Do not prompt. Use default values.
-  --no-backup           Do not backup the old configuration file.
-  --dry-run             Print what would happen, but do not actually do it.
-</code></pre></div></p>
-<h3 id="-configfilename_2">--config=FILENAME<a class="headerlink" href="#-configfilename_2" title="Permanent link">&para;</a></h3>
-<p>Path to the configuration file to be updated. The directory of the path will
-become the value for <code>WEEWX_ROOT</code> in the configuration file. Default is
-<code>~/weewx-data/weewx.conf</code>.</p>
-<h3 id="-what">--what<a class="headerlink" href="#-what" title="Permanent link">&para;</a></h3>
-<p>By default, <code>weectl station upgrade</code> will upgrade the configuration file,
-documentation, examples, and daemon utility files. However, you can customize
-exactly what gets upgraded. </p>
-<div class="admonition note">
-<p class="admonition-title">Note</p>
-<p>The <code>--what</code> option does not take an equal sign (<code>=</code>). Just list the
-desired things to be upgraded, without commas between them.</p>
-</div>
-<p>For example, to upgrade the configuration file and skins only, you would
-specify</p>
-<div class="highlight"><pre><span></span><code>weectl station upgrade --what config skins
-</code></pre></div>
-<h3 id="root-options_1">root options<a class="headerlink" href="#root-options_1" title="Permanent link">&para;</a></h3>
-<p>"Root options" include</p>
-<p><code>--skin-root</code><br/>
-<code>--docs-root</code><br/>
-<code>--examples-root</code></p>
-<p>All of these root options are <em>relative to <code>WEEWX_ROOT</code></em>. Of course, like any
-other path, if the option starts with a slash (<code>/</code>), it becomes an absolute
-path. So, for example,</p>
-<div class="highlight"><pre><span></span><code>--docs-root=/usr/local/doc/weewx
-</code></pre></div>
-<p>will cause documentation files to be put in <code>/usr/local/doc/weewx</code>.</p>
 
 
 
 
 
                 
               </article>
```

#### html2text {}

```diff
@@ -79,36 +79,41 @@
           o Extensions
           o Report_options
           o Appendix
     * *  Utilities      Utilities
           o weewxd
           o *  weectl      weectl
                 # ⁰  weectl station   weectl_station    Table of contents
-                      # Create_a_new_user_data_aera
+                      # Create_a_new_user_data_area
+                            # Create_user_data_with_prompting
+                            # Create_user_data_without_prompting
+                      # Reconfigure_an_existing_station
+                            # Reconfigure_with_prompting
+                            # Reconfigure_without_prompting
+                      # Upgrade_an_existing_station
+                            # --what
+                      # Common_options
                             # --driver=DRIVER
                             # --location=LOCATION
                             # --altitude=ALTITUDE
                             # --latitude=LATITUDE
                             # --longitude=LONGITUDE
                             # --register={y|n}
                             # --station-url=URL
                             # --units=UNIT_SYSTEM
+                            # --skin-root=SKIN_ROOT
+                            # --sqlite-root=SQLITE_ROOT
+                            # --html-root=HTML_ROOT
+                            # --user-root=USER_ROOT
+                            # --docs-root=DOCS_ROOT
+                            # --examples-root=EXAMPLES_ROOT
+                            # --no-backup
                             # --no-prompt
                             # --config=FILENAME
                             # --dry-run
-                            # root_options
-                      # weectl_station_reconfigure
-                            # --config=FILENAME
-                            # --no-prompt
-                            # --dry-run
-                            # --no-backup
-                      # weectl_station_upgrade
-                            # --config=FILENAME
-                            # --what
-                            # root_options
                 # weectl_extension
                 # weectl_database
           o wee_database
           o wee_debug
           o wee_device
           o wee_import
           o wee_reports
@@ -126,270 +131,211 @@
           o WS1
           o WS23xx
           o WS28xx
     * Upgrade_guide
     * Notes_for_developers
     * Change_log
    Table of contents
-    * Create_a_new_user_data_aera
+    * Create_a_new_user_data_area
+          o Create_user_data_with_prompting
+          o Create_user_data_without_prompting
+    * Reconfigure_an_existing_station
+          o Reconfigure_with_prompting
+          o Reconfigure_without_prompting
+    * Upgrade_an_existing_station
+          o --what
+    * Common_options
           o --driver=DRIVER
           o --location=LOCATION
           o --altitude=ALTITUDE
           o --latitude=LATITUDE
           o --longitude=LONGITUDE
           o --register={y|n}
           o --station-url=URL
           o --units=UNIT_SYSTEM
+          o --skin-root=SKIN_ROOT
+          o --sqlite-root=SQLITE_ROOT
+          o --html-root=HTML_ROOT
+          o --user-root=USER_ROOT
+          o --docs-root=DOCS_ROOT
+          o --examples-root=EXAMPLES_ROOT
+          o --no-backup
           o --no-prompt
           o --config=FILENAME
           o --dry-run
-          o root_options
-    * weectl_station_reconfigure
-          o --config=FILENAME
-          o --no-prompt
-          o --dry-run
-          o --no-backup
-    * weectl_station_upgrade
-          o --config=FILENAME
-          o --what
-          o root_options
 ****** weectl station¶ ******
 Use the weectl subcommand station to manage the user data for a station,
-including its configuration file
+including its configuration file.
 Specify --help to see the actions and options.
 In the documentation that follows, the exact output will depend on your
 operating system and username. What is shown below is for Linux and user
 tkeffer.
-***** Create a new user data aera¶ *****
+***** Create a new user data area¶ *****
 weectl station create
-    [--dist-config=DIST-CONFIG-PATH]
     [--driver=DRIVER]
     [--location=LOCATION]
     [--altitude=ALTITUDE,(foot|meter)]
     [--latitude=LATITUDE] [--longitude=LONGITUDE]
     [--register=(y,n) [--station-url=STATION_URL]]
     [--units=(us|metricwx|metric)]
     [--skin-root=SKIN_ROOT]
     [--sqlite-root=SQLITE_ROOT]
     [--html-root=HTML_ROOT]
     [--user-root=USER_ROOT]
     [--docs-root=DOCS_ROOT]
     [--examples-root=EXAMPLES_ROOT]
     [--no-prompt]
     [--config=CONFIG-PATH]
+    [--dist-config=DIST-CONFIG-PATH]
     [--dry-run]
 This action will create a new area for user data. After the command completes,
 the area will include
     * A configuration file, weewx.conf;
     * Documentation;
     * Examples;
     * Utility files; and
     * Skins.
 weectl station create is typically used when installing using pip, or when you
 want to create multiple stations.
+**** Create user data with prompting¶ ****
+If invoked without any options, weectl station create will prompt you for
+various settings, such as the type of hardware you are using, the station
+altitude and location, etc. This is what most users will want.
+**** Create user data without prompting¶ ****
+A new user data area can be created without prompting by using option --no-
+prompt. This is most useful when creating a station with an automated script.
+For example,
+weectl station create --no-prompt --driver=weewx.drivers.vantage \
+    --altitude="400,foot" --latitude=45.1 --longitude=-105.9 \
+    --location="My Special Station"
+will create a station with the indicated values. If a value is not specified, a
+default will be used.
+See the section Common_options for details of the various options.
+***** Reconfigure an existing station¶ *****
+weectl station reconfigure
+    [--driver=DRIVER]
+    [--location=LOCATION]
+    [--altitude=ALTITUDE,(foot|meter)]
+    [--latitude=LATITUDE] [--longitude=LONGITUDE]
+    [--register=(y,n) [--station-url=STATION_URL]]
+    [--units=(us|metricwx|metric)]
+    [--skin-root=SKIN_ROOT]
+    [--sqlite-root=SQLITE_ROOT]
+    [--html-root=HTML_ROOT]
+    [--no-backup]
+    [--no-prompt]
+    [--config=CONFIG-PATH]
+    [--dry-run]
+This action will reconfigure the contents of an existing configuration file
+(generally named weewx.conf).
+It is often used for changing drivers.
+**** Reconfigure with prompting¶ ****
+If invoked without the --no-prompt option, weectl station reconfigure will
+prompt you for new settings.
+**** Reconfigure without prompting¶ ****
+If the option --no-prompt is specified, weectl station reconfigure will
+reconfigure the configuration file using whatever options you've specified on
+the command line.
+For example, to keep all settings, but change to the Vantage driver you would
+use
+weectl station reconfigure --no-prompt --driver=weewx.drivers.vantage
+***** Upgrade an existing station¶ *****
+weectl station upgrade
+    [--docs-root=DOCS_ROOT]
+    [--examples-root=EXAMPLES_ROOT]
+    [--skin-root=SKIN_ROOT]
+    [--what (config|docs|examples|util|skins)...]
+    [--no-backup]
+    [--no-prompt]
+    [--config=CONFIG-PATH]
+    [--dist-config=DIST-CONFIG-PATH]]
+    [--dry-run]
+If you installed using pip, then do an upgrade using pip, it will only upgrade
+the code base. It does not touch the user data area. Use this action to upgrade
+all or part of the user data area.
+It can also be useful for upgrading a package install. While these generally
+**** --what¶ ****
+By default, weectl station upgrade will upgrade the configuration file,
+documentation, examples, and utility files. However, you can customize exactly
+what gets upgraded.
+Note
+The --what option does not take an equal sign (=). Just list the desired things
+to be upgraded, without commas between them.
+For example, to upgrade the configuration file and skins only, you would
+specify
+weectl station upgrade --what config skins
+***** Common options¶ *****
+In what follows, WEEWX_ROOT is the directory holding the configuration file.
+For a pip install, this is typically ~/weewx-data/. For package installs, it is
+usually /etc/weewx/.
 **** --driver=DRIVER¶ ****
-Which driver to use. Default is simulator.
+Which driver to use. Default is weewx.drivers.simulator.
 **** --location=LOCATION¶ ****
 A description of your station, such as --location="A small town in Rongovia"
+Default is WeeWX.
 **** --altitude=ALTITUDE¶ ****
 The altitude of your station, along with the unit it is measured in. For
 example, --altitude=50,meter. Note that the unit is measured in the singular
-(foot, not feet).
+(foot, not feet). Default is "0,foot".
 **** --latitude=LATITUDE¶ ****
 The station latitude in decimal degrees. Negative for the southern hemisphere.
+Default is 0.
 **** --longitude=LONGITUDE¶ ****
 The station longitude in decimal degrees. Negative for the western hemisphere.
+Default is 0.
 **** --register={y|n}¶ ****
-Whether to include the station in the WeeWX registry and map. If you set --
-register, you must also specify a unique URL for your station with option --
-station-url.
+Whether to include the station in the WeeWX registry and map. If you choose to
+register your station, you must also specify a unique URL for your station with
+option --station-url. Default is n (do not register).
 **** --station-url=URL¶ ****
 A unique URL for your station.
-Example: --station-url=https://www.wunderground.com/dashboard/pws/KNDPETE15.
+Example: --station-url=https://www.wunderground.com/dashboard/pws/KNDPETE15. No
+default.
 **** --units=UNIT_SYSTEM¶ ****
 What units to use for your reports. Options are us, metricwx, or metric. See
-the Appendix Units for details.
+the Appendix Units for details. Default is us.
+**** --skin-root=SKIN_ROOT¶ ****
+The location of the directory holding the skins relative to WEEWX_ROOT. Of
+course, like any other path, if the option starts with a slash (/), it becomes
+an absolute path. Default is skins.
+**** --sqlite-root=SQLITE_ROOT¶ ****
+The location of the directory holding the SQLite database relative to
+WEEWX_ROOT. Of course, like any other path, if the option starts with a slash
+(/), it becomes an absolute path. Default is skins.
+**** --html-root=HTML_ROOT¶ ****
+Where generated HTML files should be placed, relative to WEEWX_ROOT. Of course,
+like any other path, if the option starts with a slash (/), it becomes an
+absolute path. Default is public_html.
+**** --user-root=USER_ROOT¶ ****
+Where user extensions can be found, relative to WEEWX_ROOT. Of course, like any
+other path, if the option starts with a slash (/), it becomes an absolute path.
+Default is bin/user.
+**** --docs-root=DOCS_ROOT¶ ****
+Where the WeeWX documentation can be found, relative to WEEWX_ROOT. Of course,
+like any other path, if the option starts with a slash (/), it becomes an
+absolute path. Default is docs.
+**** --examples-root=EXAMPLES_ROOT¶ ****
+Where the WeeWX examples can be found, relative to WEEWX_ROOT. Of course, like
+any other path, if the option starts with a slash (/), it becomes an absolute
+path. Default is examples.
+**** --no-backup¶ ****
+Generally, if weectl station changes your configuration file, it will save a
+timestamped version of your original configuration file. If you specify --no-
+backup, then it will not save a copy.
 **** --no-prompt¶ ****
 Generally, the utility will prompt for values unless --no-prompt has been set.
 With --no-prompt, the values to be used are the default values, replaced with
 whatever options have been set on the command line. For example,
 weectl station create --driver='weewx.drivers.vantage' --no-prompt
 will cause the defaults to be used for all values except --driver, which will
 use the Vantage driver.
 **** --config=FILENAME¶ ****
 Path to the configuration file to be created. The directory of the path will
 become the value for WEEWX_ROOT in the configuration file. Default is ~/weewx-
 data/weewx.conf.
 **** --dry-run¶ ****
-With option --dry-run you can test what weect station create would do without
-actually doing it. It will print out the steps, but not actually write
-anything.
-**** root options¶ ****
-"Root options" include
---skin-root
---sqlite-root
---html-root
---user-root
---docs-root
---examples-root
-All of these root options are relative to WEEWX_ROOT. Of course, like any other
-path, if the option starts with a slash (/), it becomes an absolute path. So,
-for example,
---html-root=/var/www/html
-will cause HTML files to be put in the traditional system WWW directory /var/
-www/html.
-***** weectl station reconfigure¶ *****
-This action will reconfigure the contents of the configuration file weewx.conf.
-Unless option --no-prompt has been specified, it will prompt you for each
-setting, using the previous settings as default values, and give you a chance
-to change them.
-Specify --help to see the options:
-weectl station reconfigure  --help
-usage: weectl station reconfigure [--config=CONFIG-PATH]
-                                  [--driver=DRIVER]
-                                  [--location=LOCATION]
-                                  [--altitude=ALTITUDE,{foot|meter}]
-                                  [--latitude=LATITUDE] [--longitude=LONGITUDE]
-                                  [--register={y,n} [--station-
-url=STATION_URL]]
-                                  [--units={us,metricwx,metric}]
-                                  [--skin-root=SKIN_ROOT]
-                                  [--sqlite-root=SQLITE_ROOT]
-                                  [--html-root=HTML_ROOT]
-                                  [--no-prompt]
-                                  [--no-backup]
-                                  [--dry-run]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --config CONFIG-PATH  Path to configuration file. Default is
-                        "/home/tkeffer/weewx-data/weewx.conf"
-  --driver DRIVER       Driver to use. Default is "weewx.drivers.simulator".
-  --location LOCATION   A description of the station. This will be used for
-                        report titles. Default is "WeeWX".
-  --altitude ALTITUDE,{foot|meter}
-                        The station altitude in either feet or meters. For
-                        example, "750,foot" or "320,meter". Default is "0,
-                        foot".
-  --latitude LATITUDE   The station latitude in decimal degrees. Default is
-                        "0.00".
-  --longitude LONGITUDE
-                        The station longitude in decimal degrees. Default is
-                        "0.00".
-  --register {y,n}      Register this station in the weewx registry? Default
-                        is "n" (do not register).
-  --station-url STATION_URL
-                        Unique URL to be used if registering the station.
-                        Required if the station is to be registered.
-  --units {us,metricwx,metric}
-                        Set display units to us, metricwx, or metric. Default
-                        is "us".
-  --skin-root SKIN_ROOT
-                        Where to put the skins, relatve to WEEWX_ROOT. Default
-                        is "skins".
-  --sqlite-root SQLITE_ROOT
-                        Where to put the SQLite database, relative to
-                        WEEWX_ROOT. Default is "archive".
-  --html-root HTML_ROOT
-                        Where to put the generated HTML and images, relative
-                        to WEEWX_ROOT. Default is "public_html".
-  --no-prompt           Do not prompt. Use default values.
-  --no-backup           Do not backup the old configuration file.
-  --dry-run             Print what would happen, but do not actually do it.
-**** --config=FILENAME¶ ****
-Path to the configuration file to be updated. The directory of the path will
-become the value for WEEWX_ROOT in the configuration file. Default is ~/weewx-
-data/weewx.conf.
-**** --no-prompt¶ ****
-When used with the --no-prompt option, weectl station reconfigure will modify
-specific parameters with no interaction. For example, this would set the
-station altitude to 35 feet:
-weectl station reconfigure --altitude=35,foot --no-prompt
-This would change the driver to a user-installed netatmo driver:
-weectl station reconfigure --driver=user.netatmo --no-prompt
-**** --dry-run¶ ****
-With option --dry-run you can test what weect station create would do without
-actually doing it. It will print out the steps, but not actually write
-anything.
-**** --no-backup¶ ****
-Do not create a copy of the previous configuration file.
-Other options are as described in the weectl_station_create section.
-***** weectl station upgrade¶ *****
-This action can upgrade the configuration file, documentation, examples, daemon
-utility files, and skins. When you upgrade the WeeWX software, that process
-does not modify existing configurations or skins. In most cases, the WeeWX
-developers will maintain backward-compatibility, so older configurations and
-skins will continue to work with new WeeWX updates. However, if you want to get
-new features, you might have to update your configurations or skins. Use this
-utility to do that.
-Specify --help to see the options:
-weectl station upgrade --help
-usage: weectl station upgrade [--config=CONFIG-PATH]
-                              [--dist-config=DIST-CONFIG-PATH]]
-                              [--docs-root=DOCS_ROOT]
-                              [--examples-root=EXAMPLES_ROOT]
-                              [--skin-root=SKIN_ROOT]
-                              [--what [{config,docs,examples,util,skins} ... ]
-                              [--no-prompt]
-                              [--no-backup]
-                              [--dry-run]
-
-Upgrade an existing user data area, including any combination of the
-configuration file, docs, examples, daemon utility files, and skins. In what
-follows, WEEWX_ROOT is the directory that contains the configuration
-file. For example, if "--config=/home/tkeffer/weewx-data/weewx.conf", then
-WEEWX_ROOT will be "/home/tkeffer/weewx-data".
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --config CONFIG-PATH  Path to configuration file. Default is
-                        "/home/tkeffer/weewx-data/weewx.conf"
-  --dist-config DIST-CONFIG-PATH
-                        Use configuration file DIST-CONFIG-PATH as the new
-                        configuration file. Default is to retrieve it from
-                        package resources. The average user is unlikely to
-                        need this option.
-  --docs-root DOCS_ROOT
-                        Where to put the new documentation, relative to
-                        WEEWX_ROOT. Default is "docs".
-  --examples-root EXAMPLES_ROOT
-                        Where to put the new examples, relative to WEEWX_ROOT.
-                        Default is "examples".
-  --skin-root SKIN_ROOT
-                        Where to put the skins, relative to WEEWX_ROOT.
-                        Default is "skins".
-  --what {config,docs,examples,util,skins} [{config,docs,examples,util,skins}
-...]
-                        What to upgrade. Default is to upgrade the
-                        configuration file, documentation, examples, and
-                        daemon utility files.
-  --no-prompt           Do not prompt. Use default values.
-  --no-backup           Do not backup the old configuration file.
-  --dry-run             Print what would happen, but do not actually do it.
-**** --config=FILENAME¶ ****
-Path to the configuration file to be updated. The directory of the path will
-become the value for WEEWX_ROOT in the configuration file. Default is ~/weewx-
-data/weewx.conf.
-**** --what¶ ****
-By default, weectl station upgrade will upgrade the configuration file,
-documentation, examples, and daemon utility files. However, you can customize
-exactly what gets upgraded.
-Note
-The --what option does not take an equal sign (=). Just list the desired things
-to be upgraded, without commas between them.
-For example, to upgrade the configuration file and skins only, you would
-specify
-weectl station upgrade --what config skins
-**** root options¶ ****
-"Root options" include
---skin-root
---docs-root
---examples-root
-All of these root options are relative to WEEWX_ROOT. Of course, like any other
-path, if the option starts with a slash (/), it becomes an absolute path. So,
-for example,
---docs-root=/usr/local/doc/weewx
-will cause documentation files to be put in /usr/local/doc/weewx.
+With option --dry-run you can test what weect station would do without actually
+doing it. It will print out the steps, but not actually write anything.
   Back to top
 Copyright Â© 2009-2023 Thomas Keffer, Matthew Wall, and Gary Roderick, all
 rights reserved
 Made with Material_for_MkDocs
```

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/utilities/weewxd/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/utilities/weewxd/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/docs/versions/index.html` & `weewx-5.0.0b9/bin/wee_resources/docs/versions/index.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-37.pyc` & `weewx-5.0.0b9/bin/wee_resources/examples/__pycache__/vaporpressure.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/alarm.py` & `weewx-5.0.0b9/bin/wee_resources/examples/alarm.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/basic/install.py` & `weewx-5.0.0b9/bin/wee_resources/examples/basic/install.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/basic/readme.md` & `weewx-5.0.0b9/bin/wee_resources/examples/basic/readme.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/basic/skins/basic/basic.css` & `weewx-5.0.0b9/bin/wee_resources/examples/basic/skins/basic/basic.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/basic/skins/basic/current.inc` & `weewx-5.0.0b9/bin/wee_resources/examples/basic/skins/basic/current.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/basic/skins/basic/favicon.ico` & `weewx-5.0.0b9/bin/wee_resources/examples/basic/skins/basic/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/basic/skins/basic/hilo.inc` & `weewx-5.0.0b9/bin/wee_resources/examples/basic/skins/basic/hilo.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/basic/skins/basic/index.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/examples/basic/skins/basic/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/basic/skins/basic/lang/en.conf` & `weewx-5.0.0b9/bin/wee_resources/examples/basic/skins/basic/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/basic/skins/basic/lang/fr.conf` & `weewx-5.0.0b9/bin/wee_resources/examples/basic/skins/basic/lang/fr.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/basic/skins/basic/skin.conf` & `weewx-5.0.0b9/bin/wee_resources/examples/basic/skins/basic/skin.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/colorize/__pycache__/colorize_1.cpython-37.pyc` & `weewx-5.0.0b9/bin/wee_resources/examples/colorize/__pycache__/colorize_1.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/colorize/__pycache__/colorize_2.cpython-37.pyc` & `weewx-5.0.0b9/bin/wee_resources/examples/colorize/__pycache__/colorize_2.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/colorize/__pycache__/colorize_3.cpython-37.pyc` & `weewx-5.0.0b9/bin/wee_resources/examples/colorize/__pycache__/colorize_3.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/colorize/colorize_1.py` & `weewx-5.0.0b9/bin/wee_resources/examples/colorize/colorize_1.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/colorize/colorize_2.py` & `weewx-5.0.0b9/bin/wee_resources/examples/colorize/colorize_2.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/colorize/colorize_3.py` & `weewx-5.0.0b9/bin/wee_resources/examples/colorize/colorize_3.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/fileparse/bin/user/fileparse.py` & `weewx-5.0.0b9/bin/wee_resources/examples/fileparse/bin/user/fileparse.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/fileparse/install.py` & `weewx-5.0.0b9/bin/wee_resources/examples/fileparse/install.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/fileparse/readme.md` & `weewx-5.0.0b9/bin/wee_resources/examples/fileparse/readme.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/lowBattery.py` & `weewx-5.0.0b9/bin/wee_resources/examples/lowBattery.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/mem.py` & `weewx-5.0.0b9/bin/wee_resources/examples/mem.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/pmon/bin/user/pmon.py` & `weewx-5.0.0b9/bin/wee_resources/examples/pmon/bin/user/pmon.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/pmon/install.py` & `weewx-5.0.0b9/bin/wee_resources/examples/pmon/install.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/pmon/readme.md` & `weewx-5.0.0b9/bin/wee_resources/examples/pmon/readme.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/pmon/skins/pmon/skin.conf` & `weewx-5.0.0b9/bin/wee_resources/examples/pmon/skins/pmon/skin.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/tests/test_vaporpressure.py` & `weewx-5.0.0b9/bin/wee_resources/examples/tests/test_vaporpressure.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/vaporpressure.py` & `weewx-5.0.0b9/bin/wee_resources/examples/vaporpressure.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/xstats/bin/user/__pycache__/xstats.cpython-37.pyc` & `weewx-5.0.0b9/bin/wee_resources/examples/xstats/bin/user/__pycache__/xstats.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/xstats/bin/user/xstats.py` & `weewx-5.0.0b9/bin/wee_resources/examples/xstats/bin/user/xstats.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/xstats/install.py` & `weewx-5.0.0b9/bin/wee_resources/examples/xstats/install.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/xstats/readme.txt` & `weewx-5.0.0b9/bin/wee_resources/examples/xstats/readme.txt`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/xstats/skins/xstats/index.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/examples/xstats/skins/xstats/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/examples/xstats/skins/xstats/skin.conf` & `weewx-5.0.0b9/bin/wee_resources/examples/xstats/skins/xstats/skin.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Ftp/skin.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Ftp/skin.conf`

 * *Files 1% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 #                                                                             #
 # FTP CONFIGURATION FILE                                                      #
 #   This 'report' does not generate any files. Instead, we use the report     #
 #   engine to invoke FTP, which copies files to another location.             #
 ###############################################################################
 
 SKIN_NAME = Ftp
-SKIN_VERSION = 5.0.0b8
+SKIN_VERSION = 5.0.0b9
 
 [Generators]
     generator_list = weewx.reportengine.FtpGenerator
```

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Mobile/favicon.ico` & `weewx-5.0.0b9/bin/wee_resources/skins/Mobile/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Mobile/index.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Mobile/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Mobile/lang/de.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Mobile/lang/de.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Mobile/lang/en.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Mobile/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Mobile/lang/nl.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Mobile/lang/nl.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Mobile/lang/no.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Mobile/lang/no.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Mobile/mobile.css` & `weewx-5.0.0b9/bin/wee_resources/skins/Mobile/mobile.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Mobile/skin.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Mobile/skin.conf`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # configuration file for Mobile skin
 
 SKIN_NAME = Mobile
-SKIN_VERSION = 5.0.0b8
+SKIN_VERSION = 5.0.0b9
 
 [Extras]
     # Set this URL to display a radar image
     #radar_img = http://radar.weather.gov/ridge/lite/N0R/RTX_loop.gif
     # Set this URL for the radar image link
     #radar_url = http://radar.weather.gov/ridge/radar.php?product=NCR&rid=RTX&loop=yes
```

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Rsync/skin.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Rsync/skin.conf`

 * *Files 1% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 #                                                                             #
 # RSYNC CONFIGURATION FILE                                                    #
 #   This 'report' does not generate any files. Instead, we use the report     #
 #   engine to invoke rsync, which synchronizes files between two locations.   #
 ###############################################################################
 
 SKIN_NAME = Rsync
-SKIN_VERSION = 5.0.0b8
+SKIN_VERSION = 5.0.0b9
 
 [Generators]
     generator_list = weewx.reportengine.RsyncGenerator
```

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y-%m.txt.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y-%m.txt.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y.txt.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/NOAA/NOAA-%Y.txt.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/about.inc` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/about.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/analytics.inc` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/analytics.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/celestial.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/celestial.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/celestial.inc` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/celestial.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/current.inc` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/current.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/favicon.ico` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/font/Kanit-Bold.ttf` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/font/Kanit-Bold.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/font/Kanit-Regular.ttf` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/font/Kanit-Regular.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/font/OFL.txt` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/font/OFL.txt`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/font/OpenSans-Bold.ttf` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/font/OpenSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/font/OpenSans-Regular.ttf` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/font/OpenSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/font/OpenSans.woff` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/font/OpenSans.woff`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/font/OpenSans.woff2` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/font/OpenSans.woff2`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/font/license.txt` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/font/license.txt`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/hilo.inc` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/hilo.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/identifier.inc` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/identifier.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/index.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/cn.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/cn.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/cz.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/cz.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/de.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/de.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/en.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/es.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/es.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/fr.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/fr.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/gr.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/gr.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/it.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/it.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/nl.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/nl.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/no.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/no.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/lang/th.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/lang/th.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/map.inc` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/map.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/radar.inc` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/radar.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/rss.xml.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/rss.xml.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/satellite.inc` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/satellite.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/seasons.css` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/seasons.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/seasons.js` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/seasons.js`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/sensors.inc` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/sensors.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/skin.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/skin.conf`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ###############################################################################
 # SEASONS SKIN CONFIGURATION FILE                                             #
 # Copyright (c) 2018-2021 Tom Keffer <tkeffer@gmail.com> and Matthew Wall     #
 # See the file LICENSE.txt for your rights.                                   #
 ###############################################################################
 
 SKIN_NAME = Seasons
-SKIN_VERSION = 5.0.0b8
+SKIN_VERSION = 5.0.0b9
 
 ###############################################################################
 
 # The following section is for any extra tags that you want to be available in
 # the templates
 
 [Extras]
```

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/statistics.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/statistics.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/statistics.inc` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/statistics.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/sunmoon.inc` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/sunmoon.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/tabular.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/tabular.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/telemetry.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/telemetry.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Seasons/titlebar.inc` & `weewx-5.0.0b9/bin/wee_resources/skins/Seasons/titlebar.inc`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/barometer.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/barometer.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/favicon.ico` & `weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/humidity.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/humidity.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x1.png` & `weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x1.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x2.png` & `weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/icons/icon_ipad_x2.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x1.png` & `weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x1.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x2.png` & `weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/icons/icon_iphone_x2.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/index.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/lang/de.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/lang/de.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/lang/en.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/lang/nl.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/lang/nl.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/lang/no.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/lang/no.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/rain.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/rain.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/skin.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/skin.conf`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # configuration file for Smartphone skin
 
 SKIN_NAME = Smartphone
-SKIN_VERSION = 5.0.0b8
+SKIN_VERSION = 5.0.0b9
 
 [Extras]
     # Set this URL to display a radar image
     #radar_img = http://radar.weather.gov/ridge/lite/N0R/RTX_loop.gif
     # Set this URL for the radar image link
     #radar_url = http://radar.weather.gov/ridge/radar.php?product=NCR&rid=RTX&loop=yes
```

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/temp.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/temp.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Smartphone/wind.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Smartphone/wind.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y-%m.txt.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y-%m.txt.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y.txt.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/NOAA/NOAA-%Y.txt.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/RSS/weewx_rss.xml.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/RSS/weewx_rss.xml.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/backgrounds/butterfly.jpg` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/backgrounds/butterfly.jpg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/backgrounds/drops.gif` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/backgrounds/drops.gif`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/backgrounds/flower.jpg` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/backgrounds/flower.jpg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/backgrounds/leaf.jpg` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/backgrounds/leaf.jpg`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/backgrounds/night.gif` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/backgrounds/night.gif`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/favicon.ico` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/favicon.ico`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/font/DejaVuSansMono-Bold.ttf` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/font/DejaVuSansMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/index.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/lang/de.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/lang/de.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/lang/en.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/lang/en.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/lang/fr.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/lang/fr.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/lang/nl.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/lang/nl.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/lang/no.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/lang/no.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/month.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/month.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/skin.conf` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/skin.conf`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ###############################################################################
 # STANDARD SKIN CONFIGURATION FILE                                            #
 # Copyright (c) 2010-2021 Tom Keffer <tkeffer@gmail.com>                      #
 # See the file LICENSE.txt for your rights.                                   #
 ###############################################################################
 
 SKIN_NAME = Standard
-SKIN_VERSION = 5.0.0b8
+SKIN_VERSION = 5.0.0b9
 
 ###############################################################################
 
 # The following section is for any extra tags that you want to be available in the templates
 [Extras]
     
     # This radar image would be available as $Extras.radar_img
```

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/barometer.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/barometer.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/humidity.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/humidity.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x1.png` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x1.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x2.png` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/icons/icon_ipad_x2.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x1.png` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x1.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x2.png` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/icons/icon_iphone_x2.png`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/index.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/index.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/radar.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/radar.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/rain.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/rain.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/temp_outside.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/temp_outside.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/smartphone/wind.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/smartphone/wind.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/week.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/week.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/weewx.css` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/weewx.css`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/skins/Standard/year.html.tmpl` & `weewx-5.0.0b9/bin/wee_resources/skins/Standard/year.html.tmpl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/i18n/i18n-report` & `weewx-5.0.0b9/bin/wee_resources/util/i18n/i18n-report`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/import/csv-example.conf` & `weewx-5.0.0b9/bin/wee_resources/util/import/csv-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/import/cumulus-example.conf` & `weewx-5.0.0b9/bin/wee_resources/util/import/cumulus-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/import/wd-example.conf` & `weewx-5.0.0b9/bin/wee_resources/util/import/wd-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/import/weathercat-example.conf` & `weewx-5.0.0b9/bin/wee_resources/util/import/weathercat-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/import/wu-example.conf` & `weewx-5.0.0b9/bin/wee_resources/util/import/wu-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/init.d/weewx-multi` & `weewx-5.0.0b9/bin/wee_resources/util/init.d/weewx-multi`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/init.d/weewx.bsd` & `weewx-5.0.0b9/bin/wee_resources/util/init.d/weewx.bsd`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/init.d/weewx.debian` & `weewx-5.0.0b9/bin/wee_resources/util/init.d/weewx.debian`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/init.d/weewx.freebsd` & `weewx-5.0.0b9/bin/wee_resources/util/init.d/weewx.freebsd`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/init.d/weewx.lsb` & `weewx-5.0.0b9/bin/wee_resources/util/init.d/weewx.lsb`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/init.d/weewx.redhat` & `weewx-5.0.0b9/bin/wee_resources/util/init.d/weewx.redhat`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/init.d/weewx.suse` & `weewx-5.0.0b9/bin/wee_resources/util/init.d/weewx.suse`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/launchd/com.weewx.weewxd.plist` & `weewx-5.0.0b9/bin/wee_resources/util/launchd/com.weewx.weewxd.plist`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/logrotate.d/weewx` & `weewx-5.0.0b9/bin/wee_resources/util/logrotate.d/weewx`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/logwatch/scripts/services/weewx` & `weewx-5.0.0b9/bin/wee_resources/util/logwatch/scripts/services/weewx`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/rsyslog.d/weewx.conf` & `weewx-5.0.0b9/bin/wee_resources/util/rsyslog.d/weewx.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/solaris/weewx-smf.xml` & `weewx-5.0.0b9/bin/wee_resources/util/solaris/weewx-smf.xml`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/systemd/weewx.service` & `weewx-5.0.0b9/bin/wee_resources/util/systemd/weewx.service`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/udev/rules.d/vantage.rules` & `weewx-5.0.0b9/bin/wee_resources/util/udev/rules.d/vantage.rules`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/util/udev/rules.d/weewx.rules` & `weewx-5.0.0b9/bin/wee_resources/util/udev/rules.d/weewx.rules`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/wee_resources/weewx.conf` & `weewx-5.0.0b9/bin/wee_resources/weewx.conf`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # Whether to log successful operations. May get overridden below.
 log_success = True
 
 # Whether to log unsuccessful operations. May get overridden below.
 log_failure = True
 
 # Do not modify this. It is used when installing and updating weewx.
-version = 5.0.0b8
+version = 5.0.0b9
 
 ##############################################################################
 
 #   This section is for information about the station.
 
 [Station]
```

### Comparing `weewx-5.0.0b8/bin/weecfg/__init__.py` & `weewx-5.0.0b9/bin/weecfg/__init__.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weecfg/database.py` & `weewx-5.0.0b9/bin/weecfg/database.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weecfg/extension.py` & `weewx-5.0.0b9/bin/weecfg/extension.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weecfg/station_config.py` & `weewx-5.0.0b9/bin/weecfg/station_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -642,15 +642,15 @@
         # For Apache
         r"/home/weewx/public_html": rf"{os.path.join(weewx_root, 'public_html')}",
     }
     # Convert to a list of two-way tuples.
     re_list = [(re.compile(key), re_dict[key]) for key in re_dict]
 
     with weeutil.weeutil.path_to_resource('wee_resources', 'util') as util_resources:
-        dstdir = os.path.join(config_dict['WEEWX_ROOT'], 'util')
+        dstdir = os.path.join(weewx_root, 'util')
         print(f"Creating utility files in {dstdir}.")
         if not dry_run:
             _process_files(util_resources, dstdir, re_list)
 
     return dstdir
 
 
@@ -699,15 +699,15 @@
         print("This is a dry run. Nothing will actually be done.")
 
     # Retrieve the old configuration file as a ConfigObj:
     config_path, config_dict = weecfg.read_config(config_path)
 
     abbrev = {'config': 'configuration file',
               'docs': 'documentation',
-              'util': 'daemon utility files'}
+              'util': 'utility files'}
     choices = ', '.join([abbrev.get(p, p) for p in what])
     msg = f"\nUpgrade {choices} at {config_path}? (Y/n) "
 
     ans = weeutil.weeutil.y_or_n(msg, noprompt=no_prompt, default='y')
 
     if ans != 'y':
         print("Nothing done.")
```

### Comparing `weewx-5.0.0b8/bin/weecfg/update_config.py` & `weewx-5.0.0b9/bin/weecfg/update_config.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weectl.py` & `weewx-5.0.0b9/bin/weectl.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weectllib/__init__.py` & `weewx-5.0.0b9/bin/weectllib/__init__.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weectllib/database_cmd.py` & `weewx-5.0.0b9/bin/weectllib/database_cmd.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weectllib/db_actions.py` & `weewx-5.0.0b9/bin/weectllib/db_actions.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weectllib/extension_cmd.py` & `weewx-5.0.0b9/bin/weectllib/extension_cmd.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weectllib/station_cmd.py` & `weewx-5.0.0b9/bin/weectllib/station_cmd.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weedb/NOTES.md` & `weewx-5.0.0b9/bin/weedb/NOTES.md`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weedb/__init__.py` & `weewx-5.0.0b9/bin/weedb/__init__.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weedb/mysql.py` & `weewx-5.0.0b9/bin/weedb/mysql.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weedb/sqlite.py` & `weewx-5.0.0b9/bin/weedb/sqlite.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weeimport/csvimport.py` & `weewx-5.0.0b9/bin/weeimport/csvimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weeimport/cumulusimport.py` & `weewx-5.0.0b9/bin/weeimport/cumulusimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weeimport/wdimport.py` & `weewx-5.0.0b9/bin/weeimport/wdimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weeimport/weathercatimport.py` & `weewx-5.0.0b9/bin/weeimport/weathercatimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weeimport/weeimport.py` & `weewx-5.0.0b9/bin/weeimport/weeimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weeimport/wuimport.py` & `weewx-5.0.0b9/bin/weeimport/wuimport.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weeplot/genplot.py` & `weewx-5.0.0b9/bin/weeplot/genplot.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weeplot/utilities.py` & `weewx-5.0.0b9/bin/weeplot/utilities.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weeutil/Moon.py` & `weewx-5.0.0b9/bin/weeutil/Moon.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weeutil/Sun.py` & `weewx-5.0.0b9/bin/weeutil/Sun.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weeutil/config.py` & `weewx-5.0.0b9/bin/weeutil/config.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weeutil/ftpupload.py` & `weewx-5.0.0b9/bin/weeutil/ftpupload.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weeutil/log.py` & `weewx-5.0.0b9/bin/weeutil/log.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weeutil/logger.py` & `weewx-5.0.0b9/bin/weeutil/logger.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weeutil/rsyncupload.py` & `weewx-5.0.0b9/bin/weeutil/rsyncupload.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weeutil/timediff.py` & `weewx-5.0.0b9/bin/weeutil/timediff.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weeutil/weeutil.py` & `weewx-5.0.0b9/bin/weeutil/weeutil.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/__init__.py` & `weewx-5.0.0b9/bin/weewx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #    See the file LICENSE.txt for your full rights.
 #
 """Package weewx, containing modules specific to the weewx runtime engine."""
 import os.path
 import sys
 import time
 
-__version__ = "5.0.0b8"
+__version__ = "5.0.0b9"
 
 # Holds the program launch time in unix epoch seconds:
 # Useful for calculating 'uptime.'
 launchtime_ts = time.time()
 
 # Set to true for extra debug information:
 debug = False
```

### Comparing `weewx-5.0.0b8/bin/weewx/accum.py` & `weewx-5.0.0b9/bin/weewx/accum.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#    Copyright (c) 2009-2020 Tom Keffer <tkeffer@gmail.com>
+#    Copyright (c) 2009-2023 Tom Keffer <tkeffer@gmail.com>
 #
 #    See the file LICENSE.txt for your full rights.
 #
 """Statistical accumulators. They accumulate the highs, lows, averages, etc.,
 of a sequence of records."""
 #
 # General strategy.
@@ -100,90 +100,143 @@
 """
 defaults_dict = weeutil.config.config_from_str(DEFAULTS_INI)
 
 accum_dict = ListOfDicts(defaults_dict['Accumulator'].dict())
 
 
 class OutOfSpan(ValueError):
-    """Raised when attempting to add a record outside of the timespan held by an accumulator"""
+    """Raised when attempting to add a record outside the timespan held by an accumulator"""
 
 
 # ===============================================================================
-#                             ScalarStats
+#                             FirstLastAccum
 # ===============================================================================
 
-class ScalarStats(object):
-    """Accumulates statistics (min, max, average, etc.) for a scalar value.
-    
-    Property 'last' is the last non-None value seen. Property 'lasttime' is
-    the time it was seen. """
+class FirstLastAccum(object):
+    """Minimal accumulator, suitable for strings.
+    It can only return the first and last value it has seen, along with their timestamps.
+    """
 
     default_init = (None, None, None, None, 0.0, 0, 0.0, 0)
 
     def __init__(self, stats_tuple=None):
-        self.setStats(stats_tuple)
+        self.first = None
+        self.firsttime = None
         self.last = None
         self.lasttime = None
 
     def setStats(self, stats_tuple=None):
+        pass
+
+    def getStatsTuple(self):
+        """Return a stats-tuple. That is, a tuple containing the gathered statistics.
+        This tuple can be used to update the stats database"""
+        return FirstLastAccum.default_init
+
+    def mergeHiLo(self, x_stats):
+        """Merge the highs and lows of another accumulator into myself."""
+        if x_stats.firsttime is not None:
+            if self.firsttime is None or x_stats.firsttime < self.firsttime:
+                self.firsttime = x_stats.firsttime
+                self.first = x_stats.first
+        if x_stats.lasttime is not None:
+            if self.lasttime is None or x_stats.lasttime >= self.lasttime:
+                self.lasttime = x_stats.lasttime
+                self.last = x_stats.last
+
+    def mergeSum(self, x_stats):
+        """Merge the count of another accumulator into myself."""
+        pass
+
+    def addHiLo(self, val, ts):
+        """Include a value in my stats.
+        val: A value of almost any type.
+        ts:  The timestamp.
+        """
+        if val is not None:
+            if self.firsttime is None or ts < self.firsttime:
+                self.first = val
+                self.firsttime = ts
+            if self.lasttime is None or ts >= self.lasttime:
+                self.last = val
+                self.lasttime = ts
+
+    def addSum(self, val, weight=1):
+        """Add a scalar value to my running count."""
+        pass
+
+
+# ===============================================================================
+#                             ScalarStats
+# ===============================================================================
+
+class ScalarStats(FirstLastAccum):
+    """Accumulates statistics (min, max, average, etc.) for a scalar value."""
+
+    def __init__(self, stats_tuple=None):
+        # Call my superclass's version
+        FirstLastAccum.__init__(self, stats_tuple)
+        self.setStats(stats_tuple)
+
+    def setStats(self, stats_tuple=None):
         (self.min, self.mintime,
          self.max, self.maxtime,
          self.sum, self.count,
-         self.wsum, self.sumtime) = stats_tuple if stats_tuple else ScalarStats.default_init
+         self.wsum, self.sumtime) = stats_tuple if stats_tuple else FirstLastAccum.default_init
 
     def getStatsTuple(self):
         """Return a stats-tuple. That is, a tuple containing the gathered statistics.
         This tuple can be used to update the stats database"""
         return (self.min, self.mintime, self.max, self.maxtime,
                 self.sum, self.count, self.wsum, self.sumtime)
 
     def mergeHiLo(self, x_stats):
         """Merge the highs and lows of another accumulator into myself."""
+
+        # Call my superclass's version
+        FirstLastAccum.mergeHiLo(self, x_stats)
+
         if x_stats.min is not None:
             if self.min is None or x_stats.min < self.min:
                 self.min = x_stats.min
                 self.mintime = x_stats.mintime
         if x_stats.max is not None:
             if self.max is None or x_stats.max > self.max:
                 self.max = x_stats.max
                 self.maxtime = x_stats.maxtime
-        if x_stats.lasttime is not None:
-            if self.lasttime is None or x_stats.lasttime >= self.lasttime:
-                self.lasttime = x_stats.lasttime
-                self.last = x_stats.last
 
     def mergeSum(self, x_stats):
         """Merge the sum and count of another accumulator into myself."""
         self.sum += x_stats.sum
         self.count += x_stats.count
         self.wsum += x_stats.wsum
         self.sumtime += x_stats.sumtime
 
     def addHiLo(self, val, ts):
         """Include a scalar value in my highs and lows.
         val: A scalar value
         ts:  The timestamp. """
 
+        # Call my superclass's version:
+        FirstLastAccum.addHiLo(self, val, ts)
+
         # If necessary, convert to float. Be prepared to catch an exception if not possible.
         try:
             val = to_float(val)
         except ValueError:
             val = None
 
         # Check for None and NaN:
         if val is not None and val == val:
             if self.min is None or val < self.min:
                 self.min = val
                 self.mintime = ts
             if self.max is None or val > self.max:
                 self.max = val
                 self.maxtime = ts
-            if self.lasttime is None or ts >= self.lasttime:
-                self.last = val
-                self.lasttime = ts
 
     def addSum(self, val, weight=1):
         """Add a scalar value to my running sum and count."""
 
         # If necessary, convert to float. Be prepared to catch an exception if not possible.
         try:
             val = to_float(val)
@@ -198,14 +251,18 @@
             self.sumtime += weight
 
     @property
     def avg(self):
         return self.wsum / self.sumtime if self.count else None
 
 
+# ===============================================================================
+#                             VecStats
+# ===============================================================================
+
 class VecStats(object):
     """Accumulates statistics for a vector value.
      
     Property 'last' is the last non-None value seen. It is a two-way tuple (mag, dir).
     Property 'lasttime' is the time it was seen. """
 
     default_init = (None, None, None, None,
@@ -344,74 +401,14 @@
                 _result += 360.0
             return _result
         # Return the last known direction when our vector sum is 0
         return self.last[1]
 
 
 # ===============================================================================
-#                             FirstLastAccum
-# ===============================================================================
-
-class FirstLastAccum(object):
-    """Minimal accumulator, suitable for strings.
-    It can only return the first and last strings it has seen, along with their timestamps.
-    """
-
-    default_init = (None, None, None, None)
-
-    def __init__(self, stats_tuple=None):
-        self.first = None
-        self.firsttime = None
-        self.last = None
-        self.lasttime = None
-
-    def setStats(self, stats_tuple=None):
-        self.first, self.firsttime, self.last, self.lasttime = stats_tuple \
-            if stats_tuple else FirstLastAccum.default_init
-
-    def getStatsTuple(self):
-        """Return a stats-tuple. That is, a tuple containing the gathered statistics.
-        This tuple can be used to update the stats database"""
-        return self.first, self.firsttime, self.last, self.lasttime
-
-    def mergeHiLo(self, x_stats):
-        """Merge the highs and lows of another accumulator into myself."""
-        if x_stats.firsttime is not None:
-            if self.firsttime is None or x_stats.firsttime < self.firsttime:
-                self.firsttime = x_stats.firsttime
-                self.first = x_stats.first
-        if x_stats.lasttime is not None:
-            if self.lasttime is None or x_stats.lasttime >= self.lasttime:
-                self.lasttime = x_stats.lasttime
-                self.last = x_stats.last
-
-    def mergeSum(self, x_stats):
-        """Merge the count of another accumulator into myself."""
-        pass
-
-    def addHiLo(self, val, ts):
-        """Include a value in my stats.
-        val: A value of almost any type. It will be converted to a string before being accumulated.
-        ts:  The timestamp.
-        """
-        if val is not None:
-            string_val = val
-            if self.firsttime is None or ts < self.firsttime:
-                self.first = string_val
-                self.firsttime = ts
-            if self.lasttime is None or ts >= self.lasttime:
-                self.last = string_val
-                self.lasttime = ts
-
-    def addSum(self, val, weight=1):
-        """Add a scalar value to my running count."""
-        pass
-
-
-# ===============================================================================
 #                             Class Accum
 # ===============================================================================
 
 class Accum(dict):
     """Accumulates statistics for a set of observation types."""
 
     def __init__(self, timespan, unit_system=None):
@@ -579,14 +576,17 @@
             record['windGust'] = self[obs_type].max
         if 'windGustDir' not in record:
             record['windGustDir'] = self[obs_type].max_dir
 
     def extract_sum(self, record, obs_type):
         record[obs_type] = self[obs_type].sum if self[obs_type].count else None
 
+    def extract_first(self, record, obs_type):
+        record[obs_type] = self[obs_type].first
+
     def extract_last(self, record, obs_type):
         record[obs_type] = self[obs_type].last
 
     def extract_avg(self, record, obs_type):
         record[obs_type] = self[obs_type].avg
 
     def extract_min(self, record, obs_type):
@@ -653,14 +653,15 @@
     'minmax': Accum.merge_minmax,
     'avg': Accum.merge_avg
 }
 
 EXTRACT_FUNCTIONS = {
     'avg': Accum.extract_avg,
     'count': Accum.extract_count,
+    'first' : Accum.extract_first,
     'last': Accum.extract_last,
     'max': Accum.extract_max,
     'min': Accum.extract_min,
     'noop': Accum.noop,
     'sum': Accum.extract_sum,
     'wind': Accum.extract_wind,
 }
```

### Comparing `weewx-5.0.0b8/bin/weewx/almanac.py` & `weewx-5.0.0b9/bin/weewx/almanac.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,15 +370,18 @@
 
 
 class AlmanacBinder(object):
     """This class binds the observer properties held in Almanac, with the heavenly
     body to be observed."""
 
     pyephem_map = {'azimuth': 'az', 'altitude': 'alt', 'astro_ra': 'a_ra', 'astro_dec': 'a_dec',
-                   'geo_ra': 'g_ra', 'geo_dec': 'g_dec', 'topo_ra': 'ra', 'topo_dec': 'dec'}
+                   'geo_ra': 'g_ra', 'topo_ra': 'ra', 'geo_dec': 'g_dec','topo_dec': 'dec',
+                   'elongation':'elong', 'radius_size': 'radius',
+                   'hlongitude': 'hlon', 'hlatitude': 'hlat',
+                   'sublatitude': 'sublat', 'sublongitude': 'sublong'}
 
     def __init__(self, almanac, heavenly_body):
         self.almanac = almanac
 
         # Calculate and store the start-of-day in Dublin Julian Days. 
         y, m, d = time.localtime(self.almanac.time_ts)[0:3]
         self.sod_djd = timestamp_to_djd(time.mktime((y, m, d, 0, 0, 0, 0, 0, -1)))
@@ -479,32 +482,35 @@
         else:
             # These functions need the current time in Dublin Julian Days
             observer = _get_observer(self.almanac, self.almanac.time_djd)
             ephem_body.compute(observer)
             # V5.0 changed the name of some attributes, so they could be returned as
             # a ValueHelper, instead of a floating point number. This would break existing skins,
             # so new attribute names are being used.
-            if attr in {'azimuth', 'altitude', 'astro_ra', 'astro_dec',
-                        'geo_ra', 'geo_dec', 'topo_ra', 'topo_dec', 'elong', 'radius',
-                        'hlon', 'hlat', 'sublat', 'sublong'}:
+            if attr in AlmanacBinder.pyephem_map:
                 # Map the name to the name pyephem uses...
-                pyephem_name = AlmanacBinder.pyephem_map.get(attr, attr)
+                pyephem_name = AlmanacBinder.pyephem_map[attr]
                 # ... then calculate the value in radians ...
                 val = getattr(ephem_body, pyephem_name)
                 # ... form the proper ValueTuple ...
-                if attr in {'azimuth', 'astro_ra', 'geo_ra', 'topo_ra', 'hlon', 'sublong'}:
+                if attr in {'azimuth', 'astro_ra', 'geo_ra', 'topo_ra',
+                            'hlongitude', 'sublongitude'}:
                     vt = ValueTuple(math.degrees(val), 'degree_compass', 'group_direction')
                 else:
                     vt = ValueTuple(val, 'radian', 'group_angle')
                 # ... and, finally, return the ValueHelper:
                 return weewx.units.ValueHelper(vt,
                                                context="ephem_day",
                                                formatter=self.almanac.formatter,
                                                converter=self.almanac.converter)
-            elif attr in {'az', 'alt', 'a_ra', 'a_dec', 'g_ra', 'ra', 'g_dec', 'dec',}:
+            elif attr in {'az', 'alt', 'a_ra', 'a_dec',
+                          'g_ra', 'ra', 'g_dec', 'dec',
+                          'elong', 'radius',
+                          'hlong', 'hlat',
+                          'sublat', 'sublong'}:
                 # These are the old names, which return a floating point number in decimal degrees.
                 return math.degrees(getattr(ephem_body, attr))
             elif attr == 'moon_fullness':
                 # The attribute "moon_fullness" is the percentage of the moon surface that is
                 # illuminated. Unfortunately, phephem calls it "moon_phase", so call ephem with
                 # that name. Return the result in percent.
                 return 100.0 * ephem_body.moon_phase
```

### Comparing `weewx-5.0.0b8/bin/weewx/cheetahgenerator.py` & `weewx-5.0.0b9/bin/weewx/cheetahgenerator.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/crc16.py` & `weewx-5.0.0b9/bin/weewx/crc16.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/daemon.py` & `weewx-5.0.0b9/bin/weewx/daemon.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/defaults.py` & `weewx-5.0.0b9/bin/weewx/defaults.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/drivers/__init__.py` & `weewx-5.0.0b9/bin/weewx/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/drivers/acurite.py` & `weewx-5.0.0b9/bin/weewx/drivers/acurite.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/drivers/cc3000.py` & `weewx-5.0.0b9/bin/weewx/drivers/cc3000.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/drivers/fousb.py` & `weewx-5.0.0b9/bin/weewx/drivers/fousb.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/drivers/simulator.py` & `weewx-5.0.0b9/bin/weewx/drivers/simulator.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/drivers/te923.py` & `weewx-5.0.0b9/bin/weewx/drivers/te923.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/drivers/ultimeter.py` & `weewx-5.0.0b9/bin/weewx/drivers/ultimeter.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/drivers/vantage.py` & `weewx-5.0.0b9/bin/weewx/drivers/vantage.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/drivers/wmr100.py` & `weewx-5.0.0b9/bin/weewx/drivers/wmr100.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/drivers/wmr300.py` & `weewx-5.0.0b9/bin/weewx/drivers/wmr300.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/drivers/wmr9x8.py` & `weewx-5.0.0b9/bin/weewx/drivers/wmr9x8.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/drivers/ws1.py` & `weewx-5.0.0b9/bin/weewx/drivers/ws1.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/drivers/ws23xx.py` & `weewx-5.0.0b9/bin/weewx/drivers/ws23xx.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/drivers/ws28xx.py` & `weewx-5.0.0b9/bin/weewx/drivers/ws28xx.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/engine.py` & `weewx-5.0.0b9/bin/weewx/engine.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/imagegenerator.py` & `weewx-5.0.0b9/bin/weewx/imagegenerator.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/manager.py` & `weewx-5.0.0b9/bin/weewx/manager.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/qc.py` & `weewx-5.0.0b9/bin/weewx/qc.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/reportengine.py` & `weewx-5.0.0b9/bin/weewx/reportengine.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/restx.py` & `weewx-5.0.0b9/bin/weewx/restx.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/station.py` & `weewx-5.0.0b9/bin/weewx/station.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/tags.py` & `weewx-5.0.0b9/bin/weewx/tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,27 +31,27 @@
 
     def __init__(self, db_lookup, report_time,
                  formatter=None,
                  converter=None,
                  **option_dict):
         """Initialize an instance of DatabaseBinder.
 
-        db_lookup: A function with call signature db_lookup(data_binding), which returns a database
-        manager and where data_binding is an optional binding name. If not given, then a default
-        binding will be used.
-
-        report_time: The time for which the report should be run.
-
-        formatter: An instance of weewx.units.Formatter() holding the formatting information to be
-        used. [Optional. If not given, the default Formatter will be used.]
-
-        converter: An instance of weewx.units.Converter() holding the target unit information to be
-        used. [Optional. If not given, the default Converter will be used.]
-
-        option_dict: Other options which can be used to customize calculations. [Optional.]
+        Args:
+            db_lookup (function|None): A function with call signature db_lookup(data_binding),
+                which returns a database manager and where data_binding is an optional binding
+                name. If not given, then a default binding will be used.
+            report_time(float): The time for which the report should be run.
+            formatter (weewx.units.Formatter|None): An instance of weewx.units.Formatter() holding
+                the formatting information to be used. [Optional. If not given, the default
+                Formatter will be used.]
+            converter (weewx.units.Converter|None): An instance of weewx.units.Converter() holding
+                the target unit information to be used. [Optional. If not given, the default
+                Converter will be used.]
+            option_dict (dict|None): Other options which can be used to customize calculations.
+                [Optional.]
         """
         self.db_lookup = db_lookup
         self.report_time = report_time
         self.formatter = formatter or weewx.units.Formatter()
         self.converter = converter or weewx.units.Converter()
         self.option_dict = option_dict
 
@@ -319,28 +319,27 @@
         """ Initialize an instance of ObservationBinder
 
         Args:
             obs_type (str): A string with the stats type (e.g., 'outTemp') for which the query is
                 to be done.
             timespan (weeutil.weeutil.TimeSpan): An instance of TimeSpan holding the time period
                 over which the query is to be run.
-            db_lookup (function): A function with call signature db_lookup(data_binding), which
-                returns a database manager and where data_binding is an optional binding name. If
-                not given, then a default binding will be used.
-
+            db_lookup (function|None): A function with call signature db_lookup(data_binding),
+                which returns a database manager and where data_binding is an optional binding
+                name. If not given, then a default binding will be used.
             data_binding (str): If non-None, then use this data binding.
             context (str): A tag name for the timespan. This is something like 'current', 'day',
                 'week', etc. This is used to find an appropriate label, if necessary.
             formatter (weewx.units.Formatter|None): An instance of weewx.units.Formatter() holding
                 the formatting information to be used. [Optional. If not given, the default
                 Formatter will be used.]
             converter (weewx.units.Converter|None): An instance of weewx.units.Converter() holding
                 the target unit information to be used. [Optional. If not given, the default
                 Converter will be used.]
-            option_dict (dict|None: Other options which can be used to customize calculations.
+            option_dict (dict|None): Other options which can be used to customize calculations.
                 [Optional.]
         """
 
         self.obs_type = obs_type
         self.timespan = timespan
         self.db_lookup = db_lookup
         self.data_binding = data_binding
```

### Comparing `weewx-5.0.0b8/bin/weewx/units.py` & `weewx-5.0.0b9/bin/weewx/units.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/uwxutils.py` & `weewx-5.0.0b9/bin/weewx/uwxutils.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/wxformulas.py` & `weewx-5.0.0b9/bin/weewx/wxformulas.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/wxservices.py` & `weewx-5.0.0b9/bin/weewx/wxservices.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/wxxtypes.py` & `weewx-5.0.0b9/bin/weewx/wxxtypes.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewx/xtypes.py` & `weewx-5.0.0b9/bin/weewx/xtypes.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/bin/weewxd.py` & `weewx-5.0.0b9/bin/weewxd.py`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/pkg/changelog.el` & `weewx-5.0.0b9/pkg/changelog.el`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/pkg/changelog.suse` & `weewx-5.0.0b9/pkg/changelog.suse`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/pkg/debian/README` & `weewx-5.0.0b9/pkg/debian/README`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/pkg/debian/changelog` & `weewx-5.0.0b9/pkg/debian/changelog`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+weewx (5.0.0b9-1) unstable; urgency=low
+  * new upstream release
+ -- Thomas Keffer (Author of weewx) <tkeffer@gmail.com>  Fri, 14 Jul 2023 06:25:50 -0700
 weewx (5.0.0b3-1) unstable; urgency=low
   * Update version numbers
  -- Thomas Keffer (Author of weewx) <tkeffer@gmail.com>  Sat, 27 May 2023 08:03:33 -0700
 weewx (5.0.0b2-1) unstable; urgency=low
   * Remove utility wunderfixer.
   * Most almanac attributes now return a ValueHelper.
  -- Thomas Keffer (Author of weewx) <tkeffer@gmail.com>  Sat, 27 May 2023 05:07:43 -0700
```

### Comparing `weewx-5.0.0b8/pkg/debian/config` & `weewx-5.0.0b9/pkg/debian/config`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/pkg/debian/control` & `weewx-5.0.0b9/pkg/debian/control`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/pkg/debian/copyright` & `weewx-5.0.0b9/pkg/debian/copyright`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/pkg/debian/postinst` & `weewx-5.0.0b9/pkg/debian/postinst`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/pkg/debian/postrm` & `weewx-5.0.0b9/pkg/debian/postrm`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/pkg/debian/prerm` & `weewx-5.0.0b9/pkg/debian/prerm`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/pkg/debian/rules` & `weewx-5.0.0b9/pkg/debian/rules`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/pkg/debian/templates` & `weewx-5.0.0b9/pkg/debian/templates`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/pkg/index-apt.html` & `weewx-5.0.0b9/pkg/index-apt.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/pkg/index-suse.html` & `weewx-5.0.0b9/pkg/index-suse.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/pkg/index-yum.html` & `weewx-5.0.0b9/pkg/index-yum.html`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/pkg/mkchangelog.pl` & `weewx-5.0.0b9/pkg/mkchangelog.pl`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/pkg/weewx.smf` & `weewx-5.0.0b9/pkg/weewx.smf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/pkg/weewx.spec.in` & `weewx-5.0.0b9/pkg/weewx.spec.in`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/pyproject.toml` & `weewx-5.0.0b9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weewx"
-version = "5.0.0b8"
+version = "5.0.0b9"
 description = "The WeeWX weather software system. This is an BETA release, and may have many bugs!"
 authors = ["Tom Keffer <tkeffer@gmail.com>"]
 license = "GPL3"
 readme = 'README.md'
 repository = "https://github.com/weewx/weewx"
 homepage = "https://weewx.com"
 documentation = "https://weewx.com/docs"
```

### Comparing `weewx-5.0.0b8/util/i18n/i18n-report` & `weewx-5.0.0b9/util/i18n/i18n-report`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/import/csv-example.conf` & `weewx-5.0.0b9/util/import/csv-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/import/cumulus-example.conf` & `weewx-5.0.0b9/util/import/cumulus-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/import/wd-example.conf` & `weewx-5.0.0b9/util/import/wd-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/import/weathercat-example.conf` & `weewx-5.0.0b9/util/import/weathercat-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/import/wu-example.conf` & `weewx-5.0.0b9/util/import/wu-example.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/init.d/weewx-multi` & `weewx-5.0.0b9/util/init.d/weewx-multi`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/init.d/weewx.bsd` & `weewx-5.0.0b9/util/init.d/weewx.bsd`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/init.d/weewx.debian` & `weewx-5.0.0b9/util/init.d/weewx.debian`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/init.d/weewx.freebsd` & `weewx-5.0.0b9/util/init.d/weewx.freebsd`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/init.d/weewx.lsb` & `weewx-5.0.0b9/util/init.d/weewx.lsb`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/init.d/weewx.redhat` & `weewx-5.0.0b9/util/init.d/weewx.redhat`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/init.d/weewx.suse` & `weewx-5.0.0b9/util/init.d/weewx.suse`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/launchd/com.weewx.weewxd.plist` & `weewx-5.0.0b9/util/launchd/com.weewx.weewxd.plist`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/logrotate.d/weewx` & `weewx-5.0.0b9/util/logrotate.d/weewx`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/logwatch/scripts/services/weewx` & `weewx-5.0.0b9/util/logwatch/scripts/services/weewx`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/rsyslog.d/weewx.conf` & `weewx-5.0.0b9/util/rsyslog.d/weewx.conf`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/solaris/weewx-smf.xml` & `weewx-5.0.0b9/util/solaris/weewx-smf.xml`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/systemd/weewx.service` & `weewx-5.0.0b9/util/systemd/weewx.service`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/udev/rules.d/vantage.rules` & `weewx-5.0.0b9/util/udev/rules.d/vantage.rules`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/util/udev/rules.d/weewx.rules` & `weewx-5.0.0b9/util/udev/rules.d/weewx.rules`

 * *Files identical despite different names*

### Comparing `weewx-5.0.0b8/PKG-INFO` & `weewx-5.0.0b9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weewx
-Version: 5.0.0b8
+Version: 5.0.0b9
 Summary: The WeeWX weather software system. This is an BETA release, and may have many bugs!
 Home-page: https://weewx.com
 License: GPL3
 Author: Tom Keffer
 Author-email: tkeffer@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

