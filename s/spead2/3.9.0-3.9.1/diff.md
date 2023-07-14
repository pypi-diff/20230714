# Comparing `tmp/spead2-3.9.0.tar.gz` & `tmp/spead2-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spead2-3.9.0.tar", last modified: Mon Mar 28 07:57:34 2022, max compression
+gzip compressed data, was "spead2-3.9.1.tar", last modified: Thu Apr  7 10:56:27 2022, max compression
```

## Comparing `spead2-3.9.0.tar` & `spead2-3.9.1.tar`

### file list

```diff
@@ -1,278 +1,278 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.269672 spead2-3.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.249672 spead2-3.9.0/.ci/
--rwxr-xr-x   0 runner    (1001) docker     (121)      246 2022-03-28 07:56:58.000000 spead2-3.9.0/.ci/ccache-path.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      458 2022-03-28 07:56:58.000000 spead2-3.9.0/.ci/configure.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      550 2022-03-28 07:56:58.000000 spead2-3.9.0/.ci/coverage.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)       95 2022-03-28 07:56:58.000000 spead2-3.9.0/.ci/cxx-tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      545 2022-03-28 07:56:58.000000 spead2-3.9.0/.ci/install-sys-pkgs.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)       91 2022-03-28 07:56:58.000000 spead2-3.9.0/.ci/py-requirements.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      269 2022-03-28 07:56:58.000000 spead2-3.9.0/.ci/py-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-03-28 07:56:58.000000 spead2-3.9.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.245672 spead2-3.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.249672 spead2-3.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     6425 2022-03-28 07:56:58.000000 spead2-3.9.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-28 07:56:58.000000 spead2-3.9.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-03-28 07:56:58.000000 spead2-3.9.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-03-28 07:56:58.000000 spead2-3.9.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-03-28 07:56:58.000000 spead2-3.9.0/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (121)    15752 2022-03-28 07:56:58.000000 spead2-3.9.0/INSTALL
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-03-28 07:56:58.000000 spead2-3.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-03-28 07:56:58.000000 spead2-3.9.0/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (121)    28743 2022-03-28 07:57:23.000000 spead2-3.9.0/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (121)     2278 2022-03-28 07:57:34.269672 spead2-3.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-03-28 07:56:58.000000 spead2-3.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-03-28 07:56:58.000000 spead2-3.9.0/RELEASE-PROCESS
--rw-r--r--   0 runner    (1001) docker     (121)    51672 2022-03-28 07:57:22.000000 spead2-3.9.0/aclocal.m4
--rwxr-xr-x   0 runner    (1001) docker     (121)      481 2022-03-28 07:56:58.000000 spead2-3.9.0/bootstrap.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.249672 spead2-3.9.0/build-aux/
--rwxr-xr-x   0 runner    (1001) docker     (121)    23568 2022-03-28 07:57:23.000000 spead2-3.9.0/build-aux/depcomp
--rwxr-xr-x   0 runner    (1001) docker     (121)    15368 2022-03-28 07:57:23.000000 spead2-3.9.0/build-aux/install-sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     6878 2022-03-28 07:57:23.000000 spead2-3.9.0/build-aux/missing
--rwxr-xr-x   0 runner    (1001) docker     (121)     4642 2022-03-28 07:57:23.000000 spead2-3.9.0/build-aux/test-driver
--rwxr-xr-x   0 runner    (1001) docker     (121)   189637 2022-03-28 07:57:23.000000 spead2-3.9.0/configure
--rw-r--r--   0 runner    (1001) docker     (121)    10516 2022-03-28 07:56:58.000000 spead2-3.9.0/configure.ac
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.253672 spead2-3.9.0/doc/
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2456 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (121)     7331 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.253672 spead2-3.9.0/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/_static/.keep
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/advanced.rst
--rw-r--r--   0 runner    (1001) docker     (121)    38038 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3569 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/cpp-asio.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/cpp-ibverbs.rst
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/cpp-inproc.rst
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/cpp-logging.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/cpp-recv-chunk.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6537 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/cpp-recv.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/cpp-send.rst
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/cpp-stability.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1660 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/cpp.rst
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4761 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6581 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/migrate-3.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13435 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/perf.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1835 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/py-flavour.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8360 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/py-ibverbs.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2733 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/py-inproc.rst
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/py-items.rst
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/py-logging.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3007 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/py-protocol.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8875 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/py-recv-chunk.rst
--rw-r--r--   0 runner    (1001) docker     (121)    21644 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/py-recv.rst
--rw-r--r--   0 runner    (1001) docker     (121)    18872 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/py-send.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/py-thread-pools.rst
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/py.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7423 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/recv-chunk.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6525 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/recv-stats.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6221 2022-03-28 07:56:58.000000 spead2-3.9.0/doc/tools.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.253672 spead2-3.9.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-03-28 07:56:58.000000 spead2-3.9.0/examples/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (121)    26334 2022-03-28 07:57:23.000000 spead2-3.9.0/examples/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (121)     9302 2022-03-28 07:56:58.000000 spead2-3.9.0/examples/gdrapi_example.cu
--rw-r--r--   0 runner    (1001) docker     (121)     5341 2022-03-28 07:56:58.000000 spead2-3.9.0/examples/gpudirect_example.cu
--rw-r--r--   0 runner    (1001) docker     (121)     4072 2022-03-28 07:56:58.000000 spead2-3.9.0/examples/recv_chunk_example.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3948 2022-03-28 07:56:58.000000 spead2-3.9.0/examples/recv_chunk_ring_example.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     2963 2022-03-28 07:56:58.000000 spead2-3.9.0/examples/recv_chunk_ring_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     4841 2022-03-28 07:56:58.000000 spead2-3.9.0/examples/test_recv.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1434 2022-03-28 07:56:58.000000 spead2-3.9.0/examples/test_recv.py
--rw-r--r--   0 runner    (1001) docker     (121)     5998 2022-03-28 07:56:58.000000 spead2-3.9.0/examples/test_ringbuffer.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2653 2022-03-28 07:56:58.000000 spead2-3.9.0/examples/test_send.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1271 2022-03-28 07:56:58.000000 spead2-3.9.0/examples/test_send.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1550 2022-03-28 07:56:58.000000 spead2-3.9.0/examples/test_send_asyncio.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.253672 spead2-3.9.0/gen/
--rwxr-xr-x   0 runner    (1001) docker     (121)     8561 2022-03-28 07:56:58.000000 spead2-3.9.0/gen/gen_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1499 2022-03-28 07:56:58.000000 spead2-3.9.0/gen/get_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3563 2022-03-28 07:56:58.000000 spead2-3.9.0/gen/template.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-03-28 07:56:58.000000 spead2-3.9.0/gen/template.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.253672 spead2-3.9.0/include/
--rw-r--r--   0 runner    (1001) docker     (121)     2043 2022-03-28 07:56:58.000000 spead2-3.9.0/include/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (121)    18941 2022-03-28 07:57:23.000000 spead2-3.9.0/include/Makefile.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.257672 spead2-3.9.0/include/spead2/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     3888 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/common_bind.h
--rw-r--r--   0 runner    (1001) docker     (121)     4456 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/common_defines.h
--rw-r--r--   0 runner    (1001) docker     (121)     2141 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/common_endian.h
--rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/common_features.h.in
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/common_flavour.h
--rw-r--r--   0 runner    (1001) docker     (121)    16301 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/common_ibv.h
--rw-r--r--   0 runner    (1001) docker     (121)     1733 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/common_inproc.h
--rw-r--r--   0 runner    (1001) docker     (121)     3220 2022-03-28 07:57:18.000000 spead2-3.9.0/include/spead2/common_loader_ibv.h
--rw-r--r--   0 runner    (1001) docker     (121)     1628 2022-03-28 07:57:18.000000 spead2-3.9.0/include/spead2/common_loader_mlx5dv.h
--rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-03-28 07:57:18.000000 spead2-3.9.0/include/spead2/common_loader_rdmacm.h
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/common_loader_utils.h
--rw-r--r--   0 runner    (1001) docker     (121)     4097 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/common_logging.h
--rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/common_memcpy.h
--rw-r--r--   0 runner    (1001) docker     (121)     6496 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/common_memory_allocator.h
--rw-r--r--   0 runner    (1001) docker     (121)     4046 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/common_memory_pool.h
--rw-r--r--   0 runner    (1001) docker     (121)     6305 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/common_raw_packet.h
--rw-r--r--   0 runner    (1001) docker     (121)    16530 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/common_ringbuffer.h
--rw-r--r--   0 runner    (1001) docker     (121)     5147 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/common_semaphore.h
--rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/common_socket.h
--rw-r--r--   0 runner    (1001) docker     (121)     4318 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/common_thread_pool.h
--rw-r--r--   0 runner    (1001) docker     (121)     5442 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/common_unbounded_queue.h
--rw-r--r--   0 runner    (1001) docker     (121)     4036 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/portable_endian.h
--rw-r--r--   0 runner    (1001) docker     (121)    19043 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/py_common.h
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/py_recv.h
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/py_send.h
--rw-r--r--   0 runner    (1001) docker     (121)    19055 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/recv_chunk_stream.h
--rw-r--r--   0 runner    (1001) docker     (121)     7043 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/recv_heap.h
--rw-r--r--   0 runner    (1001) docker     (121)     1726 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/recv_inproc.h
--rw-r--r--   0 runner    (1001) docker     (121)     8089 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/recv_live_heap.h
--rw-r--r--   0 runner    (1001) docker     (121)     1609 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/recv_mem.h
--rw-r--r--   0 runner    (1001) docker     (121)     2638 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/recv_packet.h
--rw-r--r--   0 runner    (1001) docker     (121)     3252 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/recv_reader.h
--rw-r--r--   0 runner    (1001) docker     (121)     8866 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/recv_ring_stream.h
--rw-r--r--   0 runner    (1001) docker     (121)    29221 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/recv_stream.h
--rw-r--r--   0 runner    (1001) docker     (121)     5470 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/recv_tcp.h
--rw-r--r--   0 runner    (1001) docker     (121)     7533 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/recv_udp.h
--rw-r--r--   0 runner    (1001) docker     (121)     1848 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/recv_udp_base.h
--rw-r--r--   0 runner    (1001) docker     (121)    16817 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/recv_udp_ibv.h
--rw-r--r--   0 runner    (1001) docker     (121)     7221 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/recv_udp_ibv_mprq.h
--rw-r--r--   0 runner    (1001) docker     (121)     1730 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/recv_udp_pcap.h
--rw-r--r--   0 runner    (1001) docker     (121)     3196 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/recv_utils.h
--rw-r--r--   0 runner    (1001) docker     (121)     7464 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/send_heap.h
--rw-r--r--   0 runner    (1001) docker     (121)     2355 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/send_inproc.h
--rw-r--r--   0 runner    (1001) docker     (121)     3075 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/send_packet.h
--rw-r--r--   0 runner    (1001) docker     (121)    17629 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/send_stream.h
--rw-r--r--   0 runner    (1001) docker     (121)     3293 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/send_stream_config.h
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/send_streambuf.h
--rw-r--r--   0 runner    (1001) docker     (121)     4053 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/send_tcp.h
--rw-r--r--   0 runner    (1001) docker     (121)     7757 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/send_udp.h
--rw-r--r--   0 runner    (1001) docker     (121)     4903 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/send_udp_ibv.h
--rw-r--r--   0 runner    (1001) docker     (121)     2084 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/send_utils.h
--rw-r--r--   0 runner    (1001) docker     (121)     8347 2022-03-28 07:56:58.000000 spead2-3.9.0/include/spead2/send_writer.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.257672 spead2-3.9.0/m4/
--rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-03-28 07:56:58.000000 spead2-3.9.0/m4/spead2_arg_with.m4
--rw-r--r--   0 runner    (1001) docker     (121)     2734 2022-03-28 07:56:58.000000 spead2-3.9.0/m4/spead2_check_feature.m4
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-03-28 07:56:58.000000 spead2-3.9.0/m4/spead2_print_feature.m4
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.257672 spead2-3.9.0/manylinux/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1327 2022-03-28 07:56:58.000000 spead2-3.9.0/manylinux/before_all.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      142 2022-03-28 07:56:58.000000 spead2-3.9.0/manylinux/before_build.sh
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-03-28 07:56:58.000000 spead2-3.9.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      537 2022-03-28 07:56:58.000000 spead2-3.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-03-28 07:56:58.000000 spead2-3.9.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-03-28 07:56:58.000000 spead2-3.9.0/python-build.cfg.in
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-03-28 07:56:58.000000 spead2-3.9.0/requirements-readthedocs.txt
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-03-28 07:56:58.000000 spead2-3.9.0/requirements.in
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-03-28 07:56:58.000000 spead2-3.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-28 07:57:34.269672 spead2-3.9.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     7038 2022-03-28 07:56:58.000000 spead2-3.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-03-28 07:56:58.000000 spead2-3.9.0/spead2.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.265672 spead2-3.9.0/src/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-03-28 07:56:58.000000 spead2-3.9.0/src/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2919 2022-03-28 07:56:58.000000 spead2-3.9.0/src/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (121)    86899 2022-03-28 07:57:23.000000 spead2-3.9.0/src/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-03-28 07:56:58.000000 spead2-3.9.0/src/Makefile.inc.am
--rw-r--r--   0 runner    (1001) docker     (121)     1805 2022-03-28 07:56:58.000000 spead2-3.9.0/src/common_flavour.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    19642 2022-03-28 07:56:58.000000 spead2-3.9.0/src/common_ibv.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-03-28 07:56:58.000000 spead2-3.9.0/src/common_inproc.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    14888 2022-03-28 07:57:19.000000 spead2-3.9.0/src/common_loader_ibv.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4386 2022-03-28 07:57:19.000000 spead2-3.9.0/src/common_loader_mlx5dv.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4698 2022-03-28 07:57:18.000000 spead2-3.9.0/src/common_loader_rdmacm.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3075 2022-03-28 07:56:58.000000 spead2-3.9.0/src/common_loader_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2492 2022-03-28 07:56:58.000000 spead2-3.9.0/src/common_logging.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2979 2022-03-28 07:56:58.000000 spead2-3.9.0/src/common_memcpy.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-03-28 07:56:58.000000 spead2-3.9.0/src/common_memory_allocator.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8519 2022-03-28 07:56:58.000000 spead2-3.9.0/src/common_memory_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8280 2022-03-28 07:56:58.000000 spead2-3.9.0/src/common_raw_packet.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8674 2022-03-28 07:56:58.000000 spead2-3.9.0/src/common_semaphore.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2913 2022-03-28 07:56:58.000000 spead2-3.9.0/src/common_socket.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4652 2022-03-28 07:56:58.000000 spead2-3.9.0/src/common_thread_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    38689 2022-03-28 07:56:58.000000 spead2-3.9.0/src/mcdump.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    15689 2022-03-28 07:56:58.000000 spead2-3.9.0/src/py_common.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    38568 2022-03-28 07:56:58.000000 spead2-3.9.0/src/py_recv.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-03-28 07:56:58.000000 spead2-3.9.0/src/py_register.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    42108 2022-03-28 07:56:58.000000 spead2-3.9.0/src/py_send.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    12133 2022-03-28 07:56:58.000000 spead2-3.9.0/src/recv_chunk_stream.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    11730 2022-03-28 07:56:58.000000 spead2-3.9.0/src/recv_heap.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3209 2022-03-28 07:56:58.000000 spead2-3.9.0/src/recv_inproc.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     9723 2022-03-28 07:56:58.000000 spead2-3.9.0/src/recv_live_heap.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-03-28 07:56:58.000000 spead2-3.9.0/src/recv_mem.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     5884 2022-03-28 07:56:58.000000 spead2-3.9.0/src/recv_packet.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1354 2022-03-28 07:56:58.000000 spead2-3.9.0/src/recv_reader.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-03-28 07:56:58.000000 spead2-3.9.0/src/recv_ring_stream.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    21726 2022-03-28 07:56:58.000000 spead2-3.9.0/src/recv_stream.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     7689 2022-03-28 07:56:58.000000 spead2-3.9.0/src/recv_tcp.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    12040 2022-03-28 07:56:58.000000 spead2-3.9.0/src/recv_udp.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2007 2022-03-28 07:56:58.000000 spead2-3.9.0/src/recv_udp_base.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    10772 2022-03-28 07:56:58.000000 spead2-3.9.0/src/recv_udp_ibv.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     9823 2022-03-28 07:56:58.000000 spead2-3.9.0/src/recv_udp_ibv_mprq.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3845 2022-03-28 07:56:58.000000 spead2-3.9.0/src/recv_udp_pcap.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6197 2022-03-28 07:56:58.000000 spead2-3.9.0/src/send_heap.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4553 2022-03-28 07:56:58.000000 spead2-3.9.0/src/send_inproc.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8536 2022-03-28 07:56:58.000000 spead2-3.9.0/src/send_packet.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4406 2022-03-28 07:56:58.000000 spead2-3.9.0/src/send_stream.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2512 2022-03-28 07:56:58.000000 spead2-3.9.0/src/send_stream_config.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3042 2022-03-28 07:56:58.000000 spead2-3.9.0/src/send_streambuf.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8078 2022-03-28 07:56:58.000000 spead2-3.9.0/src/send_tcp.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    12571 2022-03-28 07:56:58.000000 spead2-3.9.0/src/send_udp.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    22615 2022-03-28 07:56:58.000000 spead2-3.9.0/src/send_udp_ibv.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    10244 2022-03-28 07:56:58.000000 spead2-3.9.0/src/send_writer.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.265672 spead2-3.9.0/src/spead2/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    30015 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5757 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1937 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/numba.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/numba.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.265672 spead2-3.9.0/src/spead2/recv/
--rw-r--r--   0 runner    (1001) docker     (121)     2768 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/recv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9638 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/recv/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6171 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/recv/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/recv/asyncio.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/recv/numba.py
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/recv/numba.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      850 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/recv/stream_stat_indices.py
--rw-r--r--   0 runner    (1001) docker     (121)      886 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/recv/stream_stat_indices.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.269672 spead2-3.9.0/src/spead2/send/
--rw-r--r--   0 runner    (1001) docker     (121)     6215 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/send/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8544 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/send/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7912 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/send/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/send/asyncio.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.269672 spead2-3.9.0/src/spead2/tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12484 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/tools/bench_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)    15325 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/tools/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (121)     4893 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/tools/recv_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)     5387 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2/tools/send_asyncio.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.265672 spead2-3.9.0/src/spead2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2278 2022-03-28 07:57:33.000000 spead2-3.9.0/src/spead2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6067 2022-03-28 07:57:34.000000 spead2-3.9.0/src/spead2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-28 07:57:33.000000 spead2-3.9.0/src/spead2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-03-28 07:57:33.000000 spead2-3.9.0/src/spead2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-03-28 07:57:34.000000 spead2-3.9.0/src/spead2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-28 07:57:34.000000 spead2-3.9.0/src/spead2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    23651 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2_bench.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    13135 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2_cmdline.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    11309 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2_cmdline.h
--rw-r--r--   0 runner    (1001) docker     (121)     2523 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2_net_raw.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    12575 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2_recv.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    11395 2022-03-28 07:56:58.000000 spead2-3.9.0/src/spead2_send.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     5295 2022-03-28 07:56:58.000000 spead2-3.9.0/src/unittest_logging.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      885 2022-03-28 07:56:58.000000 spead2-3.9.0/src/unittest_main.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2310 2022-03-28 07:56:58.000000 spead2-3.9.0/src/unittest_memcpy.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-03-28 07:56:58.000000 spead2-3.9.0/src/unittest_memory_allocator.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     7372 2022-03-28 07:56:58.000000 spead2-3.9.0/src/unittest_memory_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     9844 2022-03-28 07:56:58.000000 spead2-3.9.0/src/unittest_raw_packet.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3460 2022-03-28 07:56:58.000000 spead2-3.9.0/src/unittest_recv_custom_memcpy.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6792 2022-03-28 07:56:58.000000 spead2-3.9.0/src/unittest_recv_live_heap.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     7044 2022-03-28 07:56:58.000000 spead2-3.9.0/src/unittest_recv_stream_stats.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     4578 2022-03-28 07:56:58.000000 spead2-3.9.0/src/unittest_semaphore.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1856 2022-03-28 07:56:58.000000 spead2-3.9.0/src/unittest_send_heap.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2272 2022-03-28 07:56:58.000000 spead2-3.9.0/src/unittest_send_streambuf.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2184 2022-03-28 07:56:58.000000 spead2-3.9.0/src/unittest_send_tcp.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 07:57:34.269672 spead2-3.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-28 07:56:58.000000 spead2-3.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-03-28 07:56:58.000000 spead2-3.9.0/tests/shutdown.py
--rw-r--r--   0 runner    (1001) docker     (121)     9766 2022-03-28 07:56:58.000000 spead2-3.9.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (121)    26781 2022-03-28 07:56:58.000000 spead2-3.9.0/tests/test_passthrough.py
--rw-r--r--   0 runner    (1001) docker     (121)     8662 2022-03-28 07:56:58.000000 spead2-3.9.0/tests/test_passthrough_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)    49946 2022-03-28 07:56:58.000000 spead2-3.9.0/tests/test_recv.py
--rw-r--r--   0 runner    (1001) docker     (121)     4575 2022-03-28 07:56:58.000000 spead2-3.9.0/tests/test_recv_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)    24263 2022-03-28 07:56:58.000000 spead2-3.9.0/tests/test_recv_chunk_stream.py
--rw-r--r--   0 runner    (1001) docker     (121)    39859 2022-03-28 07:56:58.000000 spead2-3.9.0/tests/test_send.py
--rw-r--r--   0 runner    (1001) docker     (121)     3622 2022-03-28 07:56:58.000000 spead2-3.9.0/tests/test_send_asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.813269 spead2-3.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.789269 spead2-3.9.1/.ci/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      246 2022-04-07 10:55:54.000000 spead2-3.9.1/.ci/ccache-path.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      458 2022-04-07 10:55:54.000000 spead2-3.9.1/.ci/configure.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      550 2022-04-07 10:55:54.000000 spead2-3.9.1/.ci/coverage.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)       95 2022-04-07 10:55:54.000000 spead2-3.9.1/.ci/cxx-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      545 2022-04-07 10:55:54.000000 spead2-3.9.1/.ci/install-sys-pkgs.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)       91 2022-04-07 10:55:54.000000 spead2-3.9.1/.ci/py-requirements.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      269 2022-04-07 10:55:54.000000 spead2-3.9.1/.ci/py-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2022-04-07 10:55:54.000000 spead2-3.9.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.785269 spead2-3.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.789269 spead2-3.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     6425 2022-04-07 10:55:54.000000 spead2-3.9.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-07 10:55:54.000000 spead2-3.9.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-04-07 10:55:54.000000 spead2-3.9.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-04-07 10:55:54.000000 spead2-3.9.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-04-07 10:55:54.000000 spead2-3.9.1/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (121)    15752 2022-04-07 10:55:54.000000 spead2-3.9.1/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2022-04-07 10:55:54.000000 spead2-3.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      806 2022-04-07 10:55:54.000000 spead2-3.9.1/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (121)    28743 2022-04-07 10:56:16.000000 spead2-3.9.1/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2278 2022-04-07 10:56:27.813269 spead2-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-04-07 10:55:54.000000 spead2-3.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      539 2022-04-07 10:55:54.000000 spead2-3.9.1/RELEASE-PROCESS
+-rw-r--r--   0 runner    (1001) docker     (121)    51672 2022-04-07 10:56:14.000000 spead2-3.9.1/aclocal.m4
+-rwxr-xr-x   0 runner    (1001) docker     (121)      481 2022-04-07 10:55:54.000000 spead2-3.9.1/bootstrap.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.789269 spead2-3.9.1/build-aux/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    23568 2022-04-07 10:56:16.000000 spead2-3.9.1/build-aux/depcomp
+-rwxr-xr-x   0 runner    (1001) docker     (121)    15368 2022-04-07 10:56:16.000000 spead2-3.9.1/build-aux/install-sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6878 2022-04-07 10:56:16.000000 spead2-3.9.1/build-aux/missing
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4642 2022-04-07 10:56:16.000000 spead2-3.9.1/build-aux/test-driver
+-rwxr-xr-x   0 runner    (1001) docker     (121)   189637 2022-04-07 10:56:15.000000 spead2-3.9.1/configure
+-rw-r--r--   0 runner    (1001) docker     (121)    10516 2022-04-07 10:55:54.000000 spead2-3.9.1/configure.ac
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.793269 spead2-3.9.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     2456 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (121)     7331 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.793269 spead2-3.9.1/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/_static/.keep
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/advanced.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    38240 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3569 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/cpp-asio.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/cpp-ibverbs.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/cpp-inproc.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/cpp-logging.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/cpp-recv-chunk.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6537 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/cpp-recv.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/cpp-send.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      374 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/cpp-stability.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1660 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/cpp.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4761 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      649 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/license.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6581 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/migrate-3.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    13435 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/perf.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1835 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/py-flavour.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8360 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/py-ibverbs.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2733 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/py-inproc.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      868 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/py-items.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/py-logging.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3007 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/py-protocol.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8875 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/py-recv-chunk.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    21644 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/py-recv.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    18872 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/py-send.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/py-thread-pools.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      492 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/py.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7423 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/recv-chunk.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6525 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/recv-stats.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6221 2022-04-07 10:55:54.000000 spead2-3.9.1/doc/tools.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.793269 spead2-3.9.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-04-07 10:55:54.000000 spead2-3.9.1/examples/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (121)    26334 2022-04-07 10:56:16.000000 spead2-3.9.1/examples/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (121)     9302 2022-04-07 10:55:54.000000 spead2-3.9.1/examples/gdrapi_example.cu
+-rw-r--r--   0 runner    (1001) docker     (121)     5341 2022-04-07 10:55:54.000000 spead2-3.9.1/examples/gpudirect_example.cu
+-rw-r--r--   0 runner    (1001) docker     (121)     4072 2022-04-07 10:55:54.000000 spead2-3.9.1/examples/recv_chunk_example.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3948 2022-04-07 10:55:54.000000 spead2-3.9.1/examples/recv_chunk_ring_example.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2963 2022-04-07 10:55:54.000000 spead2-3.9.1/examples/recv_chunk_ring_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4841 2022-04-07 10:55:54.000000 spead2-3.9.1/examples/test_recv.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1434 2022-04-07 10:55:54.000000 spead2-3.9.1/examples/test_recv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5998 2022-04-07 10:55:54.000000 spead2-3.9.1/examples/test_ringbuffer.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2653 2022-04-07 10:55:54.000000 spead2-3.9.1/examples/test_send.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1271 2022-04-07 10:55:54.000000 spead2-3.9.1/examples/test_send.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1550 2022-04-07 10:55:54.000000 spead2-3.9.1/examples/test_send_asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.793269 spead2-3.9.1/gen/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8561 2022-04-07 10:55:54.000000 spead2-3.9.1/gen/gen_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1499 2022-04-07 10:55:54.000000 spead2-3.9.1/gen/get_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3563 2022-04-07 10:55:54.000000 spead2-3.9.1/gen/template.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-04-07 10:55:54.000000 spead2-3.9.1/gen/template.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.793269 spead2-3.9.1/include/
+-rw-r--r--   0 runner    (1001) docker     (121)     2043 2022-04-07 10:55:54.000000 spead2-3.9.1/include/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (121)    18941 2022-04-07 10:56:16.000000 spead2-3.9.1/include/Makefile.in
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.801269 spead2-3.9.1/include/spead2/
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     3888 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/common_bind.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4456 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/common_defines.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2141 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/common_endian.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/common_features.h.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1584 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/common_flavour.h
+-rw-r--r--   0 runner    (1001) docker     (121)    16301 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/common_ibv.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1733 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/common_inproc.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3220 2022-04-07 10:56:11.000000 spead2-3.9.1/include/spead2/common_loader_ibv.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1628 2022-04-07 10:56:11.000000 spead2-3.9.1/include/spead2/common_loader_mlx5dv.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-04-07 10:56:11.000000 spead2-3.9.1/include/spead2/common_loader_rdmacm.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/common_loader_utils.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4097 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/common_logging.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/common_memcpy.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6496 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/common_memory_allocator.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4046 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/common_memory_pool.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6305 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/common_raw_packet.h
+-rw-r--r--   0 runner    (1001) docker     (121)    16530 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/common_ringbuffer.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5147 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/common_semaphore.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/common_socket.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4318 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/common_thread_pool.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5442 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/common_unbounded_queue.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4036 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/portable_endian.h
+-rw-r--r--   0 runner    (1001) docker     (121)    19043 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/py_common.h
+-rw-r--r--   0 runner    (1001) docker     (121)      949 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/py_recv.h
+-rw-r--r--   0 runner    (1001) docker     (121)      949 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/py_send.h
+-rw-r--r--   0 runner    (1001) docker     (121)    19055 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/recv_chunk_stream.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7043 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/recv_heap.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1726 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/recv_inproc.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8089 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/recv_live_heap.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1609 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/recv_mem.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2638 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/recv_packet.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3252 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/recv_reader.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8866 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/recv_ring_stream.h
+-rw-r--r--   0 runner    (1001) docker     (121)    29221 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/recv_stream.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5470 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/recv_tcp.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7533 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/recv_udp.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1848 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/recv_udp_base.h
+-rw-r--r--   0 runner    (1001) docker     (121)    16817 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/recv_udp_ibv.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7221 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/recv_udp_ibv_mprq.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1730 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/recv_udp_pcap.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3196 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/recv_utils.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7464 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/send_heap.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2355 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/send_inproc.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3075 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/send_packet.h
+-rw-r--r--   0 runner    (1001) docker     (121)    17629 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/send_stream.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3293 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/send_stream_config.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/send_streambuf.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4053 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/send_tcp.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7757 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/send_udp.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4903 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/send_udp_ibv.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2084 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/send_utils.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8347 2022-04-07 10:55:54.000000 spead2-3.9.1/include/spead2/send_writer.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.801269 spead2-3.9.1/m4/
+-rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-04-07 10:55:54.000000 spead2-3.9.1/m4/spead2_arg_with.m4
+-rw-r--r--   0 runner    (1001) docker     (121)     2734 2022-04-07 10:55:54.000000 spead2-3.9.1/m4/spead2_check_feature.m4
+-rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-04-07 10:55:54.000000 spead2-3.9.1/m4/spead2_print_feature.m4
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.801269 spead2-3.9.1/manylinux/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1327 2022-04-07 10:55:54.000000 spead2-3.9.1/manylinux/before_all.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      142 2022-04-07 10:55:54.000000 spead2-3.9.1/manylinux/before_build.sh
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-04-07 10:55:54.000000 spead2-3.9.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      537 2022-04-07 10:55:54.000000 spead2-3.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-04-07 10:55:54.000000 spead2-3.9.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2022-04-07 10:55:54.000000 spead2-3.9.1/python-build.cfg.in
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-04-07 10:55:54.000000 spead2-3.9.1/requirements-readthedocs.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-04-07 10:55:54.000000 spead2-3.9.1/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-04-07 10:55:54.000000 spead2-3.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-07 10:56:27.813269 spead2-3.9.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7038 2022-04-07 10:55:54.000000 spead2-3.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2022-04-07 10:55:54.000000 spead2-3.9.1/spead2.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.809269 spead2-3.9.1/src/
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2022-04-07 10:55:54.000000 spead2-3.9.1/src/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     2919 2022-04-07 10:55:54.000000 spead2-3.9.1/src/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (121)    86899 2022-04-07 10:56:16.000000 spead2-3.9.1/src/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-04-07 10:55:54.000000 spead2-3.9.1/src/Makefile.inc.am
+-rw-r--r--   0 runner    (1001) docker     (121)     1805 2022-04-07 10:55:54.000000 spead2-3.9.1/src/common_flavour.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    19642 2022-04-07 10:55:54.000000 spead2-3.9.1/src/common_ibv.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-04-07 10:55:54.000000 spead2-3.9.1/src/common_inproc.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    14888 2022-04-07 10:56:11.000000 spead2-3.9.1/src/common_loader_ibv.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4386 2022-04-07 10:56:11.000000 spead2-3.9.1/src/common_loader_mlx5dv.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4698 2022-04-07 10:56:11.000000 spead2-3.9.1/src/common_loader_rdmacm.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3075 2022-04-07 10:55:54.000000 spead2-3.9.1/src/common_loader_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2492 2022-04-07 10:55:54.000000 spead2-3.9.1/src/common_logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2979 2022-04-07 10:55:54.000000 spead2-3.9.1/src/common_memcpy.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-04-07 10:55:54.000000 spead2-3.9.1/src/common_memory_allocator.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     8519 2022-04-07 10:55:54.000000 spead2-3.9.1/src/common_memory_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     8280 2022-04-07 10:55:54.000000 spead2-3.9.1/src/common_raw_packet.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     8674 2022-04-07 10:55:54.000000 spead2-3.9.1/src/common_semaphore.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2913 2022-04-07 10:55:54.000000 spead2-3.9.1/src/common_socket.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4652 2022-04-07 10:55:54.000000 spead2-3.9.1/src/common_thread_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    38689 2022-04-07 10:55:54.000000 spead2-3.9.1/src/mcdump.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    15689 2022-04-07 10:55:54.000000 spead2-3.9.1/src/py_common.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    38568 2022-04-07 10:55:54.000000 spead2-3.9.1/src/py_recv.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-04-07 10:55:54.000000 spead2-3.9.1/src/py_register.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    42108 2022-04-07 10:55:54.000000 spead2-3.9.1/src/py_send.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    12133 2022-04-07 10:55:54.000000 spead2-3.9.1/src/recv_chunk_stream.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    11730 2022-04-07 10:55:54.000000 spead2-3.9.1/src/recv_heap.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3209 2022-04-07 10:55:54.000000 spead2-3.9.1/src/recv_inproc.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     9723 2022-04-07 10:55:54.000000 spead2-3.9.1/src/recv_live_heap.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-04-07 10:55:54.000000 spead2-3.9.1/src/recv_mem.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     5884 2022-04-07 10:55:54.000000 spead2-3.9.1/src/recv_packet.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1354 2022-04-07 10:55:54.000000 spead2-3.9.1/src/recv_reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-04-07 10:55:54.000000 spead2-3.9.1/src/recv_ring_stream.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    21726 2022-04-07 10:55:54.000000 spead2-3.9.1/src/recv_stream.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     7689 2022-04-07 10:55:54.000000 spead2-3.9.1/src/recv_tcp.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    12040 2022-04-07 10:55:54.000000 spead2-3.9.1/src/recv_udp.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2007 2022-04-07 10:55:54.000000 spead2-3.9.1/src/recv_udp_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    10772 2022-04-07 10:55:54.000000 spead2-3.9.1/src/recv_udp_ibv.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     9823 2022-04-07 10:55:54.000000 spead2-3.9.1/src/recv_udp_ibv_mprq.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3845 2022-04-07 10:55:54.000000 spead2-3.9.1/src/recv_udp_pcap.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     6197 2022-04-07 10:55:54.000000 spead2-3.9.1/src/send_heap.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4553 2022-04-07 10:55:54.000000 spead2-3.9.1/src/send_inproc.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     8536 2022-04-07 10:55:54.000000 spead2-3.9.1/src/send_packet.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4406 2022-04-07 10:55:54.000000 spead2-3.9.1/src/send_stream.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2512 2022-04-07 10:55:54.000000 spead2-3.9.1/src/send_stream_config.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3042 2022-04-07 10:55:54.000000 spead2-3.9.1/src/send_streambuf.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     8078 2022-04-07 10:55:54.000000 spead2-3.9.1/src/send_tcp.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    12571 2022-04-07 10:55:54.000000 spead2-3.9.1/src/send_udp.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    22615 2022-04-07 10:55:54.000000 spead2-3.9.1/src/send_udp_ibv.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    10244 2022-04-07 10:55:54.000000 spead2-3.9.1/src/send_writer.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.809269 spead2-3.9.1/src/spead2/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)    30015 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5757 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1937 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/numba.py
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/numba.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.809269 spead2-3.9.1/src/spead2/recv/
+-rw-r--r--   0 runner    (1001) docker     (121)     2768 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/recv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9638 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/recv/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     6171 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/recv/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/recv/asyncio.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/recv/numba.py
+-rw-r--r--   0 runner    (1001) docker     (121)      775 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/recv/numba.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      850 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/recv/stream_stat_indices.py
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/recv/stream_stat_indices.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.809269 spead2-3.9.1/src/spead2/send/
+-rw-r--r--   0 runner    (1001) docker     (121)     6215 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/send/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8544 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/send/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     8066 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/send/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/send/asyncio.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.809269 spead2-3.9.1/src/spead2/tools/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12484 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/tools/bench_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15325 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/tools/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4893 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/tools/recv_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5387 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2/tools/send_asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.809269 spead2-3.9.1/src/spead2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2278 2022-04-07 10:56:27.000000 spead2-3.9.1/src/spead2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6067 2022-04-07 10:56:27.000000 spead2-3.9.1/src/spead2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-07 10:56:27.000000 spead2-3.9.1/src/spead2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-04-07 10:56:27.000000 spead2-3.9.1/src/spead2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-04-07 10:56:27.000000 spead2-3.9.1/src/spead2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-04-07 10:56:27.000000 spead2-3.9.1/src/spead2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    23651 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2_bench.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    13135 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2_cmdline.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    11309 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2_cmdline.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2523 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2_net_raw.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    12575 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2_recv.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    11395 2022-04-07 10:55:54.000000 spead2-3.9.1/src/spead2_send.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     5295 2022-04-07 10:55:54.000000 spead2-3.9.1/src/unittest_logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      885 2022-04-07 10:55:54.000000 spead2-3.9.1/src/unittest_main.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2310 2022-04-07 10:55:54.000000 spead2-3.9.1/src/unittest_memcpy.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-04-07 10:55:54.000000 spead2-3.9.1/src/unittest_memory_allocator.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     7372 2022-04-07 10:55:54.000000 spead2-3.9.1/src/unittest_memory_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     9844 2022-04-07 10:55:54.000000 spead2-3.9.1/src/unittest_raw_packet.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3460 2022-04-07 10:55:54.000000 spead2-3.9.1/src/unittest_recv_custom_memcpy.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     6792 2022-04-07 10:55:54.000000 spead2-3.9.1/src/unittest_recv_live_heap.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     7044 2022-04-07 10:55:54.000000 spead2-3.9.1/src/unittest_recv_stream_stats.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4578 2022-04-07 10:55:54.000000 spead2-3.9.1/src/unittest_semaphore.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1856 2022-04-07 10:55:54.000000 spead2-3.9.1/src/unittest_send_heap.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2272 2022-04-07 10:55:54.000000 spead2-3.9.1/src/unittest_send_streambuf.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2184 2022-04-07 10:55:54.000000 spead2-3.9.1/src/unittest_send_tcp.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 10:56:27.809269 spead2-3.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-07 10:55:54.000000 spead2-3.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-04-07 10:55:54.000000 spead2-3.9.1/tests/shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9766 2022-04-07 10:55:54.000000 spead2-3.9.1/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26781 2022-04-07 10:55:54.000000 spead2-3.9.1/tests/test_passthrough.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8662 2022-04-07 10:55:54.000000 spead2-3.9.1/tests/test_passthrough_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49946 2022-04-07 10:55:54.000000 spead2-3.9.1/tests/test_recv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4575 2022-04-07 10:55:54.000000 spead2-3.9.1/tests/test_recv_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24263 2022-04-07 10:55:54.000000 spead2-3.9.1/tests/test_recv_chunk_stream.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39859 2022-04-07 10:55:54.000000 spead2-3.9.1/tests/test_send.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4284 2022-04-07 10:55:54.000000 spead2-3.9.1/tests/test_send_asyncio.py
```

### Comparing `spead2-3.9.0/.ci/coverage.sh` & `spead2-3.9.1/.ci/coverage.sh`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/.ci/install-sys-pkgs.sh` & `spead2-3.9.1/.ci/install-sys-pkgs.sh`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/.github/workflows/test.yml` & `spead2-3.9.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/COPYING` & `spead2-3.9.1/COPYING`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/COPYING.LESSER` & `spead2-3.9.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/INSTALL` & `spead2-3.9.1/INSTALL`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/Makefile.am` & `spead2-3.9.1/Makefile.am`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/Makefile.in` & `spead2-3.9.1/Makefile.in`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/PKG-INFO` & `spead2-3.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spead2
-Version: 3.9.0
+Version: 3.9.1
 Summary: High-performance SPEAD implementation
 Home-page: https://github.com/ska-sa/spead2
 Author: Bruce Merry
 Author-email: bmerry@sarao.ac.za
 License: LGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `spead2-3.9.0/README.rst` & `spead2-3.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/RELEASE-PROCESS` & `spead2-3.9.1/RELEASE-PROCESS`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/aclocal.m4` & `spead2-3.9.1/aclocal.m4`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/build-aux/depcomp` & `spead2-3.9.1/build-aux/depcomp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/build-aux/install-sh` & `spead2-3.9.1/build-aux/install-sh`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/build-aux/missing` & `spead2-3.9.1/build-aux/missing`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/build-aux/test-driver` & `spead2-3.9.1/build-aux/test-driver`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/configure` & `spead2-3.9.1/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.69 for spead2 3.9.0.
+# Generated by GNU Autoconf 2.69 for spead2 3.9.1.
 #
 #
 # Copyright (C) 1992-1996, 1998-2012 Free Software Foundation, Inc.
 #
 #
 # This configure script is free software; the Free Software Foundation
 # gives unlimited permission to copy, distribute and modify it.
@@ -572,16 +572,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='spead2'
 PACKAGE_TARNAME='spead2'
-PACKAGE_VERSION='3.9.0'
-PACKAGE_STRING='spead2 3.9.0'
+PACKAGE_VERSION='3.9.1'
+PACKAGE_STRING='spead2 3.9.1'
 PACKAGE_BUGREPORT=''
 PACKAGE_URL=''
 
 ac_unique_file="src/common_logging.cpp"
 ac_subst_vars='am__EXEEXT_FALSE
 am__EXEEXT_TRUE
 LTLIBOBJS
@@ -1312,15 +1312,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures spead2 3.9.0 to adapt to many kinds of systems.
+\`configure' configures spead2 3.9.1 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1379,15 +1379,15 @@
   --program-suffix=SUFFIX            append SUFFIX to installed program names
   --program-transform-name=PROGRAM   run sed PROGRAM on installed program names
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of spead2 3.9.0:";;
+     short | recursive ) echo "Configuration of spead2 3.9.1:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1513,15 +1513,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-spead2 configure 3.9.0
+spead2 configure 3.9.1
 generated by GNU Autoconf 2.69
 
 Copyright (C) 2012 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -1681,15 +1681,15 @@
   eval $as_lineno_stack; ${as_lineno_stack:+:} unset as_lineno
 
 } # ac_fn_cxx_check_func
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by spead2 $as_me 3.9.0, which was
+It was created by spead2 $as_me 3.9.1, which was
 generated by GNU Autoconf 2.69.  Invocation command line was
 
   $ $0 $@
 
 _ACEOF
 exec 5>>config.log
 {
@@ -2548,15 +2548,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='spead2'
- VERSION='3.9.0'
+ VERSION='3.9.1'
 
 
 cat >>confdefs.h <<_ACEOF
 #define PACKAGE "$PACKAGE"
 _ACEOF
 
 
@@ -5303,17 +5303,17 @@
 fi
 
 
 SPEAD2_MAJOR=3
 
 SPEAD2_MINOR=9
 
-SPEAD2_PATCH=0
+SPEAD2_PATCH=1
 
-SPEAD2_VERSION=3.9.0
+SPEAD2_VERSION=3.9.1
 
 
 ac_config_files="$ac_config_files Makefile src/Makefile examples/Makefile include/Makefile include/spead2/common_features.h spead2.pc python-build.cfg"
 
 cat >confcache <<\_ACEOF
 # This file is a shell script that caches the results of configure
 # tests run on this system so they can be shared between configure
@@ -5912,15 +5912,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by spead2 $as_me 3.9.0, which was
+This file was extended by spead2 $as_me 3.9.1, which was
 generated by GNU Autoconf 2.69.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -5969,15 +5969,15 @@
 
 Report bugs to the package provider."
 
 _ACEOF
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config="`$as_echo "$ac_configure_args" | sed 's/^ //; s/[\\""\`\$]/\\\\&/g'`"
 ac_cs_version="\\
-spead2 config.status 3.9.0
+spead2 config.status 3.9.1
 configured by $0, generated by GNU Autoconf 2.69,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2012 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `spead2-3.9.0/configure.ac` & `spead2-3.9.1/configure.ac`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/Doxyfile` & `spead2-3.9.1/doc/Doxyfile`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/Makefile` & `spead2-3.9.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/changelog.rst` & `spead2-3.9.1/doc/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+.. rubric:: 3.9.1
+
+- Fix an :exc:`asyncio.InvalidStateError` that occurs when the future returned by
+  :py:meth:`~.async_send_heap` or :py:meth:`~.async_send_heaps` is cancelled
+  before it completes.
+
 .. rubric:: 3.9.0
 
 - Added ``substreams`` to :py:class:`spead2.recv.StreamConfig` to improve
   handling of interleaved heaps from multiple senders.
 - Add libdivide to the dependencies.
 
 .. rubric:: 3.8.0
```

### Comparing `spead2-3.9.0/doc/conf.py` & `spead2-3.9.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/cpp-asio.rst` & `spead2-3.9.1/doc/cpp-asio.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/cpp-ibverbs.rst` & `spead2-3.9.1/doc/cpp-ibverbs.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/cpp-recv-chunk.rst` & `spead2-3.9.1/doc/cpp-recv-chunk.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/cpp-recv.rst` & `spead2-3.9.1/doc/cpp-recv.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/cpp-send.rst` & `spead2-3.9.1/doc/cpp-send.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/cpp.rst` & `spead2-3.9.1/doc/cpp.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/index.rst` & `spead2-3.9.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/introduction.rst` & `spead2-3.9.1/doc/introduction.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/license.rst` & `spead2-3.9.1/doc/license.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/migrate-3.rst` & `spead2-3.9.1/doc/migrate-3.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/perf.rst` & `spead2-3.9.1/doc/perf.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/py-flavour.rst` & `spead2-3.9.1/doc/py-flavour.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/py-ibverbs.rst` & `spead2-3.9.1/doc/py-ibverbs.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/py-inproc.rst` & `spead2-3.9.1/doc/py-inproc.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/py-items.rst` & `spead2-3.9.1/doc/py-items.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/py-protocol.rst` & `spead2-3.9.1/doc/py-protocol.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/py-recv-chunk.rst` & `spead2-3.9.1/doc/py-recv-chunk.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/py-recv.rst` & `spead2-3.9.1/doc/py-recv.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/py-send.rst` & `spead2-3.9.1/doc/py-send.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/py-thread-pools.rst` & `spead2-3.9.1/doc/py-thread-pools.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/recv-chunk.rst` & `spead2-3.9.1/doc/recv-chunk.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/recv-stats.rst` & `spead2-3.9.1/doc/recv-stats.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/doc/tools.rst` & `spead2-3.9.1/doc/tools.rst`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/examples/Makefile.am` & `spead2-3.9.1/examples/Makefile.am`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/examples/Makefile.in` & `spead2-3.9.1/examples/Makefile.in`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/examples/gdrapi_example.cu` & `spead2-3.9.1/examples/gdrapi_example.cu`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/examples/gpudirect_example.cu` & `spead2-3.9.1/examples/gpudirect_example.cu`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/examples/recv_chunk_example.cpp` & `spead2-3.9.1/examples/recv_chunk_example.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/examples/recv_chunk_ring_example.cpp` & `spead2-3.9.1/examples/recv_chunk_ring_example.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/examples/recv_chunk_ring_example.py` & `spead2-3.9.1/examples/recv_chunk_ring_example.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/examples/test_recv.cpp` & `spead2-3.9.1/examples/test_recv.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/examples/test_recv.py` & `spead2-3.9.1/examples/test_recv.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/examples/test_ringbuffer.cpp` & `spead2-3.9.1/examples/test_ringbuffer.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/examples/test_send.cpp` & `spead2-3.9.1/examples/test_send.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/examples/test_send.py` & `spead2-3.9.1/examples/test_send.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/examples/test_send_asyncio.py` & `spead2-3.9.1/examples/test_send_asyncio.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/gen/gen_loader.py` & `spead2-3.9.1/gen/gen_loader.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/gen/get_version.py` & `spead2-3.9.1/gen/get_version.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/gen/template.cpp` & `spead2-3.9.1/gen/template.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/gen/template.h` & `spead2-3.9.1/gen/template.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/Makefile.am` & `spead2-3.9.1/include/Makefile.am`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/Makefile.in` & `spead2-3.9.1/include/Makefile.in`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_bind.h` & `spead2-3.9.1/include/spead2/common_bind.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_defines.h` & `spead2-3.9.1/include/spead2/common_defines.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_endian.h` & `spead2-3.9.1/include/spead2/common_endian.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_features.h.in` & `spead2-3.9.1/include/spead2/common_features.h.in`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_flavour.h` & `spead2-3.9.1/include/spead2/common_flavour.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_ibv.h` & `spead2-3.9.1/include/spead2/common_ibv.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_inproc.h` & `spead2-3.9.1/include/spead2/common_inproc.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_loader_ibv.h` & `spead2-3.9.1/include/spead2/common_loader_ibv.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_loader_mlx5dv.h` & `spead2-3.9.1/include/spead2/common_loader_mlx5dv.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_loader_rdmacm.h` & `spead2-3.9.1/include/spead2/common_loader_rdmacm.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_loader_utils.h` & `spead2-3.9.1/include/spead2/common_loader_utils.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_logging.h` & `spead2-3.9.1/include/spead2/common_logging.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_memcpy.h` & `spead2-3.9.1/include/spead2/common_memcpy.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_memory_allocator.h` & `spead2-3.9.1/include/spead2/common_memory_allocator.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_memory_pool.h` & `spead2-3.9.1/include/spead2/common_memory_pool.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_raw_packet.h` & `spead2-3.9.1/include/spead2/common_raw_packet.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_ringbuffer.h` & `spead2-3.9.1/include/spead2/common_ringbuffer.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_semaphore.h` & `spead2-3.9.1/include/spead2/common_semaphore.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_socket.h` & `spead2-3.9.1/include/spead2/common_socket.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_thread_pool.h` & `spead2-3.9.1/include/spead2/common_thread_pool.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/common_unbounded_queue.h` & `spead2-3.9.1/include/spead2/common_unbounded_queue.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/portable_endian.h` & `spead2-3.9.1/include/spead2/portable_endian.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/py_common.h` & `spead2-3.9.1/include/spead2/py_common.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/py_recv.h` & `spead2-3.9.1/include/spead2/py_recv.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/py_send.h` & `spead2-3.9.1/include/spead2/py_send.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/recv_chunk_stream.h` & `spead2-3.9.1/include/spead2/recv_chunk_stream.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/recv_heap.h` & `spead2-3.9.1/include/spead2/recv_heap.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/recv_inproc.h` & `spead2-3.9.1/include/spead2/recv_inproc.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/recv_live_heap.h` & `spead2-3.9.1/include/spead2/recv_live_heap.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/recv_mem.h` & `spead2-3.9.1/include/spead2/recv_mem.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/recv_packet.h` & `spead2-3.9.1/include/spead2/recv_packet.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/recv_reader.h` & `spead2-3.9.1/include/spead2/recv_reader.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/recv_ring_stream.h` & `spead2-3.9.1/include/spead2/recv_ring_stream.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/recv_stream.h` & `spead2-3.9.1/include/spead2/recv_stream.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/recv_tcp.h` & `spead2-3.9.1/include/spead2/recv_tcp.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/recv_udp.h` & `spead2-3.9.1/include/spead2/recv_udp.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/recv_udp_base.h` & `spead2-3.9.1/include/spead2/recv_udp_base.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/recv_udp_ibv.h` & `spead2-3.9.1/include/spead2/recv_udp_ibv.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/recv_udp_ibv_mprq.h` & `spead2-3.9.1/include/spead2/recv_udp_ibv_mprq.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/recv_udp_pcap.h` & `spead2-3.9.1/include/spead2/recv_udp_pcap.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/recv_utils.h` & `spead2-3.9.1/include/spead2/recv_utils.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/send_heap.h` & `spead2-3.9.1/include/spead2/send_heap.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/send_inproc.h` & `spead2-3.9.1/include/spead2/send_inproc.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/send_packet.h` & `spead2-3.9.1/include/spead2/send_packet.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/send_stream.h` & `spead2-3.9.1/include/spead2/send_stream.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/send_stream_config.h` & `spead2-3.9.1/include/spead2/send_stream_config.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/send_streambuf.h` & `spead2-3.9.1/include/spead2/send_streambuf.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/send_tcp.h` & `spead2-3.9.1/include/spead2/send_tcp.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/send_udp.h` & `spead2-3.9.1/include/spead2/send_udp.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/send_udp_ibv.h` & `spead2-3.9.1/include/spead2/send_udp_ibv.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/send_utils.h` & `spead2-3.9.1/include/spead2/send_utils.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/include/spead2/send_writer.h` & `spead2-3.9.1/include/spead2/send_writer.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/m4/spead2_arg_with.m4` & `spead2-3.9.1/m4/spead2_arg_with.m4`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/m4/spead2_check_feature.m4` & `spead2-3.9.1/m4/spead2_check_feature.m4`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/m4/spead2_print_feature.m4` & `spead2-3.9.1/m4/spead2_print_feature.m4`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/manylinux/before_all.sh` & `spead2-3.9.1/manylinux/before_all.sh`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/pyproject.toml` & `spead2-3.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/requirements.txt` & `spead2-3.9.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/setup.py` & `spead2-3.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/Makefile.am` & `spead2-3.9.1/src/Makefile.am`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/Makefile.in` & `spead2-3.9.1/src/Makefile.in`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/Makefile.inc.am` & `spead2-3.9.1/src/Makefile.inc.am`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/common_flavour.cpp` & `spead2-3.9.1/src/common_flavour.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/common_ibv.cpp` & `spead2-3.9.1/src/common_ibv.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/common_inproc.cpp` & `spead2-3.9.1/src/common_inproc.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/common_loader_ibv.cpp` & `spead2-3.9.1/src/common_loader_ibv.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/common_loader_mlx5dv.cpp` & `spead2-3.9.1/src/common_loader_mlx5dv.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/common_loader_rdmacm.cpp` & `spead2-3.9.1/src/common_loader_rdmacm.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/common_loader_utils.cpp` & `spead2-3.9.1/src/common_loader_utils.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/common_logging.cpp` & `spead2-3.9.1/src/common_logging.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/common_memcpy.cpp` & `spead2-3.9.1/src/common_memcpy.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/common_memory_allocator.cpp` & `spead2-3.9.1/src/common_memory_allocator.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/common_memory_pool.cpp` & `spead2-3.9.1/src/common_memory_pool.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/common_raw_packet.cpp` & `spead2-3.9.1/src/common_raw_packet.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/common_semaphore.cpp` & `spead2-3.9.1/src/common_semaphore.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/common_socket.cpp` & `spead2-3.9.1/src/common_socket.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/common_thread_pool.cpp` & `spead2-3.9.1/src/common_thread_pool.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/mcdump.cpp` & `spead2-3.9.1/src/mcdump.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/py_common.cpp` & `spead2-3.9.1/src/py_common.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/py_recv.cpp` & `spead2-3.9.1/src/py_recv.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/py_register.cpp` & `spead2-3.9.1/src/py_register.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/py_send.cpp` & `spead2-3.9.1/src/py_send.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/recv_chunk_stream.cpp` & `spead2-3.9.1/src/recv_chunk_stream.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/recv_heap.cpp` & `spead2-3.9.1/src/recv_heap.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/recv_inproc.cpp` & `spead2-3.9.1/src/recv_inproc.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/recv_live_heap.cpp` & `spead2-3.9.1/src/recv_live_heap.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/recv_mem.cpp` & `spead2-3.9.1/src/recv_mem.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/recv_packet.cpp` & `spead2-3.9.1/src/recv_packet.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/recv_reader.cpp` & `spead2-3.9.1/src/recv_reader.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/recv_ring_stream.cpp` & `spead2-3.9.1/src/recv_ring_stream.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/recv_stream.cpp` & `spead2-3.9.1/src/recv_stream.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/recv_tcp.cpp` & `spead2-3.9.1/src/recv_tcp.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/recv_udp.cpp` & `spead2-3.9.1/src/recv_udp.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/recv_udp_base.cpp` & `spead2-3.9.1/src/recv_udp_base.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/recv_udp_ibv.cpp` & `spead2-3.9.1/src/recv_udp_ibv.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/recv_udp_ibv_mprq.cpp` & `spead2-3.9.1/src/recv_udp_ibv_mprq.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/recv_udp_pcap.cpp` & `spead2-3.9.1/src/recv_udp_pcap.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/send_heap.cpp` & `spead2-3.9.1/src/send_heap.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/send_inproc.cpp` & `spead2-3.9.1/src/send_inproc.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/send_packet.cpp` & `spead2-3.9.1/src/send_packet.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/send_stream.cpp` & `spead2-3.9.1/src/send_stream.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/send_stream_config.cpp` & `spead2-3.9.1/src/send_stream_config.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/send_streambuf.cpp` & `spead2-3.9.1/src/send_streambuf.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/send_tcp.cpp` & `spead2-3.9.1/src/send_tcp.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/send_udp.cpp` & `spead2-3.9.1/src/send_udp.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/send_udp_ibv.cpp` & `spead2-3.9.1/src/send_udp_ibv.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/send_writer.cpp` & `spead2-3.9.1/src/send_writer.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2/__init__.py` & `spead2-3.9.1/src/spead2/__init__.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2/__init__.pyi` & `spead2-3.9.1/src/spead2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2/numba.py` & `spead2-3.9.1/src/spead2/numba.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2/numba.pyi` & `spead2-3.9.1/src/spead2/numba.pyi`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2/recv/__init__.py` & `spead2-3.9.1/src/spead2/recv/__init__.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2/recv/__init__.pyi` & `spead2-3.9.1/src/spead2/recv/__init__.pyi`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2/recv/asyncio.py` & `spead2-3.9.1/src/spead2/recv/asyncio.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2/recv/asyncio.pyi` & `spead2-3.9.1/src/spead2/recv/asyncio.pyi`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2/recv/numba.py` & `spead2-3.9.1/src/spead2/recv/numba.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2/recv/numba.pyi` & `spead2-3.9.1/src/spead2/recv/numba.pyi`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2/recv/stream_stat_indices.py` & `spead2-3.9.1/src/spead2/recv/stream_stat_indices.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2/recv/stream_stat_indices.pyi` & `spead2-3.9.1/src/spead2/recv/stream_stat_indices.pyi`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2/send/__init__.py` & `spead2-3.9.1/src/spead2/send/__init__.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2/send/__init__.pyi` & `spead2-3.9.1/src/spead2/send/__init__.pyi`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2/send/asyncio.py` & `spead2-3.9.1/src/spead2/send/asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015, 2019-2020 National Research Foundation (SARAO)
+# Copyright 2015, 2019-2020, 2022 National Research Foundation (SARAO)
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
@@ -21,30 +21,40 @@
 
 
 from spead2._spead2.send import UdpStreamAsyncio as _UdpStreamAsyncio
 from spead2._spead2.send import TcpStreamAsyncio as _TcpStreamAsyncio
 from spead2._spead2.send import InprocStreamAsyncio as _InprocStreamAsyncio
 
 
+def _set_result(future, result):
+    if not future.done():
+        future.set_result(result)
+
+
+def _set_exception(future, exc):
+    if not future.done():
+        future.set_exception(exc)
+
+
 def _wrap_class(name, base_class):
     class Wrapped(base_class):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
             self._active = 0
             self._last_queued_future = None
 
         def _async_send(self, call):
             future = asyncio.Future()
             loop = asyncio.get_event_loop()
 
             def callback(exc, bytes_transferred):
                 if exc is not None:
-                    future.set_exception(exc)
+                    _set_exception(future, exc)
                 else:
-                    future.set_result(bytes_transferred)
+                    _set_result(future, bytes_transferred)
                 self._active -= 1
                 if self._active == 0:
                     loop.remove_reader(self.fd)
                     self._last_queued_future = None  # Purely to free the memory
             queued = call(callback)
             if self._active == 0:
                 loop.add_reader(self.fd, self.process_callbacks)
@@ -133,19 +143,18 @@
         The arguments are the same as for the constructor of
         :py:class:`spead2.send.TcpStream`.
         """
         future = asyncio.Future()
         loop = asyncio.get_event_loop()
 
         def callback(arg):
-            if not future.done():
-                if isinstance(arg, Exception):
-                    loop.call_soon_threadsafe(future.set_exception, arg)
-                else:
-                    loop.call_soon_threadsafe(future.set_result, arg)
+            if isinstance(arg, Exception):
+                loop.call_soon_threadsafe(_set_exception, future, arg)
+            else:
+                loop.call_soon_threadsafe(_set_result, future, arg)
 
         stream = cls(callback, *args, **kwargs)
         await future
         return stream
 
 
 InprocStream = _wrap_class('InprocStream', _InprocStreamAsyncio)
```

### Comparing `spead2-3.9.0/src/spead2/send/asyncio.pyi` & `spead2-3.9.1/src/spead2/send/asyncio.pyi`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2/tools/bench_asyncio.py` & `spead2-3.9.1/src/spead2/tools/bench_asyncio.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2/tools/cmdline.py` & `spead2-3.9.1/src/spead2/tools/cmdline.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2/tools/recv_asyncio.py` & `spead2-3.9.1/src/spead2/tools/recv_asyncio.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2/tools/send_asyncio.py` & `spead2-3.9.1/src/spead2/tools/send_asyncio.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2.egg-info/PKG-INFO` & `spead2-3.9.1/src/spead2.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spead2
-Version: 3.9.0
+Version: 3.9.1
 Summary: High-performance SPEAD implementation
 Home-page: https://github.com/ska-sa/spead2
 Author: Bruce Merry
 Author-email: bmerry@sarao.ac.za
 License: LGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `spead2-3.9.0/src/spead2.egg-info/SOURCES.txt` & `spead2-3.9.1/src/spead2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2_bench.cpp` & `spead2-3.9.1/src/spead2_bench.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2_cmdline.cpp` & `spead2-3.9.1/src/spead2_cmdline.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2_cmdline.h` & `spead2-3.9.1/src/spead2_cmdline.h`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2_net_raw.cpp` & `spead2-3.9.1/src/spead2_net_raw.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2_recv.cpp` & `spead2-3.9.1/src/spead2_recv.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/spead2_send.cpp` & `spead2-3.9.1/src/spead2_send.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/unittest_logging.cpp` & `spead2-3.9.1/src/unittest_logging.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/unittest_main.cpp` & `spead2-3.9.1/src/unittest_main.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/unittest_memcpy.cpp` & `spead2-3.9.1/src/unittest_memcpy.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/unittest_memory_allocator.cpp` & `spead2-3.9.1/src/unittest_memory_allocator.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/unittest_memory_pool.cpp` & `spead2-3.9.1/src/unittest_memory_pool.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/unittest_raw_packet.cpp` & `spead2-3.9.1/src/unittest_raw_packet.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/unittest_recv_custom_memcpy.cpp` & `spead2-3.9.1/src/unittest_recv_custom_memcpy.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/unittest_recv_live_heap.cpp` & `spead2-3.9.1/src/unittest_recv_live_heap.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/unittest_recv_stream_stats.cpp` & `spead2-3.9.1/src/unittest_recv_stream_stats.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/unittest_semaphore.cpp` & `spead2-3.9.1/src/unittest_semaphore.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/unittest_send_heap.cpp` & `spead2-3.9.1/src/unittest_send_heap.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/unittest_send_streambuf.cpp` & `spead2-3.9.1/src/unittest_send_streambuf.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/src/unittest_send_tcp.cpp` & `spead2-3.9.1/src/unittest_send_tcp.cpp`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/tests/shutdown.py` & `spead2-3.9.1/tests/shutdown.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/tests/test_common.py` & `spead2-3.9.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/tests/test_passthrough.py` & `spead2-3.9.1/tests/test_passthrough.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/tests/test_passthrough_asyncio.py` & `spead2-3.9.1/tests/test_passthrough_asyncio.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/tests/test_recv.py` & `spead2-3.9.1/tests/test_recv.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/tests/test_recv_asyncio.py` & `spead2-3.9.1/tests/test_recv_asyncio.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/tests/test_recv_chunk_stream.py` & `spead2-3.9.1/tests/test_recv_chunk_stream.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/tests/test_send.py` & `spead2-3.9.1/tests/test_send.py`

 * *Files identical despite different names*

### Comparing `spead2-3.9.0/tests/test_send_asyncio.py` & `spead2-3.9.1/tests/test_send_asyncio.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015, 2019-2020 National Research Foundation (SARAO)
+# Copyright 2015, 2019-2022 National Research Foundation (SARAO)
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option) any
 # later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
@@ -10,14 +10,15 @@
 # FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import asyncio
+import logging
 import gc
 import weakref
 
 import numpy as np
 import pytest
 
 import spead2
@@ -82,14 +83,27 @@
                                               spead2.send.GroupMode.ROUND_ROBIN)
         self.heap = None
         await future
         for i in range(5):  # Try extra hard to make PyPy release things
             gc.collect()
         assert weak() is None
 
+    async def test_cancel(self, caplog):
+        """Cancelling the future must work gracefully."""
+        with caplog.at_level(logging.ERROR):
+            future = self.stream.async_send_heap(self.heap)
+            future.cancel()
+            with pytest.raises(asyncio.CancelledError):
+                await future
+            # Send another heap to ensure that process_callbacks has time to run.
+            await self.stream.async_send_heap(self.heap)
+        # An exception in process_callbacks doesn't propagate anywhere we can
+        # easily access it, but it does cause the event loop to log an error.
+        assert not caplog.records
+
 
 @pytest.mark.asyncio
 class TestTcpStream:
     async def test_connect_failed(self):
         thread_pool = spead2.ThreadPool()
         with pytest.raises(IOError):
             await spead2.send.asyncio.TcpStream.connect(thread_pool, [('127.0.0.1', 8887)])
```

