# Comparing `tmp/ork.build.tools-0.0.3.tar.gz` & `tmp/ork.build.tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ork.build.tools-0.0.3.tar", last modified: Fri Jul 14 18:53:09 2023, max compression
+gzip compressed data, was "ork.build.tools-0.0.4.tar", last modified: Fri Jul 14 18:55:49 2023, max compression
```

## Comparing `ork.build.tools-0.0.3.tar` & `ork.build.tools-0.0.4.tar`

### file list

```diff
@@ -1,419 +1,419 @@
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:09.014072 ork.build.tools-0.0.3/
--rw-r--r--   0 michael    (501) wheel        (0)    14849 2023-07-14 18:53:09.012826 ork.build.tools-0.0.3/PKG-INFO
--rw-r--r--   0 michael    (501) wheel        (0)    14749 2023-07-14 17:52:14.000000 ork.build.tools-0.0.3/README.md
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.835234 ork.build.tools-0.0.3/bin_pub/
--rwxr-xr-x   0 michael    (501) wheel        (0)     5555 2023-07-14 17:52:14.000000 ork.build.tools-0.0.3/bin_pub/obt.create.env.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     8042 2023-07-14 17:52:14.000000 ork.build.tools-0.0.3/bin_pub/obt.init.env.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      445 2023-07-14 17:52:14.000000 ork.build.tools-0.0.3/bin_pub/obt.ix.installdeps.gentoo.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2951 2023-07-14 17:52:14.000000 ork.build.tools-0.0.3/bin_pub/obt.ix.installdeps.linuxcnc.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2779 2023-07-14 17:52:14.000000 ork.build.tools-0.0.3/bin_pub/obt.ix.installdeps.ubuntu_aarch64.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     3176 2023-07-14 17:52:14.000000 ork.build.tools-0.0.3/bin_pub/obt.ix.installdeps.ubuntu_x86_64.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      734 2023-07-14 17:52:14.000000 ork.build.tools-0.0.3/bin_pub/obt.osx.installdeps.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.821710 ork.build.tools-0.0.3/examples/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.835591 ork.build.tools-0.0.3/examples/dep-overrides/
--rw-r--r--   0 michael    (501) wheel        (0)     1530 2022-09-08 21:51:23.000000 ork.build.tools-0.0.3/examples/dep-overrides/orkid.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.838744 ork.build.tools-0.0.3/examples/litex1/
--rwxr-xr-x   0 michael    (501) wheel        (0)     4642 2022-09-08 21:51:23.000000 ork.build.tools-0.0.3/examples/litex1/arty.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      389 2022-09-08 21:51:23.000000 ork.build.tools-0.0.3/examples/litex1/bit2svf_nexysv.tcl
--rw-r--r--   0 michael    (501) wheel        (0)    11759 2022-09-08 21:51:23.000000 ork.build.tools-0.0.3/examples/litex1/cmod_a7_platform.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     3002 2022-09-08 21:51:23.000000 ork.build.tools-0.0.3/examples/litex1/cmod_a7_target.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     4526 2022-09-08 21:51:23.000000 ork.build.tools-0.0.3/examples/litex1/nexys_video.py
--rw-r--r--   0 michael    (501) wheel        (0)      628 2022-09-08 21:51:23.000000 ork.build.tools-0.0.3/examples/litex1/nexysv.cfg
--rwxr-xr-x   0 michael    (501) wheel        (0)      247 2022-09-08 21:51:23.000000 ork.build.tools-0.0.3/examples/litex1/soc_arty.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2559 2022-09-08 21:51:23.000000 ork.build.tools-0.0.3/examples/litex1/soc_nexysv.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.841561 ork.build.tools-0.0.3/examples/litex_zephyrtest/
--rw-r--r--   0 michael    (501) wheel        (0)      213 2022-09-08 21:51:23.000000 ork.build.tools-0.0.3/examples/litex_zephyrtest/CMakeLists.txt
--rw-r--r--   0 michael    (501) wheel        (0)    11415 2022-09-08 21:51:23.000000 ork.build.tools-0.0.3/examples/litex_zephyrtest/LICENSE
--rw-r--r--   0 michael    (501) wheel        (0)     1015 2022-09-08 21:51:23.000000 ork.build.tools-0.0.3/examples/litex_zephyrtest/README.rst
--rwxr-xr-x   0 michael    (501) wheel        (0)      315 2022-09-08 21:51:23.000000 ork.build.tools-0.0.3/examples/litex_zephyrtest/build.py
--rw-r--r--   0 michael    (501) wheel        (0)      111 2022-09-08 21:51:23.000000 ork.build.tools-0.0.3/examples/litex_zephyrtest/main.c
--rw-r--r--   0 michael    (501) wheel        (0)       75 2022-09-08 21:51:23.000000 ork.build.tools-0.0.3/examples/litex_zephyrtest/prj.conf
--rw-r--r--   0 michael    (501) wheel        (0)      703 2022-09-08 21:51:23.000000 ork.build.tools-0.0.3/examples/litex_zephyrtest/sample.yaml
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.842040 ork.build.tools-0.0.3/examples/litex_zephyrtest/src/
--rw-r--r--   0 michael    (501) wheel        (0)     2515 2022-09-08 21:51:23.000000 ork.build.tools-0.0.3/examples/litex_zephyrtest/src/main.c
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.829049 ork.build.tools-0.0.3/modules/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.917562 ork.build.tools-0.0.3/modules/dep/
--rw-r--r--   0 michael    (501) wheel        (0)      718 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     8257 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     1276 2023-05-09 20:23:50.000000 ork.build.tools-0.0.3/modules/dep/_nnsvs.py
--rw-r--r--   0 michael    (501) wheel        (0)     1910 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/apitrace.py
--rw-r--r--   0 michael    (501) wheel        (0)     1776 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/arachnepnr.py
--rw-r--r--   0 michael    (501) wheel        (0)     1663 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/arm64_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     1580 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/arm64_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     2051 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/dep/assimp.py
--rw-r--r--   0 michael    (501) wheel        (0)     1712 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/astcencoder.py
--rw-r--r--   0 michael    (501) wheel        (0)     1675 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/audiofile.py
--rw-r--r--   0 michael    (501) wheel        (0)     1611 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/avr_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     2206 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/avr_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     2209 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/avr_libc.py
--rw-r--r--   0 michael    (501) wheel        (0)     1793 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/bazel.py
--rw-r--r--   0 michael    (501) wheel        (0)     1302 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/blosc.py
--rw-r--r--   0 michael    (501) wheel        (0)     9272 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/boost.py
--rw-r--r--   0 michael    (501) wheel        (0)     1248 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/bullet.py
--rw-r--r--   0 michael    (501) wheel        (0)     2004 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/calf.py
--rw-r--r--   0 michael    (501) wheel        (0)     1541 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/cgal.py
--rw-r--r--   0 michael    (501) wheel        (0)     2422 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/dep/clang.py
--rw-r--r--   0 michael    (501) wheel        (0)     1408 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/cmake.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1428 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/dep/cpppeglib.py
--rw-r--r--   0 michael    (501) wheel        (0)     1632 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/cppzmq.py
--rw-r--r--   0 michael    (501) wheel        (0)     1563 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/csvparser.py
--rw-r--r--   0 michael    (501) wheel        (0)     1257 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/cuda.py
--rw-r--r--   0 michael    (501) wheel        (0)     1684 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/curlpp.py
--rw-r--r--   0 michael    (501) wheel        (0)     1757 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/cycles.py
--rw-r--r--   0 michael    (501) wheel        (0)     1579 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/dep/depthaicore.py
--rw-r--r--   0 michael    (501) wheel        (0)      992 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/drawtext.py
--rw-r--r--   0 michael    (501) wheel        (0)     1491 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/easyprof.py
--rw-r--r--   0 michael    (501) wheel        (0)     1454 2023-02-18 06:09:54.000000 ork.build.tools-0.0.3/modules/dep/eigen.py
--rw-r--r--   0 michael    (501) wheel        (0)     2047 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/embree.py
--rw-r--r--   0 michael    (501) wheel        (0)     1871 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/faust.py
--rw-r--r--   0 michael    (501) wheel        (0)     1577 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/fcollada.py
--rw-r--r--   0 michael    (501) wheel        (0)     1737 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/ffmpeg.py
--rw-r--r--   0 michael    (501) wheel        (0)     1997 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/dep/flatcam.py
--rw-r--r--   0 michael    (501) wheel        (0)     1676 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/fltk.py
--rw-r--r--   0 michael    (501) wheel        (0)     1891 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/fluidsynth.py
--rw-r--r--   0 michael    (501) wheel        (0)     1866 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/frameretrace.py
--rw-r--r--   0 michael    (501) wheel        (0)     1438 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/gcode_gpr.py
--rw-r--r--   0 michael    (501) wheel        (0)     2148 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/giflib.py
--rw-r--r--   0 michael    (501) wheel        (0)     1175 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/gitpython.py
--rw-r--r--   0 michael    (501) wheel        (0)     2601 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/glfw.py
--rw-r--r--   0 michael    (501) wheel        (0)     1544 2023-02-18 06:09:54.000000 ork.build.tools-0.0.3/modules/dep/glm.py
--rw-r--r--   0 michael    (501) wheel        (0)      894 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/gnutar.py
--rw-r--r--   0 michael    (501) wheel        (0)      756 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/houdini.py
--rw-r--r--   0 michael    (501) wheel        (0)     1731 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/icestorm.py
--rw-r--r--   0 michael    (501) wheel        (0)     2898 2023-03-18 06:31:34.000000 ork.build.tools-0.0.3/modules/dep/igl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1767 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/irix65_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     6593 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/irix65_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     1150 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/irrlicht.py
--rw-r--r--   0 michael    (501) wheel        (0)     3478 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/ispc.py
--rw-r--r--   0 michael    (501) wheel        (0)     2331 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/ispctexc.py
--rw-r--r--   0 michael    (501) wheel        (0)     1316 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/jpegturbo.py
--rw-r--r--   0 michael    (501) wheel        (0)     1719 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/dep/klein.py
--rw-r--r--   0 michael    (501) wheel        (0)     1079 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/lapack.py
--rw-r--r--   0 michael    (501) wheel        (0)     1065 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/lemongraph.py
--rw-r--r--   0 michael    (501) wheel        (0)     1301 2023-06-17 04:32:01.000000 ork.build.tools-0.0.3/modules/dep/lexertl14.py
--rw-r--r--   0 michael    (501) wheel        (0)     1664 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/libcurl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1701 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/libfive.py
--rw-r--r--   0 michael    (501) wheel        (0)     1490 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/libpqpp.py
--rw-r--r--   0 michael    (501) wheel        (0)     1425 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/libsocket.py
--rw-r--r--   0 michael    (501) wheel        (0)     1419 2023-05-12 22:40:05.000000 ork.build.tools-0.0.3/modules/dep/libsurvive.py
--rw-r--r--   0 michael    (501) wheel        (0)     7892 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/libtorch.py
--rw-r--r--   0 michael    (501) wheel        (0)     1926 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/linuxcnc.py
--rw-r--r--   0 michael    (501) wheel        (0)     2487 2023-07-14 17:52:14.000000 ork.build.tools-0.0.3/modules/dep/litex.py
--rw-r--r--   0 michael    (501) wheel        (0)     2529 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/llvm.py
--rw-r--r--   0 michael    (501) wheel        (0)     1339 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/lm32_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     1066 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/lm32_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     2937 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/lua.py
--rw-r--r--   0 michael    (501) wheel        (0)     2135 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/luajit.py
--rw-r--r--   0 michael    (501) wheel        (0)     1664 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/m68k_amiga_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     1555 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/m68k_amiga_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     3841 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/minetest.py
--rw-r--r--   0 michael    (501) wheel        (0)     2009 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/moltenvk.py
--rw-r--r--   0 michael    (501) wheel        (0)     1244 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/nextpnr.py
--rw-r--r--   0 michael    (501) wheel        (0)     2117 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/ngc.py
--rw-r--r--   0 michael    (501) wheel        (0)     1426 2023-04-27 00:04:32.000000 ork.build.tools-0.0.3/modules/dep/nlohmannjson.py
--rw-r--r--   0 michael    (501) wheel        (0)     1633 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/nss.py
--rw-r--r--   0 michael    (501) wheel        (0)     1464 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/nsync_cpp.py
--rw-r--r--   0 michael    (501) wheel        (0)     3022 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/nvtt.py
--rw-r--r--   0 michael    (501) wheel        (0)     1562 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/ocio.py
--rw-r--r--   0 michael    (501) wheel        (0)     2587 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/dep/oiio.py
--rw-r--r--   0 michael    (501) wheel        (0)     1738 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/oneapimkl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1406 2023-04-27 00:04:41.000000 ork.build.tools-0.0.3/modules/dep/openblas.py
--rw-r--r--   0 michael    (501) wheel        (0)     2857 2023-04-25 17:02:18.000000 ork.build.tools-0.0.3/modules/dep/opencv.py
--rw-r--r--   0 michael    (501) wheel        (0)     1358 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/dep/opencv_contrib.py
--rw-r--r--   0 michael    (501) wheel        (0)     1217 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/opendb.py
--rw-r--r--   0 michael    (501) wheel        (0)     1556 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/dep/openexr.py
--rw-r--r--   0 michael    (501) wheel        (0)     1332 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/openjpeg.py
--rw-r--r--   0 michael    (501) wheel        (0)     1270 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/openroad.py
--rw-r--r--   0 michael    (501) wheel        (0)     1791 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/opensubdiv.py
--rw-r--r--   0 michael    (501) wheel        (0)     1447 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/dep/openvdb.py
--rw-r--r--   0 michael    (501) wheel        (0)     1376 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/openvr.py
--rw-r--r--   0 michael    (501) wheel        (0)     5172 2023-06-23 17:21:13.000000 ork.build.tools-0.0.3/modules/dep/orkid.py
--rw-r--r--   0 michael    (501) wheel        (0)     1306 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/osgeolaszip.py
--rw-r--r--   0 michael    (501) wheel        (0)     1495 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/osgeoliblas.py
--rw-r--r--   0 michael    (501) wheel        (0)     1345 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/osgeoproj.py
--rw-r--r--   0 michael    (501) wheel        (0)     1543 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/osgeotiff.py
--rw-r--r--   0 michael    (501) wheel        (0)     1447 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/osl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1249 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/dep/ozzanim.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1619 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/pangolin.py
--rw-r--r--   0 michael    (501) wheel        (0)     1874 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/dep/parsertl14.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.823209 ork.build.tools-0.0.3/modules/dep/patches/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.822565 ork.build.tools-0.0.3/modules/dep/patches/boost/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.918824 ork.build.tools-0.0.3/modules/dep/patches/boost/chg/
--rw-r--r--   0 michael    (501) wheel        (0)    22151 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/patches/boost/chg/darwin.jam
--rw-r--r--   0 michael    (501) wheel        (0)     1111 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/patches/boost/chg/project-config.jam
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.919346 ork.build.tools-0.0.3/modules/dep/patches/boost/ori/
--rw-r--r--   0 michael    (501) wheel        (0)    22062 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/patches/boost/ori/darwin.jam
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.922238 ork.build.tools-0.0.3/modules/dep/patches/gcc/
--rw-r--r--   0 michael    (501) wheel        (0)   116535 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/patches/gcc/gcc.sgifixes.patch
--rw-r--r--   0 michael    (501) wheel        (0)      522 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/patches/gcc/gcc.sgifixlibstdcpp01.patch
--rw-r--r--   0 michael    (501) wheel        (0)      475 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/patches/gcc/gcc.sgifixlibstdcpp02.patch
--rw-r--r--   0 michael    (501) wheel        (0)      801 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/patches/gcc/newlib.sgifixes.patch
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.823027 ork.build.tools-0.0.3/modules/dep/patches/giflib/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.922801 ork.build.tools-0.0.3/modules/dep/patches/giflib/chg/
--rw-r--r--   0 michael    (501) wheel        (0)     5546 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/patches/giflib/chg/Makefile
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.923363 ork.build.tools-0.0.3/modules/dep/patches/giflib/ori/
--rw-r--r--   0 michael    (501) wheel        (0)     4712 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/patches/giflib/ori/Makefile
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.823684 ork.build.tools-0.0.3/modules/dep/patches/pillar/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.923914 ork.build.tools-0.0.3/modules/dep/patches/pillar/chg/
--rw-r--r--   0 michael    (501) wheel        (0)     1660 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/patches/pillar/chg/markdown.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.924494 ork.build.tools-0.0.3/modules/dep/patches/pillar/ori/
--rw-r--r--   0 michael    (501) wheel        (0)     1645 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/patches/pillar/ori/markdown.py
--rw-r--r--   0 michael    (501) wheel        (0)     1748 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/pillar.py
--rw-r--r--   0 michael    (501) wheel        (0)     2152 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/pkgconfig.py
--rw-r--r--   0 michael    (501) wheel        (0)     1362 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/portaudio.py
--rw-r--r--   0 michael    (501) wheel        (0)     2133 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/postgresql.py
--rw-r--r--   0 michael    (501) wheel        (0)     1989 2023-03-30 23:28:01.000000 ork.build.tools-0.0.3/modules/dep/premake.py
--rw-r--r--   0 michael    (501) wheel        (0)     1526 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/ptex.py
--rw-r--r--   0 michael    (501) wheel        (0)     1298 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/pugixml.py
--rw-r--r--   0 michael    (501) wheel        (0)     1488 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/pybind11.py
--rw-r--r--   0 michael    (501) wheel        (0)     1459 2023-02-05 19:15:34.000000 ork.build.tools-0.0.3/modules/dep/pydefaults.py
--rw-r--r--   0 michael    (501) wheel        (0)      822 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/pyopengl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1954 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/pyqt5.py
--rw-r--r--   0 michael    (501) wheel        (0)      814 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/pyside2.py
--rw-r--r--   0 michael    (501) wheel        (0)     7450 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/dep/python.py
--rw-r--r--   0 michael    (501) wheel        (0)     5932 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/qt5.py
--rw-r--r--   0 michael    (501) wheel        (0)     1781 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/qt5ct.py
--rw-r--r--   0 michael    (501) wheel        (0)     5913 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/qt5forpython.py
--rw-r--r--   0 michael    (501) wheel        (0)     1942 2023-03-06 06:24:34.000000 ork.build.tools-0.0.3/modules/dep/rapidjson.py
--rw-r--r--   0 michael    (501) wheel        (0)     3538 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/dep/realsense2.py
--rw-r--r--   0 michael    (501) wheel        (0)     1032 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/root.py
--rw-r--r--   0 michael    (501) wheel        (0)     1344 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/rtmidi.py
--rw-r--r--   0 michael    (501) wheel        (0)     1345 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/rv32_binutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     1069 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/rv32_gcc.py
--rw-r--r--   0 michael    (501) wheel        (0)     1355 2023-03-30 23:28:01.000000 ork.build.tools-0.0.3/modules/dep/sigslot.py
--rw-r--r--   0 michael    (501) wheel        (0)     1215 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/simavr.py
--rw-r--r--   0 michael    (501) wheel        (0)     1370 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/dep/sse2neon.py
--rw-r--r--   0 michael    (501) wheel        (0)     2929 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/dep/tbb.py
--rw-r--r--   0 michael    (501) wheel        (0)     6552 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/tflite.py
--rw-r--r--   0 michael    (501) wheel        (0)     3343 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/ue5.py
--rw-r--r--   0 michael    (501) wheel        (0)     6344 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/ue5_cesium.py
--rw-r--r--   0 michael    (501) wheel        (0)     1669 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/unittestpp.py
--rw-r--r--   0 michael    (501) wheel        (0)     2361 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/usd.py
--rw-r--r--   0 michael    (501) wheel        (0)     1289 2023-03-30 23:28:01.000000 ork.build.tools-0.0.3/modules/dep/vhacd.py
--rw-r--r--   0 michael    (501) wheel        (0)     1316 2023-07-14 17:52:14.000000 ork.build.tools-0.0.3/modules/dep/vivado.py
--rw-r--r--   0 michael    (501) wheel        (0)     2962 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/vpf.py
--rw-r--r--   0 michael    (501) wheel        (0)     1892 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/vrx.py
--rw-r--r--   0 michael    (501) wheel        (0)     1972 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/vst3sdk.py
--rw-r--r--   0 michael    (501) wheel        (0)     4325 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/dep/vulkan.py
--rw-r--r--   0 michael    (501) wheel        (0)     2772 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/wt4.py
--rw-r--r--   0 michael    (501) wheel        (0)     2144 2023-03-30 23:28:01.000000 ork.build.tools-0.0.3/modules/dep/xatlas.py
--rw-r--r--   0 michael    (501) wheel        (0)     1107 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/yarl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1887 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/yosys.py
--rw-r--r--   0 michael    (501) wheel        (0)     1922 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/zephyr.py
--rw-r--r--   0 michael    (501) wheel        (0)     1719 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/dep/zmq.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.827727 ork.build.tools-0.0.3/modules/docker/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.925617 ork.build.tools-0.0.3/modules/docker/amigadev/
--rw-r--r--   0 michael    (501) wheel        (0)     1042 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/amigadev/Dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     2813 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/docker/amigadev/amigadev.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.928904 ork.build.tools-0.0.3/modules/docker/amigadev/test1/
--rw-r--r--   0 michael    (501) wheel        (0)      280 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/amigadev/test1/Makefile
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.929436 ork.build.tools-0.0.3/modules/docker/amigadev/test1/S/
--rw-r--r--   0 michael    (501) wheel        (0)        8 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/amigadev/test1/S/Startup-Sequence
--rwxr-xr-x   0 michael    (501) wheel        (0)      418 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/amigadev/test1/_build.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)      527 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/amigadev/test1/build.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.930566 ork.build.tools-0.0.3/modules/docker/amigadev/test1/libs/
--rw-r--r--   0 michael    (501) wheel        (0)     4688 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/amigadev/test1/libs/mathieeedoubbas.library
--rw-r--r--   0 michael    (501) wheel        (0)    15728 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/amigadev/test1/libs/mathieeedoubtrans.library
--rw-r--r--   0 michael    (501) wheel        (0)     5351 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/amigadev/test1/main.cpp
--rwxr-xr-x   0 michael    (501) wheel        (0)     1177 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/amigadev/test1/test_fsuae.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      391 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/amigadev/test1/test_vamos.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.931787 ork.build.tools-0.0.3/modules/docker/androiddev/
--rw-r--r--   0 michael    (501) wheel        (0)     1679 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/androiddev/Dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     2071 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/androiddev/androiddev.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.937104 ork.build.tools-0.0.3/modules/docker/cicd/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.943282 ork.build.tools-0.0.3/modules/docker/cicd/bin/
--rw-r--r--   0 michael    (501) wheel        (0)        1 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/bin/__init__.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      457 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/bin/build_master_image.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      276 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/bin/build_worker_android_image.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      271 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/bin/build_worker_ub20_image.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      271 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/bin/build_worker_ub22_image.py
--rw-r--r--   0 michael    (501) wheel        (0)      644 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/bin/ci_common.py
--rwxr-xr-x   0 michael    (501) wheel        (0)       66 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/bin/launch_attached.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)       64 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/bin/launch_detached.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)       83 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/bin/launch_testnossl.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)       46 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/bin/terminate.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)     1188 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/bin/test_worker_android.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1235 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/bin/test_worker_ub20.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1255 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/bin/test_worker_ub22.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.952187 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/
--rw-r--r--   0 michael    (501) wheel        (0)      307 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/TODO.txt
--rw-r--r--   0 michael    (501) wheel        (0)     9906 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/_masterimpl.py
--rw-r--r--   0 michael    (501) wheel        (0)     6829 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/_watcher.py
--rw-r--r--   0 michael    (501) wheel        (0)     1087 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/_workerimpl.py
--rw-r--r--   0 michael    (501) wheel        (0)     3772 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/_zmqssh.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.953969 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/assets/
--rw-r--r--   0 michael    (501) wheel        (0)    71033 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/assets/OrkidLogo.png
--rw-r--r--   0 michael    (501) wheel        (0)     1778 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/assets/index.template
--rw-r--r--   0 michael    (501) wheel        (0)     3091 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/assets/variant.template
--rw-r--r--   0 michael    (501) wheel        (0)     4134 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/badge.py
--rw-r--r--   0 michael    (501) wheel        (0)      218 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/dummy.svg
--rw-r--r--   0 michael    (501) wheel        (0)     2881 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/httphandler.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1768 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/master.py
--rw-r--r--   0 michael    (501) wheel        (0)     2597 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/orkbb.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1538 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/process_log.py
--rw-r--r--   0 michael    (501) wheel        (0)     7766 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/scheduler.py
--rwxr-xr-x   0 michael    (501) wheel        (0)       53 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/spin.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/start-master.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/start-worker.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)     7710 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/worker.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     4005 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/worker_build_branch.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1335 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/worker_fetch_branch.py
--rw-r--r--   0 michael    (501) wheel        (0)     1708 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/cicd.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.954921 ork.build.tools-0.0.3/modules/docker/cicd/conf/
--rw-r--r--   0 michael    (501) wheel        (0)      420 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/conf/nginx_app.conf
--rw-r--r--   0 michael    (501) wheel        (0)      898 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/conf/nginx_ssl.conf
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.959025 ork.build.tools-0.0.3/modules/docker/cicd/container-scripts/
--rwxr-xr-x   0 michael    (501) wheel        (0)     2542 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu19.py
--rw-r--r--   0 michael    (501) wheel        (0)     2641 2023-07-14 17:52:14.000000 ork.build.tools-0.0.3/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu22.py
--rw-r--r--   0 michael    (501) wheel        (0)       53 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/container-scripts/spin.sh
--rw-r--r--   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/container-scripts/start-master.sh
--rw-r--r--   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/container-scripts/start-worker.sh
--rw-r--r--   0 michael    (501) wheel        (0)       20 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/container-scripts/worker.bashrc
--rw-r--r--   0 michael    (501) wheel        (0)      221 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/container-scripts/worker.test.sh
--rw-r--r--   0 michael    (501) wheel        (0)     1126 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/docker-compose-nossl.yml
--rw-r--r--   0 michael    (501) wheel        (0)     1222 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/docker-compose.yml
--rw-r--r--   0 michael    (501) wheel        (0)     2043 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/master.dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     1037 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/master.json
--rw-r--r--   0 michael    (501) wheel        (0)      228 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/readme.md
--rw-r--r--   0 michael    (501) wheel        (0)     3551 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/worker-android.dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     3138 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/worker-ub20.dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     3138 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/worker-ub22.dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)      203 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/worker20.json
--rw-r--r--   0 michael    (501) wheel        (0)      203 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/cicd/worker22.json
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.961824 ork.build.tools-0.0.3/modules/docker/ps1dev/
--rw-r--r--   0 michael    (501) wheel        (0)     1019 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/ps1dev/Dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     2268 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/ps1dev/Makefile.cfg
--rwxr-xr-x   0 michael    (501) wheel        (0)      223 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/ps1dev/fetch.sh
--rw-r--r--   0 michael    (501) wheel        (0)     2750 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/ps1dev/ps1dev.py
--rw-r--r--   0 michael    (501) wheel        (0)       71 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/ps1dev/readme.md
--rwxr-xr-x   0 michael    (501) wheel        (0)      756 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/ps1dev/setup.sh
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.962339 ork.build.tools-0.0.3/modules/docker/ps1dev/testprograms/
--rw-r--r--   0 michael    (501) wheel        (0)      890 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/ps1dev/testprograms/project.mk
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.963315 ork.build.tools-0.0.3/modules/docker/ps1dev/testprograms/test1/
--rw-r--r--   0 michael    (501) wheel        (0)       86 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/ps1dev/testprograms/test1/Makefile
--rw-r--r--   0 michael    (501) wheel        (0)     7821 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/ps1dev/testprograms/test1/test1.c
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.964208 ork.build.tools-0.0.3/modules/docker/realsense2/
--rw-r--r--   0 michael    (501) wheel        (0)     2325 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/docker/realsense2/Dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     3446 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/modules/docker/realsense2/realsense2.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.966080 ork.build.tools-0.0.3/modules/docker/sagemath/
--rw-r--r--   0 michael    (501) wheel        (0)     2646 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/sagemath/Dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)      347 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/sagemath/docker-compose.yml
--rwxr-xr-x   0 michael    (501) wheel        (0)      100 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/sagemath/entrypoint.sh
--rw-r--r--   0 michael    (501) wheel        (0)     2757 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/sagemath/sagemath.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.968435 ork.build.tools-0.0.3/modules/docker/tflow2gpu/
--rwxr-xr-x   0 michael    (501) wheel        (0)     2775 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/tflow2gpu/Dockerfile
--rwxr-xr-x   0 michael    (501) wheel        (0)      519 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/tflow2gpu/test_mediapipe.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)     2533 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/tflow2gpu/test_multi_gpu.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1715 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/tflow2gpu/test_single_gpu.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     2483 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/tflow2gpu/tflow2gpu.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.969349 ork.build.tools-0.0.3/modules/docker/ub-focal/
--rw-r--r--   0 michael    (501) wheel        (0)      517 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/ub-focal/Dockerfile
--rw-r--r--   0 michael    (501) wheel        (0)     1702 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/docker/ub-focal/ub-focal.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.971204 ork.build.tools-0.0.3/modules/host/
--rw-r--r--   0 michael    (501) wheel        (0)     1181 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/host/aarch64-linux.py
--rw-r--r--   0 michael    (501) wheel        (0)     1629 2023-03-06 06:24:34.000000 ork.build.tools-0.0.3/modules/host/aarch64-macos.py
--rw-r--r--   0 michael    (501) wheel        (0)     1409 2023-05-09 20:23:50.000000 ork.build.tools-0.0.3/modules/host/x86_64-linux.py
--rw-r--r--   0 michael    (501) wheel        (0)     2165 2023-04-05 23:31:27.000000 ork.build.tools-0.0.3/modules/host/x86_64-macos.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.974225 ork.build.tools-0.0.3/modules/sdk/
--rw-r--r--   0 michael    (501) wheel        (0)     4088 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/sdk/aarch64-android.py
--rw-r--r--   0 michael    (501) wheel        (0)     1678 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/sdk/aarch64-ios.py
--rw-r--r--   0 michael    (501) wheel        (0)      782 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/sdk/aarch64-macos.py
--rw-r--r--   0 michael    (501) wheel        (0)      222 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/sdk/cuda.py
--rw-r--r--   0 michael    (501) wheel        (0)      618 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/sdk/x86_64-linux.py
--rw-r--r--   0 michael    (501) wheel        (0)      625 2023-04-05 23:26:33.000000 ork.build.tools-0.0.3/modules/sdk/x86_64-macos.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.976252 ork.build.tools-0.0.3/modules/subspace/
--rw-r--r--   0 michael    (501) wheel        (0)     7785 2023-06-24 23:47:10.000000 ork.build.tools-0.0.3/modules/subspace/conda.py
--rw-r--r--   0 michael    (501) wheel        (0)     1227 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/subspace/host.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.976732 ork.build.tools-0.0.3/modules/subspace/nnsvs/
--rwxr-xr-x   0 michael    (501) wheel        (0)     3419 2023-05-09 20:23:50.000000 ork.build.tools-0.0.3/modules/subspace/nnsvs/test.py
--rw-r--r--   0 michael    (501) wheel        (0)     4513 2023-06-24 23:47:10.000000 ork.build.tools-0.0.3/modules/subspace/nnsvs.py
--rw-r--r--   0 michael    (501) wheel        (0)     1187 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/subspace/yo.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.979560 ork.build.tools-0.0.3/modules/target/
--rw-r--r--   0 michael    (501) wheel        (0)      558 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/target/aarch64-android.py
--rw-r--r--   0 michael    (501) wheel        (0)      551 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/target/aarch64-ios.py
--rw-r--r--   0 michael    (501) wheel        (0)      554 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/target/aarch64-linux.py
--rw-r--r--   0 michael    (501) wheel        (0)      554 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/target/aarch64-macos.py
--rw-r--r--   0 michael    (501) wheel        (0)      556 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/target/x86_64-linux.py
--rw-r--r--   0 michael    (501) wheel        (0)      556 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/modules/target/x86_64-macos.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:08.829904 ork.build.tools-0.0.3/scripts/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:09.003201 ork.build.tools-0.0.3/scripts/ork/
--rw-r--r--   0 michael    (501) wheel        (0)       67 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/scripts/ork/__init__.py
--rw-r--r--   0 michael    (501) wheel        (0)    12346 2023-04-25 17:02:18.000000 ork.build.tools-0.0.3/scripts/ork/_dep_build.py
--rw-r--r--   0 michael    (501) wheel        (0)     1460 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/_dep_dl.py
--rw-r--r--   0 michael    (501) wheel        (0)     1619 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/_dep_enumerate.py
--rw-r--r--   0 michael    (501) wheel        (0)     8444 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/scripts/ork/_dep_fetch.py
--rw-r--r--   0 michael    (501) wheel        (0)     2872 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/scripts/ork/_dep_impl.py
--rw-r--r--   0 michael    (501) wheel        (0)     4822 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/scripts/ork/_dep_node.py
--rw-r--r--   0 michael    (501) wheel        (0)    13516 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/scripts/ork/_dep_provider.py
--rw-r--r--   0 michael    (501) wheel        (0)     3450 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/_dep_x.py
--rw-r--r--   0 michael    (501) wheel        (0)    12708 2023-06-24 23:47:10.000000 ork.build.tools-0.0.3/scripts/ork/_envutils.py
--rw-r--r--   0 michael    (501) wheel        (0)     1925 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/_globals.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      375 2023-06-24 23:47:39.000000 ork.build.tools-0.0.3/scripts/ork/_obt_dep_completions.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      418 2023-06-24 23:47:39.000000 ork.build.tools-0.0.3/scripts/ork/_obt_dep_completions_shell.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      322 2023-06-24 23:47:10.000000 ork.build.tools-0.0.3/scripts/ork/_obt_subspace_completions.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:09.005609 ork.build.tools-0.0.3/scripts/ork/build/
--rw-r--r--   0 michael    (501) wheel        (0)       23 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/build/__init__.py
--rw-r--r--   0 michael    (501) wheel        (0)     1365 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/build/manifest.py
--rw-r--r--   0 michael    (501) wheel        (0)     5607 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/buildtrace.py
--rw-r--r--   0 michael    (501) wheel        (0)     2959 2023-04-26 23:56:07.000000 ork.build.tools-0.0.3/scripts/ork/cmake.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:09.006551 ork.build.tools-0.0.3/scripts/ork/cnc/
--rw-r--r--   0 michael    (501) wheel        (0)        2 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/scripts/ork/cnc/__init__.py
--rw-r--r--   0 michael    (501) wheel        (0)     7782 2023-02-05 19:12:10.000000 ork.build.tools-0.0.3/scripts/ork/cnc/saf.py
--rw-r--r--   0 michael    (501) wheel        (0)     8668 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/command.py
--rw-r--r--   0 michael    (501) wheel        (0)     1486 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/common.py
--rw-r--r--   0 michael    (501) wheel        (0)      803 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/config.py
--rw-r--r--   0 michael    (501) wheel        (0)     8068 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/deco.py
--rw-r--r--   0 michael    (501) wheel        (0)      849 2023-06-24 23:47:10.000000 ork.build.tools-0.0.3/scripts/ork/dep.py
--rw-r--r--   0 michael    (501) wheel        (0)     2756 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/docker.py
--rw-r--r--   0 michael    (501) wheel        (0)     1266 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/env.py
--rw-r--r--   0 michael    (501) wheel        (0)     1806 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/executors.py
--rw-r--r--   0 michael    (501) wheel        (0)     1241 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/gen_pkgconfig.py
--rw-r--r--   0 michael    (501) wheel        (0)     5172 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/git.py
--rw-r--r--   0 michael    (501) wheel        (0)     2868 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/host.py
--rw-r--r--   0 michael    (501) wheel        (0)      268 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/libav.py
--rw-r--r--   0 michael    (501) wheel        (0)      927 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/litex.py
--rw-r--r--   0 michael    (501) wheel        (0)      285 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/log.py
--rw-r--r--   0 michael    (501) wheel        (0)     2849 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/macos.py
--rw-r--r--   0 michael    (501) wheel        (0)      141 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/macos_homebrew.py
--rw-r--r--   0 michael    (501) wheel        (0)     1080 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/make.py
--rw-r--r--   0 michael    (501) wheel        (0)       75 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/math.py
--rw-r--r--   0 michael    (501) wheel        (0)     2040 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/module.py
--rw-r--r--   0 michael    (501) wheel        (0)      145 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/net.py
--rw-r--r--   0 michael    (501) wheel        (0)     1194 2023-05-12 22:40:05.000000 ork.build.tools-0.0.3/scripts/ork/osrelease.py
--rw-r--r--   0 michael    (501) wheel        (0)      983 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/patch.py
--rw-r--r--   0 michael    (501) wheel        (0)     8359 2023-06-24 23:47:10.000000 ork.build.tools-0.0.3/scripts/ork/path.py
--rw-r--r--   0 michael    (501) wheel        (0)     8544 2023-04-25 17:02:18.000000 ork.build.tools-0.0.3/scripts/ork/pathtools.py
--rw-r--r--   0 michael    (501) wheel        (0)      668 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/pip.py
--rw-r--r--   0 michael    (501) wheel        (0)       75 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/pybind11.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1341 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/scp.py
--rw-r--r--   0 michael    (501) wheel        (0)     1747 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/sdk.py
--rw-r--r--   0 michael    (501) wheel        (0)     4538 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/search.py
--rw-r--r--   0 michael    (501) wheel        (0)     3241 2023-04-25 17:02:18.000000 ork.build.tools-0.0.3/scripts/ork/subspace.py
--rw-r--r--   0 michael    (501) wheel        (0)     1334 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/target.py
--rw-r--r--   0 michael    (501) wheel        (0)     1559 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/template.py
--rw-r--r--   0 michael    (501) wheel        (0)     6511 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/utils.py
--rw-r--r--   0 michael    (501) wheel        (0)     2080 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/wget.py
--rw-r--r--   0 michael    (501) wheel        (0)      591 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/scripts/ork/xcode.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:09.004917 ork.build.tools-0.0.3/scripts/ork.build.tools.egg-info/
--rw-r--r--   0 michael    (501) wheel        (0)    14849 2023-07-14 18:53:08.000000 ork.build.tools-0.0.3/scripts/ork.build.tools.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) wheel        (0)    10954 2023-07-14 18:53:08.000000 ork.build.tools-0.0.3/scripts/ork.build.tools.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) wheel        (0)        1 2023-07-14 18:53:08.000000 ork.build.tools-0.0.3/scripts/ork.build.tools.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) wheel        (0)        1 2023-07-14 18:53:08.000000 ork.build.tools-0.0.3/scripts/ork.build.tools.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) wheel        (0)       38 2023-07-14 18:53:09.014196 ork.build.tools-0.0.3/setup.cfg
--rw-r--r--   0 michael    (501) wheel        (0)     1255 2023-07-14 18:53:03.000000 ork.build.tools-0.0.3/setup.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:09.007480 ork.build.tools-0.0.3/tests/
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:09.009349 ork.build.tools-0.0.3/tests/docker-gpu/
--rw-r--r--   0 michael    (501) wheel        (0)      411 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/tests/docker-gpu/Dockerfile
--rwxr-xr-x   0 michael    (501) wheel        (0)       53 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/tests/docker-gpu/build.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)      358 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/tests/docker-gpu/launch_glmark.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)      369 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/tests/docker-gpu/launch_nvtopo.sh
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:09.011209 ork.build.tools-0.0.3/tests/docker-gpu-tensorflow/
--rw-r--r--   0 michael    (501) wheel        (0)      505 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/tests/docker-gpu-tensorflow/Dockerfile
--rwxr-xr-x   0 michael    (501) wheel        (0)       55 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/tests/docker-gpu-tensorflow/build.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)      379 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/tests/docker-gpu-tensorflow/launch_nvtopo.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)      391 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/tests/docker-gpu-tensorflow/launch_tf.sh
--rwxr-xr-x   0 michael    (501) wheel        (0)     1543 2023-07-14 17:52:14.000000 ork.build.tools-0.0.3/tests/litex1_nx4.py
--rwxr-xr-x   0 michael    (501) wheel        (0)      178 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/tests/osx_rpaths.py
-drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:53:09.012135 ork.build.tools-0.0.3/tests/pytorch/
--rwxr-xr-x   0 michael    (501) wheel        (0)      916 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/tests/pytorch/install.py
--rwxr-xr-x   0 michael    (501) wheel        (0)     1190 2022-09-08 21:51:24.000000 ork.build.tools-0.0.3/tests/pytorch/training.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:49.040183 ork.build.tools-0.0.4/
+-rw-r--r--   0 michael    (501) wheel        (0)    14849 2023-07-14 18:55:49.039609 ork.build.tools-0.0.4/PKG-INFO
+-rw-r--r--   0 michael    (501) wheel        (0)    14749 2023-07-14 17:52:14.000000 ork.build.tools-0.0.4/README.md
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.846628 ork.build.tools-0.0.4/bin_pub/
+-rwxr-xr-x   0 michael    (501) wheel        (0)     5555 2023-07-14 17:52:14.000000 ork.build.tools-0.0.4/bin_pub/obt.create.env.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     8042 2023-07-14 17:52:14.000000 ork.build.tools-0.0.4/bin_pub/obt.init.env.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      445 2023-07-14 17:52:14.000000 ork.build.tools-0.0.4/bin_pub/obt.ix.installdeps.gentoo.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2951 2023-07-14 17:52:14.000000 ork.build.tools-0.0.4/bin_pub/obt.ix.installdeps.linuxcnc.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2779 2023-07-14 17:52:14.000000 ork.build.tools-0.0.4/bin_pub/obt.ix.installdeps.ubuntu_aarch64.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     3176 2023-07-14 17:52:14.000000 ork.build.tools-0.0.4/bin_pub/obt.ix.installdeps.ubuntu_x86_64.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      734 2023-07-14 17:52:14.000000 ork.build.tools-0.0.4/bin_pub/obt.osx.installdeps.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.833161 ork.build.tools-0.0.4/examples/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.847016 ork.build.tools-0.0.4/examples/dep-overrides/
+-rw-r--r--   0 michael    (501) wheel        (0)     1530 2022-09-08 21:51:23.000000 ork.build.tools-0.0.4/examples/dep-overrides/orkid.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.850639 ork.build.tools-0.0.4/examples/litex1/
+-rwxr-xr-x   0 michael    (501) wheel        (0)     4642 2022-09-08 21:51:23.000000 ork.build.tools-0.0.4/examples/litex1/arty.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      389 2022-09-08 21:51:23.000000 ork.build.tools-0.0.4/examples/litex1/bit2svf_nexysv.tcl
+-rw-r--r--   0 michael    (501) wheel        (0)    11759 2022-09-08 21:51:23.000000 ork.build.tools-0.0.4/examples/litex1/cmod_a7_platform.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     3002 2022-09-08 21:51:23.000000 ork.build.tools-0.0.4/examples/litex1/cmod_a7_target.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     4526 2022-09-08 21:51:23.000000 ork.build.tools-0.0.4/examples/litex1/nexys_video.py
+-rw-r--r--   0 michael    (501) wheel        (0)      628 2022-09-08 21:51:23.000000 ork.build.tools-0.0.4/examples/litex1/nexysv.cfg
+-rwxr-xr-x   0 michael    (501) wheel        (0)      247 2022-09-08 21:51:23.000000 ork.build.tools-0.0.4/examples/litex1/soc_arty.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2559 2022-09-08 21:51:23.000000 ork.build.tools-0.0.4/examples/litex1/soc_nexysv.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.853559 ork.build.tools-0.0.4/examples/litex_zephyrtest/
+-rw-r--r--   0 michael    (501) wheel        (0)      213 2022-09-08 21:51:23.000000 ork.build.tools-0.0.4/examples/litex_zephyrtest/CMakeLists.txt
+-rw-r--r--   0 michael    (501) wheel        (0)    11415 2022-09-08 21:51:23.000000 ork.build.tools-0.0.4/examples/litex_zephyrtest/LICENSE
+-rw-r--r--   0 michael    (501) wheel        (0)     1015 2022-09-08 21:51:23.000000 ork.build.tools-0.0.4/examples/litex_zephyrtest/README.rst
+-rwxr-xr-x   0 michael    (501) wheel        (0)      315 2022-09-08 21:51:23.000000 ork.build.tools-0.0.4/examples/litex_zephyrtest/build.py
+-rw-r--r--   0 michael    (501) wheel        (0)      111 2022-09-08 21:51:23.000000 ork.build.tools-0.0.4/examples/litex_zephyrtest/main.c
+-rw-r--r--   0 michael    (501) wheel        (0)       75 2022-09-08 21:51:23.000000 ork.build.tools-0.0.4/examples/litex_zephyrtest/prj.conf
+-rw-r--r--   0 michael    (501) wheel        (0)      703 2022-09-08 21:51:23.000000 ork.build.tools-0.0.4/examples/litex_zephyrtest/sample.yaml
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.853966 ork.build.tools-0.0.4/examples/litex_zephyrtest/src/
+-rw-r--r--   0 michael    (501) wheel        (0)     2515 2022-09-08 21:51:23.000000 ork.build.tools-0.0.4/examples/litex_zephyrtest/src/main.c
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.840644 ork.build.tools-0.0.4/modules/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.938223 ork.build.tools-0.0.4/modules/dep/
+-rw-r--r--   0 michael    (501) wheel        (0)      718 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     8257 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1276 2023-05-09 20:23:50.000000 ork.build.tools-0.0.4/modules/dep/_nnsvs.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1910 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/apitrace.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1776 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/arachnepnr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1663 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/arm64_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1580 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/arm64_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2051 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/dep/assimp.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1712 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/astcencoder.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1675 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/audiofile.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1611 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/avr_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2206 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/avr_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2209 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/avr_libc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1793 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/bazel.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1302 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/blosc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     9272 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/boost.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1248 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/bullet.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2004 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/calf.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1541 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/cgal.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2422 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/dep/clang.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1408 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/cmake.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1428 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/dep/cpppeglib.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1632 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/cppzmq.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1563 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/csvparser.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1257 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/cuda.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1684 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/curlpp.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1757 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/cycles.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1579 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/dep/depthaicore.py
+-rw-r--r--   0 michael    (501) wheel        (0)      992 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/drawtext.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1491 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/easyprof.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1454 2023-02-18 06:09:54.000000 ork.build.tools-0.0.4/modules/dep/eigen.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2047 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/embree.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1871 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/faust.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1577 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/fcollada.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1737 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/ffmpeg.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1997 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/dep/flatcam.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1676 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/fltk.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1891 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/fluidsynth.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1866 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/frameretrace.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1438 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/gcode_gpr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2148 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/giflib.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1175 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/gitpython.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2601 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/glfw.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1544 2023-02-18 06:09:54.000000 ork.build.tools-0.0.4/modules/dep/glm.py
+-rw-r--r--   0 michael    (501) wheel        (0)      894 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/gnutar.py
+-rw-r--r--   0 michael    (501) wheel        (0)      756 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/houdini.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1731 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/icestorm.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2898 2023-03-18 06:31:34.000000 ork.build.tools-0.0.4/modules/dep/igl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1767 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/irix65_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     6593 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/irix65_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1150 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/irrlicht.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3478 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/ispc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2331 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/ispctexc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1316 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/jpegturbo.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1719 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/dep/klein.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1079 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/lapack.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1065 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/lemongraph.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1301 2023-06-17 04:32:01.000000 ork.build.tools-0.0.4/modules/dep/lexertl14.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1664 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/libcurl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1701 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/libfive.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1490 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/libpqpp.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1425 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/libsocket.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1419 2023-05-12 22:40:05.000000 ork.build.tools-0.0.4/modules/dep/libsurvive.py
+-rw-r--r--   0 michael    (501) wheel        (0)     7892 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/libtorch.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1926 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/linuxcnc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2487 2023-07-14 17:52:14.000000 ork.build.tools-0.0.4/modules/dep/litex.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2529 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/llvm.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1339 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/lm32_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1066 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/lm32_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2937 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/lua.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2135 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/luajit.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1664 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/m68k_amiga_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1555 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/m68k_amiga_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3841 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/minetest.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2009 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/moltenvk.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1244 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/nextpnr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2117 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/ngc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1426 2023-04-27 00:04:32.000000 ork.build.tools-0.0.4/modules/dep/nlohmannjson.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1633 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/nss.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1464 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/nsync_cpp.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3022 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/nvtt.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1562 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/ocio.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2587 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/dep/oiio.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1738 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/oneapimkl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1406 2023-04-27 00:04:41.000000 ork.build.tools-0.0.4/modules/dep/openblas.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2857 2023-04-25 17:02:18.000000 ork.build.tools-0.0.4/modules/dep/opencv.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1358 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/dep/opencv_contrib.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1217 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/opendb.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1556 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/dep/openexr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1332 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/openjpeg.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1270 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/openroad.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1791 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/opensubdiv.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1447 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/dep/openvdb.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1376 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/openvr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     5172 2023-06-23 17:21:13.000000 ork.build.tools-0.0.4/modules/dep/orkid.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1306 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/osgeolaszip.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1495 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/osgeoliblas.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1345 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/osgeoproj.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1543 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/osgeotiff.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1447 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/osl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1249 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/dep/ozzanim.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1619 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/pangolin.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1874 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/dep/parsertl14.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.834726 ork.build.tools-0.0.4/modules/dep/patches/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.833960 ork.build.tools-0.0.4/modules/dep/patches/boost/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.939449 ork.build.tools-0.0.4/modules/dep/patches/boost/chg/
+-rw-r--r--   0 michael    (501) wheel        (0)    22151 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/patches/boost/chg/darwin.jam
+-rw-r--r--   0 michael    (501) wheel        (0)     1111 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/patches/boost/chg/project-config.jam
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.940023 ork.build.tools-0.0.4/modules/dep/patches/boost/ori/
+-rw-r--r--   0 michael    (501) wheel        (0)    22062 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/patches/boost/ori/darwin.jam
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.943199 ork.build.tools-0.0.4/modules/dep/patches/gcc/
+-rw-r--r--   0 michael    (501) wheel        (0)   116535 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/patches/gcc/gcc.sgifixes.patch
+-rw-r--r--   0 michael    (501) wheel        (0)      522 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/patches/gcc/gcc.sgifixlibstdcpp01.patch
+-rw-r--r--   0 michael    (501) wheel        (0)      475 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/patches/gcc/gcc.sgifixlibstdcpp02.patch
+-rw-r--r--   0 michael    (501) wheel        (0)      801 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/patches/gcc/newlib.sgifixes.patch
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.834430 ork.build.tools-0.0.4/modules/dep/patches/giflib/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.943739 ork.build.tools-0.0.4/modules/dep/patches/giflib/chg/
+-rw-r--r--   0 michael    (501) wheel        (0)     5546 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/patches/giflib/chg/Makefile
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.944258 ork.build.tools-0.0.4/modules/dep/patches/giflib/ori/
+-rw-r--r--   0 michael    (501) wheel        (0)     4712 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/patches/giflib/ori/Makefile
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.835088 ork.build.tools-0.0.4/modules/dep/patches/pillar/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.944785 ork.build.tools-0.0.4/modules/dep/patches/pillar/chg/
+-rw-r--r--   0 michael    (501) wheel        (0)     1660 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/patches/pillar/chg/markdown.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.945285 ork.build.tools-0.0.4/modules/dep/patches/pillar/ori/
+-rw-r--r--   0 michael    (501) wheel        (0)     1645 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/patches/pillar/ori/markdown.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1748 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/pillar.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2152 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/pkgconfig.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1362 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/portaudio.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2133 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/postgresql.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1989 2023-03-30 23:28:01.000000 ork.build.tools-0.0.4/modules/dep/premake.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1526 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/ptex.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1298 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/pugixml.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1488 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/pybind11.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1459 2023-02-05 19:15:34.000000 ork.build.tools-0.0.4/modules/dep/pydefaults.py
+-rw-r--r--   0 michael    (501) wheel        (0)      822 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/pyopengl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1954 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/pyqt5.py
+-rw-r--r--   0 michael    (501) wheel        (0)      814 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/pyside2.py
+-rw-r--r--   0 michael    (501) wheel        (0)     7450 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/dep/python.py
+-rw-r--r--   0 michael    (501) wheel        (0)     5932 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/qt5.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1781 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/qt5ct.py
+-rw-r--r--   0 michael    (501) wheel        (0)     5913 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/qt5forpython.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1942 2023-03-06 06:24:34.000000 ork.build.tools-0.0.4/modules/dep/rapidjson.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3538 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/dep/realsense2.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1032 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/root.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1344 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/rtmidi.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1345 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/rv32_binutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1069 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/rv32_gcc.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1355 2023-03-30 23:28:01.000000 ork.build.tools-0.0.4/modules/dep/sigslot.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1215 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/simavr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1370 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/dep/sse2neon.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2929 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/dep/tbb.py
+-rw-r--r--   0 michael    (501) wheel        (0)     6552 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/tflite.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3343 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/ue5.py
+-rw-r--r--   0 michael    (501) wheel        (0)     6344 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/ue5_cesium.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1669 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/unittestpp.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2361 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/usd.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1289 2023-03-30 23:28:01.000000 ork.build.tools-0.0.4/modules/dep/vhacd.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1316 2023-07-14 17:52:14.000000 ork.build.tools-0.0.4/modules/dep/vivado.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2962 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/vpf.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1892 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/vrx.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1972 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/vst3sdk.py
+-rw-r--r--   0 michael    (501) wheel        (0)     4325 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/dep/vulkan.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2772 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/wt4.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2144 2023-03-30 23:28:01.000000 ork.build.tools-0.0.4/modules/dep/xatlas.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1107 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/yarl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1887 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/yosys.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1922 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/zephyr.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1719 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/dep/zmq.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.839387 ork.build.tools-0.0.4/modules/docker/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.946248 ork.build.tools-0.0.4/modules/docker/amigadev/
+-rw-r--r--   0 michael    (501) wheel        (0)     1042 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/amigadev/Dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     2813 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/docker/amigadev/amigadev.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.949172 ork.build.tools-0.0.4/modules/docker/amigadev/test1/
+-rw-r--r--   0 michael    (501) wheel        (0)      280 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/amigadev/test1/Makefile
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.949704 ork.build.tools-0.0.4/modules/docker/amigadev/test1/S/
+-rw-r--r--   0 michael    (501) wheel        (0)        8 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/amigadev/test1/S/Startup-Sequence
+-rwxr-xr-x   0 michael    (501) wheel        (0)      418 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/amigadev/test1/_build.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)      527 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/amigadev/test1/build.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.950655 ork.build.tools-0.0.4/modules/docker/amigadev/test1/libs/
+-rw-r--r--   0 michael    (501) wheel        (0)     4688 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/amigadev/test1/libs/mathieeedoubbas.library
+-rw-r--r--   0 michael    (501) wheel        (0)    15728 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/amigadev/test1/libs/mathieeedoubtrans.library
+-rw-r--r--   0 michael    (501) wheel        (0)     5351 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/amigadev/test1/main.cpp
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1177 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/amigadev/test1/test_fsuae.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      391 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/amigadev/test1/test_vamos.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.951925 ork.build.tools-0.0.4/modules/docker/androiddev/
+-rw-r--r--   0 michael    (501) wheel        (0)     1679 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/androiddev/Dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     2071 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/androiddev/androiddev.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.957977 ork.build.tools-0.0.4/modules/docker/cicd/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.965730 ork.build.tools-0.0.4/modules/docker/cicd/bin/
+-rw-r--r--   0 michael    (501) wheel        (0)        1 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/bin/__init__.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      457 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/bin/build_master_image.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      276 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/bin/build_worker_android_image.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      271 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/bin/build_worker_ub20_image.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      271 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/bin/build_worker_ub22_image.py
+-rw-r--r--   0 michael    (501) wheel        (0)      644 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/bin/ci_common.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)       66 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/bin/launch_attached.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)       64 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/bin/launch_detached.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)       83 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/bin/launch_testnossl.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)       46 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/bin/terminate.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1188 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/bin/test_worker_android.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1235 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/bin/test_worker_ub20.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1255 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/bin/test_worker_ub22.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.974599 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/
+-rw-r--r--   0 michael    (501) wheel        (0)      307 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/TODO.txt
+-rw-r--r--   0 michael    (501) wheel        (0)     9906 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/_masterimpl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     6829 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/_watcher.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1087 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/_workerimpl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3772 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/_zmqssh.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.976259 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/assets/
+-rw-r--r--   0 michael    (501) wheel        (0)    71033 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/assets/OrkidLogo.png
+-rw-r--r--   0 michael    (501) wheel        (0)     1778 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/assets/index.template
+-rw-r--r--   0 michael    (501) wheel        (0)     3091 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/assets/variant.template
+-rw-r--r--   0 michael    (501) wheel        (0)     4134 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/badge.py
+-rw-r--r--   0 michael    (501) wheel        (0)      218 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/dummy.svg
+-rw-r--r--   0 michael    (501) wheel        (0)     2881 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/httphandler.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1768 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/master.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2597 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/orkbb.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1538 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/process_log.py
+-rw-r--r--   0 michael    (501) wheel        (0)     7766 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/scheduler.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)       53 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/spin.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/start-master.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/start-worker.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)     7710 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/worker.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     4005 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/worker_build_branch.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1335 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/worker_fetch_branch.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1708 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/cicd.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.977230 ork.build.tools-0.0.4/modules/docker/cicd/conf/
+-rw-r--r--   0 michael    (501) wheel        (0)      420 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/conf/nginx_app.conf
+-rw-r--r--   0 michael    (501) wheel        (0)      898 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/conf/nginx_ssl.conf
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.980574 ork.build.tools-0.0.4/modules/docker/cicd/container-scripts/
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2542 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu19.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2641 2023-07-14 17:52:14.000000 ork.build.tools-0.0.4/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu22.py
+-rw-r--r--   0 michael    (501) wheel        (0)       53 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/container-scripts/spin.sh
+-rw-r--r--   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/container-scripts/start-master.sh
+-rw-r--r--   0 michael    (501) wheel        (0)       80 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/container-scripts/start-worker.sh
+-rw-r--r--   0 michael    (501) wheel        (0)       20 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/container-scripts/worker.bashrc
+-rw-r--r--   0 michael    (501) wheel        (0)      221 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/container-scripts/worker.test.sh
+-rw-r--r--   0 michael    (501) wheel        (0)     1126 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/docker-compose-nossl.yml
+-rw-r--r--   0 michael    (501) wheel        (0)     1222 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/docker-compose.yml
+-rw-r--r--   0 michael    (501) wheel        (0)     2043 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/master.dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     1037 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/master.json
+-rw-r--r--   0 michael    (501) wheel        (0)      228 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/readme.md
+-rw-r--r--   0 michael    (501) wheel        (0)     3551 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/worker-android.dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     3138 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/worker-ub20.dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     3138 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/worker-ub22.dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)      203 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/worker20.json
+-rw-r--r--   0 michael    (501) wheel        (0)      203 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/cicd/worker22.json
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.983370 ork.build.tools-0.0.4/modules/docker/ps1dev/
+-rw-r--r--   0 michael    (501) wheel        (0)     1019 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/ps1dev/Dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     2268 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/ps1dev/Makefile.cfg
+-rwxr-xr-x   0 michael    (501) wheel        (0)      223 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/ps1dev/fetch.sh
+-rw-r--r--   0 michael    (501) wheel        (0)     2750 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/ps1dev/ps1dev.py
+-rw-r--r--   0 michael    (501) wheel        (0)       71 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/ps1dev/readme.md
+-rwxr-xr-x   0 michael    (501) wheel        (0)      756 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/ps1dev/setup.sh
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.983837 ork.build.tools-0.0.4/modules/docker/ps1dev/testprograms/
+-rw-r--r--   0 michael    (501) wheel        (0)      890 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/ps1dev/testprograms/project.mk
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.984829 ork.build.tools-0.0.4/modules/docker/ps1dev/testprograms/test1/
+-rw-r--r--   0 michael    (501) wheel        (0)       86 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/ps1dev/testprograms/test1/Makefile
+-rw-r--r--   0 michael    (501) wheel        (0)     7821 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/ps1dev/testprograms/test1/test1.c
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.985768 ork.build.tools-0.0.4/modules/docker/realsense2/
+-rw-r--r--   0 michael    (501) wheel        (0)     2325 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/docker/realsense2/Dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     3446 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/modules/docker/realsense2/realsense2.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.987734 ork.build.tools-0.0.4/modules/docker/sagemath/
+-rw-r--r--   0 michael    (501) wheel        (0)     2646 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/sagemath/Dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)      347 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/sagemath/docker-compose.yml
+-rwxr-xr-x   0 michael    (501) wheel        (0)      100 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/sagemath/entrypoint.sh
+-rw-r--r--   0 michael    (501) wheel        (0)     2757 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/sagemath/sagemath.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.990115 ork.build.tools-0.0.4/modules/docker/tflow2gpu/
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2775 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/tflow2gpu/Dockerfile
+-rwxr-xr-x   0 michael    (501) wheel        (0)      519 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/tflow2gpu/test_mediapipe.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2533 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/tflow2gpu/test_multi_gpu.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1715 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/tflow2gpu/test_single_gpu.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     2483 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/tflow2gpu/tflow2gpu.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.991050 ork.build.tools-0.0.4/modules/docker/ub-focal/
+-rw-r--r--   0 michael    (501) wheel        (0)      517 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/ub-focal/Dockerfile
+-rw-r--r--   0 michael    (501) wheel        (0)     1702 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/docker/ub-focal/ub-focal.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.992938 ork.build.tools-0.0.4/modules/host/
+-rw-r--r--   0 michael    (501) wheel        (0)     1181 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/host/aarch64-linux.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1629 2023-03-06 06:24:34.000000 ork.build.tools-0.0.4/modules/host/aarch64-macos.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1409 2023-05-09 20:23:50.000000 ork.build.tools-0.0.4/modules/host/x86_64-linux.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2165 2023-04-05 23:31:27.000000 ork.build.tools-0.0.4/modules/host/x86_64-macos.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.995816 ork.build.tools-0.0.4/modules/sdk/
+-rw-r--r--   0 michael    (501) wheel        (0)     4088 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/sdk/aarch64-android.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1678 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/sdk/aarch64-ios.py
+-rw-r--r--   0 michael    (501) wheel        (0)      782 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/sdk/aarch64-macos.py
+-rw-r--r--   0 michael    (501) wheel        (0)      222 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/sdk/cuda.py
+-rw-r--r--   0 michael    (501) wheel        (0)      618 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/sdk/x86_64-linux.py
+-rw-r--r--   0 michael    (501) wheel        (0)      625 2023-04-05 23:26:33.000000 ork.build.tools-0.0.4/modules/sdk/x86_64-macos.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.997667 ork.build.tools-0.0.4/modules/subspace/
+-rw-r--r--   0 michael    (501) wheel        (0)     7785 2023-06-24 23:47:10.000000 ork.build.tools-0.0.4/modules/subspace/conda.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1227 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/subspace/host.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.998129 ork.build.tools-0.0.4/modules/subspace/nnsvs/
+-rwxr-xr-x   0 michael    (501) wheel        (0)     3419 2023-05-09 20:23:50.000000 ork.build.tools-0.0.4/modules/subspace/nnsvs/test.py
+-rw-r--r--   0 michael    (501) wheel        (0)     4513 2023-06-24 23:47:10.000000 ork.build.tools-0.0.4/modules/subspace/nnsvs.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1187 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/subspace/yo.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:49.001035 ork.build.tools-0.0.4/modules/target/
+-rw-r--r--   0 michael    (501) wheel        (0)      558 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/target/aarch64-android.py
+-rw-r--r--   0 michael    (501) wheel        (0)      551 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/target/aarch64-ios.py
+-rw-r--r--   0 michael    (501) wheel        (0)      554 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/target/aarch64-linux.py
+-rw-r--r--   0 michael    (501) wheel        (0)      554 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/target/aarch64-macos.py
+-rw-r--r--   0 michael    (501) wheel        (0)      556 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/target/x86_64-linux.py
+-rw-r--r--   0 michael    (501) wheel        (0)      556 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/modules/target/x86_64-macos.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:48.841276 ork.build.tools-0.0.4/scripts/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:49.026538 ork.build.tools-0.0.4/scripts/ork/
+-rw-r--r--   0 michael    (501) wheel        (0)       67 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/scripts/ork/__init__.py
+-rw-r--r--   0 michael    (501) wheel        (0)    12346 2023-04-25 17:02:18.000000 ork.build.tools-0.0.4/scripts/ork/_dep_build.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1460 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/_dep_dl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1619 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/_dep_enumerate.py
+-rw-r--r--   0 michael    (501) wheel        (0)     8444 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/scripts/ork/_dep_fetch.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2872 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/scripts/ork/_dep_impl.py
+-rw-r--r--   0 michael    (501) wheel        (0)     4822 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/scripts/ork/_dep_node.py
+-rw-r--r--   0 michael    (501) wheel        (0)    13516 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/scripts/ork/_dep_provider.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3450 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/_dep_x.py
+-rw-r--r--   0 michael    (501) wheel        (0)    12708 2023-06-24 23:47:10.000000 ork.build.tools-0.0.4/scripts/ork/_envutils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1925 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/_globals.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      375 2023-06-24 23:47:39.000000 ork.build.tools-0.0.4/scripts/ork/_obt_dep_completions.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      418 2023-06-24 23:47:39.000000 ork.build.tools-0.0.4/scripts/ork/_obt_dep_completions_shell.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      322 2023-06-24 23:47:10.000000 ork.build.tools-0.0.4/scripts/ork/_obt_subspace_completions.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:49.031996 ork.build.tools-0.0.4/scripts/ork/build/
+-rw-r--r--   0 michael    (501) wheel        (0)       23 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/build/__init__.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1365 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/build/manifest.py
+-rw-r--r--   0 michael    (501) wheel        (0)     5607 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/buildtrace.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2959 2023-04-26 23:56:07.000000 ork.build.tools-0.0.4/scripts/ork/cmake.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:49.033059 ork.build.tools-0.0.4/scripts/ork/cnc/
+-rw-r--r--   0 michael    (501) wheel        (0)        2 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/scripts/ork/cnc/__init__.py
+-rw-r--r--   0 michael    (501) wheel        (0)     7782 2023-02-05 19:12:10.000000 ork.build.tools-0.0.4/scripts/ork/cnc/saf.py
+-rw-r--r--   0 michael    (501) wheel        (0)     8668 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/command.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1486 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/common.py
+-rw-r--r--   0 michael    (501) wheel        (0)      803 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/config.py
+-rw-r--r--   0 michael    (501) wheel        (0)     8068 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/deco.py
+-rw-r--r--   0 michael    (501) wheel        (0)      849 2023-06-24 23:47:10.000000 ork.build.tools-0.0.4/scripts/ork/dep.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2756 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/docker.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1266 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/env.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1806 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/executors.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1241 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/gen_pkgconfig.py
+-rw-r--r--   0 michael    (501) wheel        (0)     5172 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/git.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2868 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/host.py
+-rw-r--r--   0 michael    (501) wheel        (0)      268 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/libav.py
+-rw-r--r--   0 michael    (501) wheel        (0)      927 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/litex.py
+-rw-r--r--   0 michael    (501) wheel        (0)      285 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/log.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2849 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/macos.py
+-rw-r--r--   0 michael    (501) wheel        (0)      141 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/macos_homebrew.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1080 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/make.py
+-rw-r--r--   0 michael    (501) wheel        (0)       75 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/math.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2040 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/module.py
+-rw-r--r--   0 michael    (501) wheel        (0)      145 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/net.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1194 2023-05-12 22:40:05.000000 ork.build.tools-0.0.4/scripts/ork/osrelease.py
+-rw-r--r--   0 michael    (501) wheel        (0)      983 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/patch.py
+-rw-r--r--   0 michael    (501) wheel        (0)     8359 2023-06-24 23:47:10.000000 ork.build.tools-0.0.4/scripts/ork/path.py
+-rw-r--r--   0 michael    (501) wheel        (0)     8544 2023-04-25 17:02:18.000000 ork.build.tools-0.0.4/scripts/ork/pathtools.py
+-rw-r--r--   0 michael    (501) wheel        (0)      668 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/pip.py
+-rw-r--r--   0 michael    (501) wheel        (0)       75 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/pybind11.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1341 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/scp.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1747 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/sdk.py
+-rw-r--r--   0 michael    (501) wheel        (0)     4538 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/search.py
+-rw-r--r--   0 michael    (501) wheel        (0)     3241 2023-04-25 17:02:18.000000 ork.build.tools-0.0.4/scripts/ork/subspace.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1334 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/target.py
+-rw-r--r--   0 michael    (501) wheel        (0)     1559 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/template.py
+-rw-r--r--   0 michael    (501) wheel        (0)     6511 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/utils.py
+-rw-r--r--   0 michael    (501) wheel        (0)     2080 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/wget.py
+-rw-r--r--   0 michael    (501) wheel        (0)      591 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/scripts/ork/xcode.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:49.030706 ork.build.tools-0.0.4/scripts/ork.build.tools.egg-info/
+-rw-r--r--   0 michael    (501) wheel        (0)    14849 2023-07-14 18:55:48.000000 ork.build.tools-0.0.4/scripts/ork.build.tools.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) wheel        (0)    10954 2023-07-14 18:55:48.000000 ork.build.tools-0.0.4/scripts/ork.build.tools.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) wheel        (0)        1 2023-07-14 18:55:48.000000 ork.build.tools-0.0.4/scripts/ork.build.tools.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) wheel        (0)        1 2023-07-14 18:55:48.000000 ork.build.tools-0.0.4/scripts/ork.build.tools.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) wheel        (0)       38 2023-07-14 18:55:49.040316 ork.build.tools-0.0.4/setup.cfg
+-rw-r--r--   0 michael    (501) wheel        (0)     1255 2023-07-14 18:55:44.000000 ork.build.tools-0.0.4/setup.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:49.034030 ork.build.tools-0.0.4/tests/
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:49.035931 ork.build.tools-0.0.4/tests/docker-gpu/
+-rw-r--r--   0 michael    (501) wheel        (0)      411 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/tests/docker-gpu/Dockerfile
+-rwxr-xr-x   0 michael    (501) wheel        (0)       53 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/tests/docker-gpu/build.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)      358 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/tests/docker-gpu/launch_glmark.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)      369 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/tests/docker-gpu/launch_nvtopo.sh
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:49.037871 ork.build.tools-0.0.4/tests/docker-gpu-tensorflow/
+-rw-r--r--   0 michael    (501) wheel        (0)      505 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/tests/docker-gpu-tensorflow/Dockerfile
+-rwxr-xr-x   0 michael    (501) wheel        (0)       55 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/tests/docker-gpu-tensorflow/build.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)      379 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/tests/docker-gpu-tensorflow/launch_nvtopo.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)      391 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/tests/docker-gpu-tensorflow/launch_tf.sh
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1543 2023-07-14 17:52:14.000000 ork.build.tools-0.0.4/tests/litex1_nx4.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)      178 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/tests/osx_rpaths.py
+drwxr-xr-x   0 michael    (501) wheel        (0)        0 2023-07-14 18:55:49.038850 ork.build.tools-0.0.4/tests/pytorch/
+-rwxr-xr-x   0 michael    (501) wheel        (0)      916 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/tests/pytorch/install.py
+-rwxr-xr-x   0 michael    (501) wheel        (0)     1190 2022-09-08 21:51:24.000000 ork.build.tools-0.0.4/tests/pytorch/training.py
```

### Comparing `ork.build.tools-0.0.3/PKG-INFO` & `ork.build.tools-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ork.build.tools
-Version: 0.0.3
+Version: 0.0.4
 Description-Content-Type: text/markdown
 
 # ORK.BUILD TOOLS (OBT)  
 
 ## [BuildStatus](https://www.orkid-engine.dev:4431)
 
 * Ubuntu 22.04 [![CISTATUS](https://www.orkid-engine.dev:4431/orkdotbuild-ix-ub2204/develop/status.svg)](https://www.orkid-engine.dev:4431)
```

### Comparing `ork.build.tools-0.0.3/README.md` & `ork.build.tools-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/bin_pub/obt.create.env.py` & `ork.build.tools-0.0.4/bin_pub/obt.create.env.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/bin_pub/obt.init.env.py` & `ork.build.tools-0.0.4/bin_pub/obt.init.env.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/bin_pub/obt.ix.installdeps.linuxcnc.py` & `ork.build.tools-0.0.4/bin_pub/obt.ix.installdeps.linuxcnc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/bin_pub/obt.ix.installdeps.ubuntu_aarch64.py` & `ork.build.tools-0.0.4/bin_pub/obt.ix.installdeps.ubuntu_aarch64.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/bin_pub/obt.ix.installdeps.ubuntu_x86_64.py` & `ork.build.tools-0.0.4/bin_pub/obt.ix.installdeps.ubuntu_x86_64.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/bin_pub/obt.osx.installdeps.py` & `ork.build.tools-0.0.4/bin_pub/obt.osx.installdeps.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/examples/dep-overrides/orkid.py` & `ork.build.tools-0.0.4/examples/dep-overrides/orkid.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/examples/litex1/arty.py` & `ork.build.tools-0.0.4/examples/litex1/arty.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/examples/litex1/cmod_a7_platform.py` & `ork.build.tools-0.0.4/examples/litex1/cmod_a7_platform.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/examples/litex1/cmod_a7_target.py` & `ork.build.tools-0.0.4/examples/litex1/cmod_a7_target.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/examples/litex1/nexys_video.py` & `ork.build.tools-0.0.4/examples/litex1/nexys_video.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/examples/litex1/nexysv.cfg` & `ork.build.tools-0.0.4/examples/litex1/nexysv.cfg`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/examples/litex1/soc_nexysv.py` & `ork.build.tools-0.0.4/examples/litex1/soc_nexysv.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/examples/litex_zephyrtest/LICENSE` & `ork.build.tools-0.0.4/examples/litex_zephyrtest/LICENSE`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/examples/litex_zephyrtest/README.rst` & `ork.build.tools-0.0.4/examples/litex_zephyrtest/README.rst`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/examples/litex_zephyrtest/sample.yaml` & `ork.build.tools-0.0.4/examples/litex_zephyrtest/sample.yaml`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/examples/litex_zephyrtest/src/main.c` & `ork.build.tools-0.0.4/examples/litex_zephyrtest/src/main.c`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/_binutils.py` & `ork.build.tools-0.0.4/modules/dep/_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/_gcc.py` & `ork.build.tools-0.0.4/modules/dep/_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/_nnsvs.py` & `ork.build.tools-0.0.4/modules/dep/_nnsvs.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/apitrace.py` & `ork.build.tools-0.0.4/modules/dep/apitrace.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/arachnepnr.py` & `ork.build.tools-0.0.4/modules/dep/arachnepnr.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/arm64_binutils.py` & `ork.build.tools-0.0.4/modules/dep/arm64_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/arm64_gcc.py` & `ork.build.tools-0.0.4/modules/dep/arm64_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/assimp.py` & `ork.build.tools-0.0.4/modules/dep/assimp.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/astcencoder.py` & `ork.build.tools-0.0.4/modules/dep/astcencoder.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/audiofile.py` & `ork.build.tools-0.0.4/modules/dep/audiofile.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/avr_binutils.py` & `ork.build.tools-0.0.4/modules/dep/avr_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/avr_gcc.py` & `ork.build.tools-0.0.4/modules/dep/avr_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/avr_libc.py` & `ork.build.tools-0.0.4/modules/dep/avr_libc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/bazel.py` & `ork.build.tools-0.0.4/modules/dep/bazel.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/blosc.py` & `ork.build.tools-0.0.4/modules/dep/blosc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/boost.py` & `ork.build.tools-0.0.4/modules/dep/boost.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/bullet.py` & `ork.build.tools-0.0.4/modules/dep/bullet.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/calf.py` & `ork.build.tools-0.0.4/modules/dep/calf.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/cgal.py` & `ork.build.tools-0.0.4/modules/dep/cgal.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/clang.py` & `ork.build.tools-0.0.4/modules/dep/clang.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/cmake.py` & `ork.build.tools-0.0.4/modules/dep/cmake.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/cpppeglib.py` & `ork.build.tools-0.0.4/modules/dep/cpppeglib.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/cppzmq.py` & `ork.build.tools-0.0.4/modules/dep/cppzmq.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/csvparser.py` & `ork.build.tools-0.0.4/modules/dep/csvparser.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/cuda.py` & `ork.build.tools-0.0.4/modules/dep/cuda.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/curlpp.py` & `ork.build.tools-0.0.4/modules/dep/curlpp.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/cycles.py` & `ork.build.tools-0.0.4/modules/dep/cycles.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/depthaicore.py` & `ork.build.tools-0.0.4/modules/dep/depthaicore.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/drawtext.py` & `ork.build.tools-0.0.4/modules/dep/drawtext.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/easyprof.py` & `ork.build.tools-0.0.4/modules/dep/easyprof.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/eigen.py` & `ork.build.tools-0.0.4/modules/dep/eigen.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/embree.py` & `ork.build.tools-0.0.4/modules/dep/embree.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/faust.py` & `ork.build.tools-0.0.4/modules/dep/faust.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/fcollada.py` & `ork.build.tools-0.0.4/modules/dep/fcollada.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/ffmpeg.py` & `ork.build.tools-0.0.4/modules/dep/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/flatcam.py` & `ork.build.tools-0.0.4/modules/dep/flatcam.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/fltk.py` & `ork.build.tools-0.0.4/modules/dep/fltk.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/fluidsynth.py` & `ork.build.tools-0.0.4/modules/dep/fluidsynth.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/frameretrace.py` & `ork.build.tools-0.0.4/modules/dep/frameretrace.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/gcode_gpr.py` & `ork.build.tools-0.0.4/modules/dep/gcode_gpr.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/giflib.py` & `ork.build.tools-0.0.4/modules/dep/giflib.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/gitpython.py` & `ork.build.tools-0.0.4/modules/dep/gitpython.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/glfw.py` & `ork.build.tools-0.0.4/modules/dep/glfw.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/glm.py` & `ork.build.tools-0.0.4/modules/dep/glm.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/gnutar.py` & `ork.build.tools-0.0.4/modules/dep/gnutar.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/houdini.py` & `ork.build.tools-0.0.4/modules/dep/houdini.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/icestorm.py` & `ork.build.tools-0.0.4/modules/dep/icestorm.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/igl.py` & `ork.build.tools-0.0.4/modules/dep/igl.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/irix65_binutils.py` & `ork.build.tools-0.0.4/modules/dep/irix65_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/irix65_gcc.py` & `ork.build.tools-0.0.4/modules/dep/irix65_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/irrlicht.py` & `ork.build.tools-0.0.4/modules/dep/irrlicht.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/ispc.py` & `ork.build.tools-0.0.4/modules/dep/ispc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/ispctexc.py` & `ork.build.tools-0.0.4/modules/dep/ispctexc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/jpegturbo.py` & `ork.build.tools-0.0.4/modules/dep/jpegturbo.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/klein.py` & `ork.build.tools-0.0.4/modules/dep/klein.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/lapack.py` & `ork.build.tools-0.0.4/modules/dep/lapack.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/lemongraph.py` & `ork.build.tools-0.0.4/modules/dep/lemongraph.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/lexertl14.py` & `ork.build.tools-0.0.4/modules/dep/lexertl14.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/libcurl.py` & `ork.build.tools-0.0.4/modules/dep/libcurl.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/libfive.py` & `ork.build.tools-0.0.4/modules/dep/libfive.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/libpqpp.py` & `ork.build.tools-0.0.4/modules/dep/libpqpp.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/libsocket.py` & `ork.build.tools-0.0.4/modules/dep/libsocket.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/libsurvive.py` & `ork.build.tools-0.0.4/modules/dep/libsurvive.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/libtorch.py` & `ork.build.tools-0.0.4/modules/dep/libtorch.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/linuxcnc.py` & `ork.build.tools-0.0.4/modules/dep/linuxcnc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/litex.py` & `ork.build.tools-0.0.4/modules/dep/litex.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/llvm.py` & `ork.build.tools-0.0.4/modules/dep/llvm.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/lm32_binutils.py` & `ork.build.tools-0.0.4/modules/dep/lm32_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/lm32_gcc.py` & `ork.build.tools-0.0.4/modules/dep/lm32_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/lua.py` & `ork.build.tools-0.0.4/modules/dep/lua.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/luajit.py` & `ork.build.tools-0.0.4/modules/dep/luajit.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/m68k_amiga_binutils.py` & `ork.build.tools-0.0.4/modules/dep/m68k_amiga_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/m68k_amiga_gcc.py` & `ork.build.tools-0.0.4/modules/dep/m68k_amiga_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/minetest.py` & `ork.build.tools-0.0.4/modules/dep/minetest.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/moltenvk.py` & `ork.build.tools-0.0.4/modules/dep/moltenvk.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/nextpnr.py` & `ork.build.tools-0.0.4/modules/dep/nextpnr.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/ngc.py` & `ork.build.tools-0.0.4/modules/dep/ngc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/nlohmannjson.py` & `ork.build.tools-0.0.4/modules/dep/nlohmannjson.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/nss.py` & `ork.build.tools-0.0.4/modules/dep/nss.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/nsync_cpp.py` & `ork.build.tools-0.0.4/modules/dep/nsync_cpp.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/nvtt.py` & `ork.build.tools-0.0.4/modules/dep/nvtt.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/ocio.py` & `ork.build.tools-0.0.4/modules/dep/ocio.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/oiio.py` & `ork.build.tools-0.0.4/modules/dep/oiio.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/oneapimkl.py` & `ork.build.tools-0.0.4/modules/dep/oneapimkl.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/openblas.py` & `ork.build.tools-0.0.4/modules/dep/openblas.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/opencv.py` & `ork.build.tools-0.0.4/modules/dep/opencv.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/opencv_contrib.py` & `ork.build.tools-0.0.4/modules/dep/opencv_contrib.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/opendb.py` & `ork.build.tools-0.0.4/modules/dep/opendb.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/openexr.py` & `ork.build.tools-0.0.4/modules/dep/openexr.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/openjpeg.py` & `ork.build.tools-0.0.4/modules/dep/openjpeg.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/openroad.py` & `ork.build.tools-0.0.4/modules/dep/openroad.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/opensubdiv.py` & `ork.build.tools-0.0.4/modules/dep/opensubdiv.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/openvdb.py` & `ork.build.tools-0.0.4/modules/dep/openvdb.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/openvr.py` & `ork.build.tools-0.0.4/modules/dep/openvr.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/orkid.py` & `ork.build.tools-0.0.4/modules/dep/orkid.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/osgeolaszip.py` & `ork.build.tools-0.0.4/modules/dep/osgeolaszip.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/osgeoliblas.py` & `ork.build.tools-0.0.4/modules/dep/osgeoliblas.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/osgeoproj.py` & `ork.build.tools-0.0.4/modules/dep/osgeoproj.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/osgeotiff.py` & `ork.build.tools-0.0.4/modules/dep/osgeotiff.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/osl.py` & `ork.build.tools-0.0.4/modules/dep/osl.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/ozzanim.py` & `ork.build.tools-0.0.4/modules/dep/ozzanim.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/pangolin.py` & `ork.build.tools-0.0.4/modules/dep/pangolin.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/parsertl14.py` & `ork.build.tools-0.0.4/modules/dep/parsertl14.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/patches/boost/chg/darwin.jam` & `ork.build.tools-0.0.4/modules/dep/patches/boost/chg/darwin.jam`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/patches/boost/chg/project-config.jam` & `ork.build.tools-0.0.4/modules/dep/patches/boost/chg/project-config.jam`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/patches/boost/ori/darwin.jam` & `ork.build.tools-0.0.4/modules/dep/patches/boost/ori/darwin.jam`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/patches/gcc/gcc.sgifixes.patch` & `ork.build.tools-0.0.4/modules/dep/patches/gcc/gcc.sgifixes.patch`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/patches/gcc/gcc.sgifixlibstdcpp01.patch` & `ork.build.tools-0.0.4/modules/dep/patches/gcc/gcc.sgifixlibstdcpp01.patch`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/patches/gcc/newlib.sgifixes.patch` & `ork.build.tools-0.0.4/modules/dep/patches/gcc/newlib.sgifixes.patch`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/patches/giflib/chg/Makefile` & `ork.build.tools-0.0.4/modules/dep/patches/giflib/chg/Makefile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/patches/giflib/ori/Makefile` & `ork.build.tools-0.0.4/modules/dep/patches/giflib/ori/Makefile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/patches/pillar/chg/markdown.py` & `ork.build.tools-0.0.4/modules/dep/patches/pillar/chg/markdown.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/patches/pillar/ori/markdown.py` & `ork.build.tools-0.0.4/modules/dep/patches/pillar/ori/markdown.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/pillar.py` & `ork.build.tools-0.0.4/modules/dep/pillar.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/pkgconfig.py` & `ork.build.tools-0.0.4/modules/dep/pkgconfig.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/portaudio.py` & `ork.build.tools-0.0.4/modules/dep/portaudio.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/postgresql.py` & `ork.build.tools-0.0.4/modules/dep/postgresql.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/premake.py` & `ork.build.tools-0.0.4/modules/dep/premake.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/ptex.py` & `ork.build.tools-0.0.4/modules/dep/ptex.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/pugixml.py` & `ork.build.tools-0.0.4/modules/dep/pugixml.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/pybind11.py` & `ork.build.tools-0.0.4/modules/dep/pybind11.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/pydefaults.py` & `ork.build.tools-0.0.4/modules/dep/pydefaults.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/pyopengl.py` & `ork.build.tools-0.0.4/modules/dep/pyopengl.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/pyqt5.py` & `ork.build.tools-0.0.4/modules/dep/pyqt5.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/pyside2.py` & `ork.build.tools-0.0.4/modules/dep/pyside2.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/python.py` & `ork.build.tools-0.0.4/modules/dep/python.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/qt5.py` & `ork.build.tools-0.0.4/modules/dep/qt5.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/qt5ct.py` & `ork.build.tools-0.0.4/modules/dep/qt5ct.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/qt5forpython.py` & `ork.build.tools-0.0.4/modules/dep/qt5forpython.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/rapidjson.py` & `ork.build.tools-0.0.4/modules/dep/rapidjson.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/realsense2.py` & `ork.build.tools-0.0.4/modules/dep/realsense2.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/root.py` & `ork.build.tools-0.0.4/modules/dep/root.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/rtmidi.py` & `ork.build.tools-0.0.4/modules/dep/rtmidi.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/rv32_binutils.py` & `ork.build.tools-0.0.4/modules/dep/rv32_binutils.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/rv32_gcc.py` & `ork.build.tools-0.0.4/modules/dep/rv32_gcc.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/sigslot.py` & `ork.build.tools-0.0.4/modules/dep/sigslot.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/simavr.py` & `ork.build.tools-0.0.4/modules/dep/simavr.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/sse2neon.py` & `ork.build.tools-0.0.4/modules/dep/sse2neon.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/tbb.py` & `ork.build.tools-0.0.4/modules/dep/tbb.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/tflite.py` & `ork.build.tools-0.0.4/modules/dep/tflite.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/ue5.py` & `ork.build.tools-0.0.4/modules/dep/ue5.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/ue5_cesium.py` & `ork.build.tools-0.0.4/modules/dep/ue5_cesium.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/unittestpp.py` & `ork.build.tools-0.0.4/modules/dep/unittestpp.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/usd.py` & `ork.build.tools-0.0.4/modules/dep/usd.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/vhacd.py` & `ork.build.tools-0.0.4/modules/dep/vhacd.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/vivado.py` & `ork.build.tools-0.0.4/modules/dep/vivado.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/vpf.py` & `ork.build.tools-0.0.4/modules/dep/vpf.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/vrx.py` & `ork.build.tools-0.0.4/modules/dep/vrx.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/vst3sdk.py` & `ork.build.tools-0.0.4/modules/dep/vst3sdk.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/vulkan.py` & `ork.build.tools-0.0.4/modules/dep/vulkan.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/wt4.py` & `ork.build.tools-0.0.4/modules/dep/wt4.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/xatlas.py` & `ork.build.tools-0.0.4/modules/dep/xatlas.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/yarl.py` & `ork.build.tools-0.0.4/modules/dep/yarl.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/yosys.py` & `ork.build.tools-0.0.4/modules/dep/yosys.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/zephyr.py` & `ork.build.tools-0.0.4/modules/dep/zephyr.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/dep/zmq.py` & `ork.build.tools-0.0.4/modules/dep/zmq.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/amigadev/Dockerfile` & `ork.build.tools-0.0.4/modules/docker/amigadev/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/amigadev/amigadev.py` & `ork.build.tools-0.0.4/modules/docker/amigadev/amigadev.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/amigadev/test1/build.py` & `ork.build.tools-0.0.4/modules/docker/amigadev/test1/build.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/amigadev/test1/libs/mathieeedoubbas.library` & `ork.build.tools-0.0.4/modules/docker/amigadev/test1/libs/mathieeedoubbas.library`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/amigadev/test1/libs/mathieeedoubtrans.library` & `ork.build.tools-0.0.4/modules/docker/amigadev/test1/libs/mathieeedoubtrans.library`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/amigadev/test1/main.cpp` & `ork.build.tools-0.0.4/modules/docker/amigadev/test1/main.cpp`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/amigadev/test1/test_fsuae.py` & `ork.build.tools-0.0.4/modules/docker/amigadev/test1/test_fsuae.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/androiddev/Dockerfile` & `ork.build.tools-0.0.4/modules/docker/androiddev/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/androiddev/androiddev.py` & `ork.build.tools-0.0.4/modules/docker/androiddev/androiddev.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/bin/ci_common.py` & `ork.build.tools-0.0.4/modules/docker/cicd/bin/ci_common.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/bin/test_worker_android.py` & `ork.build.tools-0.0.4/modules/docker/cicd/bin/test_worker_android.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/bin/test_worker_ub20.py` & `ork.build.tools-0.0.4/modules/docker/cicd/bin/test_worker_ub20.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/bin/test_worker_ub22.py` & `ork.build.tools-0.0.4/modules/docker/cicd/bin/test_worker_ub22.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/_masterimpl.py` & `ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/_masterimpl.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/_watcher.py` & `ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/_watcher.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/_workerimpl.py` & `ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/_workerimpl.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/_zmqssh.py` & `ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/_zmqssh.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/assets/OrkidLogo.png` & `ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/assets/OrkidLogo.png`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/assets/index.template` & `ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/assets/index.template`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/assets/variant.template` & `ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/assets/variant.template`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/badge.py` & `ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/badge.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/httphandler.py` & `ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/httphandler.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/master.py` & `ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/master.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/orkbb.py` & `ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/orkbb.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/process_log.py` & `ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/process_log.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/scheduler.py` & `ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/scheduler.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/worker.py` & `ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/worker.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/worker_build_branch.py` & `ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/worker_build_branch.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/ci_impl/worker_fetch_branch.py` & `ork.build.tools-0.0.4/modules/docker/cicd/ci_impl/worker_fetch_branch.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/cicd.py` & `ork.build.tools-0.0.4/modules/docker/cicd/cicd.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/conf/nginx_ssl.conf` & `ork.build.tools-0.0.4/modules/docker/cicd/conf/nginx_ssl.conf`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu19.py` & `ork.build.tools-0.0.4/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu19.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu22.py` & `ork.build.tools-0.0.4/modules/docker/cicd/container-scripts/obt.ix.installdeps.ubuntu22.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/docker-compose-nossl.yml` & `ork.build.tools-0.0.4/modules/docker/cicd/docker-compose-nossl.yml`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/docker-compose.yml` & `ork.build.tools-0.0.4/modules/docker/cicd/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/master.dockerfile` & `ork.build.tools-0.0.4/modules/docker/cicd/master.dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/master.json` & `ork.build.tools-0.0.4/modules/docker/cicd/master.json`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/worker-android.dockerfile` & `ork.build.tools-0.0.4/modules/docker/cicd/worker-android.dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/worker-ub20.dockerfile` & `ork.build.tools-0.0.4/modules/docker/cicd/worker-ub20.dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/cicd/worker-ub22.dockerfile` & `ork.build.tools-0.0.4/modules/docker/cicd/worker-ub22.dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/ps1dev/Dockerfile` & `ork.build.tools-0.0.4/modules/docker/ps1dev/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/ps1dev/Makefile.cfg` & `ork.build.tools-0.0.4/modules/docker/ps1dev/Makefile.cfg`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/ps1dev/ps1dev.py` & `ork.build.tools-0.0.4/modules/docker/ps1dev/ps1dev.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/ps1dev/setup.sh` & `ork.build.tools-0.0.4/modules/docker/ps1dev/setup.sh`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/ps1dev/testprograms/project.mk` & `ork.build.tools-0.0.4/modules/docker/ps1dev/testprograms/project.mk`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/ps1dev/testprograms/test1/test1.c` & `ork.build.tools-0.0.4/modules/docker/ps1dev/testprograms/test1/test1.c`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/realsense2/Dockerfile` & `ork.build.tools-0.0.4/modules/docker/realsense2/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/realsense2/realsense2.py` & `ork.build.tools-0.0.4/modules/docker/realsense2/realsense2.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/sagemath/Dockerfile` & `ork.build.tools-0.0.4/modules/docker/sagemath/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/sagemath/sagemath.py` & `ork.build.tools-0.0.4/modules/docker/sagemath/sagemath.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/tflow2gpu/Dockerfile` & `ork.build.tools-0.0.4/modules/docker/tflow2gpu/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/tflow2gpu/test_mediapipe.sh` & `ork.build.tools-0.0.4/modules/docker/tflow2gpu/test_mediapipe.sh`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/tflow2gpu/test_multi_gpu.py` & `ork.build.tools-0.0.4/modules/docker/tflow2gpu/test_multi_gpu.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/tflow2gpu/test_single_gpu.py` & `ork.build.tools-0.0.4/modules/docker/tflow2gpu/test_single_gpu.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/tflow2gpu/tflow2gpu.py` & `ork.build.tools-0.0.4/modules/docker/tflow2gpu/tflow2gpu.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/ub-focal/Dockerfile` & `ork.build.tools-0.0.4/modules/docker/ub-focal/Dockerfile`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/docker/ub-focal/ub-focal.py` & `ork.build.tools-0.0.4/modules/docker/ub-focal/ub-focal.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/host/aarch64-linux.py` & `ork.build.tools-0.0.4/modules/host/aarch64-linux.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/host/aarch64-macos.py` & `ork.build.tools-0.0.4/modules/host/aarch64-macos.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/host/x86_64-linux.py` & `ork.build.tools-0.0.4/modules/host/x86_64-linux.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/host/x86_64-macos.py` & `ork.build.tools-0.0.4/modules/host/x86_64-macos.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/sdk/aarch64-android.py` & `ork.build.tools-0.0.4/modules/sdk/aarch64-android.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/sdk/aarch64-ios.py` & `ork.build.tools-0.0.4/modules/sdk/aarch64-ios.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/sdk/aarch64-macos.py` & `ork.build.tools-0.0.4/modules/sdk/aarch64-macos.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/sdk/x86_64-linux.py` & `ork.build.tools-0.0.4/modules/sdk/x86_64-linux.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/sdk/x86_64-macos.py` & `ork.build.tools-0.0.4/modules/sdk/x86_64-macos.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/subspace/conda.py` & `ork.build.tools-0.0.4/modules/subspace/conda.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/subspace/host.py` & `ork.build.tools-0.0.4/modules/subspace/host.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/subspace/nnsvs/test.py` & `ork.build.tools-0.0.4/modules/subspace/nnsvs/test.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/subspace/nnsvs.py` & `ork.build.tools-0.0.4/modules/subspace/nnsvs.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/subspace/yo.py` & `ork.build.tools-0.0.4/modules/subspace/yo.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/target/aarch64-android.py` & `ork.build.tools-0.0.4/modules/target/aarch64-android.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/target/aarch64-ios.py` & `ork.build.tools-0.0.4/modules/target/aarch64-ios.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/target/aarch64-linux.py` & `ork.build.tools-0.0.4/modules/target/aarch64-linux.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/target/aarch64-macos.py` & `ork.build.tools-0.0.4/modules/target/aarch64-macos.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/target/x86_64-linux.py` & `ork.build.tools-0.0.4/modules/target/x86_64-linux.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/modules/target/x86_64-macos.py` & `ork.build.tools-0.0.4/modules/target/x86_64-macos.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/_dep_build.py` & `ork.build.tools-0.0.4/scripts/ork/_dep_build.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/_dep_dl.py` & `ork.build.tools-0.0.4/scripts/ork/_dep_dl.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/_dep_enumerate.py` & `ork.build.tools-0.0.4/scripts/ork/_dep_enumerate.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/_dep_fetch.py` & `ork.build.tools-0.0.4/scripts/ork/_dep_fetch.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/_dep_impl.py` & `ork.build.tools-0.0.4/scripts/ork/_dep_impl.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/_dep_node.py` & `ork.build.tools-0.0.4/scripts/ork/_dep_node.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/_dep_provider.py` & `ork.build.tools-0.0.4/scripts/ork/_dep_provider.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/_dep_x.py` & `ork.build.tools-0.0.4/scripts/ork/_dep_x.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/_envutils.py` & `ork.build.tools-0.0.4/scripts/ork/_envutils.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/_globals.py` & `ork.build.tools-0.0.4/scripts/ork/_globals.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/build/manifest.py` & `ork.build.tools-0.0.4/scripts/ork/build/manifest.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/buildtrace.py` & `ork.build.tools-0.0.4/scripts/ork/buildtrace.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/cmake.py` & `ork.build.tools-0.0.4/scripts/ork/cmake.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/cnc/saf.py` & `ork.build.tools-0.0.4/scripts/ork/cnc/saf.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/command.py` & `ork.build.tools-0.0.4/scripts/ork/command.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/common.py` & `ork.build.tools-0.0.4/scripts/ork/common.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/config.py` & `ork.build.tools-0.0.4/scripts/ork/config.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/deco.py` & `ork.build.tools-0.0.4/scripts/ork/deco.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/dep.py` & `ork.build.tools-0.0.4/scripts/ork/dep.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/docker.py` & `ork.build.tools-0.0.4/scripts/ork/docker.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/env.py` & `ork.build.tools-0.0.4/scripts/ork/env.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/executors.py` & `ork.build.tools-0.0.4/scripts/ork/executors.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/gen_pkgconfig.py` & `ork.build.tools-0.0.4/scripts/ork/gen_pkgconfig.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/git.py` & `ork.build.tools-0.0.4/scripts/ork/git.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/host.py` & `ork.build.tools-0.0.4/scripts/ork/host.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/litex.py` & `ork.build.tools-0.0.4/scripts/ork/litex.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/macos.py` & `ork.build.tools-0.0.4/scripts/ork/macos.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/make.py` & `ork.build.tools-0.0.4/scripts/ork/make.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/module.py` & `ork.build.tools-0.0.4/scripts/ork/module.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/osrelease.py` & `ork.build.tools-0.0.4/scripts/ork/osrelease.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/patch.py` & `ork.build.tools-0.0.4/scripts/ork/patch.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/path.py` & `ork.build.tools-0.0.4/scripts/ork/path.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/pathtools.py` & `ork.build.tools-0.0.4/scripts/ork/pathtools.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/pip.py` & `ork.build.tools-0.0.4/scripts/ork/pip.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/scp.py` & `ork.build.tools-0.0.4/scripts/ork/scp.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/sdk.py` & `ork.build.tools-0.0.4/scripts/ork/sdk.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/search.py` & `ork.build.tools-0.0.4/scripts/ork/search.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/subspace.py` & `ork.build.tools-0.0.4/scripts/ork/subspace.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/target.py` & `ork.build.tools-0.0.4/scripts/ork/target.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/template.py` & `ork.build.tools-0.0.4/scripts/ork/template.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/utils.py` & `ork.build.tools-0.0.4/scripts/ork/utils.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/wget.py` & `ork.build.tools-0.0.4/scripts/ork/wget.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork/xcode.py` & `ork.build.tools-0.0.4/scripts/ork/xcode.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/scripts/ork.build.tools.egg-info/PKG-INFO` & `ork.build.tools-0.0.4/scripts/ork.build.tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ork.build.tools
-Version: 0.0.3
+Version: 0.0.4
 Description-Content-Type: text/markdown
 
 # ORK.BUILD TOOLS (OBT)  
 
 ## [BuildStatus](https://www.orkid-engine.dev:4431)
 
 * Ubuntu 22.04 [![CISTATUS](https://www.orkid-engine.dev:4431/orkdotbuild-ix-ub2204/develop/status.svg)](https://www.orkid-engine.dev:4431)
```

### Comparing `ork.build.tools-0.0.3/scripts/ork.build.tools.egg-info/SOURCES.txt` & `ork.build.tools-0.0.4/scripts/ork.build.tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/setup.py` & `ork.build.tools-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 for pkg in extra_packages:
     package_dir[pkg] = pkg
     package_data["ork.build.tools."+pkg] = package_files(pkg)
 
 setup(
     name="ork.build.tools",
-    version="0.0.3",
+    version="0.0.4",
     packages=find_packages(where=["scripts"]+extra_packages),
     package_dir=package_dir,
     package_data=package_data,
     scripts=glob.glob('bin_pub/*'),
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

### Comparing `ork.build.tools-0.0.3/tests/litex1_nx4.py` & `ork.build.tools-0.0.4/tests/litex1_nx4.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/tests/pytorch/install.py` & `ork.build.tools-0.0.4/tests/pytorch/install.py`

 * *Files identical despite different names*

### Comparing `ork.build.tools-0.0.3/tests/pytorch/training.py` & `ork.build.tools-0.0.4/tests/pytorch/training.py`

 * *Files identical despite different names*

