# Comparing `tmp/laok-0.2.18.tar.gz` & `tmp/laok-0.2.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laok-0.2.18.tar", last modified: Tue Jul  4 02:41:42 2023, max compression
+gzip compressed data, was "laok-0.2.19.tar", last modified: Fri Jul 14 03:08:54 2023, max compression
```

## Comparing `laok-0.2.18.tar` & `laok-0.2.19.tar`

### file list

```diff
@@ -1,200 +1,182 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.576877 laok-0.2.18/
--rw-rw-rw-   0        0        0      217 2023-07-04 02:41:42.576877 laok-0.2.18/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.383395 laok-0.2.18/laok/
--rw-rw-rw-   0        0        0       21 2023-06-01 07:56:50.000000 laok-0.2.18/laok/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.389380 laok-0.2.18/laok/base/
--rw-rw-rw-   0        0        0      248 2023-06-06 13:49:22.000000 laok-0.2.18/laok/base/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.391374 laok-0.2.18/laok/base/alg/
--rw-rw-rw-   0        0        0       26 2023-04-20 13:21:17.000000 laok-0.2.18/laok/base/alg/__init__.py
--rw-rw-rw-   0        0        0     4923 2023-04-20 13:20:53.000000 laok-0.2.18/laok/base/alg/addict.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.396360 laok-0.2.18/laok/base/conf/
--rw-rw-rw-   0        0        0       32 2023-06-10 01:32:44.000000 laok-0.2.18/laok/base/conf/__init__.py
--rw-rw-rw-   0        0        0      360 2023-04-19 14:40:47.000000 laok-0.2.18/laok/base/conf/conf_global.py
--rw-rw-rw-   0        0        0     3022 2023-06-10 01:32:49.000000 laok-0.2.18/laok/base/conf/factory.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.400349 laok-0.2.18/laok/base/dataset/
--rw-rw-rw-   0        0        0        0 2023-04-21 04:27:16.000000 laok-0.2.18/laok/base/dataset/__init__.py
--rw-rw-rw-   0        0        0     6406 2023-04-21 04:29:54.000000 laok-0.2.18/laok/base/dataset/cvt_voc_yolo.py
--rw-rw-rw-   0        0        0     2405 2019-09-12 10:55:17.000000 laok-0.2.18/laok/base/dataset/darknet-voc2yolo.py
--rw-rw-rw-   0        0        0     2241 2019-02-18 15:12:05.000000 laok-0.2.18/laok/base/dataset/voc_label.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.404338 laok-0.2.18/laok/base/dtime/
--rw-rw-rw-   0        0        0       47 2022-10-21 10:13:37.000000 laok-0.2.18/laok/base/dtime/__init__.py
--rw-rw-rw-   0        0        0      556 2022-11-17 01:18:56.000000 laok-0.2.18/laok/base/dtime/datetime_.py
--rw-rw-rw-   0        0        0     2727 2023-04-19 11:27:09.000000 laok-0.2.18/laok/base/dtime/timer.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.411320 laok-0.2.18/laok/base/fs/
--rw-rw-rw-   0        0        0      134 2023-05-04 11:06:57.000000 laok-0.2.18/laok/base/fs/__init__.py
--rw-rw-rw-   0        0        0     2591 2023-06-27 16:15:40.000000 laok-0.2.18/laok/base/fs/fdata.py
--rw-rw-rw-   0        0        0     2937 2022-11-03 16:22:33.000000 laok-0.2.18/laok/base/fs/fname.py
--rw-rw-rw-   0        0        0     4629 2023-06-27 16:03:41.000000 laok-0.2.18/laok/base/fs/fpath.py
--rw-rw-rw-   0        0        0     1785 2023-05-04 11:06:06.000000 laok-0.2.18/laok/base/fs/fsearch.py
--rw-rw-rw-   0        0        0     2819 2023-05-05 03:57:37.000000 laok-0.2.18/laok/base/fs/fwalk.py
--rw-rw-rw-   0        0        0     1413 2023-04-19 09:23:34.000000 laok-0.2.18/laok/base/fs/name_index.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.413315 laok-0.2.18/laok/base/log/
--rw-rw-rw-   0        0        0       50 2023-04-19 14:41:08.000000 laok-0.2.18/laok/base/log/__init__.py
--rw-rw-rw-   0        0        0     2185 2023-04-19 14:41:16.000000 laok-0.2.18/laok/base/log/log.py
--rw-rw-rw-   0        0        0      672 2023-04-19 14:43:17.000000 laok-0.2.18/laok/base/log/log_default.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.417303 laok-0.2.18/laok/base/net/
--rw-rw-rw-   0        0        0       78 2023-06-06 16:23:58.000000 laok-0.2.18/laok/base/net/__init__.py
--rw-rw-rw-   0        0        0      691 2022-09-23 00:45:15.000000 laok-0.2.18/laok/base/net/ip.py
--rw-rw-rw-   0        0        0     3792 2023-06-27 10:59:29.000000 laok-0.2.18/laok/base/net/requests_.py
--rw-rw-rw-   0        0        0     1200 2023-06-27 10:55:31.000000 laok-0.2.18/laok/base/net/url.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.420296 laok-0.2.18/laok/base/paral/
--rw-rw-rw-   0        0        0       20 2022-10-21 10:13:37.000000 laok-0.2.18/laok/base/paral/__init__.py
--rw-rw-rw-   0        0        0     2010 2023-04-20 15:21:46.000000 laok-0.2.18/laok/base/paral/pool.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.424289 laok-0.2.18/laok/base/pkg/
--rw-rw-rw-   0        0        0       32 2023-07-03 15:46:47.000000 laok-0.2.18/laok/base/pkg/__init__.py
--rw-rw-rw-   0        0        0    27875 2023-07-03 15:50:30.000000 laok-0.2.18/laok/base/pkg/_lazy.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.433261 laok-0.2.18/laok/base/ser/
--rw-rw-rw-   0        0        0      156 2023-06-06 14:13:13.000000 laok-0.2.18/laok/base/ser/__init__.py
--rw-rw-rw-   0        0        0     1367 2023-04-25 06:50:06.000000 laok-0.2.18/laok/base/ser/json_.py
--rw-rw-rw-   0        0        0      750 2023-04-20 13:46:22.000000 laok-0.2.18/laok/base/ser/marshal_.py
--rw-rw-rw-   0        0        0      676 2023-06-01 07:58:10.000000 laok-0.2.18/laok/base/ser/numpy_.py
--rw-rw-rw-   0        0        0      621 2023-04-25 06:50:29.000000 laok-0.2.18/laok/base/ser/pickle_.py
--rw-rw-rw-   0        0        0     1369 2023-06-10 01:42:11.000000 laok-0.2.18/laok/base/ser/torch_.py
--rw-rw-rw-   0        0        0     1452 2023-06-06 17:03:52.000000 laok-0.2.18/laok/base/ser/xml_.py
--rw-rw-rw-   0        0        0     1341 2023-06-01 07:57:17.000000 laok-0.2.18/laok/base/ser/yaml_.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.443234 laok-0.2.18/laok/base/str/
--rw-rw-rw-   0        0        0       84 2023-06-10 01:11:15.000000 laok-0.2.18/laok/base/str/__init__.py
--rw-rw-rw-   0        0        0      735 2023-06-10 01:09:44.000000 laok-0.2.18/laok/base/str/cvt.py
--rw-rw-rw-   0        0        0      427 2023-06-10 01:10:45.000000 laok-0.2.18/laok/base/str/fmt.py
--rw-rw-rw-   0        0        0     1705 2023-06-10 01:10:56.000000 laok-0.2.18/laok/base/str/misc.py
--rw-rw-rw-   0        0        0     2588 2023-06-01 07:58:57.000000 laok-0.2.18/laok/base/str/print_info.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.446226 laok-0.2.18/laok/base/syst/
--rw-rw-rw-   0        0        0       74 2023-07-03 11:23:20.000000 laok-0.2.18/laok/base/syst/__init__.py
--rw-rw-rw-   0        0        0      518 2023-05-04 15:23:10.000000 laok-0.2.18/laok/base/syst/platform_.py
--rw-rw-rw-   0        0        0     1871 2022-10-21 10:13:37.000000 laok-0.2.18/laok/base/syst/print_info.py
--rw-rw-rw-   0        0        0      380 2023-07-03 11:23:24.000000 laok-0.2.18/laok/base/syst/sys_.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.451216 laok-0.2.18/laok/base/test/
--rw-rw-rw-   0        0        0       43 2022-10-21 10:13:37.000000 laok-0.2.18/laok/base/test/__init__.py
--rw-rw-rw-   0        0        0     8046 2023-06-01 03:25:20.000000 laok-0.2.18/laok/base/test/_dump.py
--rw-rw-rw-   0        0        0     4551 2023-06-01 05:41:11.000000 laok-0.2.18/laok/base/test/_run.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.452212 laok-0.2.18/laok/cv2d/
--rw-rw-rw-   0        0        0       62 2023-05-12 07:14:57.000000 laok-0.2.18/laok/cv2d/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.461186 laok-0.2.18/laok/cv2d/cvt/
--rw-rw-rw-   0        0        0       86 2022-11-15 13:19:23.000000 laok-0.2.18/laok/cv2d/cvt/__init__.py
--rw-rw-rw-   0        0        0     2974 2022-11-15 13:18:48.000000 laok-0.2.18/laok/cv2d/cvt/cv2_.py
--rw-rw-rw-   0        0        0     2075 2022-10-16 09:36:58.000000 laok-0.2.18/laok/cv2d/cvt/misc_.py
--rw-rw-rw-   0        0        0      430 2022-09-04 16:11:38.000000 laok-0.2.18/laok/cv2d/cvt/pil_.py
--rw-rw-rw-   0        0        0      469 2022-09-04 16:11:47.000000 laok-0.2.18/laok/cv2d/cvt/sk_.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.465175 laok-0.2.18/laok/cv2d/draw/
--rw-rw-rw-   0        0        0       45 2022-10-24 11:22:11.000000 laok-0.2.18/laok/cv2d/draw/__init__.py
--rw-rw-rw-   0        0        0     8383 2022-10-18 15:38:38.000000 laok-0.2.18/laok/cv2d/draw/color.py
--rw-rw-rw-   0        0        0      975 2023-06-01 05:40:03.000000 laok-0.2.18/laok/cv2d/draw/cv2_.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.469167 laok-0.2.18/laok/cv2d/io/
--rw-rw-rw-   0        0        0       42 2023-05-12 07:11:13.000000 laok-0.2.18/laok/cv2d/io/__init__.py
--rw-rw-rw-   0        0        0     3226 2023-06-06 13:44:51.000000 laok-0.2.18/laok/cv2d/io/cv2_.py
--rw-rw-rw-   0        0        0      592 2023-06-06 13:41:32.000000 laok-0.2.18/laok/cv2d/io/pil_.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.473156 laok-0.2.18/laok/cv2d/morph/
--rw-rw-rw-   0        0        0       21 2023-05-12 07:10:07.000000 laok-0.2.18/laok/cv2d/morph/__init__.py
--rw-rw-rw-   0        0        0     3471 2023-06-06 13:41:42.000000 laok-0.2.18/laok/cv2d/morph/cv2_.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.478143 laok-0.2.18/laok/cv2d/show/
--rw-rw-rw-   0        0        0       63 2023-05-12 07:14:23.000000 laok-0.2.18/laok/cv2d/show/__init__.py
--rw-rw-rw-   0        0        0     1164 2023-06-06 13:42:01.000000 laok-0.2.18/laok/cv2d/show/cv2_.py
--rw-rw-rw-   0        0        0        0 2023-05-12 08:19:43.000000 laok-0.2.18/laok/cv2d/show/pil_.py
--rw-rw-rw-   0        0        0     1057 2023-07-03 15:41:51.000000 laok-0.2.18/laok/cv2d/show/plt_.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.480136 laok-0.2.18/laok/cv3d/
--rw-rw-rw-   0        0        0       64 2023-04-21 09:21:19.000000 laok-0.2.18/laok/cv3d/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.483132 laok-0.2.18/laok/cv3d/io/
--rw-rw-rw-   0        0        0       24 2023-04-21 09:18:03.000000 laok-0.2.18/laok/cv3d/io/__init__.py
--rw-rw-rw-   0        0        0      832 2023-04-25 06:52:21.000000 laok-0.2.18/laok/cv3d/io/_simple.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.484130 laok-0.2.18/laok/cv3d/show/
--rw-rw-rw-   0        0        0       21 2023-04-21 09:20:03.000000 laok-0.2.18/laok/cv3d/show/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.489121 laok-0.2.18/laok/cv3d/show/vtk_/
--rw-rw-rw-   0        0        0      804 2023-04-21 09:21:01.000000 laok-0.2.18/laok/cv3d/show/vtk_/__init__.py
--rw-rw-rw-   0        0        0     3916 2022-10-21 10:13:38.000000 laok-0.2.18/laok/cv3d/show/vtk_/win.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.504075 laok-0.2.18/laok/cv3d/trans/
--rw-rw-rw-   0        0        0      220 2023-06-16 08:02:42.000000 laok-0.2.18/laok/cv3d/trans/__init__.py
--rw-rw-rw-   0        0        0      895 2023-04-25 05:31:18.000000 laok-0.2.18/laok/cv3d/trans/_dropout.py
--rw-rw-rw-   0        0        0      726 2023-04-25 05:40:44.000000 laok-0.2.18/laok/cv3d/trans/_jitter.py
--rw-rw-rw-   0        0        0      660 2023-04-25 03:33:54.000000 laok-0.2.18/laok/cv3d/trans/_normal.py
--rw-rw-rw-   0        0        0     5025 2023-04-27 08:53:41.000000 laok-0.2.18/laok/cv3d/trans/_rotate.py
--rw-rw-rw-   0        0        0     2164 2023-04-28 03:50:24.000000 laok-0.2.18/laok/cv3d/trans/_sample.py
--rw-rw-rw-   0        0        0      618 2023-04-25 02:57:52.000000 laok-0.2.18/laok/cv3d/trans/_scale.py
--rw-rw-rw-   0        0        0      585 2023-06-16 09:05:52.000000 laok-0.2.18/laok/cv3d/trans/_swap_filed.py
--rw-rw-rw-   0        0        0      485 2023-04-25 03:05:55.000000 laok-0.2.18/laok/cv3d/trans/_torch.py
--rw-rw-rw-   0        0        0      680 2023-04-25 05:38:23.000000 laok-0.2.18/laok/cv3d/trans/_translate.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.507065 laok-0.2.18/laok/dnn/
--rw-rw-rw-   0        0        0       87 2023-04-23 12:48:28.000000 laok-0.2.18/laok/dnn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.510056 laok-0.2.18/laok/dnn/backbones/
--rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.18/laok/dnn/backbones/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.512051 laok-0.2.18/laok/dnn/dataset/
--rw-rw-rw-   0        0        0       58 2023-04-25 06:10:55.000000 laok-0.2.18/laok/dnn/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.514055 laok-0.2.18/laok/dnn/dataset/cld/
--rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.18/laok/dnn/dataset/cld/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.515044 laok-0.2.18/laok/dnn/dataset/img/
--rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.18/laok/dnn/dataset/img/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.517037 laok-0.2.18/laok/dnn/dataset/txt/
--rw-rw-rw-   0        0        0       38 2023-04-25 06:10:39.000000 laok-0.2.18/laok/dnn/dataset/txt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.522024 laok-0.2.18/laok/dnn/head/
--rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.18/laok/dnn/head/__init__.py
--rw-rw-rw-   0        0        0     1090 2023-04-23 13:35:33.000000 laok-0.2.18/laok/dnn/head/classify.py
--rw-rw-rw-   0        0        0     3178 2023-04-23 13:32:56.000000 laok-0.2.18/laok/dnn/head/detect.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.524019 laok-0.2.18/laok/dnn/layer/
--rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.18/laok/dnn/layer/__init__.py
--rw-rw-rw-   0        0        0     2903 2023-04-25 02:35:22.000000 laok-0.2.18/laok/dnn/layer/pooling.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.525018 laok-0.2.18/laok/dnn/loss/
--rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.18/laok/dnn/loss/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.529006 laok-0.2.18/laok/dnn/model/
--rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.18/laok/dnn/model/__init__.py
--rw-rw-rw-   0        0        0      364 2023-04-23 13:41:53.000000 laok-0.2.18/laok/dnn/model/_torch_vision.py
--rw-rw-rw-   0        0        0        0 2023-05-25 08:13:53.000000 laok-0.2.18/laok/dnn/model/arc_face.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.530003 laok-0.2.18/laok/dnn/neck/
--rw-rw-rw-   0        0        0        0 2023-04-21 09:12:33.000000 laok-0.2.18/laok/dnn/neck/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.532995 laok-0.2.18/laok/ext/
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.18/laok/ext/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.536991 laok-0.2.18/laok/ext/flask_/
--rw-rw-rw-   0        0        0       42 2023-04-19 15:05:48.000000 laok-0.2.18/laok/ext/flask_/__init__.py
--rw-rw-rw-   0        0        0      395 2023-04-19 15:05:30.000000 laok-0.2.18/laok/ext/flask_/app.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.538979 laok-0.2.18/laok/ext/flask_/basic/
--rw-rw-rw-   0        0        0       22 2023-04-19 15:06:08.000000 laok-0.2.18/laok/ext/flask_/basic/__init__.py
--rw-rw-rw-   0        0        0      633 2023-04-19 15:38:09.000000 laok-0.2.18/laok/ext/flask_/basic/views.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.539976 laok-0.2.18/laok/ext/numpy_/
--rw-rw-rw-   0        0        0        0 2023-04-20 14:21:33.000000 laok-0.2.18/laok/ext/numpy_/__init__.py
--rw-rw-rw-   0        0        0     3022 2023-04-19 07:45:14.000000 laok-0.2.18/laok/ext/onnx_.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.540975 laok-0.2.18/laok/ext/torch_/
--rw-rw-rw-   0        0        0       88 2023-04-19 08:20:33.000000 laok-0.2.18/laok/ext/torch_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.543965 laok-0.2.18/laok/ext/torch_/datasets/
--rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.547957 laok-0.2.18/laok/ext/torch_/datasets/kitti/
--rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/datasets/kitti/__init__.py
--rw-rw-rw-   0        0        0    12031 2022-11-03 16:22:33.000000 laok-0.2.18/laok/ext/torch_/datasets/kitti/kitti.py
--rw-rw-rw-   0        0        0    27294 2022-10-28 06:48:12.000000 laok-0.2.18/laok/ext/torch_/datasets/kitti/obj.py
--rw-rw-rw-   0        0        0    26349 2022-11-03 16:22:33.000000 laok-0.2.18/laok/ext/torch_/datasets/kitti/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.555933 laok-0.2.18/laok/ext/torch_/datasets/model_net/
--rw-rw-rw-   0        0        0      954 2022-11-03 16:22:33.000000 laok-0.2.18/laok/ext/torch_/datasets/model_net/__init__.py
--rw-rw-rw-   0        0        0     3721 2022-11-03 16:22:33.000000 laok-0.2.18/laok/ext/torch_/datasets/model_net/model_net.py
--rw-rw-rw-   0        0        0     4467 2022-11-03 16:22:33.000000 laok-0.2.18/laok/ext/torch_/datasets/model_net/model_net_ineratia.py
--rw-rw-rw-   0        0        0     3895 2022-11-03 16:22:33.000000 laok-0.2.18/laok/ext/torch_/datasets/model_net/model_net_normals.py
--rw-rw-rw-   0        0        0     4553 2022-11-03 16:22:33.000000 laok-0.2.18/laok/ext/torch_/datasets/model_net/model_net_normals_diff.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.557927 laok-0.2.18/laok/ext/torch_/datasets/shape_net/
--rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/datasets/shape_net/__init__.py
--rw-rw-rw-   0        0        0     5463 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/datasets/shape_net/shape_net.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.559922 laok-0.2.18/laok/ext/torch_/datasets/stanford_indoor/
--rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/datasets/stanford_indoor/__init__.py
--rw-rw-rw-   0        0        0    11035 2022-10-12 15:00:14.000000 laok-0.2.18/laok/ext/torch_/datasets/stanford_indoor/_stanford_indoor.py
--rw-rw-rw-   0        0        0     2811 2022-11-02 07:35:53.000000 laok-0.2.18/laok/ext/torch_/datasets/ustc_lidar.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.564909 laok-0.2.18/laok/ext/torch_/io/
--rw-rw-rw-   0        0        0       80 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/io/__init__.py
--rw-rw-rw-   0        0        0      732 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/io/img.py
--rw-rw-rw-   0        0        0      844 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/io/jit.py
--rw-rw-rw-   0        0        0     1344 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/io/model.py
--rw-rw-rw-   0        0        0      466 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/io/onnx.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.568900 laok-0.2.18/laok/ext/torch_/op/
--rw-rw-rw-   0        0        0       70 2023-04-19 08:22:19.000000 laok-0.2.18/laok/ext/torch_/op/__init__.py
--rw-rw-rw-   0        0        0      965 2023-04-19 08:22:06.000000 laok-0.2.18/laok/ext/torch_/op/device.py
--rw-rw-rw-   0        0        0     1703 2023-04-19 08:27:44.000000 laok-0.2.18/laok/ext/torch_/op/module.py
--rw-rw-rw-   0        0        0     1403 2023-04-19 08:25:22.000000 laok-0.2.18/laok/ext/torch_/op/print_info.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.574882 laok-0.2.18/laok/ext/torch_/trainval/
--rw-rw-rw-   0        0        0       89 2022-10-21 10:13:37.000000 laok-0.2.18/laok/ext/torch_/trainval/__init__.py
--rw-rw-rw-   0        0        0     3943 2023-04-19 09:12:20.000000 laok-0.2.18/laok/ext/torch_/trainval/check_point.py
--rw-rw-rw-   0        0        0     2280 2023-04-19 09:25:29.000000 laok-0.2.18/laok/ext/torch_/trainval/infer.py
--rw-rw-rw-   0        0        0     2848 2023-04-19 08:44:39.000000 laok-0.2.18/laok/ext/torch_/trainval/train.py
--rw-rw-rw-   0        0        0     2308 2023-04-19 09:08:59.000000 laok-0.2.18/laok/ext/torch_/trainval/val.py
--rw-rw-rw-   0        0        0     2310 2023-07-04 02:40:34.000000 laok-0.2.18/laok/ext/ultralytics_.py
--rw-rw-rw-   0        0        0      649 2023-07-03 15:46:51.000000 laok-0.2.18/laok/third_lib.py
-drwxrwxrwx   0        0        0        0 2023-07-04 02:41:42.388381 laok-0.2.18/laok.egg-info/
--rw-rw-rw-   0        0        0      217 2023-07-04 02:41:42.000000 laok-0.2.18/laok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4146 2023-07-04 02:41:42.000000 laok-0.2.18/laok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 02:41:42.000000 laok-0.2.18/laok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-04 02:41:42.000000 laok-0.2.18/laok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 02:41:42.576877 laok-0.2.18/setup.cfg
--rw-rw-rw-   0        0        0      325 2023-07-04 02:36:00.000000 laok-0.2.18/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.868870 laok-0.2.19/
+-rw-rw-rw-   0        0        0      214 2023-07-14 03:08:54.868870 laok-0.2.19/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.708298 laok-0.2.19/laok/
+-rw-rw-rw-   0        0        0       19 2023-07-11 03:35:21.000000 laok-0.2.19/laok/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.714287 laok-0.2.19/laok/base/
+-rw-rw-rw-   0        0        0      248 2023-06-06 13:49:22.000000 laok-0.2.19/laok/base/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.718273 laok-0.2.19/laok/base/alg/
+-rw-rw-rw-   0        0        0       26 2023-04-20 13:21:17.000000 laok-0.2.19/laok/base/alg/__init__.py
+-rw-rw-rw-   0        0        0     4923 2023-04-20 13:20:53.000000 laok-0.2.19/laok/base/alg/addict.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.722262 laok-0.2.19/laok/base/conf/
+-rw-rw-rw-   0        0        0       32 2023-06-10 01:32:44.000000 laok-0.2.19/laok/base/conf/__init__.py
+-rw-rw-rw-   0        0        0      360 2023-04-19 14:40:47.000000 laok-0.2.19/laok/base/conf/conf_global.py
+-rw-rw-rw-   0        0        0     3022 2023-06-10 01:32:49.000000 laok-0.2.19/laok/base/conf/factory.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.727248 laok-0.2.19/laok/base/dataset/
+-rw-rw-rw-   0        0        0        0 2023-04-21 04:27:16.000000 laok-0.2.19/laok/base/dataset/__init__.py
+-rw-rw-rw-   0        0        0     6406 2023-04-21 04:29:54.000000 laok-0.2.19/laok/base/dataset/cvt_voc_yolo.py
+-rw-rw-rw-   0        0        0     2405 2019-09-12 10:55:17.000000 laok-0.2.19/laok/base/dataset/darknet-voc2yolo.py
+-rw-rw-rw-   0        0        0     2241 2019-02-18 15:12:05.000000 laok-0.2.19/laok/base/dataset/voc_label.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.732241 laok-0.2.19/laok/base/dtime/
+-rw-rw-rw-   0        0        0       47 2022-10-21 10:13:37.000000 laok-0.2.19/laok/base/dtime/__init__.py
+-rw-rw-rw-   0        0        0      556 2022-11-17 01:18:56.000000 laok-0.2.19/laok/base/dtime/datetime_.py
+-rw-rw-rw-   0        0        0     2727 2023-04-19 11:27:09.000000 laok-0.2.19/laok/base/dtime/timer.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.743205 laok-0.2.19/laok/base/fs/
+-rw-rw-rw-   0        0        0      134 2023-05-04 11:06:57.000000 laok-0.2.19/laok/base/fs/__init__.py
+-rw-rw-rw-   0        0        0     2591 2023-06-27 16:15:40.000000 laok-0.2.19/laok/base/fs/fdata.py
+-rw-rw-rw-   0        0        0     2937 2022-11-03 16:22:33.000000 laok-0.2.19/laok/base/fs/fname.py
+-rw-rw-rw-   0        0        0     4629 2023-06-27 16:03:41.000000 laok-0.2.19/laok/base/fs/fpath.py
+-rw-rw-rw-   0        0        0     1785 2023-05-04 11:06:06.000000 laok-0.2.19/laok/base/fs/fsearch.py
+-rw-rw-rw-   0        0        0     2819 2023-05-05 03:57:37.000000 laok-0.2.19/laok/base/fs/fwalk.py
+-rw-rw-rw-   0        0        0     1413 2023-04-19 09:23:34.000000 laok-0.2.19/laok/base/fs/name_index.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.746198 laok-0.2.19/laok/base/log/
+-rw-rw-rw-   0        0        0       50 2023-04-19 14:41:08.000000 laok-0.2.19/laok/base/log/__init__.py
+-rw-rw-rw-   0        0        0     2187 2023-07-14 02:24:25.000000 laok-0.2.19/laok/base/log/log.py
+-rw-rw-rw-   0        0        0      672 2023-04-19 14:43:17.000000 laok-0.2.19/laok/base/log/log_default.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.753179 laok-0.2.19/laok/base/net/
+-rw-rw-rw-   0        0        0       78 2023-06-06 16:23:58.000000 laok-0.2.19/laok/base/net/__init__.py
+-rw-rw-rw-   0        0        0      691 2022-09-23 00:45:15.000000 laok-0.2.19/laok/base/net/ip.py
+-rw-rw-rw-   0        0        0     3792 2023-06-27 10:59:29.000000 laok-0.2.19/laok/base/net/requests_.py
+-rw-rw-rw-   0        0        0     1200 2023-06-27 10:55:31.000000 laok-0.2.19/laok/base/net/url.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.755173 laok-0.2.19/laok/base/paral/
+-rw-rw-rw-   0        0        0       20 2022-10-21 10:13:37.000000 laok-0.2.19/laok/base/paral/__init__.py
+-rw-rw-rw-   0        0        0     2010 2023-04-20 15:21:46.000000 laok-0.2.19/laok/base/paral/pool.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.758167 laok-0.2.19/laok/base/pkg/
+-rw-rw-rw-   0        0        0       32 2023-07-03 15:46:47.000000 laok-0.2.19/laok/base/pkg/__init__.py
+-rw-rw-rw-   0        0        0    27875 2023-07-03 15:50:30.000000 laok-0.2.19/laok/base/pkg/_lazy.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.771130 laok-0.2.19/laok/base/ser/
+-rw-rw-rw-   0        0        0      156 2023-06-06 14:13:13.000000 laok-0.2.19/laok/base/ser/__init__.py
+-rw-rw-rw-   0        0        0     1367 2023-04-25 06:50:06.000000 laok-0.2.19/laok/base/ser/json_.py
+-rw-rw-rw-   0        0        0      750 2023-04-20 13:46:22.000000 laok-0.2.19/laok/base/ser/marshal_.py
+-rw-rw-rw-   0        0        0      676 2023-06-01 07:58:10.000000 laok-0.2.19/laok/base/ser/numpy_.py
+-rw-rw-rw-   0        0        0      621 2023-04-25 06:50:29.000000 laok-0.2.19/laok/base/ser/pickle_.py
+-rw-rw-rw-   0        0        0     1369 2023-06-10 01:42:11.000000 laok-0.2.19/laok/base/ser/torch_.py
+-rw-rw-rw-   0        0        0     1452 2023-06-06 17:03:52.000000 laok-0.2.19/laok/base/ser/xml_.py
+-rw-rw-rw-   0        0        0     1341 2023-06-01 07:57:17.000000 laok-0.2.19/laok/base/ser/yaml_.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.777115 laok-0.2.19/laok/base/str/
+-rw-rw-rw-   0        0        0       84 2023-06-10 01:11:15.000000 laok-0.2.19/laok/base/str/__init__.py
+-rw-rw-rw-   0        0        0      735 2023-06-10 01:09:44.000000 laok-0.2.19/laok/base/str/cvt.py
+-rw-rw-rw-   0        0        0      427 2023-06-10 01:10:45.000000 laok-0.2.19/laok/base/str/fmt.py
+-rw-rw-rw-   0        0        0     1705 2023-06-10 01:10:56.000000 laok-0.2.19/laok/base/str/misc.py
+-rw-rw-rw-   0        0        0     2588 2023-06-01 07:58:57.000000 laok-0.2.19/laok/base/str/print_info.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.785095 laok-0.2.19/laok/base/syst/
+-rw-rw-rw-   0        0        0       74 2023-07-03 11:23:20.000000 laok-0.2.19/laok/base/syst/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-05-04 15:23:10.000000 laok-0.2.19/laok/base/syst/platform_.py
+-rw-rw-rw-   0        0        0     1871 2022-10-21 10:13:37.000000 laok-0.2.19/laok/base/syst/print_info.py
+-rw-rw-rw-   0        0        0      380 2023-07-03 11:23:24.000000 laok-0.2.19/laok/base/syst/sys_.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.788089 laok-0.2.19/laok/base/test/
+-rw-rw-rw-   0        0        0       43 2022-10-21 10:13:37.000000 laok-0.2.19/laok/base/test/__init__.py
+-rw-rw-rw-   0        0        0     8790 2023-07-11 07:18:36.000000 laok-0.2.19/laok/base/test/_dump.py
+-rw-rw-rw-   0        0        0     4551 2023-06-01 05:41:11.000000 laok-0.2.19/laok/base/test/_run.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.790080 laok-0.2.19/laok/cv2d/
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.790080 laok-0.2.19/laok/cv2d/PIL_/
+-rw-rw-rw-   0        0        0        0 2023-07-12 09:00:52.000000 laok-0.2.19/laok/cv2d/PIL_/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.19/laok/cv2d/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.802048 laok-0.2.19/laok/cv2d/cv2_/
+-rw-rw-rw-   0        0        0      252 2023-07-12 14:13:06.000000 laok-0.2.19/laok/cv2d/cv2_/__init__.py
+-rw-rw-rw-   0        0        0     2115 2023-07-12 12:32:21.000000 laok-0.2.19/laok/cv2d/cv2_/bin.py
+-rw-rw-rw-   0        0        0      951 2023-07-12 14:53:01.000000 laok-0.2.19/laok/cv2d/cv2_/contours.py
+-rw-rw-rw-   0        0        0     2580 2023-07-11 11:20:43.000000 laok-0.2.19/laok/cv2d/cv2_/cvt.py
+-rw-rw-rw-   0        0        0     4358 2023-07-12 06:55:54.000000 laok-0.2.19/laok/cv2d/cv2_/draw.py
+-rw-rw-rw-   0        0        0      956 2023-07-12 14:26:53.000000 laok-0.2.19/laok/cv2d/cv2_/edge.py
+-rw-rw-rw-   0        0        0     1268 2023-07-12 13:43:27.000000 laok-0.2.19/laok/cv2d/cv2_/filter.py
+-rw-rw-rw-   0        0        0      630 2023-07-12 07:16:54.000000 laok-0.2.19/laok/cv2d/cv2_/geo.py
+-rw-rw-rw-   0        0        0     1019 2023-07-11 16:28:07.000000 laok-0.2.19/laok/cv2d/cv2_/info.py
+-rw-rw-rw-   0        0        0     3240 2023-07-11 14:03:03.000000 laok-0.2.19/laok/cv2d/cv2_/io.py
+-rw-rw-rw-   0        0        0     2787 2023-07-12 13:56:20.000000 laok-0.2.19/laok/cv2d/cv2_/morph.py
+-rw-rw-rw-   0        0        0     1230 2023-07-11 15:01:26.000000 laok-0.2.19/laok/cv2d/cv2_/show.py
+-rw-rw-rw-   0        0        0      828 2023-07-11 15:21:15.000000 laok-0.2.19/laok/cv2d/cv2_/util.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.803046 laok-0.2.19/laok/cv2d/skimage_/
+-rw-rw-rw-   0        0        0      330 2023-07-11 05:10:30.000000 laok-0.2.19/laok/cv2d/skimage_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.804044 laok-0.2.19/laok/cv3d/
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.19/laok/cv3d/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.805040 laok-0.2.19/laok/cv3d/open3d_/
+-rw-rw-rw-   0        0        0      330 2023-07-11 05:10:30.000000 laok-0.2.19/laok/cv3d/open3d_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.806038 laok-0.2.19/laok/data/
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.19/laok/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.807035 laok-0.2.19/laok/data/lxml_/
+-rw-rw-rw-   0        0        0     1982 2023-07-11 06:14:29.000000 laok-0.2.19/laok/data/lxml_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.808032 laok-0.2.19/laok/data/yaml_/
+-rw-rw-rw-   0        0        0      330 2023-07-11 05:10:30.000000 laok-0.2.19/laok/data/yaml_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.810027 laok-0.2.19/laok/dnn/
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.19/laok/dnn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.811025 laok-0.2.19/laok/dnn/onnx_/
+-rw-rw-rw-   0        0        0     3116 2023-07-11 03:56:12.000000 laok-0.2.19/laok/dnn/onnx_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.812025 laok-0.2.19/laok/dnn/torch_/
+-rw-rw-rw-   0        0        0       88 2023-04-19 08:20:33.000000 laok-0.2.19/laok/dnn/torch_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.815016 laok-0.2.19/laok/dnn/torch_/datasets/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.820000 laok-0.2.19/laok/dnn/torch_/datasets/kitti/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/datasets/kitti/__init__.py
+-rw-rw-rw-   0        0        0    12031 2022-11-03 16:22:33.000000 laok-0.2.19/laok/dnn/torch_/datasets/kitti/kitti.py
+-rw-rw-rw-   0        0        0    27294 2022-10-28 06:48:12.000000 laok-0.2.19/laok/dnn/torch_/datasets/kitti/obj.py
+-rw-rw-rw-   0        0        0    26349 2022-11-03 16:22:33.000000 laok-0.2.19/laok/dnn/torch_/datasets/kitti/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.825986 laok-0.2.19/laok/dnn/torch_/datasets/model_net/
+-rw-rw-rw-   0        0        0      954 2022-11-03 16:22:33.000000 laok-0.2.19/laok/dnn/torch_/datasets/model_net/__init__.py
+-rw-rw-rw-   0        0        0     3721 2022-11-03 16:22:33.000000 laok-0.2.19/laok/dnn/torch_/datasets/model_net/model_net.py
+-rw-rw-rw-   0        0        0     4467 2022-11-03 16:22:33.000000 laok-0.2.19/laok/dnn/torch_/datasets/model_net/model_net_ineratia.py
+-rw-rw-rw-   0        0        0     3895 2022-11-03 16:22:33.000000 laok-0.2.19/laok/dnn/torch_/datasets/model_net/model_net_normals.py
+-rw-rw-rw-   0        0        0     4553 2022-11-03 16:22:33.000000 laok-0.2.19/laok/dnn/torch_/datasets/model_net/model_net_normals_diff.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.827978 laok-0.2.19/laok/dnn/torch_/datasets/shape_net/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/datasets/shape_net/__init__.py
+-rw-rw-rw-   0        0        0     5463 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/datasets/shape_net/shape_net.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.828976 laok-0.2.19/laok/dnn/torch_/datasets/stanford_indoor/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/datasets/stanford_indoor/__init__.py
+-rw-rw-rw-   0        0        0    11035 2022-10-12 15:00:14.000000 laok-0.2.19/laok/dnn/torch_/datasets/stanford_indoor/_stanford_indoor.py
+-rw-rw-rw-   0        0        0     2811 2022-11-02 07:35:53.000000 laok-0.2.19/laok/dnn/torch_/datasets/ustc_lidar.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.835957 laok-0.2.19/laok/dnn/torch_/io/
+-rw-rw-rw-   0        0        0       80 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/io/__init__.py
+-rw-rw-rw-   0        0        0      732 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/io/img.py
+-rw-rw-rw-   0        0        0      844 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/io/jit.py
+-rw-rw-rw-   0        0        0     1344 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/io/model.py
+-rw-rw-rw-   0        0        0      466 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/io/onnx.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.839949 laok-0.2.19/laok/dnn/torch_/op/
+-rw-rw-rw-   0        0        0       70 2023-04-19 08:22:19.000000 laok-0.2.19/laok/dnn/torch_/op/__init__.py
+-rw-rw-rw-   0        0        0      965 2023-04-19 08:22:06.000000 laok-0.2.19/laok/dnn/torch_/op/device.py
+-rw-rw-rw-   0        0        0     1703 2023-04-19 08:27:44.000000 laok-0.2.19/laok/dnn/torch_/op/module.py
+-rw-rw-rw-   0        0        0     1403 2023-04-19 08:25:22.000000 laok-0.2.19/laok/dnn/torch_/op/print_info.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.844934 laok-0.2.19/laok/dnn/torch_/trainval/
+-rw-rw-rw-   0        0        0       89 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/trainval/__init__.py
+-rw-rw-rw-   0        0        0     3943 2023-04-19 09:12:20.000000 laok-0.2.19/laok/dnn/torch_/trainval/check_point.py
+-rw-rw-rw-   0        0        0     2280 2023-04-19 09:25:29.000000 laok-0.2.19/laok/dnn/torch_/trainval/infer.py
+-rw-rw-rw-   0        0        0     2848 2023-04-19 08:44:39.000000 laok-0.2.19/laok/dnn/torch_/trainval/train.py
+-rw-rw-rw-   0        0        0     2308 2023-04-19 09:08:59.000000 laok-0.2.19/laok/dnn/torch_/trainval/val.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.845932 laok-0.2.19/laok/gui/
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.19/laok/gui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.849956 laok-0.2.19/laok/gui/matplot_/
+-rw-rw-rw-   0        0        0       19 2023-07-12 09:01:52.000000 laok-0.2.19/laok/gui/matplot_/__init__.py
+-rw-rw-rw-   0        0        0     2096 2023-07-12 16:09:46.000000 laok-0.2.19/laok/gui/matplot_/show.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.853910 laok-0.2.19/laok/gui/qt_/
+-rw-rw-rw-   0        0        0       62 2023-07-14 02:30:38.000000 laok-0.2.19/laok/gui/qt_/__init__.py
+-rw-rw-rw-   0        0        0      582 2023-07-14 03:03:10.000000 laok-0.2.19/laok/gui/qt_/dialog.py
+-rw-rw-rw-   0        0        0     1004 2023-07-14 02:15:56.000000 laok-0.2.19/laok/gui/qt_/run.py
+-rw-rw-rw-   0        0        0     1692 2023-07-14 02:24:25.000000 laok-0.2.19/laok/gui/qt_/ui.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.854906 laok-0.2.19/laok/matical/
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.19/laok/matical/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.854906 laok-0.2.19/laok/matical/numpy_/
+-rw-rw-rw-   0        0        0        0 2023-04-20 14:21:33.000000 laok-0.2.19/laok/matical/numpy_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.855907 laok-0.2.19/laok/ml/
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.19/laok/ml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.856903 laok-0.2.19/laok/ml/sklearn_/
+-rw-rw-rw-   0        0        0      330 2023-07-11 05:10:30.000000 laok-0.2.19/laok/ml/sklearn_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.857899 laok-0.2.19/laok/net/
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.19/laok/net/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.859894 laok-0.2.19/laok/net/flask_/
+-rw-rw-rw-   0        0        0       42 2023-04-19 15:05:48.000000 laok-0.2.19/laok/net/flask_/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-04-19 15:05:30.000000 laok-0.2.19/laok/net/flask_/app.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.861889 laok-0.2.19/laok/net/flask_/basic/
+-rw-rw-rw-   0        0        0       22 2023-04-19 15:06:08.000000 laok-0.2.19/laok/net/flask_/basic/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-04-19 15:38:09.000000 laok-0.2.19/laok/net/flask_/basic/views.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.862886 laok-0.2.19/laok/net/requests_/
+-rw-rw-rw-   0        0        0     3808 2023-07-11 04:59:34.000000 laok-0.2.19/laok/net/requests_/__init__.py
+-rw-rw-rw-   0        0        0      649 2023-07-11 04:06:36.000000 laok-0.2.19/laok/third_lib.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.867905 laok-0.2.19/laok/tool/
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.19/laok/tool/__init__.py
+-rw-rw-rw-   0        0        0     3604 2023-07-11 06:29:13.000000 laok-0.2.19/laok/tool/download_m3u8.py
+-rw-rw-rw-   0        0        0     2310 2023-07-04 03:20:00.000000 laok-0.2.19/laok/tool/ultralytics_.py
+drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.712290 laok-0.2.19/laok.egg-info/
+-rw-rw-rw-   0        0        0      214 2023-07-14 03:08:54.000000 laok-0.2.19/laok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3708 2023-07-14 03:08:54.000000 laok-0.2.19/laok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 03:08:54.000000 laok-0.2.19/laok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-14 03:08:54.000000 laok-0.2.19/laok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 03:08:54.869867 laok-0.2.19/setup.cfg
+-rw-rw-rw-   0        0        0      322 2023-07-14 03:08:40.000000 laok-0.2.19/setup.py
```

### Comparing `laok-0.2.18/laok/base/alg/addict.py` & `laok-0.2.19/laok/base/alg/addict.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/conf/factory.py` & `laok-0.2.19/laok/base/conf/factory.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/dataset/cvt_voc_yolo.py` & `laok-0.2.19/laok/base/dataset/cvt_voc_yolo.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/dataset/darknet-voc2yolo.py` & `laok-0.2.19/laok/base/dataset/darknet-voc2yolo.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/dataset/voc_label.py` & `laok-0.2.19/laok/base/dataset/voc_label.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/dtime/datetime_.py` & `laok-0.2.19/laok/base/dtime/datetime_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/dtime/timer.py` & `laok-0.2.19/laok/base/dtime/timer.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/fs/fdata.py` & `laok-0.2.19/laok/base/fs/fdata.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/fs/fname.py` & `laok-0.2.19/laok/base/fs/fname.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/fs/fpath.py` & `laok-0.2.19/laok/base/fs/fpath.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/fs/fsearch.py` & `laok-0.2.19/laok/base/fs/fsearch.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/fs/fwalk.py` & `laok-0.2.19/laok/base/fs/fwalk.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/fs/name_index.py` & `laok-0.2.19/laok/base/fs/name_index.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/log/log.py` & `laok-0.2.19/laok/base/log/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     def inner(*args, sep=' ', **kws):
         msg = sep.join(str(x) for x in args)
         return func(msg, **kws)
     return inner
 
 def get_logger(name=None, level=logging.DEBUG):
     if name is None:
-        name = "laok"
+        name = "[laok]"
 
     if name in _logger_cache:
         return _logger_cache[name]
 
     log = logging.getLogger(name)
     _logger_cache[name] = log
     log.setLevel(level)
```

### Comparing `laok-0.2.18/laok/base/log/log_default.py` & `laok-0.2.19/laok/base/log/log_default.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/net/ip.py` & `laok-0.2.19/laok/base/net/ip.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/net/requests_.py` & `laok-0.2.19/laok/base/net/requests_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/net/url.py` & `laok-0.2.19/laok/base/net/url.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/paral/pool.py` & `laok-0.2.19/laok/base/paral/pool.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/pkg/_lazy.py` & `laok-0.2.19/laok/base/pkg/_lazy.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/ser/json_.py` & `laok-0.2.19/laok/base/ser/json_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/ser/marshal_.py` & `laok-0.2.19/laok/base/ser/marshal_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/ser/numpy_.py` & `laok-0.2.19/laok/base/ser/numpy_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/ser/pickle_.py` & `laok-0.2.19/laok/base/ser/pickle_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/ser/torch_.py` & `laok-0.2.19/laok/base/ser/torch_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/ser/xml_.py` & `laok-0.2.19/laok/base/ser/xml_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/ser/yaml_.py` & `laok-0.2.19/laok/base/ser/yaml_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/str/cvt.py` & `laok-0.2.19/laok/base/str/cvt.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/str/misc.py` & `laok-0.2.19/laok/base/str/misc.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/str/print_info.py` & `laok-0.2.19/laok/base/str/print_info.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/syst/platform_.py` & `laok-0.2.19/laok/base/syst/platform_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/syst/print_info.py` & `laok-0.2.19/laok/base/syst/print_info.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/base/test/_dump.py` & `laok-0.2.19/laok/base/test/_dump.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,22 +7,38 @@
 @copyright: Apache License, Version 2.0
 '''
 import inspect, contextlib, types, sys
 #===============================================================================
 # 
 #===============================================================================
 
-__all__ = ['dump', 'dump_help', 'is_method_overide', 'get_members']
+__all__ = ['dump', 'dump_help', 'is_method_overide', 'get_members', 'get_module_path']
 
 _MODULE_DEFAULT_FIELDS = ['__builtins__', '__cached__', '__doc__', '__file__',
                           '__loader__', '__name__', '__package__', '__path__', '__spec__']
 
 _CLASS_DEFAULT_FIELDS = ['__dict__', '__doc__', '__module__', '__weakref__',
                          '__init_subclass__', '__subclasshook__', '__class__']
 
+def get_module_path(mod):
+    pth = ''
+    if fname := getattr(mod, '__file__', ''):
+        pth = fname
+    if nsPath := getattr(mod, '__path__', tuple() ):
+        pth = nsPath[0]
+    return pth
+
+def _is_third_pkg(mod):
+    return 'site-packages' in get_module_path(mod)
+
+def _is_in_same_pkg(mod1, mod2):
+    mod1 = get_module_path(mod1)
+    mod2 = get_module_path(mod2)
+    return mod1 in mod2
+
 def is_method_overide(obj, method_name, parent=None):
     '''判断方法是否覆盖父类的方法'''
     if parent is None:
         parent = object
 
     mth = getattr(obj, method_name)
     if hasattr(parent, method_name):
@@ -36,16 +52,21 @@
     return False
 
 def dump_help(obj):
     with open('help-%s.txt' % _val_name(obj), 'w') as f, \
             contextlib.redirect_stdout(f):
         help(obj)
 
-def dump(obj, ignore_fields = tuple(), use_all = True, dump_format = None,
-              skip_moudle_defaults = True, skip_class_defaults=True, skip_underscore=True, stream=None):
+def dump(obj, ignore_fields = tuple(),
+                use_all = True,
+                dump_format = None,
+                skip_moudle_defaults = True,
+                skip_class_defaults=True,
+                skip_underscore=True,
+                stream=None):
 
     # # 空对象,直接不处理
     # if cfg is None:
     #     print('None')
     #     return
 
     all_ModuleType = [] #模块
@@ -57,20 +78,28 @@
     name_value_iter = get_members(obj, ignore_fields=ignore_fields,
                                   use_all=use_all, skip_moudle_defaults=skip_moudle_defaults,
                                   skip_class_defaults=skip_class_defaults,
                                   skip_underscore=skip_underscore)
     stream.write(f'\n########## {type(obj)} ##########\n')
     if dump_format is not None:
         stream.write(f'from {obj.__name__} import *\n')
+
     for item in name_value_iter:
         k, v = item
         if isinstance(v, type): # class类型
             all_Class.append(item)
+
         elif isinstance(v, types.ModuleType): # 模块类型
+            if not _is_third_pkg(v): # 保证是第三方库
+                continue
+            if isinstance(obj, types.ModuleType): #保证在同一个包里面
+                if not _is_in_same_pkg(obj, v):
+                    continue
             all_ModuleType.append(item)
+
         elif isinstance(v, (types.FunctionType,types.MethodType,types.WrapperDescriptorType,
                             types.MethodWrapperType, types.MethodDescriptorType, types.BuiltinFunctionType,
                             types.BuiltinMethodType) #可执行的函数类型
                         ):
             all_Funcs.append(item)
         else:
             all_Attr.append(item)
```

### Comparing `laok-0.2.18/laok/base/test/_run.py` & `laok-0.2.19/laok/base/test/_run.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/cv2d/io/cv2_.py` & `laok-0.2.19/laok/cv2d/cv2_/io.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,110 +1,108 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
-Created on 2022/4/24 21:29:16
+Created on 2023/7/11 14:36:36
 
 @author: LiuKuan
 @copyright: Apache License, Version 2.0
 '''
 import os
-from laok.third_lib import cv2, np
-from ..cvt.cv2_ import keep_bgr_cv, keep_gray_cv, image_size_cv, is_color_cv, swap_rb_cv
+import cv2
+import numpy as np
+from .cvt import swap_rb, keep_bgr, keep_gray
+from .info import is_color, image_size
 #===============================================================================
 '''     
 '''
 #===============================================================================
-__all__ = ['fix_cv_read', 'read_img_cv', 'read_color_cv', 'read_gray_cv',
-           'write_img_cv',
-           'read_video_cv', 'read_camera_cv', 'VideoWriterCv',
+__all__ = ['fix_cv_read',
+           'read_image', 'read_color', 'read_gray',
+           'write_image',
+           'read_video', 'read_camera', 'VideoWriter',
            ]
 
 ####################    读取图像
-
 def fix_cv_read():
+    '''主要功能是修复 读取中文路径时候的问题,本质上就是替换 cv2.imread函数
+    '''
     _org_read = cv2.imread
-    cv2.imread = read_img_cv
+    cv2.imread = read_image
 
-
-def read_img_cv(filename, flags = 1):
-    '''
-    :param filename:
-    :param flags: cv2.IMREAD_COLOR
-    :return:
-    '''
+def read_image(filename, flags = cv2.IMREAD_COLOR):
     return cv2.imdecode(np.fromfile(filename, dtype=np.uint8), flags)
 
-def read_color_cv(filename, bgr=True):
-    img = read_img_cv(filename, cv2.IMREAD_COLOR)
+def read_color(filename, bgr=True):
+    img = read_image(filename, cv2.IMREAD_COLOR)
     if not bgr:
-        return swap_rb_cv(img)
+        return swap_rb(img)
     return img
 
-def read_gray_cv(filename):
-    return read_img_cv(filename, cv2.IMREAD_GRAYSCALE)
+def read_gray(filename):
+    return read_image(filename, cv2.IMREAD_GRAYSCALE)
 
-def write_img_cv(data, filename):
+def write_image(data, filename):
     name, ext = os.path.splitext(filename)
     retval, buf = cv2.imencode(ext, data)
     return buf.tofile(filename)
 
 ####################    读取视频和相机
-def _read_capture_cv(fileOrId):
+def _read_capture(fileOrId):
     try:
         cap = cv2.VideoCapture(fileOrId)
         while True:
             ret, frame = cap.read()
-            if not ret:
+            if not ret:  # 如果正确读取帧，ret为True
                 break
             yield frame
     finally:
         cap.release()
 
-def read_video_cv(video_file):
-    yield from _read_capture_cv(video_file)
+def read_video(video_file):
+    yield from _read_capture(video_file)
 
-def read_camera_cv(camId = 0):
-    yield from _read_capture_cv(camId)
+def read_camera(camId = 0):
+    yield from _read_capture(camId)
 
 
-class VideoWriterCv:
+class VideoWriter:
     def __init__(self, filename, fourcc="mp4v", fps=24, frameSize=None, isColor=None):
         self.filename_ = filename
         self.frameSize_ = frameSize
         self.isColor_ = isColor
         self.fps_ = fps
         self.fourcc_ =  cv2.VideoWriter_fourcc(*fourcc)
         self.writer_ = None
 
     def _make_video(self, img):
         if self.frameSize_ is None:
-            self.frameSize_ = image_size_cv(img)
+            self.frameSize_ = image_size(img)
 
         if self.isColor_ is None:
-            self.isColor_ = is_color_cv(img)
+            self.isColor_ = is_color(img)
         self.writer_ = cv2.VideoWriter(filename=self.filename_, fourcc=self.fourcc_,
                                       fps=self.fps_, frameSize=self.frameSize_, isColor=self.isColor_)
 
     def write(self, img):
         if self.writer_ is None:
             self._make_video(img)
 
         if self.isColor_ :
-            img = keep_bgr_cv(img)
+            img = keep_bgr(img)
         else:
-            img = keep_gray_cv(img)
+            img = keep_gray(img)
 
-        if image_size_cv(img) != self.frameSize_:
+        if image_size(img) != self.frameSize_:
             img = cv2.resize(img, dsize=(self.frameSize_[0], self.frameSize_[1]),
                              interpolation=cv2.INTER_LINEAR)
-
         self.writer_.write(img)
 
     def close(self):
         if self.writer_ is not None:
             self.writer_.release()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
+
```

### Comparing `laok-0.2.18/laok/cv2d/morph/cv2_.py` & `laok-0.2.19/laok/cv2d/cv2_/morph.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
-Created on 2022/5/26 10:16:16
+Created on 2023/7/12 21:47:37
 
 @author: LiuKuan
 @copyright: Apache License, Version 2.0
 '''
-from laok.third_lib import cv2
-#===============================================================================
-'''    
-cv2.MORPH_RECT = 0
-cv2.BORDER_CONSTANT = 0         
+import cv2
+# ===============================================================================
+r'''
 '''
-#===============================================================================
-__all__ = ['morph_close_cv', 'morph_open_cv', 'morph_blackhat_cv',
-           'morph_dilate_cv', 'morph_erode_cv', 'morph_gradient_cv',
-           'morph_hitmiss_cv', 'morph_tophat_cv']
+# ===============================================================================
+__all__ = ['morph_open', 'morph_close',
+           'morph_erode', 'morph_dilate',
+           'morph_gradient', 'morph_hitmiss',
+           'morph_tophat', 'morph_blackhat',
+           'kernel_rect', 'kernel_cross', 'kernel_ellipse',
+]
 
-def _morph_impl(img, op, ksize=(3, 3), shape=0, kernel=None, anchor=(-1, -1), iterations=1, borderType=0, borderValue=(0, 0, 0)):
-    if kernel is None:
-        kernel = cv2.getStructuringElement(shape=shape, ksize=ksize, anchor=anchor)
-    return cv2.morphologyEx(img, op=op, kernel=kernel, anchor=anchor, iterations=iterations, borderType=borderType, borderValue=borderValue)
+def kernel_rect(ksize=(3, 3)):
+    return cv2.getStructuringElement(shape=cv2.MORPH_RECT, ksize=ksize)
 
-def morph_close_cv(img, ksize=(3, 3), shape=0, kernel=None, anchor=(-1, -1), iterations=1, borderType=0, borderValue=(0, 0, 0)):
-    return _morph_impl(img, op=cv2.MORPH_CLOSE, ksize=ksize, shape=shape, kernel=kernel, anchor=anchor, iterations=iterations, borderType=borderType, borderValue=borderValue)
+def kernel_cross(ksize=(3, 3)):
+    return cv2.getStructuringElement(shape=cv2.MORPH_CROSS, ksize=ksize)
 
-def morph_open_cv(img, ksize=(3, 3), shape=0, kernel=None,anchor=(-1, -1), iterations=1, borderType=0, borderValue=(0, 0, 0)):
-    return _morph_impl(img, op=cv2.MORPH_OPEN, ksize=ksize, shape=shape, kernel=kernel, anchor=anchor, iterations=iterations, borderType=borderType, borderValue=borderValue)
+def kernel_ellipse(ksize=(3, 3)):
+    return cv2.getStructuringElement(shape=cv2.MORPH_ELLIPSE, ksize=ksize)
 
-def morph_dilate_cv(img, ksize=(3, 3), shape=0, kernel=None, anchor=(-1, -1), iterations=1, borderType=0, borderValue=(0, 0, 0)):
-    return _morph_impl(img, op=cv2.MORPH_DILATE, ksize=ksize, shape=shape, kernel=kernel, anchor=anchor, iterations=iterations, borderType=borderType, borderValue=borderValue)
+def morph_open(img, kernel=None, iterations=1, borderType=cv2.BORDER_CONSTANT, borderValue=(0,0,0)):
+    return cv2.morphologyEx(img, op=cv2.MORPH_OPEN, kernel=kernel, iterations=iterations, borderType=borderType, borderValue=borderValue)
 
-def morph_erode_cv(img, ksize=(3, 3), shape=0, kernel=None, anchor=(-1, -1), iterations=1, borderType=0, borderValue=(0, 0, 0)):
-    return _morph_impl(img, op=cv2.MORPH_ERODE, ksize=ksize, shape=shape, kernel=kernel, anchor=anchor, iterations=iterations, borderType=borderType, borderValue=borderValue)
+def morph_close(img, kernel=None, iterations=1, borderType=cv2.BORDER_CONSTANT, borderValue=(0,0,0)):
+    return cv2.morphologyEx(img, op=cv2.MORPH_CLOSE, kernel=kernel, iterations=iterations, borderType=borderType, borderValue=borderValue)
 
-def morph_gradient_cv(img, ksize=(3, 3), shape=0, kernel=None, anchor=(-1, -1), iterations=1, borderType=0, borderValue=(0, 0, 0)):
-    return _morph_impl(img, op=cv2.MORPH_GRADIENT, ksize=ksize, shape=shape, kernel=kernel, anchor=anchor, iterations=iterations, borderType=borderType, borderValue=borderValue)
+def morph_erode(img, kernel=None, iterations=1, borderType=cv2.BORDER_CONSTANT, borderValue=(0,0,0)):
+    return cv2.morphologyEx(img, op=cv2.MORPH_ERODE, kernel=kernel, iterations=iterations, borderType=borderType, borderValue=borderValue)
 
-def morph_tophat_cv(img, ksize=(3, 3), shape=0, kernel=None, anchor=(-1, -1), iterations=1, borderType=0, borderValue=(0, 0, 0)):
-    return _morph_impl(img, op=cv2.MORPH_TOPHAT, ksize=ksize, shape=shape, kernel=kernel, anchor=anchor, iterations=iterations, borderType=borderType, borderValue=borderValue)
+def morph_dilate(img, kernel=None, iterations=1, borderType=cv2.BORDER_CONSTANT, borderValue=(0,0,0)):
+    return cv2.morphologyEx(img, op=cv2.MORPH_DILATE, kernel=kernel, iterations=iterations, borderType=borderType, borderValue=borderValue)
 
-def morph_blackhat_cv(img, ksize=(3, 3), shape=0, kernel=None, anchor=(-1, -1), iterations=1, borderType=0, borderValue=(0, 0, 0)):
-    return _morph_impl(img, op=cv2.MORPH_BLACKHAT, ksize=ksize, shape=shape, kernel=kernel, anchor=anchor, iterations=iterations, borderType=borderType, borderValue=borderValue)
+def morph_gradient(img, kernel=None, iterations=1, borderType=cv2.BORDER_CONSTANT, borderValue=(0,0,0)):
+    return cv2.morphologyEx(img, op=cv2.MORPH_GRADIENT, kernel=kernel, iterations=iterations, borderType=borderType, borderValue=borderValue)
 
-def morph_hitmiss_cv(img, ksize=(3, 3), shape=0, kernel=None, anchor=(-1, -1), iterations=1, borderType=0, borderValue=(0, 0, 0)):
-    return _morph_impl(img, op=cv2.MORPH_HITMISS, ksize=ksize, shape=shape, kernel=kernel, anchor=anchor, iterations=iterations, borderType=borderType, borderValue=borderValue)
+def morph_tophat(img, kernel=None, iterations=1, borderType=cv2.BORDER_CONSTANT, borderValue=(0,0,0)):
+    return cv2.morphologyEx(img, op=cv2.MORPH_TOPHAT, kernel=kernel, iterations=iterations, borderType=borderType, borderValue=borderValue)
 
+def morph_blackhat(img, kernel=None, iterations=1, borderType=cv2.BORDER_CONSTANT, borderValue=(0,0,0)):
+    return cv2.morphologyEx(img, op=cv2.MORPH_BLACKHAT, kernel=kernel, iterations=iterations, borderType=borderType, borderValue=borderValue)
+
+def morph_hitmiss(img, kernel=None, iterations=1):
+    return cv2.morphologyEx(img, op=cv2.MORPH_HITMISS, kernel=kernel, iterations=iterations)
```

### Comparing `laok-0.2.18/laok/ext/flask_/basic/views.py` & `laok-0.2.19/laok/net/flask_/basic/views.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/onnx_.py` & `laok-0.2.19/laok/dnn/onnx_/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 Created on 2022/4/19 11:14:26
 
 @author: LiuKuan
 @copyright: Apache License, Version 2.0
 '''
 import onnx
 import onnxruntime
-import laok
+from laok.base.fs import path_replace_ext, path_exist
 #===============================================================================
 '''
 '''
 #===============================================================================
+__all__ = ['check_model', 'load_model', 'dump_model_info']
+
 def check_model(onnxFile):
     '''check onnx model if it is valide
     :param onnxFile:
     :return:
     '''
     model = onnx.load_model(onnxFile)
     onnx.checker.check_model(model)
@@ -40,17 +42,17 @@
     :param onnxFile:
     :param graphFile:
     :param skip_exist:
     :param show_info:
     :return:
     '''
     if graphFile is None:
-        graphFile = laok.path_replace_ext(onnxFile, '.graph')
+        graphFile = path_replace_ext(onnxFile, '.graph')
 
-    if skip_exist and laok.path_exist(graphFile):
+    if skip_exist and path_exist(graphFile):
         return graphFile
 
     if show_info:
         print(f'start read... {onnxFile}')
 
     msg_list = []
     ###################### onnxruntime的模型信息
```

### Comparing `laok-0.2.18/laok/ext/torch_/datasets/kitti/kitti.py` & `laok-0.2.19/laok/dnn/torch_/datasets/kitti/kitti.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/datasets/kitti/obj.py` & `laok-0.2.19/laok/dnn/torch_/datasets/kitti/obj.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/datasets/kitti/utils.py` & `laok-0.2.19/laok/dnn/torch_/datasets/kitti/utils.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/datasets/model_net/__init__.py` & `laok-0.2.19/laok/dnn/torch_/datasets/model_net/__init__.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/datasets/model_net/model_net.py` & `laok-0.2.19/laok/dnn/torch_/datasets/model_net/model_net.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/datasets/model_net/model_net_ineratia.py` & `laok-0.2.19/laok/dnn/torch_/datasets/model_net/model_net_ineratia.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/datasets/model_net/model_net_normals.py` & `laok-0.2.19/laok/dnn/torch_/datasets/model_net/model_net_normals.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/datasets/model_net/model_net_normals_diff.py` & `laok-0.2.19/laok/dnn/torch_/datasets/model_net/model_net_normals_diff.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/datasets/shape_net/shape_net.py` & `laok-0.2.19/laok/dnn/torch_/datasets/shape_net/shape_net.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/datasets/stanford_indoor/_stanford_indoor.py` & `laok-0.2.19/laok/dnn/torch_/datasets/stanford_indoor/_stanford_indoor.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/datasets/ustc_lidar.py` & `laok-0.2.19/laok/dnn/torch_/datasets/ustc_lidar.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/io/img.py` & `laok-0.2.19/laok/dnn/torch_/io/img.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/io/jit.py` & `laok-0.2.19/laok/dnn/torch_/io/jit.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/io/model.py` & `laok-0.2.19/laok/dnn/torch_/io/model.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/op/device.py` & `laok-0.2.19/laok/dnn/torch_/op/device.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/op/module.py` & `laok-0.2.19/laok/dnn/torch_/op/module.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/op/print_info.py` & `laok-0.2.19/laok/dnn/torch_/op/print_info.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/trainval/check_point.py` & `laok-0.2.19/laok/dnn/torch_/trainval/check_point.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/trainval/infer.py` & `laok-0.2.19/laok/dnn/torch_/trainval/infer.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/trainval/train.py` & `laok-0.2.19/laok/dnn/torch_/trainval/train.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/torch_/trainval/val.py` & `laok-0.2.19/laok/dnn/torch_/trainval/val.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/ext/ultralytics_.py` & `laok-0.2.19/laok/tool/ultralytics_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.18/laok/third_lib.py` & `laok-0.2.19/laok/third_lib.py`

 * *Files identical despite different names*

