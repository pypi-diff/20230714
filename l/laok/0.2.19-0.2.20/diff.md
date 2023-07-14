# Comparing `tmp/laok-0.2.19.tar.gz` & `tmp/laok-0.2.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laok-0.2.19.tar", last modified: Fri Jul 14 03:08:54 2023, max compression
+gzip compressed data, was "laok-0.2.20.tar", last modified: Fri Jul 14 09:20:51 2023, max compression
```

## Comparing `laok-0.2.19.tar` & `laok-0.2.20.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.868870 laok-0.2.19/
--rw-rw-rw-   0        0        0      214 2023-07-14 03:08:54.868870 laok-0.2.19/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.708298 laok-0.2.19/laok/
--rw-rw-rw-   0        0        0       19 2023-07-11 03:35:21.000000 laok-0.2.19/laok/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.714287 laok-0.2.19/laok/base/
--rw-rw-rw-   0        0        0      248 2023-06-06 13:49:22.000000 laok-0.2.19/laok/base/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.718273 laok-0.2.19/laok/base/alg/
--rw-rw-rw-   0        0        0       26 2023-04-20 13:21:17.000000 laok-0.2.19/laok/base/alg/__init__.py
--rw-rw-rw-   0        0        0     4923 2023-04-20 13:20:53.000000 laok-0.2.19/laok/base/alg/addict.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.722262 laok-0.2.19/laok/base/conf/
--rw-rw-rw-   0        0        0       32 2023-06-10 01:32:44.000000 laok-0.2.19/laok/base/conf/__init__.py
--rw-rw-rw-   0        0        0      360 2023-04-19 14:40:47.000000 laok-0.2.19/laok/base/conf/conf_global.py
--rw-rw-rw-   0        0        0     3022 2023-06-10 01:32:49.000000 laok-0.2.19/laok/base/conf/factory.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.727248 laok-0.2.19/laok/base/dataset/
--rw-rw-rw-   0        0        0        0 2023-04-21 04:27:16.000000 laok-0.2.19/laok/base/dataset/__init__.py
--rw-rw-rw-   0        0        0     6406 2023-04-21 04:29:54.000000 laok-0.2.19/laok/base/dataset/cvt_voc_yolo.py
--rw-rw-rw-   0        0        0     2405 2019-09-12 10:55:17.000000 laok-0.2.19/laok/base/dataset/darknet-voc2yolo.py
--rw-rw-rw-   0        0        0     2241 2019-02-18 15:12:05.000000 laok-0.2.19/laok/base/dataset/voc_label.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.732241 laok-0.2.19/laok/base/dtime/
--rw-rw-rw-   0        0        0       47 2022-10-21 10:13:37.000000 laok-0.2.19/laok/base/dtime/__init__.py
--rw-rw-rw-   0        0        0      556 2022-11-17 01:18:56.000000 laok-0.2.19/laok/base/dtime/datetime_.py
--rw-rw-rw-   0        0        0     2727 2023-04-19 11:27:09.000000 laok-0.2.19/laok/base/dtime/timer.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.743205 laok-0.2.19/laok/base/fs/
--rw-rw-rw-   0        0        0      134 2023-05-04 11:06:57.000000 laok-0.2.19/laok/base/fs/__init__.py
--rw-rw-rw-   0        0        0     2591 2023-06-27 16:15:40.000000 laok-0.2.19/laok/base/fs/fdata.py
--rw-rw-rw-   0        0        0     2937 2022-11-03 16:22:33.000000 laok-0.2.19/laok/base/fs/fname.py
--rw-rw-rw-   0        0        0     4629 2023-06-27 16:03:41.000000 laok-0.2.19/laok/base/fs/fpath.py
--rw-rw-rw-   0        0        0     1785 2023-05-04 11:06:06.000000 laok-0.2.19/laok/base/fs/fsearch.py
--rw-rw-rw-   0        0        0     2819 2023-05-05 03:57:37.000000 laok-0.2.19/laok/base/fs/fwalk.py
--rw-rw-rw-   0        0        0     1413 2023-04-19 09:23:34.000000 laok-0.2.19/laok/base/fs/name_index.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.746198 laok-0.2.19/laok/base/log/
--rw-rw-rw-   0        0        0       50 2023-04-19 14:41:08.000000 laok-0.2.19/laok/base/log/__init__.py
--rw-rw-rw-   0        0        0     2187 2023-07-14 02:24:25.000000 laok-0.2.19/laok/base/log/log.py
--rw-rw-rw-   0        0        0      672 2023-04-19 14:43:17.000000 laok-0.2.19/laok/base/log/log_default.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.753179 laok-0.2.19/laok/base/net/
--rw-rw-rw-   0        0        0       78 2023-06-06 16:23:58.000000 laok-0.2.19/laok/base/net/__init__.py
--rw-rw-rw-   0        0        0      691 2022-09-23 00:45:15.000000 laok-0.2.19/laok/base/net/ip.py
--rw-rw-rw-   0        0        0     3792 2023-06-27 10:59:29.000000 laok-0.2.19/laok/base/net/requests_.py
--rw-rw-rw-   0        0        0     1200 2023-06-27 10:55:31.000000 laok-0.2.19/laok/base/net/url.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.755173 laok-0.2.19/laok/base/paral/
--rw-rw-rw-   0        0        0       20 2022-10-21 10:13:37.000000 laok-0.2.19/laok/base/paral/__init__.py
--rw-rw-rw-   0        0        0     2010 2023-04-20 15:21:46.000000 laok-0.2.19/laok/base/paral/pool.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.758167 laok-0.2.19/laok/base/pkg/
--rw-rw-rw-   0        0        0       32 2023-07-03 15:46:47.000000 laok-0.2.19/laok/base/pkg/__init__.py
--rw-rw-rw-   0        0        0    27875 2023-07-03 15:50:30.000000 laok-0.2.19/laok/base/pkg/_lazy.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.771130 laok-0.2.19/laok/base/ser/
--rw-rw-rw-   0        0        0      156 2023-06-06 14:13:13.000000 laok-0.2.19/laok/base/ser/__init__.py
--rw-rw-rw-   0        0        0     1367 2023-04-25 06:50:06.000000 laok-0.2.19/laok/base/ser/json_.py
--rw-rw-rw-   0        0        0      750 2023-04-20 13:46:22.000000 laok-0.2.19/laok/base/ser/marshal_.py
--rw-rw-rw-   0        0        0      676 2023-06-01 07:58:10.000000 laok-0.2.19/laok/base/ser/numpy_.py
--rw-rw-rw-   0        0        0      621 2023-04-25 06:50:29.000000 laok-0.2.19/laok/base/ser/pickle_.py
--rw-rw-rw-   0        0        0     1369 2023-06-10 01:42:11.000000 laok-0.2.19/laok/base/ser/torch_.py
--rw-rw-rw-   0        0        0     1452 2023-06-06 17:03:52.000000 laok-0.2.19/laok/base/ser/xml_.py
--rw-rw-rw-   0        0        0     1341 2023-06-01 07:57:17.000000 laok-0.2.19/laok/base/ser/yaml_.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.777115 laok-0.2.19/laok/base/str/
--rw-rw-rw-   0        0        0       84 2023-06-10 01:11:15.000000 laok-0.2.19/laok/base/str/__init__.py
--rw-rw-rw-   0        0        0      735 2023-06-10 01:09:44.000000 laok-0.2.19/laok/base/str/cvt.py
--rw-rw-rw-   0        0        0      427 2023-06-10 01:10:45.000000 laok-0.2.19/laok/base/str/fmt.py
--rw-rw-rw-   0        0        0     1705 2023-06-10 01:10:56.000000 laok-0.2.19/laok/base/str/misc.py
--rw-rw-rw-   0        0        0     2588 2023-06-01 07:58:57.000000 laok-0.2.19/laok/base/str/print_info.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.785095 laok-0.2.19/laok/base/syst/
--rw-rw-rw-   0        0        0       74 2023-07-03 11:23:20.000000 laok-0.2.19/laok/base/syst/__init__.py
--rw-rw-rw-   0        0        0      518 2023-05-04 15:23:10.000000 laok-0.2.19/laok/base/syst/platform_.py
--rw-rw-rw-   0        0        0     1871 2022-10-21 10:13:37.000000 laok-0.2.19/laok/base/syst/print_info.py
--rw-rw-rw-   0        0        0      380 2023-07-03 11:23:24.000000 laok-0.2.19/laok/base/syst/sys_.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.788089 laok-0.2.19/laok/base/test/
--rw-rw-rw-   0        0        0       43 2022-10-21 10:13:37.000000 laok-0.2.19/laok/base/test/__init__.py
--rw-rw-rw-   0        0        0     8790 2023-07-11 07:18:36.000000 laok-0.2.19/laok/base/test/_dump.py
--rw-rw-rw-   0        0        0     4551 2023-06-01 05:41:11.000000 laok-0.2.19/laok/base/test/_run.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.790080 laok-0.2.19/laok/cv2d/
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.790080 laok-0.2.19/laok/cv2d/PIL_/
--rw-rw-rw-   0        0        0        0 2023-07-12 09:00:52.000000 laok-0.2.19/laok/cv2d/PIL_/__init__.py
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.19/laok/cv2d/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.802048 laok-0.2.19/laok/cv2d/cv2_/
--rw-rw-rw-   0        0        0      252 2023-07-12 14:13:06.000000 laok-0.2.19/laok/cv2d/cv2_/__init__.py
--rw-rw-rw-   0        0        0     2115 2023-07-12 12:32:21.000000 laok-0.2.19/laok/cv2d/cv2_/bin.py
--rw-rw-rw-   0        0        0      951 2023-07-12 14:53:01.000000 laok-0.2.19/laok/cv2d/cv2_/contours.py
--rw-rw-rw-   0        0        0     2580 2023-07-11 11:20:43.000000 laok-0.2.19/laok/cv2d/cv2_/cvt.py
--rw-rw-rw-   0        0        0     4358 2023-07-12 06:55:54.000000 laok-0.2.19/laok/cv2d/cv2_/draw.py
--rw-rw-rw-   0        0        0      956 2023-07-12 14:26:53.000000 laok-0.2.19/laok/cv2d/cv2_/edge.py
--rw-rw-rw-   0        0        0     1268 2023-07-12 13:43:27.000000 laok-0.2.19/laok/cv2d/cv2_/filter.py
--rw-rw-rw-   0        0        0      630 2023-07-12 07:16:54.000000 laok-0.2.19/laok/cv2d/cv2_/geo.py
--rw-rw-rw-   0        0        0     1019 2023-07-11 16:28:07.000000 laok-0.2.19/laok/cv2d/cv2_/info.py
--rw-rw-rw-   0        0        0     3240 2023-07-11 14:03:03.000000 laok-0.2.19/laok/cv2d/cv2_/io.py
--rw-rw-rw-   0        0        0     2787 2023-07-12 13:56:20.000000 laok-0.2.19/laok/cv2d/cv2_/morph.py
--rw-rw-rw-   0        0        0     1230 2023-07-11 15:01:26.000000 laok-0.2.19/laok/cv2d/cv2_/show.py
--rw-rw-rw-   0        0        0      828 2023-07-11 15:21:15.000000 laok-0.2.19/laok/cv2d/cv2_/util.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.803046 laok-0.2.19/laok/cv2d/skimage_/
--rw-rw-rw-   0        0        0      330 2023-07-11 05:10:30.000000 laok-0.2.19/laok/cv2d/skimage_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.804044 laok-0.2.19/laok/cv3d/
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.19/laok/cv3d/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.805040 laok-0.2.19/laok/cv3d/open3d_/
--rw-rw-rw-   0        0        0      330 2023-07-11 05:10:30.000000 laok-0.2.19/laok/cv3d/open3d_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.806038 laok-0.2.19/laok/data/
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.19/laok/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.807035 laok-0.2.19/laok/data/lxml_/
--rw-rw-rw-   0        0        0     1982 2023-07-11 06:14:29.000000 laok-0.2.19/laok/data/lxml_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.808032 laok-0.2.19/laok/data/yaml_/
--rw-rw-rw-   0        0        0      330 2023-07-11 05:10:30.000000 laok-0.2.19/laok/data/yaml_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.810027 laok-0.2.19/laok/dnn/
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.19/laok/dnn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.811025 laok-0.2.19/laok/dnn/onnx_/
--rw-rw-rw-   0        0        0     3116 2023-07-11 03:56:12.000000 laok-0.2.19/laok/dnn/onnx_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.812025 laok-0.2.19/laok/dnn/torch_/
--rw-rw-rw-   0        0        0       88 2023-04-19 08:20:33.000000 laok-0.2.19/laok/dnn/torch_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.815016 laok-0.2.19/laok/dnn/torch_/datasets/
--rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.820000 laok-0.2.19/laok/dnn/torch_/datasets/kitti/
--rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/datasets/kitti/__init__.py
--rw-rw-rw-   0        0        0    12031 2022-11-03 16:22:33.000000 laok-0.2.19/laok/dnn/torch_/datasets/kitti/kitti.py
--rw-rw-rw-   0        0        0    27294 2022-10-28 06:48:12.000000 laok-0.2.19/laok/dnn/torch_/datasets/kitti/obj.py
--rw-rw-rw-   0        0        0    26349 2022-11-03 16:22:33.000000 laok-0.2.19/laok/dnn/torch_/datasets/kitti/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.825986 laok-0.2.19/laok/dnn/torch_/datasets/model_net/
--rw-rw-rw-   0        0        0      954 2022-11-03 16:22:33.000000 laok-0.2.19/laok/dnn/torch_/datasets/model_net/__init__.py
--rw-rw-rw-   0        0        0     3721 2022-11-03 16:22:33.000000 laok-0.2.19/laok/dnn/torch_/datasets/model_net/model_net.py
--rw-rw-rw-   0        0        0     4467 2022-11-03 16:22:33.000000 laok-0.2.19/laok/dnn/torch_/datasets/model_net/model_net_ineratia.py
--rw-rw-rw-   0        0        0     3895 2022-11-03 16:22:33.000000 laok-0.2.19/laok/dnn/torch_/datasets/model_net/model_net_normals.py
--rw-rw-rw-   0        0        0     4553 2022-11-03 16:22:33.000000 laok-0.2.19/laok/dnn/torch_/datasets/model_net/model_net_normals_diff.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.827978 laok-0.2.19/laok/dnn/torch_/datasets/shape_net/
--rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/datasets/shape_net/__init__.py
--rw-rw-rw-   0        0        0     5463 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/datasets/shape_net/shape_net.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.828976 laok-0.2.19/laok/dnn/torch_/datasets/stanford_indoor/
--rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/datasets/stanford_indoor/__init__.py
--rw-rw-rw-   0        0        0    11035 2022-10-12 15:00:14.000000 laok-0.2.19/laok/dnn/torch_/datasets/stanford_indoor/_stanford_indoor.py
--rw-rw-rw-   0        0        0     2811 2022-11-02 07:35:53.000000 laok-0.2.19/laok/dnn/torch_/datasets/ustc_lidar.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.835957 laok-0.2.19/laok/dnn/torch_/io/
--rw-rw-rw-   0        0        0       80 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/io/__init__.py
--rw-rw-rw-   0        0        0      732 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/io/img.py
--rw-rw-rw-   0        0        0      844 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/io/jit.py
--rw-rw-rw-   0        0        0     1344 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/io/model.py
--rw-rw-rw-   0        0        0      466 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/io/onnx.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.839949 laok-0.2.19/laok/dnn/torch_/op/
--rw-rw-rw-   0        0        0       70 2023-04-19 08:22:19.000000 laok-0.2.19/laok/dnn/torch_/op/__init__.py
--rw-rw-rw-   0        0        0      965 2023-04-19 08:22:06.000000 laok-0.2.19/laok/dnn/torch_/op/device.py
--rw-rw-rw-   0        0        0     1703 2023-04-19 08:27:44.000000 laok-0.2.19/laok/dnn/torch_/op/module.py
--rw-rw-rw-   0        0        0     1403 2023-04-19 08:25:22.000000 laok-0.2.19/laok/dnn/torch_/op/print_info.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.844934 laok-0.2.19/laok/dnn/torch_/trainval/
--rw-rw-rw-   0        0        0       89 2022-10-21 10:13:37.000000 laok-0.2.19/laok/dnn/torch_/trainval/__init__.py
--rw-rw-rw-   0        0        0     3943 2023-04-19 09:12:20.000000 laok-0.2.19/laok/dnn/torch_/trainval/check_point.py
--rw-rw-rw-   0        0        0     2280 2023-04-19 09:25:29.000000 laok-0.2.19/laok/dnn/torch_/trainval/infer.py
--rw-rw-rw-   0        0        0     2848 2023-04-19 08:44:39.000000 laok-0.2.19/laok/dnn/torch_/trainval/train.py
--rw-rw-rw-   0        0        0     2308 2023-04-19 09:08:59.000000 laok-0.2.19/laok/dnn/torch_/trainval/val.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.845932 laok-0.2.19/laok/gui/
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.19/laok/gui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.849956 laok-0.2.19/laok/gui/matplot_/
--rw-rw-rw-   0        0        0       19 2023-07-12 09:01:52.000000 laok-0.2.19/laok/gui/matplot_/__init__.py
--rw-rw-rw-   0        0        0     2096 2023-07-12 16:09:46.000000 laok-0.2.19/laok/gui/matplot_/show.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.853910 laok-0.2.19/laok/gui/qt_/
--rw-rw-rw-   0        0        0       62 2023-07-14 02:30:38.000000 laok-0.2.19/laok/gui/qt_/__init__.py
--rw-rw-rw-   0        0        0      582 2023-07-14 03:03:10.000000 laok-0.2.19/laok/gui/qt_/dialog.py
--rw-rw-rw-   0        0        0     1004 2023-07-14 02:15:56.000000 laok-0.2.19/laok/gui/qt_/run.py
--rw-rw-rw-   0        0        0     1692 2023-07-14 02:24:25.000000 laok-0.2.19/laok/gui/qt_/ui.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.854906 laok-0.2.19/laok/matical/
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.19/laok/matical/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.854906 laok-0.2.19/laok/matical/numpy_/
--rw-rw-rw-   0        0        0        0 2023-04-20 14:21:33.000000 laok-0.2.19/laok/matical/numpy_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.855907 laok-0.2.19/laok/ml/
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.19/laok/ml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.856903 laok-0.2.19/laok/ml/sklearn_/
--rw-rw-rw-   0        0        0      330 2023-07-11 05:10:30.000000 laok-0.2.19/laok/ml/sklearn_/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.857899 laok-0.2.19/laok/net/
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.19/laok/net/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.859894 laok-0.2.19/laok/net/flask_/
--rw-rw-rw-   0        0        0       42 2023-04-19 15:05:48.000000 laok-0.2.19/laok/net/flask_/__init__.py
--rw-rw-rw-   0        0        0      395 2023-04-19 15:05:30.000000 laok-0.2.19/laok/net/flask_/app.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.861889 laok-0.2.19/laok/net/flask_/basic/
--rw-rw-rw-   0        0        0       22 2023-04-19 15:06:08.000000 laok-0.2.19/laok/net/flask_/basic/__init__.py
--rw-rw-rw-   0        0        0      633 2023-04-19 15:38:09.000000 laok-0.2.19/laok/net/flask_/basic/views.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.862886 laok-0.2.19/laok/net/requests_/
--rw-rw-rw-   0        0        0     3808 2023-07-11 04:59:34.000000 laok-0.2.19/laok/net/requests_/__init__.py
--rw-rw-rw-   0        0        0      649 2023-07-11 04:06:36.000000 laok-0.2.19/laok/third_lib.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.867905 laok-0.2.19/laok/tool/
--rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.19/laok/tool/__init__.py
--rw-rw-rw-   0        0        0     3604 2023-07-11 06:29:13.000000 laok-0.2.19/laok/tool/download_m3u8.py
--rw-rw-rw-   0        0        0     2310 2023-07-04 03:20:00.000000 laok-0.2.19/laok/tool/ultralytics_.py
-drwxrwxrwx   0        0        0        0 2023-07-14 03:08:54.712290 laok-0.2.19/laok.egg-info/
--rw-rw-rw-   0        0        0      214 2023-07-14 03:08:54.000000 laok-0.2.19/laok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3708 2023-07-14 03:08:54.000000 laok-0.2.19/laok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 03:08:54.000000 laok-0.2.19/laok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-14 03:08:54.000000 laok-0.2.19/laok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 03:08:54.869867 laok-0.2.19/setup.cfg
--rw-rw-rw-   0        0        0      322 2023-07-14 03:08:40.000000 laok-0.2.19/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.687990 laok-0.2.20/
+-rw-rw-rw-   0        0        0      214 2023-07-14 09:20:51.687990 laok-0.2.20/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.571301 laok-0.2.20/laok/
+-rw-rw-rw-   0        0        0       19 2023-07-11 03:35:21.000000 laok-0.2.20/laok/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.575291 laok-0.2.20/laok/base/
+-rw-rw-rw-   0        0        0      266 2023-07-14 09:20:48.000000 laok-0.2.20/laok/base/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.577286 laok-0.2.20/laok/base/alg/
+-rw-rw-rw-   0        0        0       26 2023-04-20 13:21:17.000000 laok-0.2.20/laok/base/alg/__init__.py
+-rw-rw-rw-   0        0        0     4923 2023-04-20 13:20:53.000000 laok-0.2.20/laok/base/alg/addict.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.580277 laok-0.2.20/laok/base/conf/
+-rw-rw-rw-   0        0        0       32 2023-06-10 01:32:44.000000 laok-0.2.20/laok/base/conf/__init__.py
+-rw-rw-rw-   0        0        0      360 2023-04-19 14:40:47.000000 laok-0.2.20/laok/base/conf/conf_global.py
+-rw-rw-rw-   0        0        0     3022 2023-06-10 01:32:49.000000 laok-0.2.20/laok/base/conf/factory.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.583269 laok-0.2.20/laok/base/dataset/
+-rw-rw-rw-   0        0        0        0 2023-04-21 04:27:16.000000 laok-0.2.20/laok/base/dataset/__init__.py
+-rw-rw-rw-   0        0        0     6406 2023-04-21 04:29:54.000000 laok-0.2.20/laok/base/dataset/cvt_voc_yolo.py
+-rw-rw-rw-   0        0        0     2405 2019-09-12 10:55:17.000000 laok-0.2.20/laok/base/dataset/darknet-voc2yolo.py
+-rw-rw-rw-   0        0        0     2241 2019-02-18 15:12:05.000000 laok-0.2.20/laok/base/dataset/voc_label.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.586262 laok-0.2.20/laok/base/dtime/
+-rw-rw-rw-   0        0        0       47 2022-10-21 10:13:37.000000 laok-0.2.20/laok/base/dtime/__init__.py
+-rw-rw-rw-   0        0        0      556 2022-11-17 01:18:56.000000 laok-0.2.20/laok/base/dtime/datetime_.py
+-rw-rw-rw-   0        0        0     2727 2023-04-19 11:27:09.000000 laok-0.2.20/laok/base/dtime/timer.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.593243 laok-0.2.20/laok/base/fs/
+-rw-rw-rw-   0        0        0      134 2023-05-04 11:06:57.000000 laok-0.2.20/laok/base/fs/__init__.py
+-rw-rw-rw-   0        0        0     2591 2023-06-27 16:15:40.000000 laok-0.2.20/laok/base/fs/fdata.py
+-rw-rw-rw-   0        0        0     2937 2022-11-03 16:22:33.000000 laok-0.2.20/laok/base/fs/fname.py
+-rw-rw-rw-   0        0        0     4629 2023-06-27 16:03:41.000000 laok-0.2.20/laok/base/fs/fpath.py
+-rw-rw-rw-   0        0        0     1785 2023-05-04 11:06:06.000000 laok-0.2.20/laok/base/fs/fsearch.py
+-rw-rw-rw-   0        0        0     2819 2023-05-05 03:57:37.000000 laok-0.2.20/laok/base/fs/fwalk.py
+-rw-rw-rw-   0        0        0     1413 2023-04-19 09:23:34.000000 laok-0.2.20/laok/base/fs/name_index.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.595237 laok-0.2.20/laok/base/log/
+-rw-rw-rw-   0        0        0       50 2023-04-19 14:41:08.000000 laok-0.2.20/laok/base/log/__init__.py
+-rw-rw-rw-   0        0        0     2187 2023-07-14 02:24:25.000000 laok-0.2.20/laok/base/log/log.py
+-rw-rw-rw-   0        0        0      672 2023-04-19 14:43:17.000000 laok-0.2.20/laok/base/log/log_default.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.599227 laok-0.2.20/laok/base/net/
+-rw-rw-rw-   0        0        0       78 2023-06-06 16:23:58.000000 laok-0.2.20/laok/base/net/__init__.py
+-rw-rw-rw-   0        0        0      691 2022-09-23 00:45:15.000000 laok-0.2.20/laok/base/net/ip.py
+-rw-rw-rw-   0        0        0     3792 2023-06-27 10:59:29.000000 laok-0.2.20/laok/base/net/requests_.py
+-rw-rw-rw-   0        0        0     1200 2023-06-27 10:55:31.000000 laok-0.2.20/laok/base/net/url.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.600224 laok-0.2.20/laok/base/paral/
+-rw-rw-rw-   0        0        0       20 2022-10-21 10:13:37.000000 laok-0.2.20/laok/base/paral/__init__.py
+-rw-rw-rw-   0        0        0     2010 2023-04-20 15:21:46.000000 laok-0.2.20/laok/base/paral/pool.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.602219 laok-0.2.20/laok/base/pkg/
+-rw-rw-rw-   0        0        0       32 2023-07-03 15:46:47.000000 laok-0.2.20/laok/base/pkg/__init__.py
+-rw-rw-rw-   0        0        0    27875 2023-07-03 15:50:30.000000 laok-0.2.20/laok/base/pkg/_lazy.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.610197 laok-0.2.20/laok/base/ser/
+-rw-rw-rw-   0        0        0      156 2023-06-06 14:13:13.000000 laok-0.2.20/laok/base/ser/__init__.py
+-rw-rw-rw-   0        0        0     1367 2023-04-25 06:50:06.000000 laok-0.2.20/laok/base/ser/json_.py
+-rw-rw-rw-   0        0        0      750 2023-04-20 13:46:22.000000 laok-0.2.20/laok/base/ser/marshal_.py
+-rw-rw-rw-   0        0        0      676 2023-06-01 07:58:10.000000 laok-0.2.20/laok/base/ser/numpy_.py
+-rw-rw-rw-   0        0        0      621 2023-04-25 06:50:29.000000 laok-0.2.20/laok/base/ser/pickle_.py
+-rw-rw-rw-   0        0        0     1369 2023-06-10 01:42:11.000000 laok-0.2.20/laok/base/ser/torch_.py
+-rw-rw-rw-   0        0        0     1452 2023-06-06 17:03:52.000000 laok-0.2.20/laok/base/ser/xml_.py
+-rw-rw-rw-   0        0        0     1341 2023-06-01 07:57:17.000000 laok-0.2.20/laok/base/ser/yaml_.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.614187 laok-0.2.20/laok/base/str/
+-rw-rw-rw-   0        0        0       84 2023-06-10 01:11:15.000000 laok-0.2.20/laok/base/str/__init__.py
+-rw-rw-rw-   0        0        0      735 2023-06-10 01:09:44.000000 laok-0.2.20/laok/base/str/cvt.py
+-rw-rw-rw-   0        0        0      427 2023-06-10 01:10:45.000000 laok-0.2.20/laok/base/str/fmt.py
+-rw-rw-rw-   0        0        0     1705 2023-06-10 01:10:56.000000 laok-0.2.20/laok/base/str/misc.py
+-rw-rw-rw-   0        0        0     2588 2023-06-01 07:58:57.000000 laok-0.2.20/laok/base/str/print_info.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.618177 laok-0.2.20/laok/base/syst/
+-rw-rw-rw-   0        0        0       74 2023-07-03 11:23:20.000000 laok-0.2.20/laok/base/syst/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-05-04 15:23:10.000000 laok-0.2.20/laok/base/syst/platform_.py
+-rw-rw-rw-   0        0        0     1871 2022-10-21 10:13:37.000000 laok-0.2.20/laok/base/syst/print_info.py
+-rw-rw-rw-   0        0        0      380 2023-07-03 11:23:24.000000 laok-0.2.20/laok/base/syst/sys_.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.620171 laok-0.2.20/laok/base/test/
+-rw-rw-rw-   0        0        0       43 2022-10-21 10:13:37.000000 laok-0.2.20/laok/base/test/__init__.py
+-rw-rw-rw-   0        0        0     8790 2023-07-11 07:18:36.000000 laok-0.2.20/laok/base/test/_dump.py
+-rw-rw-rw-   0        0        0     4551 2023-06-01 05:41:11.000000 laok-0.2.20/laok/base/test/_run.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.621168 laok-0.2.20/laok/cv2d/
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.622166 laok-0.2.20/laok/cv2d/PIL_/
+-rw-rw-rw-   0        0        0        0 2023-07-12 09:00:52.000000 laok-0.2.20/laok/cv2d/PIL_/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.20/laok/cv2d/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.634133 laok-0.2.20/laok/cv2d/cv2_/
+-rw-rw-rw-   0        0        0      252 2023-07-12 14:13:06.000000 laok-0.2.20/laok/cv2d/cv2_/__init__.py
+-rw-rw-rw-   0        0        0     2115 2023-07-12 12:32:21.000000 laok-0.2.20/laok/cv2d/cv2_/bin.py
+-rw-rw-rw-   0        0        0      951 2023-07-12 14:53:01.000000 laok-0.2.20/laok/cv2d/cv2_/contours.py
+-rw-rw-rw-   0        0        0     2580 2023-07-11 11:20:43.000000 laok-0.2.20/laok/cv2d/cv2_/cvt.py
+-rw-rw-rw-   0        0        0     4358 2023-07-12 06:55:54.000000 laok-0.2.20/laok/cv2d/cv2_/draw.py
+-rw-rw-rw-   0        0        0      956 2023-07-12 14:26:53.000000 laok-0.2.20/laok/cv2d/cv2_/edge.py
+-rw-rw-rw-   0        0        0     1268 2023-07-12 13:43:27.000000 laok-0.2.20/laok/cv2d/cv2_/filter.py
+-rw-rw-rw-   0        0        0      630 2023-07-12 07:16:54.000000 laok-0.2.20/laok/cv2d/cv2_/geo.py
+-rw-rw-rw-   0        0        0     1019 2023-07-11 16:28:07.000000 laok-0.2.20/laok/cv2d/cv2_/info.py
+-rw-rw-rw-   0        0        0     3240 2023-07-11 14:03:03.000000 laok-0.2.20/laok/cv2d/cv2_/io.py
+-rw-rw-rw-   0        0        0     2787 2023-07-12 13:56:20.000000 laok-0.2.20/laok/cv2d/cv2_/morph.py
+-rw-rw-rw-   0        0        0     1230 2023-07-11 15:01:26.000000 laok-0.2.20/laok/cv2d/cv2_/show.py
+-rw-rw-rw-   0        0        0      828 2023-07-11 15:21:15.000000 laok-0.2.20/laok/cv2d/cv2_/util.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.635131 laok-0.2.20/laok/cv2d/skimage_/
+-rw-rw-rw-   0        0        0      330 2023-07-11 05:10:30.000000 laok-0.2.20/laok/cv2d/skimage_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.635131 laok-0.2.20/laok/cv3d/
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.20/laok/cv3d/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.636129 laok-0.2.20/laok/cv3d/open3d_/
+-rw-rw-rw-   0        0        0      330 2023-07-11 05:10:30.000000 laok-0.2.20/laok/cv3d/open3d_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.637125 laok-0.2.20/laok/data/
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.20/laok/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.638123 laok-0.2.20/laok/data/lxml_/
+-rw-rw-rw-   0        0        0     1982 2023-07-11 06:14:29.000000 laok-0.2.20/laok/data/lxml_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.639120 laok-0.2.20/laok/data/yaml_/
+-rw-rw-rw-   0        0        0      330 2023-07-11 05:10:30.000000 laok-0.2.20/laok/data/yaml_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.639120 laok-0.2.20/laok/dnn/
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.20/laok/dnn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.640117 laok-0.2.20/laok/dnn/onnx_/
+-rw-rw-rw-   0        0        0     3116 2023-07-11 03:56:12.000000 laok-0.2.20/laok/dnn/onnx_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.641115 laok-0.2.20/laok/dnn/torch_/
+-rw-rw-rw-   0        0        0       88 2023-04-19 08:20:33.000000 laok-0.2.20/laok/dnn/torch_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.643109 laok-0.2.20/laok/dnn/torch_/datasets/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.646101 laok-0.2.20/laok/dnn/torch_/datasets/kitti/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/datasets/kitti/__init__.py
+-rw-rw-rw-   0        0        0    12031 2022-11-03 16:22:33.000000 laok-0.2.20/laok/dnn/torch_/datasets/kitti/kitti.py
+-rw-rw-rw-   0        0        0    27294 2022-10-28 06:48:12.000000 laok-0.2.20/laok/dnn/torch_/datasets/kitti/obj.py
+-rw-rw-rw-   0        0        0    26349 2022-11-03 16:22:33.000000 laok-0.2.20/laok/dnn/torch_/datasets/kitti/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.652086 laok-0.2.20/laok/dnn/torch_/datasets/model_net/
+-rw-rw-rw-   0        0        0      954 2022-11-03 16:22:33.000000 laok-0.2.20/laok/dnn/torch_/datasets/model_net/__init__.py
+-rw-rw-rw-   0        0        0     3721 2022-11-03 16:22:33.000000 laok-0.2.20/laok/dnn/torch_/datasets/model_net/model_net.py
+-rw-rw-rw-   0        0        0     4467 2022-11-03 16:22:33.000000 laok-0.2.20/laok/dnn/torch_/datasets/model_net/model_net_ineratia.py
+-rw-rw-rw-   0        0        0     3895 2022-11-03 16:22:33.000000 laok-0.2.20/laok/dnn/torch_/datasets/model_net/model_net_normals.py
+-rw-rw-rw-   0        0        0     4553 2022-11-03 16:22:33.000000 laok-0.2.20/laok/dnn/torch_/datasets/model_net/model_net_normals_diff.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.653083 laok-0.2.20/laok/dnn/torch_/datasets/shape_net/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/datasets/shape_net/__init__.py
+-rw-rw-rw-   0        0        0     5463 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/datasets/shape_net/shape_net.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.655077 laok-0.2.20/laok/dnn/torch_/datasets/stanford_indoor/
+-rw-rw-rw-   0        0        0        0 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/datasets/stanford_indoor/__init__.py
+-rw-rw-rw-   0        0        0    11035 2022-10-12 15:00:14.000000 laok-0.2.20/laok/dnn/torch_/datasets/stanford_indoor/_stanford_indoor.py
+-rw-rw-rw-   0        0        0     2811 2022-11-02 07:35:53.000000 laok-0.2.20/laok/dnn/torch_/datasets/ustc_lidar.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.660064 laok-0.2.20/laok/dnn/torch_/io/
+-rw-rw-rw-   0        0        0       80 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/io/__init__.py
+-rw-rw-rw-   0        0        0      732 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/io/img.py
+-rw-rw-rw-   0        0        0      844 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/io/jit.py
+-rw-rw-rw-   0        0        0     1344 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/io/model.py
+-rw-rw-rw-   0        0        0      466 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/io/onnx.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.663056 laok-0.2.20/laok/dnn/torch_/op/
+-rw-rw-rw-   0        0        0       70 2023-04-19 08:22:19.000000 laok-0.2.20/laok/dnn/torch_/op/__init__.py
+-rw-rw-rw-   0        0        0      965 2023-04-19 08:22:06.000000 laok-0.2.20/laok/dnn/torch_/op/device.py
+-rw-rw-rw-   0        0        0     1703 2023-04-19 08:27:44.000000 laok-0.2.20/laok/dnn/torch_/op/module.py
+-rw-rw-rw-   0        0        0     1403 2023-04-19 08:25:22.000000 laok-0.2.20/laok/dnn/torch_/op/print_info.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.668043 laok-0.2.20/laok/dnn/torch_/trainval/
+-rw-rw-rw-   0        0        0       89 2022-10-21 10:13:37.000000 laok-0.2.20/laok/dnn/torch_/trainval/__init__.py
+-rw-rw-rw-   0        0        0     3943 2023-04-19 09:12:20.000000 laok-0.2.20/laok/dnn/torch_/trainval/check_point.py
+-rw-rw-rw-   0        0        0     2280 2023-04-19 09:25:29.000000 laok-0.2.20/laok/dnn/torch_/trainval/infer.py
+-rw-rw-rw-   0        0        0     2848 2023-04-19 08:44:39.000000 laok-0.2.20/laok/dnn/torch_/trainval/train.py
+-rw-rw-rw-   0        0        0     2308 2023-04-19 09:08:59.000000 laok-0.2.20/laok/dnn/torch_/trainval/val.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.669041 laok-0.2.20/laok/gui/
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.20/laok/gui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.671035 laok-0.2.20/laok/gui/matplot_/
+-rw-rw-rw-   0        0        0       19 2023-07-12 09:01:52.000000 laok-0.2.20/laok/gui/matplot_/__init__.py
+-rw-rw-rw-   0        0        0     2096 2023-07-12 16:09:46.000000 laok-0.2.20/laok/gui/matplot_/show.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.674027 laok-0.2.20/laok/gui/qt_/
+-rw-rw-rw-   0        0        0       62 2023-07-14 02:30:38.000000 laok-0.2.20/laok/gui/qt_/__init__.py
+-rw-rw-rw-   0        0        0      582 2023-07-14 03:03:10.000000 laok-0.2.20/laok/gui/qt_/dialog.py
+-rw-rw-rw-   0        0        0     1004 2023-07-14 02:15:56.000000 laok-0.2.20/laok/gui/qt_/run.py
+-rw-rw-rw-   0        0        0     1931 2023-07-14 03:22:35.000000 laok-0.2.20/laok/gui/qt_/ui.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.675024 laok-0.2.20/laok/matical/
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.20/laok/matical/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.676021 laok-0.2.20/laok/matical/numpy_/
+-rw-rw-rw-   0        0        0        0 2023-04-20 14:21:33.000000 laok-0.2.20/laok/matical/numpy_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.677019 laok-0.2.20/laok/ml/
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.20/laok/ml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.677019 laok-0.2.20/laok/ml/sklearn_/
+-rw-rw-rw-   0        0        0      330 2023-07-11 05:10:30.000000 laok-0.2.20/laok/ml/sklearn_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.678016 laok-0.2.20/laok/net/
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.20/laok/net/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.680011 laok-0.2.20/laok/net/flask_/
+-rw-rw-rw-   0        0        0       42 2023-04-19 15:05:48.000000 laok-0.2.20/laok/net/flask_/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-04-19 15:05:30.000000 laok-0.2.20/laok/net/flask_/app.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.682006 laok-0.2.20/laok/net/flask_/basic/
+-rw-rw-rw-   0        0        0       22 2023-04-19 15:06:08.000000 laok-0.2.20/laok/net/flask_/basic/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-04-19 15:38:09.000000 laok-0.2.20/laok/net/flask_/basic/views.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.683003 laok-0.2.20/laok/net/requests_/
+-rw-rw-rw-   0        0        0     3808 2023-07-11 04:59:34.000000 laok-0.2.20/laok/net/requests_/__init__.py
+-rw-rw-rw-   0        0        0      649 2023-07-11 04:06:36.000000 laok-0.2.20/laok/third_lib.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.686993 laok-0.2.20/laok/tool/
+-rw-rw-rw-   0        0        0        0 2023-03-10 09:11:01.000000 laok-0.2.20/laok/tool/__init__.py
+-rw-rw-rw-   0        0        0     3604 2023-07-11 06:29:13.000000 laok-0.2.20/laok/tool/download_m3u8.py
+-rw-rw-rw-   0        0        0     2310 2023-07-04 03:20:00.000000 laok-0.2.20/laok/tool/ultralytics_.py
+drwxrwxrwx   0        0        0        0 2023-07-14 09:20:51.575291 laok-0.2.20/laok.egg-info/
+-rw-rw-rw-   0        0        0      214 2023-07-14 09:20:51.000000 laok-0.2.20/laok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3708 2023-07-14 09:20:51.000000 laok-0.2.20/laok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 09:20:51.000000 laok-0.2.20/laok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-14 09:20:51.000000 laok-0.2.20/laok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 09:20:51.687990 laok-0.2.20/setup.cfg
+-rw-rw-rw-   0        0        0      322 2023-07-14 09:20:27.000000 laok-0.2.20/setup.py
```

### Comparing `laok-0.2.19/laok/base/alg/addict.py` & `laok-0.2.20/laok/base/alg/addict.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/conf/factory.py` & `laok-0.2.20/laok/base/conf/factory.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/dataset/cvt_voc_yolo.py` & `laok-0.2.20/laok/base/dataset/cvt_voc_yolo.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/dataset/darknet-voc2yolo.py` & `laok-0.2.20/laok/base/dataset/darknet-voc2yolo.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/dataset/voc_label.py` & `laok-0.2.20/laok/base/dataset/voc_label.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/dtime/datetime_.py` & `laok-0.2.20/laok/base/dtime/datetime_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/dtime/timer.py` & `laok-0.2.20/laok/base/dtime/timer.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/fs/fdata.py` & `laok-0.2.20/laok/base/fs/fdata.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/fs/fname.py` & `laok-0.2.20/laok/base/fs/fname.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/fs/fpath.py` & `laok-0.2.20/laok/base/fs/fpath.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/fs/fsearch.py` & `laok-0.2.20/laok/base/fs/fsearch.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/fs/fwalk.py` & `laok-0.2.20/laok/base/fs/fwalk.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/fs/name_index.py` & `laok-0.2.20/laok/base/fs/name_index.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/log/log.py` & `laok-0.2.20/laok/base/log/log.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/log/log_default.py` & `laok-0.2.20/laok/base/log/log_default.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/net/ip.py` & `laok-0.2.20/laok/base/net/ip.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/net/requests_.py` & `laok-0.2.20/laok/base/net/requests_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/net/url.py` & `laok-0.2.20/laok/base/net/url.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/paral/pool.py` & `laok-0.2.20/laok/base/paral/pool.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/pkg/_lazy.py` & `laok-0.2.20/laok/base/pkg/_lazy.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/ser/json_.py` & `laok-0.2.20/laok/base/ser/json_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/ser/marshal_.py` & `laok-0.2.20/laok/base/ser/marshal_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/ser/numpy_.py` & `laok-0.2.20/laok/base/ser/numpy_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/ser/pickle_.py` & `laok-0.2.20/laok/base/ser/pickle_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/ser/torch_.py` & `laok-0.2.20/laok/base/ser/torch_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/ser/xml_.py` & `laok-0.2.20/laok/base/ser/xml_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/ser/yaml_.py` & `laok-0.2.20/laok/base/ser/yaml_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/str/cvt.py` & `laok-0.2.20/laok/base/str/cvt.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/str/misc.py` & `laok-0.2.20/laok/base/str/misc.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/str/print_info.py` & `laok-0.2.20/laok/base/str/print_info.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/syst/platform_.py` & `laok-0.2.20/laok/base/syst/platform_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/syst/print_info.py` & `laok-0.2.20/laok/base/syst/print_info.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/test/_dump.py` & `laok-0.2.20/laok/base/test/_dump.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/base/test/_run.py` & `laok-0.2.20/laok/base/test/_run.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/cv2d/cv2_/bin.py` & `laok-0.2.20/laok/cv2d/cv2_/bin.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/cv2d/cv2_/contours.py` & `laok-0.2.20/laok/cv2d/cv2_/contours.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/cv2d/cv2_/cvt.py` & `laok-0.2.20/laok/cv2d/cv2_/cvt.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/cv2d/cv2_/draw.py` & `laok-0.2.20/laok/cv2d/cv2_/draw.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/cv2d/cv2_/edge.py` & `laok-0.2.20/laok/cv2d/cv2_/edge.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/cv2d/cv2_/filter.py` & `laok-0.2.20/laok/cv2d/cv2_/filter.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/cv2d/cv2_/geo.py` & `laok-0.2.20/laok/cv2d/cv2_/geo.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/cv2d/cv2_/info.py` & `laok-0.2.20/laok/cv2d/cv2_/info.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/cv2d/cv2_/io.py` & `laok-0.2.20/laok/cv2d/cv2_/io.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/cv2d/cv2_/morph.py` & `laok-0.2.20/laok/cv2d/cv2_/morph.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/cv2d/cv2_/show.py` & `laok-0.2.20/laok/cv2d/cv2_/show.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/cv2d/cv2_/util.py` & `laok-0.2.20/laok/cv2d/cv2_/util.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/data/lxml_/__init__.py` & `laok-0.2.20/laok/data/lxml_/__init__.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/onnx_/__init__.py` & `laok-0.2.20/laok/dnn/onnx_/__init__.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/datasets/kitti/kitti.py` & `laok-0.2.20/laok/dnn/torch_/datasets/kitti/kitti.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/datasets/kitti/obj.py` & `laok-0.2.20/laok/dnn/torch_/datasets/kitti/obj.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/datasets/kitti/utils.py` & `laok-0.2.20/laok/dnn/torch_/datasets/kitti/utils.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/datasets/model_net/__init__.py` & `laok-0.2.20/laok/dnn/torch_/datasets/model_net/__init__.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/datasets/model_net/model_net.py` & `laok-0.2.20/laok/dnn/torch_/datasets/model_net/model_net.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/datasets/model_net/model_net_ineratia.py` & `laok-0.2.20/laok/dnn/torch_/datasets/model_net/model_net_ineratia.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/datasets/model_net/model_net_normals.py` & `laok-0.2.20/laok/dnn/torch_/datasets/model_net/model_net_normals.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/datasets/model_net/model_net_normals_diff.py` & `laok-0.2.20/laok/dnn/torch_/datasets/model_net/model_net_normals_diff.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/datasets/shape_net/shape_net.py` & `laok-0.2.20/laok/dnn/torch_/datasets/shape_net/shape_net.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/datasets/stanford_indoor/_stanford_indoor.py` & `laok-0.2.20/laok/dnn/torch_/datasets/stanford_indoor/_stanford_indoor.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/datasets/ustc_lidar.py` & `laok-0.2.20/laok/dnn/torch_/datasets/ustc_lidar.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/io/img.py` & `laok-0.2.20/laok/dnn/torch_/io/img.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/io/jit.py` & `laok-0.2.20/laok/dnn/torch_/io/jit.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/io/model.py` & `laok-0.2.20/laok/dnn/torch_/io/model.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/op/device.py` & `laok-0.2.20/laok/dnn/torch_/op/device.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/op/module.py` & `laok-0.2.20/laok/dnn/torch_/op/module.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/op/print_info.py` & `laok-0.2.20/laok/dnn/torch_/op/print_info.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/trainval/check_point.py` & `laok-0.2.20/laok/dnn/torch_/trainval/check_point.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/trainval/infer.py` & `laok-0.2.20/laok/dnn/torch_/trainval/infer.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/trainval/train.py` & `laok-0.2.20/laok/dnn/torch_/trainval/train.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/dnn/torch_/trainval/val.py` & `laok-0.2.20/laok/dnn/torch_/trainval/val.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/gui/matplot_/show.py` & `laok-0.2.20/laok/gui/matplot_/show.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/gui/qt_/dialog.py` & `laok-0.2.20/laok/gui/qt_/dialog.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/gui/qt_/run.py` & `laok-0.2.20/laok/gui/qt_/run.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/gui/qt_/ui.py` & `laok-0.2.20/laok/gui/qt_/ui.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 '''
 Created on 2020/7/21 10:33:17
 
 @author: LiuKuan
 @copyright: Apache License, Version 2.0
 '''
 import os, sys
-from PyQt5.QtWidgets import QWidget, QMainWindow
+from PyQt5.QtWidgets import QWidget, QMainWindow, QDialog
 from PyQt5.uic import loadUi, compileUi
 from laok.base import log_info
 #===============================================================================
 #
 #===============================================================================
 
-__all__ = ['UiMainWindowDy', 'UiDyWidget', 'compile_ui_file']
+__all__ = ['UiMainWindowDy', 'UiDyWidget', 'UiDyDialog', 'compile_ui_file']
 
 def _init_ui_file(obj):
     if hasattr(obj, 'ui_file'):
         ui_file = getattr(obj, 'ui_file')
     else:
         module_file = sys.modules[obj.__module__].__file__
         ui_file = os.path.splitext(module_file)[0] + ".ui"
@@ -45,14 +45,24 @@
         QWidget.__init__(obj)
         _init_ui_file(obj)
         return obj
 
     def __init__(self):
         pass
 
+class UiDyDialog(QDialog):
+    def __new__(cls, *args, **kwargs):
+        obj = super().__new__(cls)
+        QDialog.__init__(obj)
+        _init_ui_file(obj)
+        return obj
+
+    def __init__(self):
+        pass
+
 def compile_ui_file(ui_file, save_file=None):
     '''
         保存 X_ui.py 文件
     '''
     if save_file is None:
         save_file = os.path.splitext(ui_file)[0] + '_ui.py'
     with open(save_file, 'w', encoding='utf8') as f:
```

### Comparing `laok-0.2.19/laok/net/flask_/basic/views.py` & `laok-0.2.20/laok/net/flask_/basic/views.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/net/requests_/__init__.py` & `laok-0.2.20/laok/net/requests_/__init__.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/third_lib.py` & `laok-0.2.20/laok/third_lib.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/tool/download_m3u8.py` & `laok-0.2.20/laok/tool/download_m3u8.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok/tool/ultralytics_.py` & `laok-0.2.20/laok/tool/ultralytics_.py`

 * *Files identical despite different names*

### Comparing `laok-0.2.19/laok.egg-info/SOURCES.txt` & `laok-0.2.20/laok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

