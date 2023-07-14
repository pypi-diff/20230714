# Comparing `tmp/py-imgui-redux-1.0.3.tar.gz` & `tmp/py-imgui-redux-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-imgui-redux-1.0.3.tar", last modified: Fri Jul 14 17:51:32 2023, max compression
+gzip compressed data, was "py-imgui-redux-1.0.4.tar", last modified: Fri Jul 14 18:08:56 2023, max compression
```

## Comparing `py-imgui-redux-1.0.3.tar` & `py-imgui-redux-1.0.4.tar`

### file list

```diff
@@ -1,769 +1,769 @@
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.753288 py-imgui-redux-1.0.3/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      374 2023-05-10 21:03:59.000000 py-imgui-redux-1.0.3/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1070 2023-03-09 01:15:58.000000 py-imgui-redux-1.0.3/LICENSE
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       91 2023-07-14 17:50:56.000000 py-imgui-redux-1.0.3/MANIFEST.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5363 2023-07-14 17:51:32.753288 py-imgui-redux-1.0.3/PKG-INFO
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4637 2023-03-18 18:20:05.000000 py-imgui-redux-1.0.3/README.md
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.703287 py-imgui-redux-1.0.3/imgui/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    79389 2023-04-08 20:08:02.000000 py-imgui-redux-1.0.3/imgui/__init__.pyi
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.703287 py-imgui-redux-1.0.3/imgui/glfw/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      592 2023-04-08 20:08:02.000000 py-imgui-redux-1.0.3/imgui/glfw/__init__.pyi
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.703287 py-imgui-redux-1.0.3/imgui/imnodes/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12577 2023-04-08 20:08:02.000000 py-imgui-redux-1.0.3/imgui/imnodes/__init__.pyi
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.703287 py-imgui-redux-1.0.3/imgui/implot/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    29707 2023-04-08 20:08:02.000000 py-imgui-redux-1.0.3/imgui/implot/__init__.pyi
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.703287 py-imgui-redux-1.0.3/py_imgui_redux.egg-info/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5363 2023-07-14 17:51:32.000000 py-imgui-redux-1.0.3/py_imgui_redux.egg-info/PKG-INFO
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    30237 2023-07-14 17:51:32.000000 py-imgui-redux-1.0.3/py_imgui_redux.egg-info/SOURCES.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)        1 2023-07-14 17:51:32.000000 py-imgui-redux-1.0.3/py_imgui_redux.egg-info/dependency_links.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)        6 2023-07-14 17:51:32.000000 py-imgui-redux-1.0.3/py_imgui_redux.egg-info/top_level.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12918 2023-05-10 21:21:35.000000 py-imgui-redux-1.0.3/pyproject.toml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       38 2023-07-14 17:51:32.753288 py-imgui-redux-1.0.3/setup.cfg
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10250 2023-05-10 22:34:33.000000 py-imgui-redux-1.0.3/setup.py
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.703287 py-imgui-redux-1.0.3/third-party/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1369 2023-03-09 02:26:26.000000 py-imgui-redux-1.0.3/third-party/CMakeLists.txt
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.703287 py-imgui-redux-1.0.3/third-party/glfw/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1206 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/.appveyor.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       44 2023-03-09 01:16:45.000000 py-imgui-redux-1.0.3/third-party/glfw/.git
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      142 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/.gitattributes
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.703287 py-imgui-redux-1.0.3/third-party/glfw/.github/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      175 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/.github/CODEOWNERS
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.706620 py-imgui-redux-1.0.3/third-party/glfw/.github/workflows/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3934 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/.github/workflows/build.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1615 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/.gitignore
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      384 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/.mailmap
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.706620 py-imgui-redux-1.0.3/third-party/glfw/CMake/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1725 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/CMake/GenerateMappings.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1297 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/CMake/MacOSXBundleInfo.plist.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      596 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/CMake/i686-w64-mingw32-clang.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      588 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/CMake/i686-w64-mingw32.cmake
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.706620 py-imgui-redux-1.0.3/third-party/glfw/CMake/modules/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      747 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/CMake/modules/FindEpollShim.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      445 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/CMake/modules/FindOSMesa.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      915 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/CMake/modules/FindWaylandProtocols.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1043 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/CMake/modules/FindXKBCommon.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      606 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/CMake/x86_64-w64-mingw32-clang.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      598 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/CMake/x86_64-w64-mingw32.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13468 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4569 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/CONTRIBUTORS.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      904 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/LICENSE.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10199 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/README.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1142 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/cmake_uninstall.cmake.in
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.706620 py-imgui-redux-1.0.3/third-party/glfw/deps/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8053 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/deps/getopt.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2136 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/deps/getopt.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.706620 py-imgui-redux-1.0.3/third-party/glfw/deps/glad/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   206323 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/deps/glad/gl.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10037 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/deps/glad/khrplatform.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2870 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/deps/glad/vk_platform.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   285262 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/deps/glad/vulkan.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   109362 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/deps/glad_gl.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    47962 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/deps/glad_vulkan.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12708 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/deps/linmath.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.706620 py-imgui-redux-1.0.3/third-party/glfw/deps/mingw/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3111 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/deps/mingw/_mingw_dxhelper.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   112560 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/deps/mingw/dinput.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7950 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/deps/mingw/xinput.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   980614 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/deps/nuklear.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14077 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/deps/nuklear_glfw_gl2.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    71221 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/deps/stb_image_write.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13065 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/deps/tinycthread.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15660 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/deps/tinycthread.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.706620 py-imgui-redux-1.0.3/third-party/glfw/deps/vs2008/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7728 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/deps/vs2008/stdint.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.709953 py-imgui-redux-1.0.3/third-party/glfw/docs/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1027 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15407 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/CONTRIBUTING.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    78840 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/Doxyfile.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2025 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/DoxygenLayout.xml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      528 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/SUPPORT.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13431 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/build.dox
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14361 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/compat.dox
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14088 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/compile.dox
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12456 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/context.dox
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6480 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/extra.css
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1552 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/extra.css.map
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9841 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/extra.scss
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      114 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/footer.html
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1296 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/header.html
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    33163 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/input.dox
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4270 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/internal.dox
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16686 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/intro.dox
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1874 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/main.dox
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8557 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/monitor.dox
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    20715 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/moving.dox
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    31730 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/news.dox
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12527 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/quick.dox
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   110258 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/spaces.svg
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8905 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/vulkan.dox
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    55273 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/docs/window.dox
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.709953 py-imgui-redux-1.0.3/third-party/glfw/examples/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3833 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/examples/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19453 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/examples/boing.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9914 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/examples/gears.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    27988 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/examples/glfw.icns
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21630 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/examples/glfw.ico
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       53 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/examples/glfw.rc
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16055 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/examples/heightmap.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5105 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/examples/offscreen.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    35958 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/examples/particles.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7135 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/examples/sharing.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4850 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/examples/simple.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15179 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/examples/splitview.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11863 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/examples/wave.c
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.699953 py-imgui-redux-1.0.3/third-party/glfw/include/
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.709953 py-imgui-redux-1.0.3/third-party/glfw/include/GLFW/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   215860 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/include/GLFW/glfw3.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    20034 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/include/GLFW/glfw3native.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.713287 py-imgui-redux-1.0.3/third-party/glfw/src/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8739 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21092 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/cocoa_init.m
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1839 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/cocoa_joystick.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15825 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/cocoa_joystick.m
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19333 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/cocoa_monitor.m
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7979 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/cocoa_platform.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2213 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/cocoa_time.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    56339 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/cocoa_window.m
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    25484 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/context.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    25469 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/egl_context.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8559 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/egl_context.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      384 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/glfw3.pc.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       56 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/glfw3Config.cmake.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2662 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/glfw_config.h.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    22638 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/glx_context.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7602 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/glx_context.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11245 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/init.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    37983 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/input.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    28080 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/internal.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12412 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/linux_joystick.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2212 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/linux_joystick.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   257037 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/mappings.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5336 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/mappings.h.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14979 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/monitor.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2475 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/nsgl_context.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11870 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/nsgl_context.m
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1879 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/null_init.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1735 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/null_joystick.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1395 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/null_joystick.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2541 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/null_monitor.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2465 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/null_platform.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8112 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/null_window.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11915 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/osmesa_context.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3766 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/osmesa_context.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3322 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/posix_thread.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1680 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/posix_thread.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2855 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/posix_time.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1512 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/posix_time.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11854 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/vulkan.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    26959 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/wgl_context.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6891 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/wgl_context.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    23700 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/win32_init.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    26362 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/win32_joystick.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2073 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/win32_joystick.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16589 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/win32_monitor.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15713 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/win32_platform.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3196 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/win32_thread.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2238 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/win32_time.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    74337 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/win32_window.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    32882 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/window.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    23736 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/wl_init.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8515 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/wl_monitor.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15591 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/wl_platform.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    86107 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/wl_window.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    47852 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/x11_init.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19712 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/x11_monitor.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16711 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/x11_platform.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   101826 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/x11_window.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    23006 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/xkb_unicode.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1288 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/src/xkb_unicode.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.716620 py-imgui-redux-1.0.3/third-party/glfw/tests/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4556 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3718 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/clipboard.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14207 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/cursor.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3411 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/empty.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21549 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/events.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5651 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/gamma.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    33949 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/glfwinfo.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3888 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/icon.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8665 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/iconify.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9145 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/inputlag.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10764 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/joysticks.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7666 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/monitors.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6134 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/msaa.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3158 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/opacity.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6725 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/reopen.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7152 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/tearing.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4098 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/threads.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2797 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/timeout.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2081 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/title.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    81253 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/triangle-vulkan.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4536 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/glfw/tests/windows.c
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.716620 py-imgui-redux-1.0.3/third-party/imconfig/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9664 2023-03-09 01:18:12.000000 py-imgui-redux-1.0.3/third-party/imconfig/bind-imconfig.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.716620 py-imgui-redux-1.0.3/third-party/imgui/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1063 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/.editorconfig
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       45 2023-03-09 01:16:54.000000 py-imgui-redux-1.0.3/third-party/imgui/.git
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      397 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/.gitattributes
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.716620 py-imgui-redux-1.0.3/third-party/imgui/.github/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       59 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/.github/FUNDING.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1820 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/.github/issue_template.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      233 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/.github/pull_request_template.md
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.716620 py-imgui-redux-1.0.3/third-party/imgui/.github/workflows/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21070 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/.github/workflows/build.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      312 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/.github/workflows/scheduled.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1826 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/.github/workflows/static-analysis.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1075 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/.gitignore
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1083 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/LICENSE.txt
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.719954 py-imgui-redux-1.0.3/third-party/imgui/backends/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    29289 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_allegro5.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2013 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_allegro5.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15360 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_android.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1857 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_android.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    27085 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_dx10.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1303 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_dx10.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    29033 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_dx11.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1368 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_dx11.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    35118 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_dx12.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2373 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_dx12.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18178 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_dx9.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1297 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_dx9.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    36958 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_glfw.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3283 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_glfw.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13715 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_glut.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2893 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_glut.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3067 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_metal.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    27036 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_metal.mm
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15020 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_opengl2.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1988 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_opengl2.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    43384 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_opengl3.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2873 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_opengl3.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    35278 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_opengl3_loader.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2165 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_osx.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    33694 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_osx.mm
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    30854 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_sdl.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2357 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_sdl.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11141 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_sdlrenderer.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1454 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_sdlrenderer.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    76113 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_vulkan.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9588 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_vulkan.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    32521 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_wgpu.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1521 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_wgpu.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    40824 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_win32.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3118 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_win32.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.719954 py-imgui-redux-1.0.3/third-party/imgui/backends/vulkan/
--rwxr-xr-x   0 alagyn    (1000) alagyn    (1000)      254 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/vulkan/generate_spv.sh
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      249 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/vulkan/glsl_shader.frag
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      454 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/backends/vulkan/glsl_shader.vert
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.719954 py-imgui-redux-1.0.3/third-party/imgui/docs/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8761 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/docs/BACKENDS.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   337104 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/docs/CHANGELOG.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9780 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/docs/CONTRIBUTING.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13012 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/docs/EXAMPLES.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    45673 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/docs/FAQ.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19502 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/docs/FONTS.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19825 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/docs/README.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    35985 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/docs/TODO.txt
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.719954 py-imgui-redux-1.0.3/third-party/imgui/examples/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      595 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/README.txt
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.719954 py-imgui-redux-1.0.3/third-party/imgui/examples/example_allegro5/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1652 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_allegro5/README.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9410 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_allegro5/example_allegro5.vcxproj
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1912 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_allegro5/example_allegro5.vcxproj.filters
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      556 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_allegro5/imconfig_allegro5.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7095 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_allegro5/main.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.719954 py-imgui-redux-1.0.3/third-party/imgui/examples/example_android_opengl3/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1156 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_android_opengl3/CMakeLists.txt
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.719954 py-imgui-redux-1.0.3/third-party/imgui/examples/example_android_opengl3/android/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      154 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_android_opengl3/android/.gitignore
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.723287 py-imgui-redux-1.0.3/third-party/imgui/examples/example_android_opengl3/android/app/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      738 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_android_opengl3/android/app/build.gradle
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.699953 py-imgui-redux-1.0.3/third-party/imgui/examples/example_android_opengl3/android/app/src/
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.723287 py-imgui-redux-1.0.3/third-party/imgui/examples/example_android_opengl3/android/app/src/main/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      899 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_android_opengl3/android/app/src/main/AndroidManifest.xml
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.723287 py-imgui-redux-1.0.3/third-party/imgui/examples/example_android_opengl3/android/app/src/main/java/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1513 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_android_opengl3/android/app/src/main/java/MainActivity.kt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      421 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_android_opengl3/android/build.gradle
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       15 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_android_opengl3/android/settings.gradle
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14267 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_android_opengl3/main.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.723287 py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_metal/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      342 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_metal/README.md
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.723287 py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_metal/example_apple_metal.xcodeproj/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    24817 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_metal/example_apple_metal.xcodeproj/project.pbxproj
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.723287 py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_metal/iOS/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1563 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_metal/iOS/Info-iOS.plist
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1805 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_metal/iOS/LaunchScreen.storyboard
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.723287 py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_metal/macOS/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      941 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_metal/macOS/Info-macOS.plist
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6256 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_metal/macOS/MainMenu.storyboard
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11827 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_metal/main.mm
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.723287 py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_opengl2/
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.723287 py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_opengl2/example_apple_opengl2.xcodeproj/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15452 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_opengl2/example_apple_opengl2.xcodeproj/project.pbxproj
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9685 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_opengl2/main.mm
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.723287 py-imgui-redux-1.0.3/third-party/imgui/examples/example_emscripten_opengl3/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3080 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_emscripten_opengl3/Makefile
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2564 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_emscripten_opengl3/README.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9269 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_emscripten_opengl3/main.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2156 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_emscripten_opengl3/shell_minimal.html
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.723287 py-imgui-redux-1.0.3/third-party/imgui/examples/example_emscripten_wgpu/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2973 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_emscripten_wgpu/Makefile
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2288 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_emscripten_wgpu/README.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10450 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_emscripten_wgpu/main.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.723287 py-imgui-redux-1.0.3/third-party/imgui/examples/example_emscripten_wgpu/web/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2650 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_emscripten_wgpu/web/index.html
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.723287 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_metal/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1250 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_metal/Makefile
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8318 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_metal/main.mm
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.723287 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl2/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2154 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl2/Makefile
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      546 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl2/build_win32.bat
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9719 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl2/example_glfw_opengl2.vcxproj
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2031 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl2/example_glfw_opengl2.vcxproj.filters
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7966 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl2/main.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.723287 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl3/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2485 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl3/Makefile
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      546 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl3/build_win32.bat
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9793 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl3/example_glfw_opengl3.vcxproj
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2151 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl3/example_glfw_opengl3.vcxproj.filters
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8463 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl3/main.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.723287 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_vulkan/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1658 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_vulkan/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      793 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_vulkan/build_win32.bat
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      754 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_vulkan/build_win64.bat
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10308 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_vulkan/example_glfw_vulkan.vcxproj
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2029 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_vulkan/example_glfw_vulkan.vcxproj.filters
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    24824 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_vulkan/main.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.723287 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glut_opengl2/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1955 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glut_opengl2/Makefile
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9715 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glut_opengl2/example_glut_opengl2.vcxproj
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2035 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glut_opengl2/example_glut_opengl2.vcxproj.filters
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7461 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_glut_opengl2/main.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.726621 py-imgui-redux-1.0.3/third-party/imgui/examples/example_null/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2701 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_null/Makefile
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      253 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_null/build_win32.bat
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1075 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_null/main.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.726621 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_directx11/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      688 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_directx11/build_win32.bat
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10106 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_directx11/example_sdl_directx11.vcxproj
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1949 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_directx11/example_sdl_directx11.vcxproj.filters
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10355 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_directx11/main.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.726621 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_metal/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1255 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_metal/Makefile
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9092 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_metal/main.mm
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.726621 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl2/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2093 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl2/Makefile
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1444 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl2/README.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      555 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl2/build_win32.bat
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9884 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl2/example_sdl_opengl2.vcxproj
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2029 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl2/example_sdl_opengl2.vcxproj.filters
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7992 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl2/main.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.726621 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl3/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2579 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl3/Makefile
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1499 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl3/README.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      555 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl3/build_win32.bat
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9958 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl3/example_sdl_opengl3.vcxproj
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2149 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl3/example_sdl_opengl3.vcxproj.filters
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8805 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl3/main.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.726621 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_sdlrenderer/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2101 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_sdlrenderer/Makefile
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1305 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_sdlrenderer/README.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      540 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_sdlrenderer/build_win32.bat
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9684 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_sdlrenderer/example_sdl_sdlrenderer.vcxproj
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2037 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_sdlrenderer/example_sdl_sdlrenderer.vcxproj.filters
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8053 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_sdlrenderer/main.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.726621 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_vulkan/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      628 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_vulkan/build_win32.bat
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10473 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_vulkan/example_sdl_vulkan.vcxproj
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2029 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_vulkan/example_sdl_vulkan.vcxproj.filters
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    24718 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_vulkan/main.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.726621 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx10/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      613 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx10/build_win32.bat
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9138 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx10/example_win32_directx10.vcxproj
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1953 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx10/example_win32_directx10.vcxproj.filters
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10382 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx10/main.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.726621 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx11/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      614 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx11/build_win32.bat
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9068 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx11/example_win32_directx11.vcxproj
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1953 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx11/example_win32_directx11.vcxproj.filters
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10818 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx11/main.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.726621 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx12/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      701 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx12/build_win32.bat
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9460 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx12/example_win32_directx12.vcxproj
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1988 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx12/example_win32_directx12.vcxproj.filters
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19566 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx12/main.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.729954 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx9/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      529 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx9/build_win32.bat
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9111 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx9/example_win32_directx9.vcxproj
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2025 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx9/example_win32_directx9.vcxproj.filters
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10140 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx9/main.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10316 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/imgui_examples.sln
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.703287 py-imgui-redux-1.0.3/third-party/imgui/examples/libs/
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.729954 py-imgui-redux-1.0.3/third-party/imgui/examples/libs/glfw/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      934 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/libs/glfw/COPYING.txt
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.703287 py-imgui-redux-1.0.3/third-party/imgui/examples/libs/glfw/include/
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.729954 py-imgui-redux-1.0.3/third-party/imgui/examples/libs/glfw/include/GLFW/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   151427 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/libs/glfw/include/GLFW/glfw3.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13600 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/libs/glfw/include/GLFW/glfw3native.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.729954 py-imgui-redux-1.0.3/third-party/imgui/examples/libs/glfw/lib-vc2010-32/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   187376 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/libs/glfw/lib-vc2010-32/glfw3.lib
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.729954 py-imgui-redux-1.0.3/third-party/imgui/examples/libs/glfw/lib-vc2010-64/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   291120 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/libs/glfw/lib-vc2010-64/glfw3.lib
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.729954 py-imgui-redux-1.0.3/third-party/imgui/examples/libs/usynergy/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      278 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/libs/usynergy/README.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18289 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/libs/usynergy/uSynergy.c
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16644 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/examples/libs/usynergy/uSynergy.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9666 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/imconfig.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   723992 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/imgui.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   303159 2023-03-15 03:29:45.000000 py-imgui-redux-1.0.3/third-party/imgui/imgui.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   408978 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/imgui_demo.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   212634 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/imgui_draw.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   235627 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/imgui_internal.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   218729 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/imgui_tables.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   416780 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/imgui_widgets.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    20344 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/imstb_rectpack.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    54857 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/imstb_textedit.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   199484 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/imstb_truetype.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.729954 py-imgui-redux-1.0.3/third-party/imgui/misc/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      998 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/misc/README.txt
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.729954 py-imgui-redux-1.0.3/third-party/imgui/misc/cpp/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      557 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/misc/cpp/README.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2954 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/misc/cpp/imgui_stdlib.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1015 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/misc/cpp/imgui_stdlib.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.729954 py-imgui-redux-1.0.3/third-party/imgui/misc/debuggers/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      487 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/misc/debuggers/README.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      555 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/misc/debuggers/imgui.gdb
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1275 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/misc/debuggers/imgui.natstepfilter
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1917 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/misc/debuggers/imgui.natvis
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.733287 py-imgui-redux-1.0.3/third-party/imgui/misc/fonts/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    43912 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/misc/fonts/Cousine-Regular.ttf
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   190044 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/misc/fonts/DroidSans.ttf
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16848 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/misc/fonts/Karla-Regular.ttf
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    41208 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/misc/fonts/ProggyClean.ttf
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    35656 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/misc/fonts/ProggyTiny.ttf
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   162588 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/misc/fonts/Roboto-Medium.ttf
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13783 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/misc/fonts/binary_to_compressed_c.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.733287 py-imgui-redux-1.0.3/third-party/imgui/misc/freetype/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1808 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/misc/freetype/README.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    38497 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/misc/freetype/imgui_freetype.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3544 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/misc/freetype/imgui_freetype.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.733287 py-imgui-redux-1.0.3/third-party/imgui/misc/single_file/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      751 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imgui/misc/single_file/imgui_single_file.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.733287 py-imgui-redux-1.0.3/third-party/imnodes/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1022 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/.clang-format
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1400 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/.clang-tidy
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       47 2023-03-09 01:16:56.000000 py-imgui-redux-1.0.3/third-party/imnodes/.git
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.703287 py-imgui-redux-1.0.3/third-party/imnodes/.github/
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.733287 py-imgui-redux-1.0.3/third-party/imnodes/.github/workflows/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      699 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/.github/workflows/build.yaml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9001 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/.gitignore
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       80 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/.gitmodules
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2180 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1072 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/LICENSE.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9463 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/README.md
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.733287 py-imgui-redux-1.0.3/third-party/imnodes/example/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    24843 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/example/color_node_editor.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9464 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/example/graph.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      977 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/example/hello.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4164 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/example/main.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3595 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/example/multi_editor.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      135 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/example/node_editor.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5865 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/example/save_load.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.733287 py-imgui-redux-1.0.3/third-party/imnodes/img/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)  1517285 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/img/imnodes.gif
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   114226 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/imnodes.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18234 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/imnodes.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12908 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/imnodes_internal.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      213 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/imnodes/vcpkg.json
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.736621 py-imgui-redux-1.0.3/third-party/implot/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       46 2023-03-09 01:16:57.000000 py-imgui-redux-1.0.3/third-party/implot/.git
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.736621 py-imgui-redux-1.0.3/third-party/implot/.github/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3117 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/implot/.github/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1480 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/implot/.github/example_implot.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.736621 py-imgui-redux-1.0.3/third-party/implot/.github/workflows/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3317 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/implot/.github/workflows/build.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1068 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/implot/LICENSE
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11842 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/implot/README.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3494 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/implot/TODO.md
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   264935 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/implot/implot.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    78669 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/implot/implot.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   111935 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/implot/implot_demo.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    67176 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/implot/implot_internal.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   118754 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/implot/implot_items.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.736621 py-imgui-redux-1.0.3/third-party/pybind11/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1271 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.appveyor.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      996 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.clang-format
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2605 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.clang-tidy
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2196 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.cmake-format.yaml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1308 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.codespell-ignore-lines
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       48 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.git
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       18 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.gitattributes
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.736621 py-imgui-redux-1.0.3/third-party/pybind11/.github/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      182 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.github/CODEOWNERS
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15271 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.github/CONTRIBUTING.md
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.739954 py-imgui-redux-1.0.3/third-party/pybind11/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2561 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      328 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      162 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.github/dependabot.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      116 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.github/labeler.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       50 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.github/labeler_merged.yml
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.739954 py-imgui-redux-1.0.3/third-party/pybind11/.github/matchers/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      668 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.github/matchers/pylint.json
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      645 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.github/pull_request_template.md
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.739954 py-imgui-redux-1.0.3/third-party/pybind11/.github/workflows/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    31868 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.github/workflows/ci.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2127 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.github/workflows/configure.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1447 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.github/workflows/format.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      559 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.github/workflows/labeler.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2558 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.github/workflows/pip.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2865 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.github/workflows/upstream.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      502 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.gitignore
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4332 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.pre-commit-config.yaml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       62 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/.readthedocs.yml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11983 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1684 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/LICENSE
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      223 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/MANIFEST.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7686 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/README.rst
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.739954 py-imgui-redux-1.0.3/third-party/pybind11/docs/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      607 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/Doxyfile
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7417 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/Makefile
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.703287 py-imgui-redux-1.0.3/third-party/pybind11/docs/_static/
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.739954 py-imgui-redux-1.0.3/third-party/pybind11/docs/_static/css/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       37 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/_static/css/custom.css
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.743287 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.743287 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/cast/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3937 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/cast/chrono.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3429 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/cast/custom.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14283 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/cast/eigen.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3889 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/cast/functional.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1556 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/cast/index.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12371 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/cast/overview.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9586 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/cast/stl.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8863 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/cast/strings.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    47796 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/classes.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8453 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/embedding.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17796 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/exceptions.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    26729 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/functions.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15651 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/misc.rst
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.743287 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/pycpp/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      278 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/pycpp/index.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17161 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/pycpp/numpy.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9030 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/pycpp/object.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5710 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/pycpp/utilities.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6377 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/smart_ptrs.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9240 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/basics.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2856 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/benchmark.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3168 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/benchmark.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   114174 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/changelog.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16380 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/classes.rst
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.743287 py-imgui-redux-1.0.3/third-party/pybind11/docs/cmake/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      273 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/cmake/index.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    25777 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/compiling.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11559 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/conf.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13177 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/faq.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      613 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/index.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3277 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/installing.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3079 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/limitations.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    61034 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/pybind11-logo.png
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    44653 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/pybind11_vs_boost_python1.png
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    87708 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    41121 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/pybind11_vs_boost_python2.png
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    85853 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2647 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/reference.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4414 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/release.rst
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      149 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/requirements.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    23489 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/docs/upgrade.rst
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.703287 py-imgui-redux-1.0.3/third-party/pybind11/include/
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.743287 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    23959 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/attr.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7069 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    65660 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/cast.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8458 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      120 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/common.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2096 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.743287 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/detail/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    28251 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    52929 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5491 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17869 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    26305 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    42613 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1625 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.743287 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/eigen/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    31418 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18108 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      316 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13471 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/embed.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4731 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/eval.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5002 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/functional.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8262 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/gil.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8862 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    79408 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9103 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/operators.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2734 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/options.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)   126420 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    94641 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.743287 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/stl/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4185 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15337 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/stl.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    29747 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2765 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/noxfile.py
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.746621 py-imgui-redux-1.0.3/third-party/pybind11/pybind11/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      414 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/pybind11/__init__.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1360 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/pybind11/__main__.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      228 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/pybind11/_version.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1226 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/pybind11/commands.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)        0 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/pybind11/py.typed
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17609 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1261 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/pyproject.toml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1618 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/setup.cfg
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4877 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/setup.py
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.749954 py-imgui-redux-1.0.3/third-party/pybind11/tests/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21675 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5741 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/conftest.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11736 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/constructor_stats.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3578 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/cross_module_gil_utils.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1776 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/cross_module_interleaved_error_already_set.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      396 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      940 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/env.py
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.749954 py-imgui-redux-1.0.3/third-party/pybind11/tests/extra_python_package/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)        0 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/extra_python_package/pytest.ini
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8296 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/extra_python_package/test_files.py
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.749954 py-imgui-redux-1.0.3/third-party/pybind11/tests/extra_setuptools/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)        0 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/extra_setuptools/pytest.ini
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4153 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2847 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/local_bindings.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5743 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/object.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6264 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4517 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/pybind11_tests.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2685 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/pybind11_tests.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      768 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/pytest.ini
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      600 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/requirements.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      855 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_async.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      534 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_async.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8567 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_buffers.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4841 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_buffers.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16025 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_builtin_casters.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17245 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_builtin_casters.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4118 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_call_policies.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6549 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_call_policies.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10858 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_callbacks.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6246 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_callbacks.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3370 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_chrono.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5695 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_chrono.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    24874 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_class.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14815 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_class.py
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.749954 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2639 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      673 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/embed.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.749954 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1171 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.749954 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1293 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.749954 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1685 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      152 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/main.cpp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.749954 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1353 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.749954 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1163 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.749954 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1368 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      198 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/test.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3831 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_const_name.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      589 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_const_name.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5615 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_constants_and_functions.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1498 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_constants_and_functions.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10886 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_copy_move.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4796 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_copy_move.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7280 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_custom_type_casters.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3980 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_custom_type_casters.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1259 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_custom_type_setup.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1089 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_custom_type_setup.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4557 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_docstring_options.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2423 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_docstring_options.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19350 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_eigen_matrix.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    28867 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_eigen_matrix.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      473 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_eigen_tensor.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10590 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_eigen_tensor.inl
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9456 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_eigen_tensor.py
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.749954 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_embed/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1798 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_embed/CMakeLists.txt
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1315 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_embed/catch.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      543 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_embed/external_module.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16535 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_embed/test_interpreter.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      237 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_embed/test_interpreter.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      275 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_embed/test_trampoline.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5722 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_enum.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8903 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_enum.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3168 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_eval.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1143 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_eval.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      119 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_eval_call.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11904 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_exceptions.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      399 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_exceptions.h
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12774 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_exceptions.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18155 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_factory_constructors.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16519 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_factory_constructors.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5311 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_gil_scoped.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8540 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_gil_scoped.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3960 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_iostream.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7286 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_iostream.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9444 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13757 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_kwargs_and_defaults.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4401 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_local_bindings.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8049 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_local_bindings.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21388 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_methods_and_attributes.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18134 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_methods_and_attributes.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4121 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_modules.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4191 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_modules.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12305 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_multiple_inheritance.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11874 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_multiple_inheritance.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19861 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_numpy_array.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    20356 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_numpy_array.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21114 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_numpy_dtypes.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14394 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_numpy_dtypes.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4487 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_numpy_vectorize.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9686 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_numpy_vectorize.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2777 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_opaque_types.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1847 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_opaque_types.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9132 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_operator_overloading.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4333 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_operator_overloading.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6719 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_pickling.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2720 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_pickling.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    30750 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_pytypes.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    23630 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_pytypes.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21153 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_sequences_and_iterators.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8021 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_sequences_and_iterators.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18898 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_smart_ptr.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9530 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_smart_ptr.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21587 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_stl.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12235 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_stl.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4622 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_stl_binders.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9174 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_stl_binders.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4617 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      741 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_tagbased_polymorphic.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1855 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_thread.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      826 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_thread.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      603 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_union.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      148 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_union.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    22991 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_virtual_functions.cpp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12919 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/test_virtual_functions.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3226 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/valgrind-numpy-scipy.supp
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2657 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tests/valgrind-python.supp
-drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 17:51:32.753288 py-imgui-redux-1.0.3/third-party/pybind11/tools/
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2350 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3105 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11190 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      817 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0 alagyn    (1000) alagyn    (1000)     1423 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tools/check-style.sh
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      952 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1040 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1031 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tools/libsize.py
--rwxr-xr-x   0 alagyn    (1000) alagyn    (1000)     1311 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tools/make_changelog.py
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)      196 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14033 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6930 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8960 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8361 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)       94 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tools/pyproject.toml
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2104 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tools/setup_global.py.in
--rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1234 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.3/third-party/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.166732 py-imgui-redux-1.0.4/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      461 2023-07-14 18:07:21.000000 py-imgui-redux-1.0.4/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1070 2023-03-09 01:15:58.000000 py-imgui-redux-1.0.4/LICENSE
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       91 2023-07-14 17:50:56.000000 py-imgui-redux-1.0.4/MANIFEST.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5363 2023-07-14 18:08:56.166732 py-imgui-redux-1.0.4/PKG-INFO
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4637 2023-03-18 18:20:05.000000 py-imgui-redux-1.0.4/README.md
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.136732 py-imgui-redux-1.0.4/imgui/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    79389 2023-04-08 20:08:02.000000 py-imgui-redux-1.0.4/imgui/__init__.pyi
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.140065 py-imgui-redux-1.0.4/imgui/glfw/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      592 2023-04-08 20:08:02.000000 py-imgui-redux-1.0.4/imgui/glfw/__init__.pyi
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.140065 py-imgui-redux-1.0.4/imgui/imnodes/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12577 2023-04-08 20:08:02.000000 py-imgui-redux-1.0.4/imgui/imnodes/__init__.pyi
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.140065 py-imgui-redux-1.0.4/imgui/implot/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    29707 2023-04-08 20:08:02.000000 py-imgui-redux-1.0.4/imgui/implot/__init__.pyi
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.140065 py-imgui-redux-1.0.4/py_imgui_redux.egg-info/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5363 2023-07-14 18:08:56.000000 py-imgui-redux-1.0.4/py_imgui_redux.egg-info/PKG-INFO
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    30237 2023-07-14 18:08:56.000000 py-imgui-redux-1.0.4/py_imgui_redux.egg-info/SOURCES.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)        1 2023-07-14 18:08:56.000000 py-imgui-redux-1.0.4/py_imgui_redux.egg-info/dependency_links.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)        6 2023-07-14 18:08:56.000000 py-imgui-redux-1.0.4/py_imgui_redux.egg-info/top_level.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12918 2023-07-14 18:08:25.000000 py-imgui-redux-1.0.4/pyproject.toml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       38 2023-07-14 18:08:56.166732 py-imgui-redux-1.0.4/setup.cfg
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10250 2023-05-10 22:34:33.000000 py-imgui-redux-1.0.4/setup.py
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.140065 py-imgui-redux-1.0.4/third-party/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1369 2023-03-09 02:26:26.000000 py-imgui-redux-1.0.4/third-party/CMakeLists.txt
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.140065 py-imgui-redux-1.0.4/third-party/glfw/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1206 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/.appveyor.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       44 2023-03-09 01:16:45.000000 py-imgui-redux-1.0.4/third-party/glfw/.git
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      142 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/.gitattributes
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.140065 py-imgui-redux-1.0.4/third-party/glfw/.github/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      175 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/.github/CODEOWNERS
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.140065 py-imgui-redux-1.0.4/third-party/glfw/.github/workflows/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3934 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/.github/workflows/build.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1615 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/.gitignore
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      384 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/.mailmap
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.140065 py-imgui-redux-1.0.4/third-party/glfw/CMake/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1725 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/CMake/GenerateMappings.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1297 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/CMake/MacOSXBundleInfo.plist.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      596 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/CMake/i686-w64-mingw32-clang.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      588 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/CMake/i686-w64-mingw32.cmake
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.140065 py-imgui-redux-1.0.4/third-party/glfw/CMake/modules/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      747 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/CMake/modules/FindEpollShim.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      445 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/CMake/modules/FindOSMesa.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      915 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/CMake/modules/FindWaylandProtocols.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1043 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/CMake/modules/FindXKBCommon.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      606 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/CMake/x86_64-w64-mingw32-clang.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      598 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/CMake/x86_64-w64-mingw32.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13468 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4569 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/CONTRIBUTORS.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      904 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/LICENSE.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10199 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/README.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1142 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/cmake_uninstall.cmake.in
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.140065 py-imgui-redux-1.0.4/third-party/glfw/deps/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8053 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/deps/getopt.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2136 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/deps/getopt.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.140065 py-imgui-redux-1.0.4/third-party/glfw/deps/glad/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   206323 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/deps/glad/gl.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10037 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/deps/glad/khrplatform.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2870 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/deps/glad/vk_platform.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   285262 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/deps/glad/vulkan.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   109362 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/deps/glad_gl.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    47962 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/deps/glad_vulkan.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12708 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/deps/linmath.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.140065 py-imgui-redux-1.0.4/third-party/glfw/deps/mingw/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3111 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/deps/mingw/_mingw_dxhelper.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   112560 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/deps/mingw/dinput.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7950 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/deps/mingw/xinput.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   980614 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/deps/nuklear.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14077 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/deps/nuklear_glfw_gl2.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    71221 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/deps/stb_image_write.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13065 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/deps/tinycthread.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15660 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/deps/tinycthread.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.140065 py-imgui-redux-1.0.4/third-party/glfw/deps/vs2008/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7728 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/deps/vs2008/stdint.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.143398 py-imgui-redux-1.0.4/third-party/glfw/docs/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1027 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15407 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/CONTRIBUTING.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    78840 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/Doxyfile.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2025 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/DoxygenLayout.xml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      528 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/SUPPORT.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13431 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/build.dox
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14361 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/compat.dox
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14088 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/compile.dox
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12456 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/context.dox
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6480 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/extra.css
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1552 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/extra.css.map
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9841 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/extra.scss
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      114 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/footer.html
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1296 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/header.html
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    33163 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/input.dox
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4270 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/internal.dox
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16686 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/intro.dox
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1874 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/main.dox
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8557 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/monitor.dox
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    20715 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/moving.dox
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    31730 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/news.dox
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12527 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/quick.dox
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   110258 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/spaces.svg
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8905 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/vulkan.dox
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    55273 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/docs/window.dox
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.143398 py-imgui-redux-1.0.4/third-party/glfw/examples/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3833 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/examples/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19453 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/examples/boing.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9914 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/examples/gears.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    27988 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/examples/glfw.icns
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21630 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/examples/glfw.ico
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       53 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/examples/glfw.rc
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16055 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/examples/heightmap.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5105 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/examples/offscreen.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    35958 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/examples/particles.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7135 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/examples/sharing.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4850 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/examples/simple.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15179 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/examples/splitview.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11863 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/examples/wave.c
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.136732 py-imgui-redux-1.0.4/third-party/glfw/include/
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.143398 py-imgui-redux-1.0.4/third-party/glfw/include/GLFW/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   215860 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/include/GLFW/glfw3.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    20034 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/include/GLFW/glfw3native.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.143398 py-imgui-redux-1.0.4/third-party/glfw/src/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8739 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21092 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/cocoa_init.m
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1839 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/cocoa_joystick.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15825 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/cocoa_joystick.m
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19333 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/cocoa_monitor.m
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7979 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/cocoa_platform.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2213 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/cocoa_time.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    56339 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/cocoa_window.m
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    25484 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/context.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    25469 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/egl_context.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8559 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/egl_context.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      384 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/glfw3.pc.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       56 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/glfw3Config.cmake.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2662 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/glfw_config.h.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    22638 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/glx_context.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7602 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/glx_context.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11245 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/init.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    37983 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/input.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    28080 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/internal.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12412 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/linux_joystick.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2212 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/linux_joystick.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   257037 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/mappings.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5336 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/mappings.h.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14979 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/monitor.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2475 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/nsgl_context.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11870 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/nsgl_context.m
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1879 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/null_init.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1735 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/null_joystick.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1395 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/null_joystick.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2541 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/null_monitor.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2465 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/null_platform.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8112 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/null_window.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11915 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/osmesa_context.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3766 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/osmesa_context.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3322 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/posix_thread.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1680 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/posix_thread.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2855 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/posix_time.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1512 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/posix_time.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11854 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/vulkan.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    26959 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/wgl_context.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6891 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/wgl_context.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    23700 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/win32_init.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    26362 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/win32_joystick.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2073 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/win32_joystick.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16589 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/win32_monitor.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15713 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/win32_platform.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3196 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/win32_thread.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2238 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/win32_time.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    74337 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/win32_window.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    32882 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/window.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    23736 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/wl_init.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8515 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/wl_monitor.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15591 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/wl_platform.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    86107 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/wl_window.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    47852 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/x11_init.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19712 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/x11_monitor.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16711 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/x11_platform.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   101826 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/x11_window.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    23006 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/xkb_unicode.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1288 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/src/xkb_unicode.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.146732 py-imgui-redux-1.0.4/third-party/glfw/tests/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4556 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3718 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/clipboard.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14207 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/cursor.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3411 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/empty.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21549 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/events.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5651 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/gamma.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    33949 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/glfwinfo.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3888 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/icon.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8665 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/iconify.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9145 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/inputlag.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10764 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/joysticks.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7666 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/monitors.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6134 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/msaa.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3158 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/opacity.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6725 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/reopen.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7152 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/tearing.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4098 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/threads.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2797 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/timeout.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2081 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/title.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    81253 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/triangle-vulkan.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4536 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/glfw/tests/windows.c
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.146732 py-imgui-redux-1.0.4/third-party/imconfig/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9664 2023-03-09 01:18:12.000000 py-imgui-redux-1.0.4/third-party/imconfig/bind-imconfig.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.146732 py-imgui-redux-1.0.4/third-party/imgui/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1063 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/.editorconfig
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       45 2023-03-09 01:16:54.000000 py-imgui-redux-1.0.4/third-party/imgui/.git
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      397 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/.gitattributes
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.146732 py-imgui-redux-1.0.4/third-party/imgui/.github/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       59 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/.github/FUNDING.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1820 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/.github/issue_template.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      233 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/.github/pull_request_template.md
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.146732 py-imgui-redux-1.0.4/third-party/imgui/.github/workflows/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21070 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/.github/workflows/build.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      312 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/.github/workflows/scheduled.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1826 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/.github/workflows/static-analysis.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1075 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/.gitignore
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1083 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/LICENSE.txt
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/backends/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    29289 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_allegro5.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2013 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_allegro5.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15360 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_android.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1857 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_android.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    27085 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_dx10.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1303 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_dx10.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    29033 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_dx11.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1368 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_dx11.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    35118 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_dx12.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2373 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_dx12.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18178 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_dx9.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1297 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_dx9.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    36958 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_glfw.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3283 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_glfw.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13715 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_glut.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2893 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_glut.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3067 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_metal.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    27036 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_metal.mm
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15020 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_opengl2.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1988 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_opengl2.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    43384 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_opengl3.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2873 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_opengl3.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    35278 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_opengl3_loader.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2165 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_osx.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    33694 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_osx.mm
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    30854 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_sdl.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2357 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_sdl.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11141 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_sdlrenderer.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1454 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_sdlrenderer.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    76113 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_vulkan.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9588 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_vulkan.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    32521 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_wgpu.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1521 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_wgpu.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    40824 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_win32.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3118 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_win32.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/backends/vulkan/
+-rwxr-xr-x   0 alagyn    (1000) alagyn    (1000)      254 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/vulkan/generate_spv.sh
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      249 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/vulkan/glsl_shader.frag
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      454 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/backends/vulkan/glsl_shader.vert
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/docs/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8761 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/docs/BACKENDS.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   337104 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/docs/CHANGELOG.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9780 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/docs/CONTRIBUTING.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13012 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/docs/EXAMPLES.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    45673 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/docs/FAQ.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19502 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/docs/FONTS.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19825 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/docs/README.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    35985 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/docs/TODO.txt
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      595 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/README.txt
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_allegro5/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1652 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_allegro5/README.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9410 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_allegro5/example_allegro5.vcxproj
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1912 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_allegro5/example_allegro5.vcxproj.filters
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      556 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_allegro5/imconfig_allegro5.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7095 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_allegro5/main.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_android_opengl3/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1156 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_android_opengl3/CMakeLists.txt
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_android_opengl3/android/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      154 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_android_opengl3/android/.gitignore
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_android_opengl3/android/app/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      738 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_android_opengl3/android/app/build.gradle
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.136732 py-imgui-redux-1.0.4/third-party/imgui/examples/example_android_opengl3/android/app/src/
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_android_opengl3/android/app/src/main/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      899 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_android_opengl3/android/app/src/main/AndroidManifest.xml
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_android_opengl3/android/app/src/main/java/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1513 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_android_opengl3/android/app/src/main/java/MainActivity.kt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      421 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_android_opengl3/android/build.gradle
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       15 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_android_opengl3/android/settings.gradle
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14267 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_android_opengl3/main.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_metal/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      342 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_metal/README.md
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_metal/example_apple_metal.xcodeproj/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    24817 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_metal/example_apple_metal.xcodeproj/project.pbxproj
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_metal/iOS/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1563 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_metal/iOS/Info-iOS.plist
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1805 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_metal/iOS/LaunchScreen.storyboard
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_metal/macOS/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      941 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_metal/macOS/Info-macOS.plist
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6256 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_metal/macOS/MainMenu.storyboard
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11827 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_metal/main.mm
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_opengl2/
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_opengl2/example_apple_opengl2.xcodeproj/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15452 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_opengl2/example_apple_opengl2.xcodeproj/project.pbxproj
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9685 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_opengl2/main.mm
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_emscripten_opengl3/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3080 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_emscripten_opengl3/Makefile
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2564 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_emscripten_opengl3/README.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9269 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_emscripten_opengl3/main.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2156 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_emscripten_opengl3/shell_minimal.html
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_emscripten_wgpu/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2973 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_emscripten_wgpu/Makefile
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2288 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_emscripten_wgpu/README.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10450 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_emscripten_wgpu/main.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_emscripten_wgpu/web/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2650 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_emscripten_wgpu/web/index.html
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_metal/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1250 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_metal/Makefile
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8318 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_metal/main.mm
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl2/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2154 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl2/Makefile
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      546 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl2/build_win32.bat
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9719 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl2/example_glfw_opengl2.vcxproj
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2031 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl2/example_glfw_opengl2.vcxproj.filters
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7966 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl2/main.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl3/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2485 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl3/Makefile
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      546 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl3/build_win32.bat
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9793 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl3/example_glfw_opengl3.vcxproj
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2151 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl3/example_glfw_opengl3.vcxproj.filters
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8463 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl3/main.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_vulkan/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1658 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_vulkan/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      793 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_vulkan/build_win32.bat
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      754 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_vulkan/build_win64.bat
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10308 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_vulkan/example_glfw_vulkan.vcxproj
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2029 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_vulkan/example_glfw_vulkan.vcxproj.filters
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    24824 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_vulkan/main.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glut_opengl2/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1955 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glut_opengl2/Makefile
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9715 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glut_opengl2/example_glut_opengl2.vcxproj
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2035 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glut_opengl2/example_glut_opengl2.vcxproj.filters
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7461 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_glut_opengl2/main.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_null/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2701 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_null/Makefile
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      253 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_null/build_win32.bat
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1075 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_null/main.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_directx11/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      688 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_directx11/build_win32.bat
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10106 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_directx11/example_sdl_directx11.vcxproj
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1949 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_directx11/example_sdl_directx11.vcxproj.filters
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10355 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_directx11/main.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.150065 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_metal/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1255 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_metal/Makefile
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9092 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_metal/main.mm
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl2/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2093 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl2/Makefile
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1444 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl2/README.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      555 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl2/build_win32.bat
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9884 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl2/example_sdl_opengl2.vcxproj
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2029 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl2/example_sdl_opengl2.vcxproj.filters
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7992 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl2/main.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl3/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2579 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl3/Makefile
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1499 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl3/README.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      555 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl3/build_win32.bat
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9958 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl3/example_sdl_opengl3.vcxproj
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2149 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl3/example_sdl_opengl3.vcxproj.filters
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8805 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl3/main.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_sdlrenderer/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2101 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_sdlrenderer/Makefile
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1305 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_sdlrenderer/README.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      540 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_sdlrenderer/build_win32.bat
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9684 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_sdlrenderer/example_sdl_sdlrenderer.vcxproj
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2037 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_sdlrenderer/example_sdl_sdlrenderer.vcxproj.filters
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8053 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_sdlrenderer/main.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_vulkan/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      628 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_vulkan/build_win32.bat
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10473 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_vulkan/example_sdl_vulkan.vcxproj
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2029 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_vulkan/example_sdl_vulkan.vcxproj.filters
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    24718 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_vulkan/main.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx10/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      613 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx10/build_win32.bat
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9138 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx10/example_win32_directx10.vcxproj
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1953 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx10/example_win32_directx10.vcxproj.filters
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10382 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx10/main.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx11/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      614 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx11/build_win32.bat
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9068 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx11/example_win32_directx11.vcxproj
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1953 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx11/example_win32_directx11.vcxproj.filters
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10818 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx11/main.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx12/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      701 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx12/build_win32.bat
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9460 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx12/example_win32_directx12.vcxproj
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1988 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx12/example_win32_directx12.vcxproj.filters
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19566 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx12/main.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx9/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      529 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx9/build_win32.bat
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9111 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx9/example_win32_directx9.vcxproj
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2025 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx9/example_win32_directx9.vcxproj.filters
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10140 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx9/main.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10316 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/imgui_examples.sln
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.136732 py-imgui-redux-1.0.4/third-party/imgui/examples/libs/
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imgui/examples/libs/glfw/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      934 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/libs/glfw/COPYING.txt
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.136732 py-imgui-redux-1.0.4/third-party/imgui/examples/libs/glfw/include/
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imgui/examples/libs/glfw/include/GLFW/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   151427 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/libs/glfw/include/GLFW/glfw3.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13600 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/libs/glfw/include/GLFW/glfw3native.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imgui/examples/libs/glfw/lib-vc2010-32/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   187376 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/libs/glfw/lib-vc2010-32/glfw3.lib
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imgui/examples/libs/glfw/lib-vc2010-64/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   291120 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/libs/glfw/lib-vc2010-64/glfw3.lib
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imgui/examples/libs/usynergy/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      278 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/libs/usynergy/README.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18289 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/libs/usynergy/uSynergy.c
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16644 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/examples/libs/usynergy/uSynergy.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9666 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/imconfig.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   723992 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/imgui.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   303159 2023-03-15 03:29:45.000000 py-imgui-redux-1.0.4/third-party/imgui/imgui.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   408978 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/imgui_demo.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   212634 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/imgui_draw.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   235627 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/imgui_internal.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   218729 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/imgui_tables.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   416780 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/imgui_widgets.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    20344 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/imstb_rectpack.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    54857 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/imstb_textedit.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   199484 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/imstb_truetype.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imgui/misc/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      998 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/misc/README.txt
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imgui/misc/cpp/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      557 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/misc/cpp/README.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2954 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/misc/cpp/imgui_stdlib.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1015 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/misc/cpp/imgui_stdlib.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imgui/misc/debuggers/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      487 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/misc/debuggers/README.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      555 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/misc/debuggers/imgui.gdb
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1275 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/misc/debuggers/imgui.natstepfilter
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1917 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/misc/debuggers/imgui.natvis
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imgui/misc/fonts/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    43912 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/misc/fonts/Cousine-Regular.ttf
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   190044 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/misc/fonts/DroidSans.ttf
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16848 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/misc/fonts/Karla-Regular.ttf
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    41208 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/misc/fonts/ProggyClean.ttf
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    35656 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/misc/fonts/ProggyTiny.ttf
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   162588 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/misc/fonts/Roboto-Medium.ttf
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13783 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/misc/fonts/binary_to_compressed_c.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imgui/misc/freetype/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1808 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/misc/freetype/README.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    38497 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/misc/freetype/imgui_freetype.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3544 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/misc/freetype/imgui_freetype.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imgui/misc/single_file/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      751 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imgui/misc/single_file/imgui_single_file.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imnodes/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1022 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/.clang-format
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1400 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/.clang-tidy
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       47 2023-03-09 01:16:56.000000 py-imgui-redux-1.0.4/third-party/imnodes/.git
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.136732 py-imgui-redux-1.0.4/third-party/imnodes/.github/
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.153398 py-imgui-redux-1.0.4/third-party/imnodes/.github/workflows/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      699 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/.github/workflows/build.yaml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9001 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/.gitignore
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       80 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/.gitmodules
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2180 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1072 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/LICENSE.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9463 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/README.md
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.156732 py-imgui-redux-1.0.4/third-party/imnodes/example/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    24843 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/example/color_node_editor.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9464 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/example/graph.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      977 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/example/hello.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4164 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/example/main.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3595 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/example/multi_editor.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      135 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/example/node_editor.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5865 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/example/save_load.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.156732 py-imgui-redux-1.0.4/third-party/imnodes/img/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)  1517285 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/img/imnodes.gif
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   114226 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/imnodes.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18234 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/imnodes.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12908 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/imnodes_internal.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      213 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/imnodes/vcpkg.json
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.156732 py-imgui-redux-1.0.4/third-party/implot/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       46 2023-03-09 01:16:57.000000 py-imgui-redux-1.0.4/third-party/implot/.git
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.156732 py-imgui-redux-1.0.4/third-party/implot/.github/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3117 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/implot/.github/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1480 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/implot/.github/example_implot.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.156732 py-imgui-redux-1.0.4/third-party/implot/.github/workflows/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3317 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/implot/.github/workflows/build.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1068 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/implot/LICENSE
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11842 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/implot/README.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3494 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/implot/TODO.md
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   264935 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/implot/implot.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    78669 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/implot/implot.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   111935 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/implot/implot_demo.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    67176 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/implot/implot_internal.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   118754 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/implot/implot_items.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.156732 py-imgui-redux-1.0.4/third-party/pybind11/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1271 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.appveyor.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      996 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.clang-format
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2605 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.clang-tidy
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2196 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.cmake-format.yaml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1308 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.codespell-ignore-lines
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       48 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.git
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       18 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.gitattributes
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.156732 py-imgui-redux-1.0.4/third-party/pybind11/.github/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      182 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.github/CODEOWNERS
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15271 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.github/CONTRIBUTING.md
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.156732 py-imgui-redux-1.0.4/third-party/pybind11/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2561 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      328 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      162 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.github/dependabot.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      116 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.github/labeler.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       50 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.github/labeler_merged.yml
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.156732 py-imgui-redux-1.0.4/third-party/pybind11/.github/matchers/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      668 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.github/matchers/pylint.json
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      645 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.github/pull_request_template.md
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.156732 py-imgui-redux-1.0.4/third-party/pybind11/.github/workflows/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    31868 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.github/workflows/ci.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2127 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.github/workflows/configure.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1447 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.github/workflows/format.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      559 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.github/workflows/labeler.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2558 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.github/workflows/pip.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2865 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.github/workflows/upstream.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      502 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.gitignore
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4332 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       62 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/.readthedocs.yml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11983 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1684 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/LICENSE
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      223 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/MANIFEST.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7686 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/README.rst
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.160065 py-imgui-redux-1.0.4/third-party/pybind11/docs/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      607 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/Doxyfile
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7417 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/Makefile
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.136732 py-imgui-redux-1.0.4/third-party/pybind11/docs/_static/
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.160065 py-imgui-redux-1.0.4/third-party/pybind11/docs/_static/css/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       37 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/_static/css/custom.css
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.160065 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.160065 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/cast/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3937 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/cast/chrono.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3429 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/cast/custom.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14283 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/cast/eigen.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3889 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/cast/functional.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1556 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/cast/index.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12371 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/cast/overview.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9586 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/cast/stl.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8863 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/cast/strings.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    47796 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/classes.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8453 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/embedding.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17796 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/exceptions.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    26729 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/functions.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15651 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/misc.rst
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.160065 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/pycpp/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      278 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/pycpp/index.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17161 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9030 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/pycpp/object.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5710 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6377 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9240 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/basics.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2856 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/benchmark.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3168 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/benchmark.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   114174 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/changelog.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16380 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/classes.rst
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.160065 py-imgui-redux-1.0.4/third-party/pybind11/docs/cmake/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      273 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/cmake/index.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    25777 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/compiling.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11559 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/conf.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13177 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/faq.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      613 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/index.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3277 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/installing.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3079 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/limitations.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    61034 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/pybind11-logo.png
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    44653 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    87708 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    41121 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    85853 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2647 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/reference.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4414 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/release.rst
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      149 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/requirements.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    23489 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/docs/upgrade.rst
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.136732 py-imgui-redux-1.0.4/third-party/pybind11/include/
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.160065 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    23959 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7069 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    65660 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8458 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      120 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/common.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2096 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.160065 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/detail/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    28251 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    52929 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5491 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17869 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    26305 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    42613 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1625 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.160065 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    31418 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18108 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      316 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13471 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4731 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5002 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8262 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8862 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    79408 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9103 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2734 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/options.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)   126420 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    94641 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.160065 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/stl/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4185 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    15337 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    29747 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2765 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/noxfile.py
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.160065 py-imgui-redux-1.0.4/third-party/pybind11/pybind11/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      414 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/pybind11/__init__.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1360 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/pybind11/__main__.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      228 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/pybind11/_version.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1226 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/pybind11/commands.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)        0 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/pybind11/py.typed
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17609 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1261 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/pyproject.toml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1618 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/setup.cfg
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4877 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/setup.py
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.163398 py-imgui-redux-1.0.4/third-party/pybind11/tests/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21675 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5741 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/conftest.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11736 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/constructor_stats.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3578 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1776 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/cross_module_interleaved_error_already_set.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      396 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      940 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/env.py
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.163398 py-imgui-redux-1.0.4/third-party/pybind11/tests/extra_python_package/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)        0 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/extra_python_package/pytest.ini
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8296 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/extra_python_package/test_files.py
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.163398 py-imgui-redux-1.0.4/third-party/pybind11/tests/extra_setuptools/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)        0 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4153 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2847 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/local_bindings.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5743 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/object.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6264 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4517 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/pybind11_tests.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2685 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      768 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/pytest.ini
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      600 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/requirements.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      855 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_async.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      534 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_async.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8567 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_buffers.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4841 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_buffers.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16025 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_builtin_casters.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    17245 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4118 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_call_policies.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6549 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_call_policies.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10858 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_callbacks.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6246 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_callbacks.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3370 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_chrono.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5695 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_chrono.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    24874 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_class.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14815 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_class.py
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.163398 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2639 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      673 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/embed.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.163398 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1171 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.163398 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1293 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.163398 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1685 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      152 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/main.cpp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.163398 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1353 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.163398 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1163 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.163398 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1368 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      198 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3831 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_const_name.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      589 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_const_name.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5615 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_constants_and_functions.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1498 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10886 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_copy_move.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4796 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_copy_move.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7280 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_custom_type_casters.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3980 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1259 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_custom_type_setup.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1089 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_custom_type_setup.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4557 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_docstring_options.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2423 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19350 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_eigen_matrix.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    28867 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_eigen_matrix.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      473 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_eigen_tensor.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    10590 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_eigen_tensor.inl
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9456 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_eigen_tensor.py
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.163398 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_embed/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1798 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1315 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_embed/catch.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      543 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_embed/external_module.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16535 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      237 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      275 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_embed/test_trampoline.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5722 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_enum.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8903 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_enum.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3168 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_eval.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1143 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_eval.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      119 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_eval_call.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11904 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_exceptions.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      399 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_exceptions.h
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12774 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_exceptions.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18155 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_factory_constructors.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    16519 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     5311 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_gil_scoped.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8540 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3960 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_iostream.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     7286 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_iostream.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9444 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    13757 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4401 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_local_bindings.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8049 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21388 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18134 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4121 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_modules.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4191 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_modules.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12305 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11874 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    19861 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_numpy_array.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    20356 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21114 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14394 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4487 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9686 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2777 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_opaque_types.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1847 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9132 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_operator_overloading.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4333 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6719 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_pickling.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2720 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_pickling.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    30750 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_pytypes.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    23630 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_pytypes.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21153 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8021 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    18898 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_smart_ptr.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9530 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    21587 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_stl.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12235 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_stl.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4622 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_stl_binders.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     9174 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     4617 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      741 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1855 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_thread.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      826 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_thread.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      603 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_union.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      148 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_union.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    22991 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_virtual_functions.cpp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    12919 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/test_virtual_functions.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3226 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2657 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tests/valgrind-python.supp
+drwxr-xr-x   0 alagyn    (1000) alagyn    (1000)        0 2023-07-14 18:08:56.166732 py-imgui-redux-1.0.4/third-party/pybind11/tools/
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2350 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     3105 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    11190 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      817 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 alagyn    (1000) alagyn    (1000)     1423 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tools/check-style.sh
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      952 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1040 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1031 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tools/libsize.py
+-rwxr-xr-x   0 alagyn    (1000) alagyn    (1000)     1311 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tools/make_changelog.py
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)      196 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)    14033 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     6930 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8960 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     8361 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)       94 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tools/pyproject.toml
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     2104 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 alagyn    (1000) alagyn    (1000)     1234 2023-03-09 01:16:58.000000 py-imgui-redux-1.0.4/third-party/pybind11/tools/setup_main.py.in
```

### Comparing `py-imgui-redux-1.0.3/LICENSE` & `py-imgui-redux-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/PKG-INFO` & `py-imgui-redux-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-imgui-redux
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python wrapper for DearImGUI and popular extensions
 Author: Alagyn
 Project-URL: Homepage, https://github.com/alagyn/PyImGui-Redux
 Project-URL: Bug Tracker, https://github.com/alagyn/PyImGui-Redux/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `py-imgui-redux-1.0.3/README.md` & `py-imgui-redux-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/imgui/__init__.pyi` & `py-imgui-redux-1.0.4/imgui/__init__.pyi`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/imgui/glfw/__init__.pyi` & `py-imgui-redux-1.0.4/imgui/glfw/__init__.pyi`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/imgui/imnodes/__init__.pyi` & `py-imgui-redux-1.0.4/imgui/imnodes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/imgui/implot/__init__.pyi` & `py-imgui-redux-1.0.4/imgui/implot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/py_imgui_redux.egg-info/PKG-INFO` & `py-imgui-redux-1.0.4/py_imgui_redux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-imgui-redux
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python wrapper for DearImGUI and popular extensions
 Author: Alagyn
 Project-URL: Homepage, https://github.com/alagyn/PyImGui-Redux
 Project-URL: Bug Tracker, https://github.com/alagyn/PyImGui-Redux/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `py-imgui-redux-1.0.3/py_imgui_redux.egg-info/SOURCES.txt` & `py-imgui-redux-1.0.4/py_imgui_redux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/pyproject.toml` & `py-imgui-redux-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel",
     "cmake>=3.25"
     ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-imgui-redux"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     {name="Alagyn"}
 ]
 description = "A python wrapper for DearImGUI and popular extensions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `py-imgui-redux-1.0.3/setup.py` & `py-imgui-redux-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/.appveyor.yml` & `py-imgui-redux-1.0.4/third-party/glfw/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/.github/workflows/build.yml` & `py-imgui-redux-1.0.4/third-party/glfw/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/.gitignore` & `py-imgui-redux-1.0.4/third-party/glfw/.gitignore`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/CMake/GenerateMappings.cmake` & `py-imgui-redux-1.0.4/third-party/glfw/CMake/GenerateMappings.cmake`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/CMake/MacOSXBundleInfo.plist.in` & `py-imgui-redux-1.0.4/third-party/glfw/CMake/MacOSXBundleInfo.plist.in`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/CMake/i686-w64-mingw32-clang.cmake` & `py-imgui-redux-1.0.4/third-party/glfw/CMake/i686-w64-mingw32-clang.cmake`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/CMake/i686-w64-mingw32.cmake` & `py-imgui-redux-1.0.4/third-party/glfw/CMake/i686-w64-mingw32.cmake`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/CMake/modules/FindEpollShim.cmake` & `py-imgui-redux-1.0.4/third-party/glfw/CMake/modules/FindEpollShim.cmake`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/CMake/modules/FindWaylandProtocols.cmake` & `py-imgui-redux-1.0.4/third-party/glfw/CMake/modules/FindWaylandProtocols.cmake`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/CMake/modules/FindXKBCommon.cmake` & `py-imgui-redux-1.0.4/third-party/glfw/CMake/modules/FindXKBCommon.cmake`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/CMake/x86_64-w64-mingw32-clang.cmake` & `py-imgui-redux-1.0.4/third-party/glfw/CMake/x86_64-w64-mingw32-clang.cmake`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/CMake/x86_64-w64-mingw32.cmake` & `py-imgui-redux-1.0.4/third-party/glfw/CMake/x86_64-w64-mingw32.cmake`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/glfw/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/CONTRIBUTORS.md` & `py-imgui-redux-1.0.4/third-party/glfw/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/LICENSE.md` & `py-imgui-redux-1.0.4/third-party/glfw/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/README.md` & `py-imgui-redux-1.0.4/third-party/glfw/README.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/cmake_uninstall.cmake.in` & `py-imgui-redux-1.0.4/third-party/glfw/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/deps/getopt.c` & `py-imgui-redux-1.0.4/third-party/glfw/deps/getopt.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/deps/getopt.h` & `py-imgui-redux-1.0.4/third-party/glfw/deps/getopt.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/deps/glad/gl.h` & `py-imgui-redux-1.0.4/third-party/glfw/deps/glad/gl.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/deps/glad/khrplatform.h` & `py-imgui-redux-1.0.4/third-party/glfw/deps/glad/khrplatform.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/deps/glad/vk_platform.h` & `py-imgui-redux-1.0.4/third-party/glfw/deps/glad/vk_platform.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/deps/glad/vulkan.h` & `py-imgui-redux-1.0.4/third-party/glfw/deps/glad/vulkan.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/deps/glad_gl.c` & `py-imgui-redux-1.0.4/third-party/glfw/deps/glad_gl.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/deps/glad_vulkan.c` & `py-imgui-redux-1.0.4/third-party/glfw/deps/glad_vulkan.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/deps/linmath.h` & `py-imgui-redux-1.0.4/third-party/glfw/deps/linmath.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/deps/mingw/_mingw_dxhelper.h` & `py-imgui-redux-1.0.4/third-party/glfw/deps/mingw/_mingw_dxhelper.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/deps/mingw/dinput.h` & `py-imgui-redux-1.0.4/third-party/glfw/deps/mingw/dinput.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/deps/mingw/xinput.h` & `py-imgui-redux-1.0.4/third-party/glfw/deps/mingw/xinput.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/deps/nuklear.h` & `py-imgui-redux-1.0.4/third-party/glfw/deps/nuklear.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/deps/nuklear_glfw_gl2.h` & `py-imgui-redux-1.0.4/third-party/glfw/deps/nuklear_glfw_gl2.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/deps/stb_image_write.h` & `py-imgui-redux-1.0.4/third-party/glfw/deps/stb_image_write.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/deps/tinycthread.c` & `py-imgui-redux-1.0.4/third-party/glfw/deps/tinycthread.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/deps/tinycthread.h` & `py-imgui-redux-1.0.4/third-party/glfw/deps/tinycthread.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/deps/vs2008/stdint.h` & `py-imgui-redux-1.0.4/third-party/glfw/deps/vs2008/stdint.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/glfw/docs/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/CONTRIBUTING.md` & `py-imgui-redux-1.0.4/third-party/glfw/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/Doxyfile.in` & `py-imgui-redux-1.0.4/third-party/glfw/docs/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/DoxygenLayout.xml` & `py-imgui-redux-1.0.4/third-party/glfw/docs/DoxygenLayout.xml`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/SUPPORT.md` & `py-imgui-redux-1.0.4/third-party/glfw/docs/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/build.dox` & `py-imgui-redux-1.0.4/third-party/glfw/docs/build.dox`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/compat.dox` & `py-imgui-redux-1.0.4/third-party/glfw/docs/compat.dox`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/compile.dox` & `py-imgui-redux-1.0.4/third-party/glfw/docs/compile.dox`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/context.dox` & `py-imgui-redux-1.0.4/third-party/glfw/docs/context.dox`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/extra.css` & `py-imgui-redux-1.0.4/third-party/glfw/docs/extra.css`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/extra.css.map` & `py-imgui-redux-1.0.4/third-party/glfw/docs/extra.css.map`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/extra.scss` & `py-imgui-redux-1.0.4/third-party/glfw/docs/extra.scss`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/header.html` & `py-imgui-redux-1.0.4/third-party/glfw/docs/header.html`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/input.dox` & `py-imgui-redux-1.0.4/third-party/glfw/docs/input.dox`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/internal.dox` & `py-imgui-redux-1.0.4/third-party/glfw/docs/internal.dox`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/intro.dox` & `py-imgui-redux-1.0.4/third-party/glfw/docs/intro.dox`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/main.dox` & `py-imgui-redux-1.0.4/third-party/glfw/docs/main.dox`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/monitor.dox` & `py-imgui-redux-1.0.4/third-party/glfw/docs/monitor.dox`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/moving.dox` & `py-imgui-redux-1.0.4/third-party/glfw/docs/moving.dox`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/news.dox` & `py-imgui-redux-1.0.4/third-party/glfw/docs/news.dox`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/quick.dox` & `py-imgui-redux-1.0.4/third-party/glfw/docs/quick.dox`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/spaces.svg` & `py-imgui-redux-1.0.4/third-party/glfw/docs/spaces.svg`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/vulkan.dox` & `py-imgui-redux-1.0.4/third-party/glfw/docs/vulkan.dox`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/docs/window.dox` & `py-imgui-redux-1.0.4/third-party/glfw/docs/window.dox`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/examples/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/glfw/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/examples/boing.c` & `py-imgui-redux-1.0.4/third-party/glfw/examples/boing.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/examples/gears.c` & `py-imgui-redux-1.0.4/third-party/glfw/examples/gears.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/examples/glfw.icns` & `py-imgui-redux-1.0.4/third-party/glfw/examples/glfw.icns`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/examples/glfw.ico` & `py-imgui-redux-1.0.4/third-party/glfw/examples/glfw.ico`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/examples/heightmap.c` & `py-imgui-redux-1.0.4/third-party/glfw/examples/heightmap.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/examples/offscreen.c` & `py-imgui-redux-1.0.4/third-party/glfw/examples/offscreen.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/examples/particles.c` & `py-imgui-redux-1.0.4/third-party/glfw/examples/particles.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/examples/sharing.c` & `py-imgui-redux-1.0.4/third-party/glfw/examples/sharing.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/examples/simple.c` & `py-imgui-redux-1.0.4/third-party/glfw/examples/simple.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/examples/splitview.c` & `py-imgui-redux-1.0.4/third-party/glfw/examples/splitview.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/examples/wave.c` & `py-imgui-redux-1.0.4/third-party/glfw/examples/wave.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/include/GLFW/glfw3.h` & `py-imgui-redux-1.0.4/third-party/glfw/include/GLFW/glfw3.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/include/GLFW/glfw3native.h` & `py-imgui-redux-1.0.4/third-party/glfw/include/GLFW/glfw3native.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/glfw/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/cocoa_init.m` & `py-imgui-redux-1.0.4/third-party/glfw/src/cocoa_init.m`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/cocoa_joystick.h` & `py-imgui-redux-1.0.4/third-party/glfw/src/cocoa_joystick.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/cocoa_joystick.m` & `py-imgui-redux-1.0.4/third-party/glfw/src/cocoa_joystick.m`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/cocoa_monitor.m` & `py-imgui-redux-1.0.4/third-party/glfw/src/cocoa_monitor.m`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/cocoa_platform.h` & `py-imgui-redux-1.0.4/third-party/glfw/src/cocoa_platform.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/cocoa_time.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/cocoa_time.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/cocoa_window.m` & `py-imgui-redux-1.0.4/third-party/glfw/src/cocoa_window.m`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/context.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/context.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/egl_context.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/egl_context.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/egl_context.h` & `py-imgui-redux-1.0.4/third-party/glfw/src/egl_context.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/glfw_config.h.in` & `py-imgui-redux-1.0.4/third-party/glfw/src/glfw_config.h.in`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/glx_context.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/glx_context.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/glx_context.h` & `py-imgui-redux-1.0.4/third-party/glfw/src/glx_context.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/init.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/init.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/input.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/input.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/internal.h` & `py-imgui-redux-1.0.4/third-party/glfw/src/internal.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/linux_joystick.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/linux_joystick.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/linux_joystick.h` & `py-imgui-redux-1.0.4/third-party/glfw/src/linux_joystick.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/mappings.h` & `py-imgui-redux-1.0.4/third-party/glfw/src/mappings.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/mappings.h.in` & `py-imgui-redux-1.0.4/third-party/glfw/src/mappings.h.in`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/monitor.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/monitor.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/nsgl_context.h` & `py-imgui-redux-1.0.4/third-party/glfw/src/nsgl_context.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/nsgl_context.m` & `py-imgui-redux-1.0.4/third-party/glfw/src/nsgl_context.m`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/null_init.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/null_init.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/null_joystick.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/null_joystick.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/null_joystick.h` & `py-imgui-redux-1.0.4/third-party/glfw/src/null_joystick.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/null_monitor.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/null_monitor.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/null_platform.h` & `py-imgui-redux-1.0.4/third-party/glfw/src/null_platform.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/null_window.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/null_window.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/osmesa_context.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/osmesa_context.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/osmesa_context.h` & `py-imgui-redux-1.0.4/third-party/glfw/src/osmesa_context.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/posix_thread.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/posix_thread.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/posix_thread.h` & `py-imgui-redux-1.0.4/third-party/glfw/src/posix_thread.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/posix_time.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/posix_time.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/posix_time.h` & `py-imgui-redux-1.0.4/third-party/glfw/src/posix_time.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/vulkan.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/vulkan.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/wgl_context.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/wgl_context.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/wgl_context.h` & `py-imgui-redux-1.0.4/third-party/glfw/src/wgl_context.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/win32_init.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/win32_init.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/win32_joystick.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/win32_joystick.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/win32_joystick.h` & `py-imgui-redux-1.0.4/third-party/glfw/src/win32_joystick.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/win32_monitor.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/win32_monitor.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/win32_platform.h` & `py-imgui-redux-1.0.4/third-party/glfw/src/win32_platform.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/win32_thread.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/win32_thread.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/win32_time.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/win32_time.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/win32_window.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/win32_window.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/window.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/window.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/wl_init.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/wl_init.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/wl_monitor.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/wl_monitor.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/wl_platform.h` & `py-imgui-redux-1.0.4/third-party/glfw/src/wl_platform.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/wl_window.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/wl_window.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/x11_init.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/x11_init.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/x11_monitor.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/x11_monitor.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/x11_platform.h` & `py-imgui-redux-1.0.4/third-party/glfw/src/x11_platform.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/x11_window.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/x11_window.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/xkb_unicode.c` & `py-imgui-redux-1.0.4/third-party/glfw/src/xkb_unicode.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/src/xkb_unicode.h` & `py-imgui-redux-1.0.4/third-party/glfw/src/xkb_unicode.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/glfw/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/clipboard.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/clipboard.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/cursor.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/cursor.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/empty.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/empty.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/events.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/events.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/gamma.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/gamma.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/glfwinfo.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/glfwinfo.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/icon.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/icon.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/iconify.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/iconify.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/inputlag.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/inputlag.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/joysticks.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/joysticks.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/monitors.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/monitors.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/msaa.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/msaa.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/opacity.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/opacity.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/reopen.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/reopen.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/tearing.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/tearing.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/threads.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/threads.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/timeout.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/timeout.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/title.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/title.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/triangle-vulkan.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/triangle-vulkan.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/glfw/tests/windows.c` & `py-imgui-redux-1.0.4/third-party/glfw/tests/windows.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imconfig/bind-imconfig.h` & `py-imgui-redux-1.0.4/third-party/imconfig/bind-imconfig.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/.editorconfig` & `py-imgui-redux-1.0.4/third-party/imgui/.editorconfig`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/.github/issue_template.md` & `py-imgui-redux-1.0.4/third-party/imgui/.github/issue_template.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/.github/workflows/build.yml` & `py-imgui-redux-1.0.4/third-party/imgui/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/.github/workflows/static-analysis.yml` & `py-imgui-redux-1.0.4/third-party/imgui/.github/workflows/static-analysis.yml`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/.gitignore` & `py-imgui-redux-1.0.4/third-party/imgui/.gitignore`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/LICENSE.txt` & `py-imgui-redux-1.0.4/third-party/imgui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_allegro5.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_allegro5.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_allegro5.h` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_allegro5.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_android.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_android.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_android.h` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_android.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_dx10.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_dx10.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_dx10.h` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_dx10.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_dx11.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_dx11.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_dx11.h` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_dx11.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_dx12.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_dx12.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_dx12.h` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_dx12.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_dx9.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_dx9.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_dx9.h` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_dx9.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_glfw.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_glfw.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_glfw.h` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_glfw.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_glut.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_glut.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_glut.h` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_glut.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_metal.h` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_metal.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_metal.mm` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_metal.mm`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_opengl2.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_opengl2.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_opengl2.h` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_opengl2.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_opengl3.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_opengl3.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_opengl3.h` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_opengl3.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_opengl3_loader.h` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_opengl3_loader.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_osx.h` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_osx.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_osx.mm` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_osx.mm`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_sdl.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_sdl.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_sdl.h` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_sdl.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_sdlrenderer.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_sdlrenderer.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_sdlrenderer.h` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_sdlrenderer.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_vulkan.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_vulkan.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_vulkan.h` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_vulkan.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_wgpu.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_wgpu.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_wgpu.h` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_wgpu.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_win32.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_win32.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/backends/imgui_impl_win32.h` & `py-imgui-redux-1.0.4/third-party/imgui/backends/imgui_impl_win32.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/docs/BACKENDS.md` & `py-imgui-redux-1.0.4/third-party/imgui/docs/BACKENDS.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/docs/CHANGELOG.txt` & `py-imgui-redux-1.0.4/third-party/imgui/docs/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/docs/CONTRIBUTING.md` & `py-imgui-redux-1.0.4/third-party/imgui/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/docs/EXAMPLES.md` & `py-imgui-redux-1.0.4/third-party/imgui/docs/EXAMPLES.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/docs/FAQ.md` & `py-imgui-redux-1.0.4/third-party/imgui/docs/FAQ.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/docs/FONTS.md` & `py-imgui-redux-1.0.4/third-party/imgui/docs/FONTS.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/docs/README.md` & `py-imgui-redux-1.0.4/third-party/imgui/docs/README.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/docs/TODO.txt` & `py-imgui-redux-1.0.4/third-party/imgui/docs/TODO.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/README.txt` & `py-imgui-redux-1.0.4/third-party/imgui/examples/README.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_allegro5/README.md` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_allegro5/README.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_allegro5/example_allegro5.vcxproj` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_allegro5/example_allegro5.vcxproj`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_allegro5/example_allegro5.vcxproj.filters` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_allegro5/example_allegro5.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_allegro5/imconfig_allegro5.h` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_allegro5/imconfig_allegro5.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_allegro5/main.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_allegro5/main.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_android_opengl3/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_android_opengl3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_android_opengl3/android/app/build.gradle` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_android_opengl3/android/app/build.gradle`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_android_opengl3/android/app/src/main/AndroidManifest.xml` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_android_opengl3/android/app/src/main/AndroidManifest.xml`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_android_opengl3/android/app/src/main/java/MainActivity.kt` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_android_opengl3/android/app/src/main/java/MainActivity.kt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_android_opengl3/main.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_android_opengl3/main.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_metal/example_apple_metal.xcodeproj/project.pbxproj` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_metal/example_apple_metal.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_metal/iOS/Info-iOS.plist` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_metal/iOS/Info-iOS.plist`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_metal/iOS/LaunchScreen.storyboard` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_metal/iOS/LaunchScreen.storyboard`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_metal/macOS/Info-macOS.plist` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_metal/macOS/Info-macOS.plist`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_metal/macOS/MainMenu.storyboard` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_metal/macOS/MainMenu.storyboard`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_metal/main.mm` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_metal/main.mm`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_opengl2/example_apple_opengl2.xcodeproj/project.pbxproj` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_opengl2/example_apple_opengl2.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_apple_opengl2/main.mm` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_apple_opengl2/main.mm`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_emscripten_opengl3/Makefile` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_emscripten_opengl3/Makefile`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_emscripten_opengl3/README.md` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_emscripten_opengl3/README.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_emscripten_opengl3/main.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_emscripten_opengl3/main.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_emscripten_opengl3/shell_minimal.html` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_emscripten_opengl3/shell_minimal.html`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_emscripten_wgpu/Makefile` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_emscripten_wgpu/Makefile`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_emscripten_wgpu/README.md` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_emscripten_wgpu/README.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_emscripten_wgpu/main.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_emscripten_wgpu/main.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_emscripten_wgpu/web/index.html` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_emscripten_wgpu/web/index.html`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_metal/Makefile` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_metal/Makefile`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_metal/main.mm` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_metal/main.mm`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl2/Makefile` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl2/Makefile`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl2/build_win32.bat` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl2/build_win32.bat`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl2/example_glfw_opengl2.vcxproj` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl2/example_glfw_opengl2.vcxproj`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl2/example_glfw_opengl2.vcxproj.filters` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl2/example_glfw_opengl2.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl2/main.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl2/main.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl3/Makefile` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl3/Makefile`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl3/build_win32.bat` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl3/build_win32.bat`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl3/example_glfw_opengl3.vcxproj` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl3/example_glfw_opengl3.vcxproj`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl3/example_glfw_opengl3.vcxproj.filters` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl3/example_glfw_opengl3.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_opengl3/main.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_opengl3/main.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_vulkan/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_vulkan/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_vulkan/build_win32.bat` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_vulkan/build_win32.bat`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_vulkan/build_win64.bat` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_vulkan/build_win64.bat`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_vulkan/example_glfw_vulkan.vcxproj` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_vulkan/example_glfw_vulkan.vcxproj`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_vulkan/example_glfw_vulkan.vcxproj.filters` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_vulkan/example_glfw_vulkan.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glfw_vulkan/main.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glfw_vulkan/main.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glut_opengl2/Makefile` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glut_opengl2/Makefile`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glut_opengl2/example_glut_opengl2.vcxproj` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glut_opengl2/example_glut_opengl2.vcxproj`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glut_opengl2/example_glut_opengl2.vcxproj.filters` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glut_opengl2/example_glut_opengl2.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_glut_opengl2/main.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_glut_opengl2/main.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_null/Makefile` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_null/Makefile`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_null/main.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_null/main.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_directx11/build_win32.bat` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_directx11/build_win32.bat`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_directx11/example_sdl_directx11.vcxproj` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_directx11/example_sdl_directx11.vcxproj`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_directx11/example_sdl_directx11.vcxproj.filters` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_directx11/example_sdl_directx11.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_directx11/main.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_directx11/main.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_metal/Makefile` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_metal/Makefile`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_metal/main.mm` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_metal/main.mm`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl2/Makefile` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl2/Makefile`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl2/README.md` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl2/README.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl2/build_win32.bat` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl2/build_win32.bat`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl2/example_sdl_opengl2.vcxproj` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl2/example_sdl_opengl2.vcxproj`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl2/example_sdl_opengl2.vcxproj.filters` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl2/example_sdl_opengl2.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl2/main.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl2/main.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl3/Makefile` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl3/Makefile`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl3/README.md` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl3/README.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl3/build_win32.bat` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl3/build_win32.bat`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl3/example_sdl_opengl3.vcxproj` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl3/example_sdl_opengl3.vcxproj`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl3/example_sdl_opengl3.vcxproj.filters` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl3/example_sdl_opengl3.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_opengl3/main.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_opengl3/main.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_sdlrenderer/Makefile` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_sdlrenderer/Makefile`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_sdlrenderer/README.md` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_sdlrenderer/README.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_sdlrenderer/build_win32.bat` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_sdlrenderer/build_win32.bat`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_sdlrenderer/example_sdl_sdlrenderer.vcxproj` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_sdlrenderer/example_sdl_sdlrenderer.vcxproj`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_sdlrenderer/example_sdl_sdlrenderer.vcxproj.filters` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_sdlrenderer/example_sdl_sdlrenderer.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_sdlrenderer/main.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_sdlrenderer/main.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_vulkan/build_win32.bat` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_vulkan/build_win32.bat`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_vulkan/example_sdl_vulkan.vcxproj` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_vulkan/example_sdl_vulkan.vcxproj`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_vulkan/example_sdl_vulkan.vcxproj.filters` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_vulkan/example_sdl_vulkan.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_sdl_vulkan/main.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_sdl_vulkan/main.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx10/build_win32.bat` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx10/build_win32.bat`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx10/example_win32_directx10.vcxproj` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx10/example_win32_directx10.vcxproj`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx10/example_win32_directx10.vcxproj.filters` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx10/example_win32_directx10.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx10/main.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx10/main.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx11/build_win32.bat` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx11/build_win32.bat`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx11/example_win32_directx11.vcxproj` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx11/example_win32_directx11.vcxproj`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx11/example_win32_directx11.vcxproj.filters` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx11/example_win32_directx11.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx11/main.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx11/main.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx12/build_win32.bat` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx12/build_win32.bat`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx12/example_win32_directx12.vcxproj` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx12/example_win32_directx12.vcxproj`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx12/example_win32_directx12.vcxproj.filters` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx12/example_win32_directx12.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx12/main.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx12/main.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx9/build_win32.bat` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx9/build_win32.bat`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx9/example_win32_directx9.vcxproj` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx9/example_win32_directx9.vcxproj`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx9/example_win32_directx9.vcxproj.filters` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx9/example_win32_directx9.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/example_win32_directx9/main.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/examples/example_win32_directx9/main.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/imgui_examples.sln` & `py-imgui-redux-1.0.4/third-party/imgui/examples/imgui_examples.sln`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/libs/glfw/COPYING.txt` & `py-imgui-redux-1.0.4/third-party/imgui/examples/libs/glfw/COPYING.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/libs/glfw/include/GLFW/glfw3.h` & `py-imgui-redux-1.0.4/third-party/imgui/examples/libs/glfw/include/GLFW/glfw3.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/libs/glfw/include/GLFW/glfw3native.h` & `py-imgui-redux-1.0.4/third-party/imgui/examples/libs/glfw/include/GLFW/glfw3native.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/libs/glfw/lib-vc2010-32/glfw3.lib` & `py-imgui-redux-1.0.4/third-party/imgui/examples/libs/glfw/lib-vc2010-32/glfw3.lib`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/libs/glfw/lib-vc2010-64/glfw3.lib` & `py-imgui-redux-1.0.4/third-party/imgui/examples/libs/glfw/lib-vc2010-64/glfw3.lib`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/libs/usynergy/uSynergy.c` & `py-imgui-redux-1.0.4/third-party/imgui/examples/libs/usynergy/uSynergy.c`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/examples/libs/usynergy/uSynergy.h` & `py-imgui-redux-1.0.4/third-party/imgui/examples/libs/usynergy/uSynergy.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/imconfig.h` & `py-imgui-redux-1.0.4/third-party/imgui/imconfig.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/imgui.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/imgui.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/imgui.h` & `py-imgui-redux-1.0.4/third-party/imgui/imgui.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/imgui_demo.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/imgui_demo.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/imgui_draw.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/imgui_draw.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/imgui_internal.h` & `py-imgui-redux-1.0.4/third-party/imgui/imgui_internal.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/imgui_tables.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/imgui_tables.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/imgui_widgets.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/imgui_widgets.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/imstb_rectpack.h` & `py-imgui-redux-1.0.4/third-party/imgui/imstb_rectpack.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/imstb_textedit.h` & `py-imgui-redux-1.0.4/third-party/imgui/imstb_textedit.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/imstb_truetype.h` & `py-imgui-redux-1.0.4/third-party/imgui/imstb_truetype.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/misc/README.txt` & `py-imgui-redux-1.0.4/third-party/imgui/misc/README.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/misc/cpp/README.txt` & `py-imgui-redux-1.0.4/third-party/imgui/misc/cpp/README.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/misc/cpp/imgui_stdlib.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/misc/cpp/imgui_stdlib.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/misc/cpp/imgui_stdlib.h` & `py-imgui-redux-1.0.4/third-party/imgui/misc/cpp/imgui_stdlib.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/misc/debuggers/imgui.gdb` & `py-imgui-redux-1.0.4/third-party/imgui/misc/debuggers/imgui.gdb`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/misc/debuggers/imgui.natstepfilter` & `py-imgui-redux-1.0.4/third-party/imgui/misc/debuggers/imgui.natstepfilter`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/misc/debuggers/imgui.natvis` & `py-imgui-redux-1.0.4/third-party/imgui/misc/debuggers/imgui.natvis`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/misc/fonts/Cousine-Regular.ttf` & `py-imgui-redux-1.0.4/third-party/imgui/misc/fonts/Cousine-Regular.ttf`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/misc/fonts/DroidSans.ttf` & `py-imgui-redux-1.0.4/third-party/imgui/misc/fonts/DroidSans.ttf`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/misc/fonts/Karla-Regular.ttf` & `py-imgui-redux-1.0.4/third-party/imgui/misc/fonts/Karla-Regular.ttf`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/misc/fonts/ProggyClean.ttf` & `py-imgui-redux-1.0.4/third-party/imgui/misc/fonts/ProggyClean.ttf`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/misc/fonts/ProggyTiny.ttf` & `py-imgui-redux-1.0.4/third-party/imgui/misc/fonts/ProggyTiny.ttf`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/misc/fonts/Roboto-Medium.ttf` & `py-imgui-redux-1.0.4/third-party/imgui/misc/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/misc/fonts/binary_to_compressed_c.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/misc/fonts/binary_to_compressed_c.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/misc/freetype/README.md` & `py-imgui-redux-1.0.4/third-party/imgui/misc/freetype/README.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/misc/freetype/imgui_freetype.cpp` & `py-imgui-redux-1.0.4/third-party/imgui/misc/freetype/imgui_freetype.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/misc/freetype/imgui_freetype.h` & `py-imgui-redux-1.0.4/third-party/imgui/misc/freetype/imgui_freetype.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imgui/misc/single_file/imgui_single_file.h` & `py-imgui-redux-1.0.4/third-party/imgui/misc/single_file/imgui_single_file.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imnodes/.clang-format` & `py-imgui-redux-1.0.4/third-party/imnodes/.clang-format`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imnodes/.clang-tidy` & `py-imgui-redux-1.0.4/third-party/imnodes/.clang-tidy`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imnodes/.github/workflows/build.yaml` & `py-imgui-redux-1.0.4/third-party/imnodes/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imnodes/.gitignore` & `py-imgui-redux-1.0.4/third-party/imnodes/.gitignore`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imnodes/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/imnodes/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imnodes/LICENSE.md` & `py-imgui-redux-1.0.4/third-party/imnodes/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imnodes/README.md` & `py-imgui-redux-1.0.4/third-party/imnodes/README.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imnodes/example/color_node_editor.cpp` & `py-imgui-redux-1.0.4/third-party/imnodes/example/color_node_editor.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imnodes/example/graph.h` & `py-imgui-redux-1.0.4/third-party/imnodes/example/graph.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imnodes/example/hello.cpp` & `py-imgui-redux-1.0.4/third-party/imnodes/example/hello.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imnodes/example/main.cpp` & `py-imgui-redux-1.0.4/third-party/imnodes/example/main.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imnodes/example/multi_editor.cpp` & `py-imgui-redux-1.0.4/third-party/imnodes/example/multi_editor.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imnodes/example/save_load.cpp` & `py-imgui-redux-1.0.4/third-party/imnodes/example/save_load.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imnodes/img/imnodes.gif` & `py-imgui-redux-1.0.4/third-party/imnodes/img/imnodes.gif`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imnodes/imnodes.cpp` & `py-imgui-redux-1.0.4/third-party/imnodes/imnodes.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imnodes/imnodes.h` & `py-imgui-redux-1.0.4/third-party/imnodes/imnodes.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/imnodes/imnodes_internal.h` & `py-imgui-redux-1.0.4/third-party/imnodes/imnodes_internal.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/implot/.github/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/implot/.github/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/implot/.github/example_implot.cpp` & `py-imgui-redux-1.0.4/third-party/implot/.github/example_implot.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/implot/.github/workflows/build.yml` & `py-imgui-redux-1.0.4/third-party/implot/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/implot/LICENSE` & `py-imgui-redux-1.0.4/third-party/implot/LICENSE`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/implot/README.md` & `py-imgui-redux-1.0.4/third-party/implot/README.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/implot/TODO.md` & `py-imgui-redux-1.0.4/third-party/implot/TODO.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/implot/implot.cpp` & `py-imgui-redux-1.0.4/third-party/implot/implot.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/implot/implot.h` & `py-imgui-redux-1.0.4/third-party/implot/implot.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/implot/implot_demo.cpp` & `py-imgui-redux-1.0.4/third-party/implot/implot_demo.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/implot/implot_internal.h` & `py-imgui-redux-1.0.4/third-party/implot/implot_internal.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/implot/implot_items.cpp` & `py-imgui-redux-1.0.4/third-party/implot/implot_items.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/.appveyor.yml` & `py-imgui-redux-1.0.4/third-party/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/.clang-format` & `py-imgui-redux-1.0.4/third-party/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/.clang-tidy` & `py-imgui-redux-1.0.4/third-party/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/.cmake-format.yaml` & `py-imgui-redux-1.0.4/third-party/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/.codespell-ignore-lines` & `py-imgui-redux-1.0.4/third-party/pybind11/.codespell-ignore-lines`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/.github/CONTRIBUTING.md` & `py-imgui-redux-1.0.4/third-party/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml` & `py-imgui-redux-1.0.4/third-party/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/.github/matchers/pylint.json` & `py-imgui-redux-1.0.4/third-party/pybind11/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/.github/pull_request_template.md` & `py-imgui-redux-1.0.4/third-party/pybind11/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/.github/workflows/ci.yml` & `py-imgui-redux-1.0.4/third-party/pybind11/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/.github/workflows/configure.yml` & `py-imgui-redux-1.0.4/third-party/pybind11/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/.github/workflows/format.yml` & `py-imgui-redux-1.0.4/third-party/pybind11/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/.github/workflows/labeler.yml` & `py-imgui-redux-1.0.4/third-party/pybind11/.github/workflows/labeler.yml`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/.github/workflows/pip.yml` & `py-imgui-redux-1.0.4/third-party/pybind11/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/.github/workflows/upstream.yml` & `py-imgui-redux-1.0.4/third-party/pybind11/.github/workflows/upstream.yml`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/.pre-commit-config.yaml` & `py-imgui-redux-1.0.4/third-party/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/LICENSE` & `py-imgui-redux-1.0.4/third-party/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/README.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/Doxyfile` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/Makefile` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/cast/chrono.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/cast/custom.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/cast/eigen.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/cast/functional.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/cast/index.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/cast/overview.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/cast/stl.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/cast/strings.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/classes.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/embedding.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/exceptions.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/functions.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/misc.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/pycpp/numpy.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/pycpp/object.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/pycpp/utilities.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/advanced/smart_ptrs.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/basics.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/benchmark.py` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/benchmark.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/changelog.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/classes.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/compiling.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/conf.py` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/faq.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/index.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/installing.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/limitations.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/pybind11-logo.png` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/pybind11_vs_boost_python1.png` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/pybind11_vs_boost_python1.svg` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/pybind11_vs_boost_python2.png` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/pybind11_vs_boost_python2.svg` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/reference.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/release.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/docs/upgrade.rst` & `py-imgui-redux-1.0.4/third-party/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/attr.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/buffer_info.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/cast.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/chrono.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/complex.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/detail/class.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/detail/common.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/detail/descr.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/detail/init.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/detail/internals.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/detail/type_caster_base.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/detail/typeid.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/eigen/matrix.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/eigen/tensor.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/embed.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/eval.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/functional.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/gil.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/iostream.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/numpy.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/operators.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/options.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/pybind11.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/pytypes.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/stl/filesystem.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/stl.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/include/pybind11/stl_bind.h` & `py-imgui-redux-1.0.4/third-party/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/noxfile.py` & `py-imgui-redux-1.0.4/third-party/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/pybind11/__main__.py` & `py-imgui-redux-1.0.4/third-party/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/pybind11/commands.py` & `py-imgui-redux-1.0.4/third-party/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/pybind11/setup_helpers.py` & `py-imgui-redux-1.0.4/third-party/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/pyproject.toml` & `py-imgui-redux-1.0.4/third-party/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/setup.cfg` & `py-imgui-redux-1.0.4/third-party/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/setup.py` & `py-imgui-redux-1.0.4/third-party/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/conftest.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/constructor_stats.h` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/cross_module_gil_utils.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/cross_module_interleaved_error_already_set.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/cross_module_interleaved_error_already_set.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/env.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/extra_python_package/test_files.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/extra_setuptools/test_setuphelper.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/local_bindings.h` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/object.h` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/pybind11_cross_module_tests.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/pybind11_tests.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/pybind11_tests.h` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/pytest.ini` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/requirements.txt` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_async.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_async.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_buffers.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_buffers.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_builtin_casters.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_builtin_casters.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_call_policies.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_call_policies.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_callbacks.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_callbacks.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_chrono.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_chrono.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_class.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_class.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/embed.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_const_name.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_const_name.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_const_name.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_const_name.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_constants_and_functions.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_constants_and_functions.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_copy_move.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_copy_move.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_custom_type_casters.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_custom_type_casters.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_custom_type_setup.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_custom_type_setup.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_custom_type_setup.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_custom_type_setup.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_docstring_options.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_docstring_options.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_eigen_matrix.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_eigen_matrix.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_eigen_matrix.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_eigen_matrix.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_eigen_tensor.inl` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_eigen_tensor.inl`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_eigen_tensor.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_eigen_tensor.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_embed/CMakeLists.txt` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_embed/catch.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_embed/external_module.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_embed/test_interpreter.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_enum.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_enum.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_eval.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_eval.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_exceptions.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_exceptions.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_factory_constructors.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_factory_constructors.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_gil_scoped.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_gil_scoped.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_iostream.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_iostream.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_kwargs_and_defaults.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_kwargs_and_defaults.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_local_bindings.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_local_bindings.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_methods_and_attributes.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_methods_and_attributes.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_modules.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_modules.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_multiple_inheritance.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_multiple_inheritance.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_numpy_array.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_numpy_array.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_numpy_dtypes.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_numpy_dtypes.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_numpy_vectorize.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_numpy_vectorize.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_opaque_types.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_opaque_types.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_operator_overloading.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_operator_overloading.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_pickling.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_pickling.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_pytypes.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_pytypes.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_sequences_and_iterators.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_sequences_and_iterators.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_smart_ptr.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_smart_ptr.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_stl.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_stl.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_stl_binders.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_stl_binders.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_tagbased_polymorphic.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_tagbased_polymorphic.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_thread.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_thread.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_thread.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_union.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_virtual_functions.cpp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/test_virtual_functions.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/valgrind-numpy-scipy.supp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tests/valgrind-python.supp` & `py-imgui-redux-1.0.4/third-party/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tools/FindCatch.cmake` & `py-imgui-redux-1.0.4/third-party/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tools/FindEigen3.cmake` & `py-imgui-redux-1.0.4/third-party/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tools/FindPythonLibsNew.cmake` & `py-imgui-redux-1.0.4/third-party/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tools/JoinPaths.cmake` & `py-imgui-redux-1.0.4/third-party/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tools/check-style.sh` & `py-imgui-redux-1.0.4/third-party/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tools/cmake_uninstall.cmake.in` & `py-imgui-redux-1.0.4/third-party/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tools/codespell_ignore_lines_from_errors.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tools/libsize.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tools/make_changelog.py` & `py-imgui-redux-1.0.4/third-party/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tools/pybind11Common.cmake` & `py-imgui-redux-1.0.4/third-party/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tools/pybind11Config.cmake.in` & `py-imgui-redux-1.0.4/third-party/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tools/pybind11NewTools.cmake` & `py-imgui-redux-1.0.4/third-party/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tools/pybind11Tools.cmake` & `py-imgui-redux-1.0.4/third-party/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tools/setup_global.py.in` & `py-imgui-redux-1.0.4/third-party/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `py-imgui-redux-1.0.3/third-party/pybind11/tools/setup_main.py.in` & `py-imgui-redux-1.0.4/third-party/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

