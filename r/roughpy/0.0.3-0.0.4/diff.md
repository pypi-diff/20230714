# Comparing `tmp/roughpy-0.0.3.tar.gz` & `tmp/roughpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roughpy-0.0.3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "roughpy-0.0.4.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `roughpy-0.0.3.tar` & `roughpy-0.0.4.tar`

### file list

```diff
@@ -1,725 +1,728 @@
--rw-r--r--   0        0        0     2003 2022-11-09 12:37:21.000000 roughpy-0.0.3/.clang-format
--rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 roughpy-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2022-11-09 12:37:21.000000 roughpy-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     3668 2022-11-09 12:37:21.000000 roughpy-0.0.3/.github/workflows/build_wheels.yml
--rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 roughpy-0.0.3/.github/workflows/manage_version.yml
--rw-r--r--   0        0        0     2733 2022-11-09 12:37:21.000000 roughpy-0.0.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0     5654 2022-11-09 12:37:21.000000 roughpy-0.0.3/.gitignore
--rw-r--r--   0        0        0      433 2022-11-09 12:37:21.000000 roughpy-0.0.3/.gitmodules
--rw-r--r--   0        0        0      757 2022-11-09 12:37:21.000000 roughpy-0.0.3/CHANGELOG
--rw-r--r--   0        0        0     9691 2022-11-09 12:37:21.000000 roughpy-0.0.3/CMakeLists.txt
--rw-r--r--   0        0        0     1489 2022-11-09 12:37:21.000000 roughpy-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     3467 2022-11-09 12:37:21.000000 roughpy-0.0.3/README.md
--rw-r--r--   0        0        0      743 2022-11-09 12:37:21.000000 roughpy-0.0.3/THANKS.txt
--rw-r--r--   0        0        0        7 2022-11-09 12:37:21.000000 roughpy-0.0.3/VERSION.txt
--rw-r--r--   0        0        0     3262 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/CMakeLists.txt
--rw-r--r--   0        0        0    16177 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_base.h
--rw-r--r--   0        0        0    23529 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_base_impl.h
--rw-r--r--   0        0        0     8043 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_bundle.h
--rw-r--r--   0        0        0    13572 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_bundle_base_impl.h
--rw-r--r--   0        0        0    26323 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_bundle_impl.h
--rw-r--r--   0        0        0     2737 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_fwd.h
--rw-r--r--   0        0        0    31744 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_impl.h
--rw-r--r--   0        0        0     3829 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_info.h
--rw-r--r--   0        0        0     7137 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_iterator.h
--rw-r--r--   0        0        0     3740 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_iterator_impl.h
--rw-r--r--   0        0        0     9250 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/basis.h
--rw-r--r--   0        0        0     6672 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/basis_impl.h
--rw-r--r--   0        0        0     6334 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/basis_info.h
--rw-r--r--   0        0        0      195 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/bundle_info.h
--rw-r--r--   0        0        0     9538 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/context.h
--rw-r--r--   0        0        0     4148 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/context_fwd.h
--rw-r--r--   0        0        0     1881 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/fallback_operations.h
--rw-r--r--   0        0        0     2634 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/free_tensor.h
--rw-r--r--   0        0        0     3750 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/free_tensor_fwd.h
--rw-r--r--   0        0        0     6431 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/free_tensor_impl.h
--rw-r--r--   0        0        0     2658 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/lie.h
--rw-r--r--   0        0        0     2088 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/lie_basis.h
--rw-r--r--   0        0        0     1852 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/lie_fwd.h
--rw-r--r--   0        0        0     2633 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/linear_operator.h
--rw-r--r--   0        0        0     2800 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/shuffle_tensor.h
--rw-r--r--   0        0        0     1858 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/shuffle_tensor_fwd.h
--rw-r--r--   0        0        0     2192 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/include/roughpy/algebra/tensor_basis.h
--rw-r--r--   0        0        0     1905 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/ContextFixture.cpp
--rw-r--r--   0        0        0     2186 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/ContextFixture.h
--rw-r--r--   0        0        0     3000 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/algebra_base.cpp
--rw-r--r--   0        0        0     1703 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/algebra_iterator.cpp
--rw-r--r--   0        0        0     1747 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/basis.cpp
--rw-r--r--   0        0        0     9768 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/context.cpp
--rw-r--r--   0        0        0     1737 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/double_lite_context.cpp
--rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/float_lite_context.cpp
--rw-r--r--   0        0        0     4084 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/free_tensor.cpp
--rw-r--r--   0        0        0     4248 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/hall_set_size.cpp
--rw-r--r--   0        0        0     2569 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/hall_set_size.h
--rw-r--r--   0        0        0     3031 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/libalgebra_lite_internal/dense_vector_iterator.h
--rw-r--r--   0        0        0     4222 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/libalgebra_lite_internal/free_tensor_info.h
--rw-r--r--   0        0        0     6669 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/libalgebra_lite_internal/lie_basis_info.h
--rw-r--r--   0        0        0     4191 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/libalgebra_lite_internal/lie_info.h
--rw-r--r--   0        0        0     3099 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/libalgebra_lite_internal/lite_vector_selector.h
--rw-r--r--   0        0        0     4223 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/libalgebra_lite_internal/shuffle_tensor_info.h
--rw-r--r--   0        0        0     5973 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/libalgebra_lite_internal/sparse_mutable_ref_scalar_trait.h
--rw-r--r--   0        0        0     2450 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/libalgebra_lite_internal/sparse_vector_iterator.h
--rw-r--r--   0        0        0     6642 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/libalgebra_lite_internal/tensor_basis_info.h
--rw-r--r--   0        0        0     2366 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/libalgebra_lite_internal/vector_type_helper.h
--rw-r--r--   0        0        0     2490 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/lie.cpp
--rw-r--r--   0        0        0     1821 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/lie_basis.cpp
--rw-r--r--   0        0        0     4732 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/lite_context.cpp
--rw-r--r--   0        0        0    28170 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/lite_context.h
--rw-r--r--   0        0        0     1737 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/rational_lite_context.cpp
--rw-r--r--   0        0        0     1739 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/rational_poly_lite_context.cpp
--rw-r--r--   0        0        0     2734 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/shuffle_tensor.cpp
--rw-r--r--   0        0        0     1883 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/tensor_basis.cpp
--rw-r--r--   0        0        0     1758 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/test_lie.cpp
--rw-r--r--   0        0        0     1631 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/testing/mock_context.cpp
--rw-r--r--   0        0        0     2139 2022-11-09 12:37:21.000000 roughpy-0.0.3/algebra/src/testing/mock_context.h
--rw-r--r--   0        0        0   106087 2022-11-09 12:37:21.000000 roughpy-0.0.3/branding/logo/logo_square_white.jpg
--rw-r--r--   0        0        0      509 2022-11-09 12:37:21.000000 roughpy-0.0.3/cmake/Modules/FindPCGRandom.cmake
--rw-r--r--   0        0        0    20264 2022-11-09 12:37:21.000000 roughpy-0.0.3/cmake/roughpy_helpers.cmake
--rw-r--r--   0        0        0      355 2022-11-09 12:37:21.000000 roughpy-0.0.3/cmake/version.py.in
--rw-r--r--   0        0        0      495 2022-11-09 12:37:21.000000 roughpy-0.0.3/core/CMakeLists.txt
--rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 roughpy-0.0.3/core/include/roughpy/core/alloc.h
--rw-r--r--   0        0        0     3627 2022-11-09 12:37:21.000000 roughpy-0.0.3/core/include/roughpy/core/helpers.h
--rw-r--r--   0        0        0     8395 2022-11-09 12:37:21.000000 roughpy-0.0.3/core/include/roughpy/core/macros.h
--rw-r--r--   0        0        0     4701 2022-11-09 12:37:21.000000 roughpy-0.0.3/core/include/roughpy/core/slice.h
--rw-r--r--   0        0        0     5000 2022-11-09 12:37:21.000000 roughpy-0.0.3/core/include/roughpy/core/traits.h
--rw-r--r--   0        0        0     2705 2022-11-09 12:37:21.000000 roughpy-0.0.3/core/include/roughpy/core/types.h
--rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 roughpy-0.0.3/device/CMakeLists.txt
--rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 roughpy-0.0.3/device/cuda/CMakeLists.txt
--rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 roughpy-0.0.3/device/cuda/CudaDeviceContext.cu
--rw-r--r--   0        0        0     1975 2022-11-09 12:37:21.000000 roughpy-0.0.3/device/cuda/CudaDeviceContext.cuh
--rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 roughpy-0.0.3/device/cuda/scalars/CMakeLists.txt
--rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 roughpy-0.0.3/device/cuda/scalars/src/CUDAFloatType.cu
--rw-r--r--   0        0        0     2005 2022-11-09 12:37:21.000000 roughpy-0.0.3/device/cuda/scalars/src/CUDAFloatType.cuh
--rw-r--r--   0        0        0     8605 2022-11-09 12:37:21.000000 roughpy-0.0.3/device/cuda/scalars/src/CUDA_standard_scalar.cuh
--rw-r--r--   0        0        0      868 2022-11-09 12:37:21.000000 roughpy-0.0.3/device/include/roughpy/device/core.h
--rw-r--r--   0        0        0    18540 2022-11-09 12:37:21.000000 roughpy-0.0.3/device/include/roughpy/device/device_algebra_base.h
--rw-r--r--   0        0        0     4377 2022-11-09 12:37:21.000000 roughpy-0.0.3/device/include/roughpy/device/device_context.h
--rw-r--r--   0        0        0     2348 2022-11-09 12:37:21.000000 roughpy-0.0.3/device/kernels/binary_kernel.cuh
--rw-r--r--   0        0        0     3972 2022-11-09 12:37:21.000000 roughpy-0.0.3/device/kernels/functors.h
--rw-r--r--   0        0        0     1712 2022-11-09 12:37:21.000000 roughpy-0.0.3/device/kernels/tmp.cu
--rw-r--r--   0        0        0     2304 2022-11-09 12:37:21.000000 roughpy-0.0.3/device/kernels/unary_kernel.cuh
--rw-r--r--   0        0        0     1801 2022-11-09 12:37:21.000000 roughpy-0.0.3/device/src/device_algebra_base.cpp
--rw-r--r--   0        0        0     1728 2022-11-09 12:37:21.000000 roughpy-0.0.3/device/src/device_context.cpp
--rw-r--r--   0        0        0     2854 2022-11-09 12:37:21.000000 roughpy-0.0.3/device/src/device_free_tensor.cpp
--rw-r--r--   0        0        0     2912 2022-11-09 12:37:21.000000 roughpy-0.0.3/device/src/device_free_tensor.h
--rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 roughpy-0.0.3/docs/make.bat
--rw-r--r--   0        0        0     1151 2022-11-09 12:37:21.000000 roughpy-0.0.3/docs/source/conf.py
--rw-r--r--   0        0        0      437 2022-11-09 12:37:21.000000 roughpy-0.0.3/docs/source/index.rst
--rw-r--r--   0        0        0     3589 2022-11-09 12:37:21.000000 roughpy-0.0.3/examples/lie_to_tensor_formulae.py
--rw-r--r--   0        0        0     1956 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/.clang-format
--rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/.git
--rw-r--r--   0        0        0     5992 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/.gitignore
--rw-r--r--   0        0        0     7502 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/CMakeLists.txt
--rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/Dockerfile
--rw-r--r--   0        0        0     1839 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/Dockerfile.remote-cpp-env
--rw-r--r--   0        0        0      335 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/LibalgebraConfig.cmake.in
--rw-r--r--   0        0        0     2706 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/README.md
--rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/benchmarks/CMakeLists.txt
--rw-r--r--   0        0        0      414 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/benchmarks/antipode/CMakeLists.txt
--rw-r--r--   0        0        0     5078 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/benchmarks/antipode/antipode_bm.cpp
--rw-r--r--   0        0        0     1941 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/benchmarks/multiplication/CMakeLists.txt
--rw-r--r--   0        0        0    14501 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/benchmarks/multiplication/multiplication_bm.cpp
--rw-r--r--   0        0        0     2363 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/benchmarks/multiplication/multiplication_single.cpp
--rw-r--r--   0        0        0     1494 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/cmake/Modules/FindBignum.cmake
--rw-r--r--   0        0        0     3540 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/cmake/Modules/UnitTestPP.cmake
--rw-r--r--   0        0        0     4012 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/cmake/Modules/UnitTestPP_DiscoverTests.cmake
--rw-r--r--   0        0        0     1602 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/cmake/libalgebra_test_helper.cmake
--rw-r--r--   0        0        0    19400 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/_tensor_basis.h
--rw-r--r--   0        0        0     5123 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/alg_types.h
--rw-r--r--   0        0        0    33383 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/algebra.h
--rw-r--r--   0        0        0     4069 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/alternative_multiplications.h
--rw-r--r--   0        0        0     2188 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/area_tensor_basis.h
--rw-r--r--   0        0        0    10008 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/area_tensor_multiplication.h
--rw-r--r--   0        0        0     1336 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/base_basis.h
--rw-r--r--   0        0        0     2600 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/base_vector.h
--rw-r--r--   0        0        0     3202 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/basis.h
--rw-r--r--   0        0        0    12663 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/coefficients/gmp_ser.h
--rw-r--r--   0        0        0     5981 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/coefficients.h
--rw-r--r--   0        0        0      389 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/complex.h
--rw-r--r--   0        0        0      772 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/composition_operator.h
--rw-r--r--   0        0        0     1291 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/constlog2.h
--rw-r--r--   0        0        0     2065 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/constpower.h
--rw-r--r--   0        0        0    25576 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/dense_storage.h
--rw-r--r--   0        0        0    32612 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/dense_vector.h
--rw-r--r--   0        0        0     1684 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/detail/caching_tags.h
--rw-r--r--   0        0        0      960 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/detail/function_extension_cache_base.h
--rw-r--r--   0        0        0     4044 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/detail/integer_maths.h
--rw-r--r--   0        0        0     1536 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/detail/level_walkers.h
--rw-r--r--   0        0        0     3387 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/detail/meta.h
--rw-r--r--   0        0        0      463 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/detail/order_trait.h
--rw-r--r--   0        0        0     1067 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/detail/platform.h
--rw-r--r--   0        0        0     3762 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/detail/reversing_permutation.h
--rw-r--r--   0        0        0      545 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/detail/smallest_int_type.h
--rw-r--r--   0        0        0     6839 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/detail/unpacked_tensor_word.h
--rw-r--r--   0        0        0     3535 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/dot_product_implementations.h
--rw-r--r--   0        0        0     2824 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/free_extension.h
--rw-r--r--   0        0        0     1303 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/functionals.h
--rw-r--r--   0        0        0     2193 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/half_shuffle_tensor_basis.h
--rw-r--r--   0        0        0    10154 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/half_shuffle_tensor_multiplication.h
--rw-r--r--   0        0        0    21063 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/hall_set.h
--rw-r--r--   0        0        0    40389 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/hybrid_vector.h
--rw-r--r--   0        0        0     2519 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/implementation_types.h
--rw-r--r--   0        0        0     3360 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/iterators.h
--rw-r--r--   0        0        0     4414 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/key_iterators.h
--rw-r--r--   0        0        0     6487 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/libalgebra.h
--rw-r--r--   0        0        0     6024 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/lie.h
--rw-r--r--   0        0        0    17479 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/lie_basis.h
--rw-r--r--   0        0        0     3791 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/lie_inner_product.h
--rw-r--r--   0        0        0     7234 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/monomial_basis.h
--rw-r--r--   0        0        0      886 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/mpfloat_coefficients.h
--rw-r--r--   0        0        0     1033 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/multi_linear_operators.h
--rw-r--r--   0        0        0     5991 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/multi_polynomial.h
--rw-r--r--   0        0        0     1693 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/multiplication_helpers.h
--rw-r--r--   0        0        0     9179 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/operators.h
--rw-r--r--   0        0        0     5565 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/poly_basis.h
--rw-r--r--   0        0        0     6082 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/poly_lie.h
--rw-r--r--   0        0        0     3450 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/poly_lie_basis.h
--rw-r--r--   0        0        0      640 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/polynomial_coefficients.h
--rw-r--r--   0        0        0     6720 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/polynomials.h
--rw-r--r--   0        0        0      779 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/rational_coefficients.h
--rw-r--r--   0        0        0     5880 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/reconfigure_operator.h
--rw-r--r--   0        0        0     8186 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/scalar_bundle.h
--rw-r--r--   0        0        0      982 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/scalar_multiply_operator.h
--rw-r--r--   0        0        0    41789 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/sparse_vector.h
--rw-r--r--   0        0        0      621 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/sum_operator.h
--rw-r--r--   0        0        0     1475 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/tags.h
--rw-r--r--   0        0        0   144218 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/tensor.h
--rw-r--r--   0        0        0    19208 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/tensor_basis.h
--rw-r--r--   0        0        0     1724 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/tensor_operator.h
--rw-r--r--   0        0        0    11862 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/utils.h
--rw-r--r--   0        0        0    24861 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/vector.h
--rw-r--r--   0        0        0    31254 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/vector_bundle.h
--rw-r--r--   0        0        0     1309 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/libalgebra/vectors.h
--rw-r--r--   0        0        0     1267 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/CMakeLists.txt
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/README.md
--rw-r--r--   0        0        0     1324 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/common/CMakeLists.txt
--rw-r--r--   0        0        0     1872 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/common/SHOW.h
--rw-r--r--   0        0        0     2676 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/common/compat.h
--rw-r--r--   0        0        0     1058 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/common/helpers.h
--rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/common/memfile.cpp
--rw-r--r--   0        0        0     3236 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/common/memfile.h
--rw-r--r--   0        0        0     4234 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/common/multi_test.h
--rw-r--r--   0        0        0     1554 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/common/random_coeffs.h
--rw-r--r--   0        0        0     2483 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/common/random_vector_generator.h
--rw-r--r--   0        0        0     1467 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/common/reporter.cpp
--rw-r--r--   0        0        0      670 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/common/reporter.h
--rw-r--r--   0        0        0     1711 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/common/rng.h
--rw-r--r--   0        0        0     2972 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/common/run_tests.cpp
--rw-r--r--   0        0        0     1102 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/common/simple_basis.h
--rw-r--r--   0        0        0     2372 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/common/time_and_details.h
--rw-r--r--   0        0        0     3181 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/AlgebraFunctionsTests.cpp
--rw-r--r--   0        0        0      477 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/CMakeLists.txt
--rw-r--r--   0        0        0     5679 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/HallSetTests.cpp
--rw-r--r--   0        0        0     4658 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/LatticePathTests.cpp
--rw-r--r--   0        0        0      511 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/LibAlgebraUnitTests.cpp
--rw-r--r--   0        0        0    43337 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/MemoryMappedFilesDocumentation.htm
--rw-r--r--   0        0        0     1250 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/OMPSigsTests.cpp
--rw-r--r--   0        0        0     2877 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/SigHelpers.h
--rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/TreeBufferHelper.cpp
--rw-r--r--   0        0        0     1516 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/TreeBufferHelper.h
--rw-r--r--   0        0        0      477 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/alg_framework.h
--rw-r--r--   0        0        0     1989 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/brown_path_increments.h
--rw-r--r--   0        0        0     2936 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/categorical_path.h
--rw-r--r--   0        0        0      440 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/log2ceil.h
--rw-r--r--   0        0        0      844 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/makebm.cpp
--rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/makebm.h
--rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/CMakeLists.txt
--rw-r--r--   0        0        0    17054 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/accuracy_suite.ins
--rw-r--r--   0        0        0     1817 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/coefficient_path_suite.ins
--rw-r--r--   0        0        0     1579 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/double_path_suite.ins
--rw-r--r--   0        0        0     1570 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/float_path_suite.ins
--rw-r--r--   0        0        0     1224 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/generic_coefficient.h
--rw-r--r--   0        0        0     1383 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/generic_lie_increment.h
--rw-r--r--   0        0        0     2240 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/generic_path.h
--rw-r--r--   0        0        0     1580 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/rational_path_suite.ins
--rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/run_tests.cpp
--rw-r--r--   0        0        0    20566 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/test_brownian_path.cpp
--rw-r--r--   0        0        0    11406 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/test_innovative_path.cpp
--rw-r--r--   0        0        0     5309 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/speed_tests.cpp
--rw-r--r--   0        0        0    12166 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/tests_TENSOR_LIE_CBH_MAPS.cpp
--rw-r--r--   0        0        0     6213 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/tests_libalgebra-demo.cpp
--rw-r--r--   0        0        0     1590 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/integration_tests/x64sigs.cpp
--rw-r--r--   0        0        0      480 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/CMakeLists.txt
--rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/adjoint/CMakeLists.txt
--rw-r--r--   0        0        0     7719 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/adjoint/test_adjoint.cpp
--rw-r--r--   0        0        0      609 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/algebra/CMakeLists.txt
--rw-r--r--   0        0        0     2223 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/algebra/alg_mul_suite.h
--rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/algebra/framework_fixture.h
--rw-r--r--   0        0        0      804 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/algebra/simple_algebra_basis.h
--rw-r--r--   0        0        0      696 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/algebra/test_algebra_product.cpp
--rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/antipode/CMakeLists.txt
--rw-r--r--   0        0        0     7994 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/antipode/test_antipode.cpp
--rw-r--r--   0        0        0      188 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/basis/CMakeLists.txt
--rw-r--r--   0        0        0     2232 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/basis/basis_iteration_suite.h
--rw-r--r--   0        0        0     3917 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/basis/test_basis_iteration.cpp
--rw-r--r--   0        0        0      612 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/basis/test_lie_basis_iteration.cpp
--rw-r--r--   0        0        0      408 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/basis/test_tensor_basis_iteration.cpp
--rw-r--r--   0        0        0      299 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/coefficients/CMakeLists.txt
--rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/coefficients/polynomial_coeff_ring.cpp
--rw-r--r--   0        0        0      791 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/coefficients/standard_coefficient_test_suite.h
--rw-r--r--   0        0        0      382 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/coefficients/test_double_field.cpp
--rw-r--r--   0        0        0      378 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/coefficients/test_float_field.cpp
--rw-r--r--   0        0        0      660 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/coefficients/test_mpfloat_fallback_field.cpp
--rw-r--r--   0        0        0      441 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/coefficients/test_mpfloat_field.cpp
--rw-r--r--   0        0        0      602 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/coefficients/test_rational_fallback_field.cpp
--rw-r--r--   0        0        0      506 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/coefficients/test_rational_field.cpp
--rw-r--r--   0        0        0     1789 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/coefficients/unital_coefficient_test_suite.h
--rw-r--r--   0        0        0       83 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/half-shuffle-tests/CMakeLists.txt
--rw-r--r--   0        0        0    19137 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/half-shuffle-tests/half_shuffle_fixture.h
--rw-r--r--   0        0        0     8440 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/half-shuffle-tests/test_half_shuffle.cpp
--rw-r--r--   0        0        0       74 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/hall_set/CMakeLists.txt
--rw-r--r--   0        0        0     8138 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/hall_set/test_hall_set.cpp
--rw-r--r--   0        0        0      208 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/lie/CMakeLists.txt
--rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/lie/run_tests.cpp
--rw-r--r--   0        0        0      541 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/lie/test_basis.cpp
--rw-r--r--   0        0        0     2083 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/lie/test_dense_lie_multiplication.cpp
--rw-r--r--   0        0        0     1771 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/lie/test_function_extension.cpp
--rw-r--r--   0        0        0     5505 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/lie/test_hall_basis.cpp
--rw-r--r--   0        0        0     1663 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/lie/test_lie_multiplication.cpp
--rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/multipoly/CMakeLists.txt
--rw-r--r--   0        0        0      499 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/multipoly/test_multipoly_prod.cpp
--rw-r--r--   0        0        0      387 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/operators/CMakeLists.txt
--rw-r--r--   0        0        0     2816 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/operators/test_free_extension.cpp
--rw-r--r--   0        0        0     1466 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/operators/test_lie_inner_product.cpp
--rw-r--r--   0        0        0     2406 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/operators/test_operator_composition.cpp
--rw-r--r--   0        0        0     1548 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/operators/test_operator_sum.cpp
--rw-r--r--   0        0        0     1791 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/operators/test_operators_smul.cpp
--rw-r--r--   0        0        0     1203 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/operators/test_recalibrate_operator.cpp
--rw-r--r--   0        0        0     4353 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/operators/test_shuffle_functional.cpp
--rw-r--r--   0        0        0     2553 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/operators/test_tensor_defined_operator.cpp
--rw-r--r--   0        0        0     1785 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/operators/test_tensor_multiplication_operator.cpp
--rw-r--r--   0        0        0      552 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/CMakeLists.txt
--rw-r--r--   0        0        0     3057 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/dense_vec_serialization.cpp
--rw-r--r--   0        0        0      398 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/fixture.cpp
--rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/fixture.h
--rw-r--r--   0        0        0     4014 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/hybrid_vector_serialization.cpp
--rw-r--r--   0        0        0     7910 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/sparse_vector_serialization.cpp
--rw-r--r--   0        0        0      548 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/temporary_directory.cpp
--rw-r--r--   0        0        0      419 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/temporary_directory.h
--rw-r--r--   0        0        0     2991 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/test_dense_storage.cpp
--rw-r--r--   0        0        0     1771 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/test_hall_set_serialize.cpp
--rw-r--r--   0        0        0     2805 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/test_higher_classes.cpp
--rw-r--r--   0        0        0       86 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/shuffle-tensor-tests/CMakeLists.txt
--rw-r--r--   0        0        0    43877 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/shuffle-tensor-tests/test_shuffle_tensor.cpp
--rw-r--r--   0        0        0      753 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tangents/CMakeLists.txt
--rw-r--r--   0        0        0    20887 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tangents/test_tangents.cpp
--rw-r--r--   0        0        0      465 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tangents/test_tangents.h
--rw-r--r--   0        0        0      983 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/CMakeLists.txt
--rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/run_tests.cpp
--rw-r--r--   0        0        0     3985 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/tensor_exp_suite.h
--rw-r--r--   0        0        0     1797 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/tensor_inverse_suite.h
--rw-r--r--   0        0        0     4055 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/tensor_log_suite.h
--rw-r--r--   0        0        0     3037 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/tensor_roundtrip_suite.h
--rw-r--r--   0        0        0     5062 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_basis.cpp
--rw-r--r--   0        0        0     2509 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_dense_tensor_functions.cpp
--rw-r--r--   0        0        0     4824 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_dense_tensor_multiplication.cpp
--rw-r--r--   0        0        0     2544 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_hybrid_tensor_functions.cpp
--rw-r--r--   0        0        0     5037 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_hybrid_tensor_multiplication.cpp
--rw-r--r--   0        0        0     2805 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_signature_calc.cpp
--rw-r--r--   0        0        0     2535 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_sparse_tensor_functions.cpp
--rw-r--r--   0        0        0     4900 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_sparse_tensor_multiplication.cpp
--rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_tensor_creation.cpp
--rw-r--r--   0        0        0     3291 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_tensor_functions.cpp
--rw-r--r--   0        0        0    38059 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_tensor_multiplication.cpp
--rw-r--r--   0        0        0     2419 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_tensor_size_info.cpp
--rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/utils/CMakeLists.txt
--rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/utils/run_tests.cpp
--rw-r--r--   0        0        0     2678 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/utils/test_integer_maths.cpp
--rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/CMakeLists.txt
--rw-r--r--   0        0        0     3599 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/framework_fixture.h
--rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/run_tests.cpp
--rw-r--r--   0        0        0      804 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/test_dense.cpp
--rw-r--r--   0        0        0    13508 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/test_dense_storage.cpp
--rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/test_hybrid.cpp
--rw-r--r--   0        0        0      968 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/test_sparse.cpp
--rw-r--r--   0        0        0    12957 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/vector_arithmetic_suite.h
--rw-r--r--   0        0        0    11707 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/vector_binary_transform_suite.h
--rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/vector_comparison_suite.h
--rw-r--r--   0        0        0     1134 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/vector_element_access_suite.h
--rw-r--r--   0        0        0     7086 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/vector_iterator_suite.h
--rw-r--r--   0        0        0     1907 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/vector_norm_suite.h
--rw-r--r--   0        0        0     2723 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/vector_properties_suite.h
--rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/width1_tests/CMakeLists.txt
--rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/width1_tests/types.cpp
--rw-r--r--   0        0        0      383 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/width1_tests/width1.h
--rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/width1_tests/width1_lie.cpp
--rw-r--r--   0        0        0     4024 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra/tests/unit_tests/width1_tests/width1_tensors.cpp
--rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/.git
--rw-r--r--   0        0        0     4566 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/CMakeLists.txt
--rw-r--r--   0        0        0       18 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/README.md
--rw-r--r--   0        0        0      485 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/cmake/Libalgebra_liteConfig.cmake.in
--rw-r--r--   0        0        0      247 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/cmake/config.h.in
--rw-r--r--   0        0        0     2787 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/cmake/lalhelpers.cmake
--rw-r--r--   0        0        0      561 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/cmake/rationals.h.in
--rw-r--r--   0        0        0    30855 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/algebra.h
--rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/basis.h
--rw-r--r--   0        0        0     3322 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/basis_traits.h
--rw-r--r--   0        0        0     3141 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/coefficients.h
--rw-r--r--   0        0        0    13187 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/dense_vector.h
--rw-r--r--   0        0        0     1370 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/detail/notnull.h
--rw-r--r--   0        0        0    22036 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/free_tensor.h
--rw-r--r--   0        0        0     6649 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/hall_set.h
--rw-r--r--   0        0        0     1622 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/implementation_types.h
--rw-r--r--   0        0        0     4878 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/index_key.h
--rw-r--r--   0        0        0      809 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/key_range.h
--rw-r--r--   0        0        0     1890 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/lie.h
--rw-r--r--   0        0        0     7253 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/maps.h
--rw-r--r--   0        0        0     6637 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/operators.h
--rw-r--r--   0        0        0     7010 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/packed_integer.h
--rw-r--r--   0        0        0     3643 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/polynomial.h
--rw-r--r--   0        0        0     4088 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/polynomial_basis.h
--rw-r--r--   0        0        0     2604 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/registry.h
--rw-r--r--   0        0        0    14411 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/shuffle_tensor.h
--rw-r--r--   0        0        0    14014 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/sparse_vector.h
--rw-r--r--   0        0        0     2590 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/tensor_basis.h
--rw-r--r--   0        0        0     2937 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/unpacked_tensor_word.h
--rw-r--r--   0        0        0    21879 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/vector.h
--rw-r--r--   0        0        0     1216 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/vector_base.h
--rw-r--r--   0        0        0     1734 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/vector_bundle.h
--rw-r--r--   0        0        0      515 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/vector_traits.h
--rw-r--r--   0        0        0      703 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/src/algebra/free_tensor_multiplier.cpp
--rw-r--r--   0        0        0     5062 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/src/algebra/half_shuffle_multiplier.cpp
--rw-r--r--   0        0        0     1618 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/src/algebra/lie_multiplier.cpp
--rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/src/algebra/polynomial.cpp
--rw-r--r--   0        0        0      794 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/src/algebra/polynomial_multiplier.cpp
--rw-r--r--   0        0        0      379 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/src/algebra/polynomial_ring.cpp
--rw-r--r--   0        0        0      812 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/src/algebra/shuffle_multiplier.cpp
--rw-r--r--   0        0        0     6227 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/src/basis/hall_set.cpp
--rw-r--r--   0        0        0      594 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/src/basis/monomial.cpp
--rw-r--r--   0        0        0     1390 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/src/basis/polynomial_basis.cpp
--rw-r--r--   0        0        0     2294 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/src/basis/tensor_basis.cpp
--rw-r--r--   0        0        0     5543 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/src/basis/unpacked_tensor_word.cpp
--rw-r--r--   0        0        0      211 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/src/coefficients/floating_fields.cpp
--rw-r--r--   0        0        0      178 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/src/coefficients/rational_field.cpp
--rw-r--r--   0        0        0     2895 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/src/maps.cpp
--rw-r--r--   0        0        0      469 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/CMakeLists.txt
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/common/main.cpp
--rw-r--r--   0        0        0      494 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/lie/CMakeLists.txt
--rw-r--r--   0        0        0     2542 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/lie/hall_basis.cpp
--rw-r--r--   0        0        0     1052 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/lie/lie_fixture.h
--rw-r--r--   0        0        0     1097 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/lie/lie_multiplier.cpp
--rw-r--r--   0        0        0      400 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/maps/CMakeLists.txt
--rw-r--r--   0        0        0     3200 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/maps/maps.cpp
--rw-r--r--   0        0        0     4683 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/maps/maps_fixture.h
--rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/polynomial/CMakeLists.txt
--rw-r--r--   0        0        0     1234 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/polynomial/polynomial_basis.cpp
--rw-r--r--   0        0        0      618 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/polynomial/polynomial_fixture.h
--rw-r--r--   0        0        0      688 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/tensors/CMakeLists.txt
--rw-r--r--   0        0        0     9809 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/tensors/dense_tensor.cpp
--rw-r--r--   0        0        0     1519 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/tensors/free_tensor_multiplier.cpp
--rw-r--r--   0        0        0      839 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/tensors/half_shuffle_multiplier.cpp
--rw-r--r--   0        0        0     2020 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/tensors/shuffle_tensor_multiplier.cpp
--rw-r--r--   0        0        0     9850 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/tensors/sparse_tensor.cpp
--rw-r--r--   0        0        0     2548 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/tensors/tensor_basis.cpp
--rw-r--r--   0        0        0     2526 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/tensors/tensor_fixture.h
--rw-r--r--   0        0        0     4677 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/tensors/tensor_multiplication.cpp
--rw-r--r--   0        0        0      479 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/utilities/CMakeLists.txt
--rw-r--r--   0        0        0     1863 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/utilities/packed_integer.cpp
--rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/tests/vector.cpp
--rw-r--r--   0        0        0      679 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/libalgebra_lite/vcpkg.json
--rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/.git
--rw-r--r--   0        0        0     2176 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/CMakeLists.txt
--rw-r--r--   0        0        0     1428 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/LICENSE.txt
--rw-r--r--   0        0        0     4666 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/README.md
--rw-r--r--   0        0        0     8441 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/recombine/CMakeLists.txt
--rw-r--r--   0        0        0     1363 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/recombine/recombine/BufferConstructor.h
--rw-r--r--   0        0        0     3270 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/recombine/recombine/Compare.cpp
--rw-r--r--   0        0        0     7934 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/recombine/recombine/LinearAlgebraReductionTool.cpp
--rw-r--r--   0        0        0     2313 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/recombine/recombine/LinearAlgebraReductionTool.h
--rw-r--r--   0        0        0    13604 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/recombine/recombine/RdToPowers.cpp
--rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/recombine/recombine/RdToPowers.h
--rw-r--r--   0        0        0   230430 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/recombine/recombine/SafeInt3.hpp
--rw-r--r--   0        0        0     1299 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/recombine/recombine/TreeBufferHelper.cpp
--rw-r--r--   0        0        0      931 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/recombine/recombine/TreeBufferHelper.h
--rw-r--r--   0        0        0     9792 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/recombine/recombine/aligned_allocator.h
--rw-r--r--   0        0        0     6660 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/recombine/recombine/lapack_defns.h
--rw-r--r--   0        0        0     3027 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/recombine/recombine/lapack_fortran_definitions.h
--rw-r--r--   0        0        0    14477 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/recombine/recombine/recombine.cpp
--rw-r--r--   0        0        0     4293 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/recombine/recombine/recombine.h
--rw-r--r--   0        0        0     7967 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/recombine/recombine/reweight.h
--rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/recombine/recombine/stdafx.h
--rw-r--r--   0        0        0     2538 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/recombine/recombine/tjlUtilities.h
--rw-r--r--   0        0        0      307 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/recombine/recombine.pc.in
--rw-r--r--   0        0        0     1661 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/test_recombine/CMakeLists.txt
--rw-r--r--   0        0        0     4086 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/test_recombine/TestVec/EvaluateAllMonomials.h
--rw-r--r--   0        0        0     1186 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/test_recombine/TestVec/OstreamContainerOverloads.h
--rw-r--r--   0        0        0      525 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/test_recombine/TestVec/ScopedWindowsPerformanceTimer.cpp
--rw-r--r--   0        0        0      314 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/test_recombine/TestVec/ScopedWindowsPerformanceTimer.h
--rw-r--r--   0        0        0      377 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/test_recombine/TestVec/stdafx.h
--rw-r--r--   0        0        0      306 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/test_recombine/TestVec/targetver.h
--rw-r--r--   0        0        0     1358 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/test_recombine/TestVec/utils.h
--rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/test_recombine/set_env_test_recombine.sh
--rw-r--r--   0        0        0     5597 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/test_recombine/test_recombine.cpp
--rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 roughpy-0.0.3/external/recombine/test_recombine/test_recombine.h
--rw-r--r--   0        0        0     1110 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/CMakeLists.txt
--rw-r--r--   0        0        0     3939 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/include/roughpy/intervals/dyadic.h
--rw-r--r--   0        0        0     4961 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/include/roughpy/intervals/dyadic_interval.h
--rw-r--r--   0        0        0     3017 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/include/roughpy/intervals/interval.h
--rw-r--r--   0        0        0     1394 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/include/roughpy/intervals/partition.h
--rw-r--r--   0        0        0     3211 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/include/roughpy/intervals/real_interval.h
--rw-r--r--   0        0        0     2131 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/include/roughpy/intervals/segmentation.h
--rw-r--r--   0        0        0     5705 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/src/dyadic.cpp
--rw-r--r--   0        0        0     8134 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/src/dyadic_interval.cpp
--rw-r--r--   0        0        0     9339 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/src/dyadic_searcher.cpp
--rw-r--r--   0        0        0     3525 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/src/dyadic_searcher.h
--rw-r--r--   0        0        0     4239 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/src/interval.cpp
--rw-r--r--   0        0        0     9360 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/src/partition.cpp
--rw-r--r--   0        0        0     1896 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/src/real_interval.cpp
--rw-r--r--   0        0        0     1964 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/src/scaled_predicate.cpp
--rw-r--r--   0        0        0     2286 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/src/scaled_predicate.h
--rw-r--r--   0        0        0     2216 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/src/segmentation.cpp
--rw-r--r--   0        0        0     2322 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/src/test_dyadic.cpp
--rw-r--r--   0        0        0    12091 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/src/test_dyadic_intervals.cpp
--rw-r--r--   0        0        0     7851 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/src/test_partition.cpp
--rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 roughpy-0.0.3/intervals/src/test_real_interval.cpp
--rw-r--r--   0        0        0     1101 2022-11-09 12:37:21.000000 roughpy-0.0.3/la_context/CMakeLists.txt
--rw-r--r--   0        0        0     4187 2022-11-09 12:37:21.000000 roughpy-0.0.3/la_context/include/roughpy/la_context/free_tensor_info.h
--rw-r--r--   0        0        0     6553 2022-11-09 12:37:21.000000 roughpy-0.0.3/la_context/include/roughpy/la_context/lie_basis_info.h
--rw-r--r--   0        0        0     4195 2022-11-09 12:37:21.000000 roughpy-0.0.3/la_context/include/roughpy/la_context/lie_info.h
--rw-r--r--   0        0        0     2650 2022-11-09 12:37:21.000000 roughpy-0.0.3/la_context/include/roughpy/la_context/shuffle_tensor_info.h
--rw-r--r--   0        0        0     6925 2022-11-09 12:37:21.000000 roughpy-0.0.3/la_context/include/roughpy/la_context/tensor_basis_info.h
--rw-r--r--   0        0        0      699 2022-11-09 12:37:21.000000 roughpy-0.0.3/la_context/include/roughpy/la_context/vector_iterator.h
--rw-r--r--   0        0        0     2428 2022-11-09 12:37:21.000000 roughpy-0.0.3/la_context/include/roughpy/la_context/vector_type_helper.h
--rw-r--r--   0        0        0     3263 2022-11-09 12:37:21.000000 roughpy-0.0.3/la_context/include/roughpy/la_context/vector_type_selector.h
--rw-r--r--   0        0        0    23080 2022-11-09 12:37:21.000000 roughpy-0.0.3/la_context/include/roughpy/la_context.h
--rw-r--r--   0        0        0     1780 2022-11-09 12:37:21.000000 roughpy-0.0.3/la_context/src/la_context.cpp
--rw-r--r--   0        0        0      524 2022-11-09 12:37:21.000000 roughpy-0.0.3/platform/CMakeLists.txt
--rw-r--r--   0        0        0     2839 2022-11-09 12:37:21.000000 roughpy-0.0.3/platform/include/roughpy/platform/configuration.h
--rw-r--r--   0        0        0     1302 2022-11-09 12:37:21.000000 roughpy-0.0.3/platform/include/roughpy/platform/filesystem.h
--rw-r--r--   0        0        0     9674 2022-11-09 12:37:21.000000 roughpy-0.0.3/platform/include/roughpy/platform/serialization.h
--rw-r--r--   0        0        0     4130 2022-11-09 12:37:21.000000 roughpy-0.0.3/platform/include/roughpy/platform/serialization_instantiations.inl
--rw-r--r--   0        0        0      547 2022-11-09 12:37:21.000000 roughpy-0.0.3/platform/include/roughpy/platform.h
--rw-r--r--   0        0        0     2022 2022-11-09 12:37:21.000000 roughpy-0.0.3/platform/src/configuration.cpp
--rw-r--r--   0        0        0     3248 2022-11-09 12:37:21.000000 roughpy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5427 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/CMakeLists.txt
--rw-r--r--   0        0        0     1329 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/__init__.py
--rw-r--r--   0        0        0       24 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/__init__.pyi
--rw-r--r--   0        0        0    10442 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/_roughpy.pyi
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/py.typed
--rw-r--r--   0        0        0     2339 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/algebra.cpp
--rw-r--r--   0        0        0     1867 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/algebra.h
--rw-r--r--   0        0        0     2673 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/algebra_iterator.cpp
--rw-r--r--   0        0        0     1903 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/algebra_iterator.h
--rw-r--r--   0        0        0     2865 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/basis.cpp
--rw-r--r--   0        0        0     1803 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/basis.h
--rw-r--r--   0        0        0    16086 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/context.cpp
--rw-r--r--   0        0        0     2243 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/context.h
--rw-r--r--   0        0        0     6864 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/free_tensor.cpp
--rw-r--r--   0        0        0     1827 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/free_tensor.h
--rw-r--r--   0        0        0     3804 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/lie.cpp
--rw-r--r--   0        0        0     1795 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/lie.h
--rw-r--r--   0        0        0    13067 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/lie_key.cpp
--rw-r--r--   0        0        0     2974 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/lie_key.h
--rw-r--r--   0        0        0     3581 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/lie_key_iterator.cpp
--rw-r--r--   0        0        0     2250 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/lie_key_iterator.h
--rw-r--r--   0        0        0     1749 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/lie_letter.cpp
--rw-r--r--   0        0        0     2578 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/lie_letter.h
--rw-r--r--   0        0        0     8011 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/setup_algebra_type.h
--rw-r--r--   0        0        0     4924 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/shuffle_tensor.cpp
--rw-r--r--   0        0        0     1839 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/shuffle_tensor.h
--rw-r--r--   0        0        0     5731 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/tensor_key.cpp
--rw-r--r--   0        0        0     2977 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/tensor_key.h
--rw-r--r--   0        0        0     3243 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/tensor_key_iterator.cpp
--rw-r--r--   0        0        0     2228 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/algebra/tensor_key_iterator.h
--rw-r--r--   0        0        0     4269 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/args/convert_timestamp.cpp
--rw-r--r--   0        0        0     2564 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/args/convert_timestamp.h
--rw-r--r--   0        0        0     8155 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/args/kwargs_to_path_metadata.cpp
--rw-r--r--   0        0        0     2315 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/args/kwargs_to_path_metadata.h
--rw-r--r--   0        0        0     3178 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/args/kwargs_to_vector_construction.cpp
--rw-r--r--   0        0        0     2549 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/args/kwargs_to_vector_construction.h
--rw-r--r--   0        0        0     4247 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/args/numpy.cpp
--rw-r--r--   0        0        0     2085 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/args/numpy.h
--rw-r--r--   0        0        0    13665 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/args/parse_schema.cpp
--rw-r--r--   0        0        0      786 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/args/parse_schema.h
--rw-r--r--   0        0        0    10164 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/dlpack.h
--rw-r--r--   0        0        0    11345 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/dlpack_LICENSE
--rw-r--r--   0        0        0     1367 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/intervals/date_time_interval.cpp
--rw-r--r--   0        0        0     2526 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/intervals/date_time_interval.h
--rw-r--r--   0        0        0     3143 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/intervals/dyadic.cpp
--rw-r--r--   0        0        0     1813 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/intervals/dyadic.h
--rw-r--r--   0        0        0     3976 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/intervals/dyadic_interval.cpp
--rw-r--r--   0        0        0     1849 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/intervals/dyadic_interval.h
--rw-r--r--   0        0        0     4391 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/intervals/interval.cpp
--rw-r--r--   0        0        0     2387 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/intervals/interval.h
--rw-r--r--   0        0        0     2248 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/intervals/intervals.cpp
--rw-r--r--   0        0        0     1825 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/intervals/intervals.h
--rw-r--r--   0        0        0     2978 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/intervals/partition.cpp
--rw-r--r--   0        0        0     1913 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/intervals/partition.h
--rw-r--r--   0        0        0     2778 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/intervals/real_interval.cpp
--rw-r--r--   0        0        0     1841 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/intervals/real_interval.h
--rw-r--r--   0        0        0     1984 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/intervals/segmentation.cpp
--rw-r--r--   0        0        0     1837 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/intervals/segmentation.h
--rw-r--r--   0        0        0     3931 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/recombine.cpp
--rw-r--r--   0        0        0     1798 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/recombine.h
--rw-r--r--   0        0        0     2234 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/roughpy_module.cpp
--rw-r--r--   0        0        0     2549 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/roughpy_module.h
--rw-r--r--   0        0        0    53300 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/scalars/r_py_polynomial.cpp
--rw-r--r--   0        0        0     2767 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/scalars/r_py_polynomial.h
--rw-r--r--   0        0        0    14251 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/scalars/scalar_type.cpp
--rw-r--r--   0        0        0     5932 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/scalars/scalar_type.h
--rw-r--r--   0        0        0    19658 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/scalars/scalars.cpp
--rw-r--r--   0        0        0     3487 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/scalars/scalars.h
--rw-r--r--   0        0        0     3871 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/BaseStream.cpp
--rw-r--r--   0        0        0     2937 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/BaseStream.h
--rw-r--r--   0        0        0     3427 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/brownian_stream.cpp
--rw-r--r--   0        0        0     1899 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/brownian_stream.h
--rw-r--r--   0        0        0     2768 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/externally_sourced_stream.cpp
--rw-r--r--   0        0        0      312 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/externally_sourced_stream.h
--rw-r--r--   0        0        0     4296 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/function_stream.cpp
--rw-r--r--   0        0        0     2584 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/function_stream.h
--rw-r--r--   0        0        0     6808 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/lie_increment_stream.cpp
--rw-r--r--   0        0        0     1863 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/lie_increment_stream.h
--rw-r--r--   0        0        0     3510 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/piecewise_abelian_stream.cpp
--rw-r--r--   0        0        0     1931 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/piecewise_abelian_stream.h
--rw-r--r--   0        0        0     1270 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/py_schema_context.cpp
--rw-r--r--   0        0        0     2540 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/py_schema_context.h
--rw-r--r--   0        0        0     5107 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/r_py_tick_construction_helper.cpp
--rw-r--r--   0        0        0     3919 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/r_py_tick_construction_helper.h
--rw-r--r--   0        0        0     6517 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/schema.cpp
--rw-r--r--   0        0        0     1867 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/schema.h
--rw-r--r--   0        0        0    22475 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/stream.cpp
--rw-r--r--   0        0        0     2024 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/stream.h
--rw-r--r--   0        0        0     2271 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/streams.cpp
--rw-r--r--   0        0        0     1811 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/streams.h
--rw-r--r--   0        0        0    15603 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/tick_stream.cpp
--rw-r--r--   0        0        0     1827 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/src/streams/tick_stream.h
--rw-r--r--   0        0        0     1561 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/streams/__init__.py
--rw-r--r--   0        0        0     6198 2022-11-09 12:37:21.000000 roughpy-0.0.3/roughpy/streams/tick_stream.py
--rw-r--r--   0        0        0     3228 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/CMakeLists.txt
--rw-r--r--   0        0        0      997 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/include/roughpy/scalars/conversion.h
--rw-r--r--   0        0        0     4783 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/include/roughpy/scalars/key_scalar_array.h
--rw-r--r--   0        0        0     2725 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/include/roughpy/scalars/owned_scalar_array.h
--rw-r--r--   0        0        0     2776 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/include/roughpy/scalars/random.h
--rw-r--r--   0        0        0     8620 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/include/roughpy/scalars/scalar.h
--rw-r--r--   0        0        0     3474 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/include/roughpy/scalars/scalar_array.h
--rw-r--r--   0        0        0     3142 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/include/roughpy/scalars/scalar_blas.h
--rw-r--r--   0        0        0     3004 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/include/roughpy/scalars/scalar_interface.h
--rw-r--r--   0        0        0     4213 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/include/roughpy/scalars/scalar_matrix.h
--rw-r--r--   0        0        0    13459 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/include/roughpy/scalars/scalar_pointer.h
--rw-r--r--   0        0        0     3012 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/include/roughpy/scalars/scalar_stream.h
--rw-r--r--   0        0        0     3109 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/include/roughpy/scalars/scalar_traits.h
--rw-r--r--   0        0        0    16541 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/include/roughpy/scalars/scalar_type.h
--rw-r--r--   0        0        0     6594 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/include/roughpy/scalars/scalars_fwd.h
--rw-r--r--   0        0        0     2035 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/include/roughpy/scalars.h
--rw-r--r--   0        0        0     1477 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/scalar_blas_defs.h.in
--rw-r--r--   0        0        0    17500 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/RationalType.cpp
--rw-r--r--   0        0        0     5477 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/RationalType.h
--rw-r--r--   0        0        0     2117 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/ScalarTests.h
--rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/b_float_16_type.cpp
--rw-r--r--   0        0        0     1989 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/b_float_16_type.h
--rw-r--r--   0        0        0     1848 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/bfloat16_random_generator.cpp
--rw-r--r--   0        0        0     6106 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/bfloat16_random_generator.h
--rw-r--r--   0        0        0     1736 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/double_type.cpp
--rw-r--r--   0        0        0     1931 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/double_type.h
--rw-r--r--   0        0        0    17637 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/float_blas.cpp
--rw-r--r--   0        0        0     3803 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/float_blas.h
--rw-r--r--   0        0        0     1732 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/float_type.cpp
--rw-r--r--   0        0        0     1925 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/float_type.h
--rw-r--r--   0        0        0     1836 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/half_random_generator.cpp
--rw-r--r--   0        0        0     5999 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/half_random_generator.h
--rw-r--r--   0        0        0     1790 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/half_type.cpp
--rw-r--r--   0        0        0     1955 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/half_type.h
--rw-r--r--   0        0        0     6399 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/key_scalar_array.cpp
--rw-r--r--   0        0        0     4579 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/owned_scalar_array.cpp
--rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/random_impl.cpp
--rw-r--r--   0        0        0      496 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/random_impl.h
--rw-r--r--   0        0        0    14466 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/rational_poly_scalar_type.cpp
--rw-r--r--   0        0        0     5089 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/rational_poly_scalar_type.h
--rw-r--r--   0        0        0    11521 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/scalar.cpp
--rw-r--r--   0        0        0     3931 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/scalar_array.cpp
--rw-r--r--   0        0        0     4835 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/scalar_blas.cpp
--rw-r--r--   0        0        0     6889 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/scalar_blas_impl.h
--rw-r--r--   0        0        0     1942 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/scalar_interface.cpp
--rw-r--r--   0        0        0     8248 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/scalar_matrix.cpp
--rw-r--r--   0        0        0     5961 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/scalar_pointer.cpp
--rw-r--r--   0        0        0     4525 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/scalar_stream.cpp
--rw-r--r--   0        0        0    16127 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/scalar_type.cpp
--rw-r--r--   0        0        0     1991 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/standard_random_generator.cpp
--rw-r--r--   0        0        0     6903 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/standard_random_generator.h
--rw-r--r--   0        0        0    21578 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/standard_scalar_type.h
--rw-r--r--   0        0        0     2731 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/test_float_blas.cpp
--rw-r--r--   0        0        0     3307 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/test_key_scalar_array.cpp
--rw-r--r--   0        0        0     2518 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/test_pcg_standard_random.cpp
--rw-r--r--   0        0        0     6701 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/test_scalar.cpp
--rw-r--r--   0        0        0     2590 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/test_scalar_array.cpp
--rw-r--r--   0        0        0     2723 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/test_scalar_matrix.cpp
--rw-r--r--   0        0        0     5404 2022-11-09 12:37:21.000000 roughpy-0.0.3/scalars/src/test_scalar_type.cpp
--rw-r--r--   0        0        0     4201 2022-11-09 12:37:21.000000 roughpy-0.0.3/setup.py
--rw-r--r--   0        0        0     1932 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/CMakeLists.txt
--rw-r--r--   0        0        0     4501 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/include/roughpy/streams/brownian_stream.h
--rw-r--r--   0        0        0     9020 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/include/roughpy/streams/channels.h
--rw-r--r--   0        0        0     3945 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/include/roughpy/streams/dyadic_caching_layer.h
--rw-r--r--   0        0        0     8489 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/include/roughpy/streams/dynamically_constructed_stream.h
--rw-r--r--   0        0        0     4118 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/include/roughpy/streams/external_data_stream.h
--rw-r--r--   0        0        0     3758 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/include/roughpy/streams/lie_increment_stream.h
--rw-r--r--   0        0        0     4018 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/include/roughpy/streams/piecewise_abelian_stream.h
--rw-r--r--   0        0        0     8084 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/include/roughpy/streams/schema.h
--rw-r--r--   0        0        0      929 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/include/roughpy/streams/schema_context.h
--rw-r--r--   0        0        0     5632 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/include/roughpy/streams/stream.h
--rw-r--r--   0        0        0     7645 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/include/roughpy/streams/stream_base.h
--rw-r--r--   0        0        0     4597 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/include/roughpy/streams/stream_construction_helper.h
--rw-r--r--   0        0        0     6020 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/include/roughpy/streams/tick_stream.h
--rw-r--r--   0        0        0     3595 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/brownian_stream.cpp
--rw-r--r--   0        0        0    15358 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/channels.cpp
--rw-r--r--   0        0        0     4949 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/dyadic_caching_layer.cpp
--rw-r--r--   0        0        0    14792 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/dynamically_constructed_stream.cpp
--rw-r--r--   0        0        0     1823 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/external_data_sources/csv_data_source.cpp
--rw-r--r--   0        0        0     2273 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/external_data_sources/csv_data_source.h
--rw-r--r--   0        0        0    10976 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/external_data_sources/sound_file_data_source.cpp
--rw-r--r--   0        0        0     4278 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/external_data_sources/sound_file_data_source.h
--rw-r--r--   0        0        0     7343 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/external_data_stream.cpp
--rw-r--r--   0        0        0     5126 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/lie_increment_stream.cpp
--rw-r--r--   0        0        0     7701 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/piecewise_abelian_stream.cpp
--rw-r--r--   0        0        0     9413 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/schema.cpp
--rw-r--r--   0        0        0     1981 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/schema_context.cpp
--rw-r--r--   0        0        0     9468 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/stream.cpp
--rw-r--r--   0        0        0     4131 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/stream_base.cpp
--rw-r--r--   0        0        0     4749 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/stream_construction_helper.cpp
--rw-r--r--   0        0        0     3902 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/test_brownian_stream.cpp
--rw-r--r--   0        0        0     5285 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/test_lie_increment_stream.cpp
--rw-r--r--   0        0        0     8105 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/test_schema.cpp
--rw-r--r--   0        0        0    10348 2022-11-09 12:37:21.000000 roughpy-0.0.3/streams/src/tick_stream.cpp
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/algebra/__init__.py
--rw-r--r--   0        0        0     3303 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/algebra/test_alg_poly_coeffs.py
--rw-r--r--   0        0        0     1975 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/algebra/test_algebra_context.py
--rw-r--r--   0        0        0    11620 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/algebra/test_free_tensor.py
--rw-r--r--   0        0        0     4614 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/algebra/test_lie.py
--rw-r--r--   0        0        0      614 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/algebra/test_lie_keys.py
--rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/algebra/test_tensor_iterator.py
--rw-r--r--   0        0        0     2039 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/algebra/test_tensor_keys.py
--rw-r--r--   0        0        0      685 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/intervals/__init__.py
--rw-r--r--   0        0        0      458 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/intervals/test_dyadic.py
--rw-r--r--   0        0        0     2507 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/intervals/test_intervals.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/scalars/__init__.py
--rw-r--r--   0        0        0     1396 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/scalars/test_monomial.py
--rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/scalars/test_polynomial.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/streams/__init__.py
--rw-r--r--   0        0        0   187338 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/streams/audio/test.flac
--rw-r--r--   0        0        0    44146 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/streams/audio/test.mp3
--rw-r--r--   0        0        0   311172 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/streams/audio/test.wav
--rw-r--r--   0        0        0     2291 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/streams/test_brownian_stream.py
--rw-r--r--   0        0        0     4341 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/streams/test_function_path.py
--rw-r--r--   0        0        0     7810 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/streams/test_lie_increment_path.py
--rw-r--r--   0        0        0     1482 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/streams/test_piecewise_lie_path.py
--rw-r--r--   0        0        0     6231 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/streams/test_schema.py
--rw-r--r--   0        0        0     2397 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/streams/test_sound_path.py
--rw-r--r--   0        0        0     4142 2022-11-09 12:37:21.000000 roughpy-0.0.3/tests/streams/test_tick_stream.py
--rw-r--r--   0        0        0     2763 2022-11-09 12:37:21.000000 roughpy-0.0.3/tools/ci/before-all-common.sh
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 roughpy-0.0.3/tools/ci/triplets/arm-uwp.cmake
--rw-r--r--   0        0        0      155 2022-11-09 12:37:21.000000 roughpy-0.0.3/tools/ci/triplets/arm64-windows.cmake
--rw-r--r--   0        0        0       30 2022-11-09 12:37:21.000000 roughpy-0.0.3/tools/ci/triplets/common.cmake
--rw-r--r--   0        0        0      184 2022-11-09 12:37:21.000000 roughpy-0.0.3/tools/ci/triplets/x64-linux.cmake
--rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 roughpy-0.0.3/tools/ci/triplets/x64-osx.cmake
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 roughpy-0.0.3/tools/ci/triplets/x64-uwp.cmake
--rw-r--r--   0        0        0      147 2022-11-09 12:37:21.000000 roughpy-0.0.3/tools/ci/triplets/x64-windows-static.cmake
--rw-r--r--   0        0        0      148 2022-11-09 12:37:21.000000 roughpy-0.0.3/tools/ci/triplets/x64-windows.cmake
--rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 roughpy-0.0.3/tools/ci/triplets/x86-windows.cmake
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.3/tools/ports/libalgebra/portfile.cmake
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.3/tools/ports/libalgebra/vcpkg.json
--rw-r--r--   0        0        0      204 2022-11-09 12:37:21.000000 roughpy-0.0.3/tools/ports/libalgebra-lite/portfile.cmake
--rw-r--r--   0        0        0      356 2022-11-09 12:37:21.000000 roughpy-0.0.3/tools/ports/libalgebra-lite/vcpkg.json
--rw-r--r--   0        0        0     4396 2022-11-09 12:37:21.000000 roughpy-0.0.3/tools/python-get-binary-obj-path.py
--rw-r--r--   0        0        0     2511 2022-11-09 12:37:21.000000 roughpy-0.0.3/tools/version_from_file.py
--rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 roughpy-0.0.3/vcpkg.json
--rw-r--r--   0        0        0     5151 2022-11-09 12:37:21.000000 roughpy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2345 2022-11-09 12:37:21.000000 roughpy-0.0.4/.clang-format
+-rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 roughpy-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2022-11-09 12:37:21.000000 roughpy-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     3994 2022-11-09 12:37:21.000000 roughpy-0.0.4/.github/workflows/build_wheels.yml
+-rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 roughpy-0.0.4/.github/workflows/manage_version.yml
+-rw-r--r--   0        0        0     2733 2022-11-09 12:37:21.000000 roughpy-0.0.4/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     5667 2022-11-09 12:37:21.000000 roughpy-0.0.4/.gitignore
+-rw-r--r--   0        0        0      433 2022-11-09 12:37:21.000000 roughpy-0.0.4/.gitmodules
+-rw-r--r--   0        0        0     1212 2022-11-09 12:37:21.000000 roughpy-0.0.4/CHANGELOG
+-rw-r--r--   0        0        0     9736 2022-11-09 12:37:21.000000 roughpy-0.0.4/CMakeLists.txt
+-rw-r--r--   0        0        0     1489 2022-11-09 12:37:21.000000 roughpy-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     4108 2022-11-09 12:37:21.000000 roughpy-0.0.4/README.md
+-rw-r--r--   0        0        0      743 2022-11-09 12:37:21.000000 roughpy-0.0.4/THANKS.txt
+-rw-r--r--   0        0        0        7 2022-11-09 12:37:21.000000 roughpy-0.0.4/VERSION.txt
+-rw-r--r--   0        0        0     3262 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/CMakeLists.txt
+-rw-r--r--   0        0        0    16233 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_base.h
+-rw-r--r--   0        0        0    23529 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_base_impl.h
+-rw-r--r--   0        0        0     8100 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_bundle.h
+-rw-r--r--   0        0        0    13572 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_bundle_base_impl.h
+-rw-r--r--   0        0        0    26323 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_bundle_impl.h
+-rw-r--r--   0        0        0     2737 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_fwd.h
+-rw-r--r--   0        0        0    31744 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_impl.h
+-rw-r--r--   0        0        0     3829 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_info.h
+-rw-r--r--   0        0        0     7137 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_iterator.h
+-rw-r--r--   0        0        0     3740 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_iterator_impl.h
+-rw-r--r--   0        0        0     9250 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/basis.h
+-rw-r--r--   0        0        0     6672 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/basis_impl.h
+-rw-r--r--   0        0        0     6334 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/basis_info.h
+-rw-r--r--   0        0        0      195 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/bundle_info.h
+-rw-r--r--   0        0        0     9538 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/context.h
+-rw-r--r--   0        0        0     4148 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/context_fwd.h
+-rw-r--r--   0        0        0     1881 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/fallback_operations.h
+-rw-r--r--   0        0        0     2707 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/free_tensor.h
+-rw-r--r--   0        0        0     3750 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/free_tensor_fwd.h
+-rw-r--r--   0        0        0     6431 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/free_tensor_impl.h
+-rw-r--r--   0        0        0     2730 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/lie.h
+-rw-r--r--   0        0        0     2088 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/lie_basis.h
+-rw-r--r--   0        0        0     1852 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/lie_fwd.h
+-rw-r--r--   0        0        0     2633 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/linear_operator.h
+-rw-r--r--   0        0        0     2874 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/shuffle_tensor.h
+-rw-r--r--   0        0        0     1858 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/shuffle_tensor_fwd.h
+-rw-r--r--   0        0        0     2192 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/include/roughpy/algebra/tensor_basis.h
+-rw-r--r--   0        0        0     1905 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/ContextFixture.cpp
+-rw-r--r--   0        0        0     2186 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/ContextFixture.h
+-rw-r--r--   0        0        0     3000 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/algebra_base.cpp
+-rw-r--r--   0        0        0     1703 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/algebra_iterator.cpp
+-rw-r--r--   0        0        0     1747 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/basis.cpp
+-rw-r--r--   0        0        0     9768 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/context.cpp
+-rw-r--r--   0        0        0     1737 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/double_lite_context.cpp
+-rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/float_lite_context.cpp
+-rw-r--r--   0        0        0     4084 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/free_tensor.cpp
+-rw-r--r--   0        0        0     4248 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/hall_set_size.cpp
+-rw-r--r--   0        0        0     2569 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/hall_set_size.h
+-rw-r--r--   0        0        0     3031 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/dense_vector_iterator.h
+-rw-r--r--   0        0        0     4222 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/free_tensor_info.h
+-rw-r--r--   0        0        0     6669 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/lie_basis_info.h
+-rw-r--r--   0        0        0     4191 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/lie_info.h
+-rw-r--r--   0        0        0     3099 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/lite_vector_selector.h
+-rw-r--r--   0        0        0     4223 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/shuffle_tensor_info.h
+-rw-r--r--   0        0        0     5973 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/sparse_mutable_ref_scalar_trait.h
+-rw-r--r--   0        0        0     2450 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/sparse_vector_iterator.h
+-rw-r--r--   0        0        0     6642 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/tensor_basis_info.h
+-rw-r--r--   0        0        0     2366 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/libalgebra_lite_internal/vector_type_helper.h
+-rw-r--r--   0        0        0     2490 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/lie.cpp
+-rw-r--r--   0        0        0     1821 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/lie_basis.cpp
+-rw-r--r--   0        0        0     4732 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/lite_context.cpp
+-rw-r--r--   0        0        0    28170 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/lite_context.h
+-rw-r--r--   0        0        0     1737 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/rational_lite_context.cpp
+-rw-r--r--   0        0        0     1739 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/rational_poly_lite_context.cpp
+-rw-r--r--   0        0        0     2734 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/shuffle_tensor.cpp
+-rw-r--r--   0        0        0     1883 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/tensor_basis.cpp
+-rw-r--r--   0        0        0     1758 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/test_lie.cpp
+-rw-r--r--   0        0        0     1631 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/testing/mock_context.cpp
+-rw-r--r--   0        0        0     2139 2022-11-09 12:37:21.000000 roughpy-0.0.4/algebra/src/testing/mock_context.h
+-rw-r--r--   0        0        0   106087 2022-11-09 12:37:21.000000 roughpy-0.0.4/branding/logo/logo_square_white.jpg
+-rw-r--r--   0        0        0      509 2022-11-09 12:37:21.000000 roughpy-0.0.4/cmake/Modules/FindPCGRandom.cmake
+-rw-r--r--   0        0        0    20238 2022-11-09 12:37:21.000000 roughpy-0.0.4/cmake/roughpy_helpers.cmake
+-rw-r--r--   0        0        0      355 2022-11-09 12:37:21.000000 roughpy-0.0.4/cmake/version.py.in
+-rw-r--r--   0        0        0      495 2022-11-09 12:37:21.000000 roughpy-0.0.4/core/CMakeLists.txt
+-rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 roughpy-0.0.4/core/include/roughpy/core/alloc.h
+-rw-r--r--   0        0        0     3627 2022-11-09 12:37:21.000000 roughpy-0.0.4/core/include/roughpy/core/helpers.h
+-rw-r--r--   0        0        0    10918 2022-11-09 12:37:21.000000 roughpy-0.0.4/core/include/roughpy/core/macros.h
+-rw-r--r--   0        0        0     4701 2022-11-09 12:37:21.000000 roughpy-0.0.4/core/include/roughpy/core/slice.h
+-rw-r--r--   0        0        0     5000 2022-11-09 12:37:21.000000 roughpy-0.0.4/core/include/roughpy/core/traits.h
+-rw-r--r--   0        0        0     2628 2022-11-09 12:37:21.000000 roughpy-0.0.4/core/include/roughpy/core/types.h
+-rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/CMakeLists.txt
+-rw-r--r--   0        0        0       66 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/cuda/CMakeLists.txt
+-rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/cuda/CudaDeviceContext.cu
+-rw-r--r--   0        0        0     1975 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/cuda/CudaDeviceContext.cuh
+-rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/cuda/scalars/CMakeLists.txt
+-rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/cuda/scalars/src/CUDAFloatType.cu
+-rw-r--r--   0        0        0     2005 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/cuda/scalars/src/CUDAFloatType.cuh
+-rw-r--r--   0        0        0     8605 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/cuda/scalars/src/CUDA_standard_scalar.cuh
+-rw-r--r--   0        0        0      868 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/include/roughpy/device/core.h
+-rw-r--r--   0        0        0    18540 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/include/roughpy/device/device_algebra_base.h
+-rw-r--r--   0        0        0     4377 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/include/roughpy/device/device_context.h
+-rw-r--r--   0        0        0     2348 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/kernels/binary_kernel.cuh
+-rw-r--r--   0        0        0     3972 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/kernels/functors.h
+-rw-r--r--   0        0        0     1712 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/kernels/tmp.cu
+-rw-r--r--   0        0        0     2304 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/kernels/unary_kernel.cuh
+-rw-r--r--   0        0        0     1801 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/src/device_algebra_base.cpp
+-rw-r--r--   0        0        0     1728 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/src/device_context.cpp
+-rw-r--r--   0        0        0     2854 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/src/device_free_tensor.cpp
+-rw-r--r--   0        0        0     2912 2022-11-09 12:37:21.000000 roughpy-0.0.4/device/src/device_free_tensor.h
+-rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 roughpy-0.0.4/docs/make.bat
+-rw-r--r--   0        0        0     1151 2022-11-09 12:37:21.000000 roughpy-0.0.4/docs/source/conf.py
+-rw-r--r--   0        0        0      437 2022-11-09 12:37:21.000000 roughpy-0.0.4/docs/source/index.rst
+-rw-r--r--   0        0        0     3589 2022-11-09 12:37:21.000000 roughpy-0.0.4/examples/lie_to_tensor_formulae.py
+-rw-r--r--   0        0        0     1956 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/.clang-format
+-rw-r--r--   0        0        0       47 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/.git
+-rw-r--r--   0        0        0     5992 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/.gitignore
+-rw-r--r--   0        0        0     7502 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/CMakeLists.txt
+-rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/Dockerfile
+-rw-r--r--   0        0        0     1839 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/Dockerfile.remote-cpp-env
+-rw-r--r--   0        0        0      335 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/LibalgebraConfig.cmake.in
+-rw-r--r--   0        0        0     2706 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/README.md
+-rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/benchmarks/CMakeLists.txt
+-rw-r--r--   0        0        0      414 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/benchmarks/antipode/CMakeLists.txt
+-rw-r--r--   0        0        0     5078 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/benchmarks/antipode/antipode_bm.cpp
+-rw-r--r--   0        0        0     1941 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/benchmarks/multiplication/CMakeLists.txt
+-rw-r--r--   0        0        0    14501 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/benchmarks/multiplication/multiplication_bm.cpp
+-rw-r--r--   0        0        0     2363 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/benchmarks/multiplication/multiplication_single.cpp
+-rw-r--r--   0        0        0     1494 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/cmake/Modules/FindBignum.cmake
+-rw-r--r--   0        0        0     3540 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/cmake/Modules/UnitTestPP.cmake
+-rw-r--r--   0        0        0     4012 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/cmake/Modules/UnitTestPP_DiscoverTests.cmake
+-rw-r--r--   0        0        0     1602 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/cmake/libalgebra_test_helper.cmake
+-rw-r--r--   0        0        0    19400 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/_tensor_basis.h
+-rw-r--r--   0        0        0     5123 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/alg_types.h
+-rw-r--r--   0        0        0    33383 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/algebra.h
+-rw-r--r--   0        0        0     4069 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/alternative_multiplications.h
+-rw-r--r--   0        0        0     2188 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/area_tensor_basis.h
+-rw-r--r--   0        0        0    10008 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/area_tensor_multiplication.h
+-rw-r--r--   0        0        0     1336 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/base_basis.h
+-rw-r--r--   0        0        0     2600 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/base_vector.h
+-rw-r--r--   0        0        0     3202 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/basis.h
+-rw-r--r--   0        0        0    12663 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/coefficients/gmp_ser.h
+-rw-r--r--   0        0        0     5981 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/coefficients.h
+-rw-r--r--   0        0        0      389 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/complex.h
+-rw-r--r--   0        0        0      772 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/composition_operator.h
+-rw-r--r--   0        0        0     1291 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/constlog2.h
+-rw-r--r--   0        0        0     2065 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/constpower.h
+-rw-r--r--   0        0        0    25576 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/dense_storage.h
+-rw-r--r--   0        0        0    32612 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/dense_vector.h
+-rw-r--r--   0        0        0     1684 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/caching_tags.h
+-rw-r--r--   0        0        0      960 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/function_extension_cache_base.h
+-rw-r--r--   0        0        0     4044 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/integer_maths.h
+-rw-r--r--   0        0        0     1536 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/level_walkers.h
+-rw-r--r--   0        0        0     3387 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/meta.h
+-rw-r--r--   0        0        0      463 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/order_trait.h
+-rw-r--r--   0        0        0     1067 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/platform.h
+-rw-r--r--   0        0        0     3762 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/reversing_permutation.h
+-rw-r--r--   0        0        0      545 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/smallest_int_type.h
+-rw-r--r--   0        0        0     6839 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/detail/unpacked_tensor_word.h
+-rw-r--r--   0        0        0     3535 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/dot_product_implementations.h
+-rw-r--r--   0        0        0     2824 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/free_extension.h
+-rw-r--r--   0        0        0     1303 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/functionals.h
+-rw-r--r--   0        0        0     2193 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/half_shuffle_tensor_basis.h
+-rw-r--r--   0        0        0    10154 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/half_shuffle_tensor_multiplication.h
+-rw-r--r--   0        0        0    21063 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/hall_set.h
+-rw-r--r--   0        0        0    40389 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/hybrid_vector.h
+-rw-r--r--   0        0        0     2519 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/implementation_types.h
+-rw-r--r--   0        0        0     3360 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/iterators.h
+-rw-r--r--   0        0        0     4414 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/key_iterators.h
+-rw-r--r--   0        0        0     6487 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/libalgebra.h
+-rw-r--r--   0        0        0     6024 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/lie.h
+-rw-r--r--   0        0        0    17479 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/lie_basis.h
+-rw-r--r--   0        0        0     3791 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/lie_inner_product.h
+-rw-r--r--   0        0        0     7234 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/monomial_basis.h
+-rw-r--r--   0        0        0      886 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/mpfloat_coefficients.h
+-rw-r--r--   0        0        0     1033 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/multi_linear_operators.h
+-rw-r--r--   0        0        0     5991 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/multi_polynomial.h
+-rw-r--r--   0        0        0     1693 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/multiplication_helpers.h
+-rw-r--r--   0        0        0     9179 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/operators.h
+-rw-r--r--   0        0        0     5565 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/poly_basis.h
+-rw-r--r--   0        0        0     6082 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/poly_lie.h
+-rw-r--r--   0        0        0     3450 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/poly_lie_basis.h
+-rw-r--r--   0        0        0      640 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/polynomial_coefficients.h
+-rw-r--r--   0        0        0     6720 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/polynomials.h
+-rw-r--r--   0        0        0      779 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/rational_coefficients.h
+-rw-r--r--   0        0        0     5880 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/reconfigure_operator.h
+-rw-r--r--   0        0        0     8186 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/scalar_bundle.h
+-rw-r--r--   0        0        0      982 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/scalar_multiply_operator.h
+-rw-r--r--   0        0        0    41789 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/sparse_vector.h
+-rw-r--r--   0        0        0      621 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/sum_operator.h
+-rw-r--r--   0        0        0     1475 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/tags.h
+-rw-r--r--   0        0        0   144218 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/tensor.h
+-rw-r--r--   0        0        0    19208 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/tensor_basis.h
+-rw-r--r--   0        0        0     1724 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/tensor_operator.h
+-rw-r--r--   0        0        0    11862 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/utils.h
+-rw-r--r--   0        0        0    24861 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/vector.h
+-rw-r--r--   0        0        0    31254 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/vector_bundle.h
+-rw-r--r--   0        0        0     1309 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/libalgebra/vectors.h
+-rw-r--r--   0        0        0     1267 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/CMakeLists.txt
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/README.md
+-rw-r--r--   0        0        0     1324 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/CMakeLists.txt
+-rw-r--r--   0        0        0     1872 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/SHOW.h
+-rw-r--r--   0        0        0     2676 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/compat.h
+-rw-r--r--   0        0        0     1058 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/helpers.h
+-rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/memfile.cpp
+-rw-r--r--   0        0        0     3236 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/memfile.h
+-rw-r--r--   0        0        0     4234 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/multi_test.h
+-rw-r--r--   0        0        0     1554 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/random_coeffs.h
+-rw-r--r--   0        0        0     2483 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/random_vector_generator.h
+-rw-r--r--   0        0        0     1467 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/reporter.cpp
+-rw-r--r--   0        0        0      670 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/reporter.h
+-rw-r--r--   0        0        0     1711 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/rng.h
+-rw-r--r--   0        0        0     2972 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/run_tests.cpp
+-rw-r--r--   0        0        0     1102 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/simple_basis.h
+-rw-r--r--   0        0        0     2372 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/common/time_and_details.h
+-rw-r--r--   0        0        0     3181 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/AlgebraFunctionsTests.cpp
+-rw-r--r--   0        0        0      477 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/CMakeLists.txt
+-rw-r--r--   0        0        0     5679 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/HallSetTests.cpp
+-rw-r--r--   0        0        0     4658 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/LatticePathTests.cpp
+-rw-r--r--   0        0        0      511 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/LibAlgebraUnitTests.cpp
+-rw-r--r--   0        0        0    43337 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/MemoryMappedFilesDocumentation.htm
+-rw-r--r--   0        0        0     1250 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/OMPSigsTests.cpp
+-rw-r--r--   0        0        0     2877 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/SigHelpers.h
+-rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/TreeBufferHelper.cpp
+-rw-r--r--   0        0        0     1516 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/TreeBufferHelper.h
+-rw-r--r--   0        0        0      477 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/alg_framework.h
+-rw-r--r--   0        0        0     1989 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/brown_path_increments.h
+-rw-r--r--   0        0        0     2936 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/categorical_path.h
+-rw-r--r--   0        0        0      440 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/log2ceil.h
+-rw-r--r--   0        0        0      844 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/makebm.cpp
+-rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/makebm.h
+-rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/CMakeLists.txt
+-rw-r--r--   0        0        0    17054 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/accuracy_suite.ins
+-rw-r--r--   0        0        0     1817 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/coefficient_path_suite.ins
+-rw-r--r--   0        0        0     1579 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/double_path_suite.ins
+-rw-r--r--   0        0        0     1570 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/float_path_suite.ins
+-rw-r--r--   0        0        0     1224 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/generic_coefficient.h
+-rw-r--r--   0        0        0     1383 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/generic_lie_increment.h
+-rw-r--r--   0        0        0     2240 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/generic_path.h
+-rw-r--r--   0        0        0     1580 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/rational_path_suite.ins
+-rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/run_tests.cpp
+-rw-r--r--   0        0        0    20566 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/test_brownian_path.cpp
+-rw-r--r--   0        0        0    11406 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/test_innovative_path.cpp
+-rw-r--r--   0        0        0     5309 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/speed_tests.cpp
+-rw-r--r--   0        0        0    12166 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/tests_TENSOR_LIE_CBH_MAPS.cpp
+-rw-r--r--   0        0        0     6213 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/tests_libalgebra-demo.cpp
+-rw-r--r--   0        0        0     1590 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/integration_tests/x64sigs.cpp
+-rw-r--r--   0        0        0      480 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/CMakeLists.txt
+-rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/adjoint/CMakeLists.txt
+-rw-r--r--   0        0        0     7719 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/adjoint/test_adjoint.cpp
+-rw-r--r--   0        0        0      609 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/CMakeLists.txt
+-rw-r--r--   0        0        0     2223 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/alg_mul_suite.h
+-rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/framework_fixture.h
+-rw-r--r--   0        0        0      804 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/simple_algebra_basis.h
+-rw-r--r--   0        0        0      696 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/test_algebra_product.cpp
+-rw-r--r--   0        0        0       57 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/antipode/CMakeLists.txt
+-rw-r--r--   0        0        0     7994 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/antipode/test_antipode.cpp
+-rw-r--r--   0        0        0      188 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/basis/CMakeLists.txt
+-rw-r--r--   0        0        0     2232 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/basis/basis_iteration_suite.h
+-rw-r--r--   0        0        0     3917 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/basis/test_basis_iteration.cpp
+-rw-r--r--   0        0        0      612 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/basis/test_lie_basis_iteration.cpp
+-rw-r--r--   0        0        0      408 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/basis/test_tensor_basis_iteration.cpp
+-rw-r--r--   0        0        0      299 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/CMakeLists.txt
+-rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/polynomial_coeff_ring.cpp
+-rw-r--r--   0        0        0      791 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/standard_coefficient_test_suite.h
+-rw-r--r--   0        0        0      382 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/test_double_field.cpp
+-rw-r--r--   0        0        0      378 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/test_float_field.cpp
+-rw-r--r--   0        0        0      660 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/test_mpfloat_fallback_field.cpp
+-rw-r--r--   0        0        0      441 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/test_mpfloat_field.cpp
+-rw-r--r--   0        0        0      602 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/test_rational_fallback_field.cpp
+-rw-r--r--   0        0        0      506 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/test_rational_field.cpp
+-rw-r--r--   0        0        0     1789 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/unital_coefficient_test_suite.h
+-rw-r--r--   0        0        0       83 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/half-shuffle-tests/CMakeLists.txt
+-rw-r--r--   0        0        0    19137 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/half-shuffle-tests/half_shuffle_fixture.h
+-rw-r--r--   0        0        0     8440 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/half-shuffle-tests/test_half_shuffle.cpp
+-rw-r--r--   0        0        0       74 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/hall_set/CMakeLists.txt
+-rw-r--r--   0        0        0     8138 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/hall_set/test_hall_set.cpp
+-rw-r--r--   0        0        0      208 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/CMakeLists.txt
+-rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/run_tests.cpp
+-rw-r--r--   0        0        0      541 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_basis.cpp
+-rw-r--r--   0        0        0     2083 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_dense_lie_multiplication.cpp
+-rw-r--r--   0        0        0     1771 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_function_extension.cpp
+-rw-r--r--   0        0        0     5505 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_hall_basis.cpp
+-rw-r--r--   0        0        0     1663 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_lie_multiplication.cpp
+-rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/multipoly/CMakeLists.txt
+-rw-r--r--   0        0        0      499 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/multipoly/test_multipoly_prod.cpp
+-rw-r--r--   0        0        0      387 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/CMakeLists.txt
+-rw-r--r--   0        0        0     2816 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_free_extension.cpp
+-rw-r--r--   0        0        0     1466 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_lie_inner_product.cpp
+-rw-r--r--   0        0        0     2406 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_operator_composition.cpp
+-rw-r--r--   0        0        0     1548 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_operator_sum.cpp
+-rw-r--r--   0        0        0     1791 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_operators_smul.cpp
+-rw-r--r--   0        0        0     1203 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_recalibrate_operator.cpp
+-rw-r--r--   0        0        0     4353 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_shuffle_functional.cpp
+-rw-r--r--   0        0        0     2553 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_tensor_defined_operator.cpp
+-rw-r--r--   0        0        0     1785 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_tensor_multiplication_operator.cpp
+-rw-r--r--   0        0        0      552 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/CMakeLists.txt
+-rw-r--r--   0        0        0     3057 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/dense_vec_serialization.cpp
+-rw-r--r--   0        0        0      398 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/fixture.cpp
+-rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/fixture.h
+-rw-r--r--   0        0        0     4014 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/hybrid_vector_serialization.cpp
+-rw-r--r--   0        0        0     7910 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/sparse_vector_serialization.cpp
+-rw-r--r--   0        0        0      548 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/temporary_directory.cpp
+-rw-r--r--   0        0        0      419 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/temporary_directory.h
+-rw-r--r--   0        0        0     2991 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/test_dense_storage.cpp
+-rw-r--r--   0        0        0     1771 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/test_hall_set_serialize.cpp
+-rw-r--r--   0        0        0     2805 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/test_higher_classes.cpp
+-rw-r--r--   0        0        0       86 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/shuffle-tensor-tests/CMakeLists.txt
+-rw-r--r--   0        0        0    43877 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/shuffle-tensor-tests/test_shuffle_tensor.cpp
+-rw-r--r--   0        0        0      753 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tangents/CMakeLists.txt
+-rw-r--r--   0        0        0    20887 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tangents/test_tangents.cpp
+-rw-r--r--   0        0        0      465 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tangents/test_tangents.h
+-rw-r--r--   0        0        0      983 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/CMakeLists.txt
+-rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/run_tests.cpp
+-rw-r--r--   0        0        0     3985 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/tensor_exp_suite.h
+-rw-r--r--   0        0        0     1797 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/tensor_inverse_suite.h
+-rw-r--r--   0        0        0     4055 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/tensor_log_suite.h
+-rw-r--r--   0        0        0     3037 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/tensor_roundtrip_suite.h
+-rw-r--r--   0        0        0     5062 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_basis.cpp
+-rw-r--r--   0        0        0     2509 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_dense_tensor_functions.cpp
+-rw-r--r--   0        0        0     4824 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_dense_tensor_multiplication.cpp
+-rw-r--r--   0        0        0     2544 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_hybrid_tensor_functions.cpp
+-rw-r--r--   0        0        0     5037 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_hybrid_tensor_multiplication.cpp
+-rw-r--r--   0        0        0     2805 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_signature_calc.cpp
+-rw-r--r--   0        0        0     2535 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_sparse_tensor_functions.cpp
+-rw-r--r--   0        0        0     4900 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_sparse_tensor_multiplication.cpp
+-rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_tensor_creation.cpp
+-rw-r--r--   0        0        0     3291 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_tensor_functions.cpp
+-rw-r--r--   0        0        0    38059 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_tensor_multiplication.cpp
+-rw-r--r--   0        0        0     2419 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_tensor_size_info.cpp
+-rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/utils/CMakeLists.txt
+-rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/utils/run_tests.cpp
+-rw-r--r--   0        0        0     2678 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/utils/test_integer_maths.cpp
+-rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/CMakeLists.txt
+-rw-r--r--   0        0        0     3599 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/framework_fixture.h
+-rw-r--r--   0        0        0      266 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/run_tests.cpp
+-rw-r--r--   0        0        0      804 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/test_dense.cpp
+-rw-r--r--   0        0        0    13508 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/test_dense_storage.cpp
+-rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/test_hybrid.cpp
+-rw-r--r--   0        0        0      968 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/test_sparse.cpp
+-rw-r--r--   0        0        0    12957 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_arithmetic_suite.h
+-rw-r--r--   0        0        0    11707 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_binary_transform_suite.h
+-rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_comparison_suite.h
+-rw-r--r--   0        0        0     1134 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_element_access_suite.h
+-rw-r--r--   0        0        0     7086 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_iterator_suite.h
+-rw-r--r--   0        0        0     1907 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_norm_suite.h
+-rw-r--r--   0        0        0     2723 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_properties_suite.h
+-rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/width1_tests/CMakeLists.txt
+-rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/width1_tests/types.cpp
+-rw-r--r--   0        0        0      383 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/width1_tests/width1.h
+-rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/width1_tests/width1_lie.cpp
+-rw-r--r--   0        0        0     4024 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra/tests/unit_tests/width1_tests/width1_tensors.cpp
+-rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/.git
+-rw-r--r--   0        0        0     5359 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/CMakeLists.txt
+-rw-r--r--   0        0        0       18 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/README.md
+-rw-r--r--   0        0        0      485 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/cmake/Libalgebra_liteConfig.cmake.in
+-rw-r--r--   0        0        0      247 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/cmake/config.h.in
+-rw-r--r--   0        0        0     2787 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/cmake/lalhelpers.cmake
+-rw-r--r--   0        0        0      561 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/cmake/rationals.h.in
+-rw-r--r--   0        0        0    31148 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/algebra.h
+-rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/basis.h
+-rw-r--r--   0        0        0     3322 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/basis_traits.h
+-rw-r--r--   0        0        0     3141 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/coefficients.h
+-rw-r--r--   0        0        0    13187 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/dense_vector.h
+-rw-r--r--   0        0        0      457 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/detail/integer_maths.h
+-rw-r--r--   0        0        0     2875 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/detail/macros.h
+-rw-r--r--   0        0        0     1370 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/detail/notnull.h
+-rw-r--r--   0        0        0     2796 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/detail/traits.h
+-rw-r--r--   0        0        0    29648 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/free_tensor.h
+-rw-r--r--   0        0        0     6649 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/hall_set.h
+-rw-r--r--   0        0        0     1242 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/implementation_types.h
+-rw-r--r--   0        0        0     4878 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/index_key.h
+-rw-r--r--   0        0        0      809 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/key_range.h
+-rw-r--r--   0        0        0     1890 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/lie.h
+-rw-r--r--   0        0        0     7253 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/maps.h
+-rw-r--r--   0        0        0     6637 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/operators.h
+-rw-r--r--   0        0        0     7010 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/packed_integer.h
+-rw-r--r--   0        0        0     3643 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/polynomial.h
+-rw-r--r--   0        0        0     4088 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/polynomial_basis.h
+-rw-r--r--   0        0        0     2604 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/registry.h
+-rw-r--r--   0        0        0    14411 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/shuffle_tensor.h
+-rw-r--r--   0        0        0    14014 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/sparse_vector.h
+-rw-r--r--   0        0        0     3125 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/tensor_basis.h
+-rw-r--r--   0        0        0     2937 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/unpacked_tensor_word.h
+-rw-r--r--   0        0        0    21879 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/vector.h
+-rw-r--r--   0        0        0     1216 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/vector_base.h
+-rw-r--r--   0        0        0     1734 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/vector_bundle.h
+-rw-r--r--   0        0        0      515 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/vector_traits.h
+-rw-r--r--   0        0        0      703 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/algebra/free_tensor_multiplier.cpp
+-rw-r--r--   0        0        0     5062 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/algebra/half_shuffle_multiplier.cpp
+-rw-r--r--   0        0        0     1618 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/algebra/lie_multiplier.cpp
+-rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/algebra/polynomial.cpp
+-rw-r--r--   0        0        0      794 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/algebra/polynomial_multiplier.cpp
+-rw-r--r--   0        0        0      379 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/algebra/polynomial_ring.cpp
+-rw-r--r--   0        0        0      812 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/algebra/shuffle_multiplier.cpp
+-rw-r--r--   0        0        0     6227 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/basis/hall_set.cpp
+-rw-r--r--   0        0        0      594 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/basis/monomial.cpp
+-rw-r--r--   0        0        0     1390 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/basis/polynomial_basis.cpp
+-rw-r--r--   0        0        0     2294 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/basis/tensor_basis.cpp
+-rw-r--r--   0        0        0     5600 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/basis/unpacked_tensor_word.cpp
+-rw-r--r--   0        0        0      188 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/coefficients/floating_fields.cpp
+-rw-r--r--   0        0        0      166 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/coefficients/rational_field.cpp
+-rw-r--r--   0        0        0     2895 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/src/maps.cpp
+-rw-r--r--   0        0        0      469 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/CMakeLists.txt
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/common/main.cpp
+-rw-r--r--   0        0        0      494 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/lie/CMakeLists.txt
+-rw-r--r--   0        0        0     2542 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/lie/hall_basis.cpp
+-rw-r--r--   0        0        0     1052 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/lie/lie_fixture.h
+-rw-r--r--   0        0        0     1097 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/lie/lie_multiplier.cpp
+-rw-r--r--   0        0        0      400 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/maps/CMakeLists.txt
+-rw-r--r--   0        0        0     3200 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/maps/maps.cpp
+-rw-r--r--   0        0        0     4683 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/maps/maps_fixture.h
+-rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/polynomial/CMakeLists.txt
+-rw-r--r--   0        0        0     1234 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/polynomial/polynomial_basis.cpp
+-rw-r--r--   0        0        0      618 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/polynomial/polynomial_fixture.h
+-rw-r--r--   0        0        0      688 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/tensors/CMakeLists.txt
+-rw-r--r--   0        0        0     9809 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/tensors/dense_tensor.cpp
+-rw-r--r--   0        0        0     1519 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/tensors/free_tensor_multiplier.cpp
+-rw-r--r--   0        0        0      839 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/tensors/half_shuffle_multiplier.cpp
+-rw-r--r--   0        0        0     2020 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/tensors/shuffle_tensor_multiplier.cpp
+-rw-r--r--   0        0        0     9850 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/tensors/sparse_tensor.cpp
+-rw-r--r--   0        0        0     2548 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/tensors/tensor_basis.cpp
+-rw-r--r--   0        0        0     2526 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/tensors/tensor_fixture.h
+-rw-r--r--   0        0        0     4677 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/tensors/tensor_multiplication.cpp
+-rw-r--r--   0        0        0      479 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/utilities/CMakeLists.txt
+-rw-r--r--   0        0        0     1863 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/utilities/packed_integer.cpp
+-rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/tests/vector.cpp
+-rw-r--r--   0        0        0      679 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/libalgebra_lite/vcpkg.json
+-rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/.git
+-rw-r--r--   0        0        0     2176 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/CMakeLists.txt
+-rw-r--r--   0        0        0     1428 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/LICENSE.txt
+-rw-r--r--   0        0        0     4666 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/README.md
+-rw-r--r--   0        0        0     8441 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/CMakeLists.txt
+-rw-r--r--   0        0        0     1363 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/BufferConstructor.h
+-rw-r--r--   0        0        0     3270 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/Compare.cpp
+-rw-r--r--   0        0        0     7934 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/LinearAlgebraReductionTool.cpp
+-rw-r--r--   0        0        0     2313 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/LinearAlgebraReductionTool.h
+-rw-r--r--   0        0        0    13604 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/RdToPowers.cpp
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/RdToPowers.h
+-rw-r--r--   0        0        0   230430 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/SafeInt3.hpp
+-rw-r--r--   0        0        0     1299 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/TreeBufferHelper.cpp
+-rw-r--r--   0        0        0      931 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/TreeBufferHelper.h
+-rw-r--r--   0        0        0     9792 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/aligned_allocator.h
+-rw-r--r--   0        0        0     6660 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/lapack_defns.h
+-rw-r--r--   0        0        0     3027 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/lapack_fortran_definitions.h
+-rw-r--r--   0        0        0    14477 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/recombine.cpp
+-rw-r--r--   0        0        0     4293 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/recombine.h
+-rw-r--r--   0        0        0     7967 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/reweight.h
+-rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/stdafx.h
+-rw-r--r--   0        0        0     2538 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine/tjlUtilities.h
+-rw-r--r--   0        0        0      307 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/recombine/recombine.pc.in
+-rw-r--r--   0        0        0     1661 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/CMakeLists.txt
+-rw-r--r--   0        0        0     4086 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/TestVec/EvaluateAllMonomials.h
+-rw-r--r--   0        0        0     1186 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/TestVec/OstreamContainerOverloads.h
+-rw-r--r--   0        0        0      525 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/TestVec/ScopedWindowsPerformanceTimer.cpp
+-rw-r--r--   0        0        0      314 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/TestVec/ScopedWindowsPerformanceTimer.h
+-rw-r--r--   0        0        0      377 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/TestVec/stdafx.h
+-rw-r--r--   0        0        0      306 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/TestVec/targetver.h
+-rw-r--r--   0        0        0     1358 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/TestVec/utils.h
+-rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/set_env_test_recombine.sh
+-rw-r--r--   0        0        0     5597 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/test_recombine.cpp
+-rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 roughpy-0.0.4/external/recombine/test_recombine/test_recombine.h
+-rw-r--r--   0        0        0     1110 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/CMakeLists.txt
+-rw-r--r--   0        0        0     3939 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/include/roughpy/intervals/dyadic.h
+-rw-r--r--   0        0        0     4961 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/include/roughpy/intervals/dyadic_interval.h
+-rw-r--r--   0        0        0     3017 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/include/roughpy/intervals/interval.h
+-rw-r--r--   0        0        0     1394 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/include/roughpy/intervals/partition.h
+-rw-r--r--   0        0        0     3802 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/include/roughpy/intervals/real_interval.h
+-rw-r--r--   0        0        0     2131 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/include/roughpy/intervals/segmentation.h
+-rw-r--r--   0        0        0     5705 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/dyadic.cpp
+-rw-r--r--   0        0        0     8134 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/dyadic_interval.cpp
+-rw-r--r--   0        0        0     9339 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/dyadic_searcher.cpp
+-rw-r--r--   0        0        0     3525 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/dyadic_searcher.h
+-rw-r--r--   0        0        0     4239 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/interval.cpp
+-rw-r--r--   0        0        0     9360 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/partition.cpp
+-rw-r--r--   0        0        0     1896 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/real_interval.cpp
+-rw-r--r--   0        0        0     1964 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/scaled_predicate.cpp
+-rw-r--r--   0        0        0     2286 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/scaled_predicate.h
+-rw-r--r--   0        0        0     2216 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/segmentation.cpp
+-rw-r--r--   0        0        0     2322 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/test_dyadic.cpp
+-rw-r--r--   0        0        0    12091 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/test_dyadic_intervals.cpp
+-rw-r--r--   0        0        0     7851 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/test_partition.cpp
+-rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 roughpy-0.0.4/intervals/src/test_real_interval.cpp
+-rw-r--r--   0        0        0     1101 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/CMakeLists.txt
+-rw-r--r--   0        0        0     4187 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/include/roughpy/la_context/free_tensor_info.h
+-rw-r--r--   0        0        0     6553 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/include/roughpy/la_context/lie_basis_info.h
+-rw-r--r--   0        0        0     4195 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/include/roughpy/la_context/lie_info.h
+-rw-r--r--   0        0        0     2650 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/include/roughpy/la_context/shuffle_tensor_info.h
+-rw-r--r--   0        0        0     6925 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/include/roughpy/la_context/tensor_basis_info.h
+-rw-r--r--   0        0        0      699 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/include/roughpy/la_context/vector_iterator.h
+-rw-r--r--   0        0        0     2428 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/include/roughpy/la_context/vector_type_helper.h
+-rw-r--r--   0        0        0     3263 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/include/roughpy/la_context/vector_type_selector.h
+-rw-r--r--   0        0        0    23080 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/include/roughpy/la_context.h
+-rw-r--r--   0        0        0     1780 2022-11-09 12:37:21.000000 roughpy-0.0.4/la_context/src/la_context.cpp
+-rw-r--r--   0        0        0      524 2022-11-09 12:37:21.000000 roughpy-0.0.4/platform/CMakeLists.txt
+-rw-r--r--   0        0        0     2839 2022-11-09 12:37:21.000000 roughpy-0.0.4/platform/include/roughpy/platform/configuration.h
+-rw-r--r--   0        0        0     1302 2022-11-09 12:37:21.000000 roughpy-0.0.4/platform/include/roughpy/platform/filesystem.h
+-rw-r--r--   0        0        0     9674 2022-11-09 12:37:21.000000 roughpy-0.0.4/platform/include/roughpy/platform/serialization.h
+-rw-r--r--   0        0        0     4130 2022-11-09 12:37:21.000000 roughpy-0.0.4/platform/include/roughpy/platform/serialization_instantiations.inl
+-rw-r--r--   0        0        0      547 2022-11-09 12:37:21.000000 roughpy-0.0.4/platform/include/roughpy/platform.h
+-rw-r--r--   0        0        0     2022 2022-11-09 12:37:21.000000 roughpy-0.0.4/platform/src/configuration.cpp
+-rw-r--r--   0        0        0     3411 2022-11-09 12:37:21.000000 roughpy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5427 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/CMakeLists.txt
+-rw-r--r--   0        0        0     1329 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/__init__.py
+-rw-r--r--   0        0        0       24 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/__init__.pyi
+-rw-r--r--   0        0        0    19063 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/_roughpy.pyi
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/py.typed
+-rw-r--r--   0        0        0     2339 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/algebra.cpp
+-rw-r--r--   0        0        0     1867 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/algebra.h
+-rw-r--r--   0        0        0     2673 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/algebra_iterator.cpp
+-rw-r--r--   0        0        0     1903 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/algebra_iterator.h
+-rw-r--r--   0        0        0     2865 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/basis.cpp
+-rw-r--r--   0        0        0     1803 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/basis.h
+-rw-r--r--   0        0        0    16086 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/context.cpp
+-rw-r--r--   0        0        0     2243 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/context.h
+-rw-r--r--   0        0        0     6914 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/free_tensor.cpp
+-rw-r--r--   0        0        0     1827 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/free_tensor.h
+-rw-r--r--   0        0        0     3804 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/lie.cpp
+-rw-r--r--   0        0        0     1795 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/lie.h
+-rw-r--r--   0        0        0    13067 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/lie_key.cpp
+-rw-r--r--   0        0        0     2974 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/lie_key.h
+-rw-r--r--   0        0        0     3581 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/lie_key_iterator.cpp
+-rw-r--r--   0        0        0     2250 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/lie_key_iterator.h
+-rw-r--r--   0        0        0     1749 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/lie_letter.cpp
+-rw-r--r--   0        0        0     2578 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/lie_letter.h
+-rw-r--r--   0        0        0     8011 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/setup_algebra_type.h
+-rw-r--r--   0        0        0     4924 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/shuffle_tensor.cpp
+-rw-r--r--   0        0        0     1839 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/shuffle_tensor.h
+-rw-r--r--   0        0        0     5731 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/tensor_key.cpp
+-rw-r--r--   0        0        0     2977 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/tensor_key.h
+-rw-r--r--   0        0        0     3243 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/tensor_key_iterator.cpp
+-rw-r--r--   0        0        0     2228 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/algebra/tensor_key_iterator.h
+-rw-r--r--   0        0        0     4269 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/convert_timestamp.cpp
+-rw-r--r--   0        0        0     2564 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/convert_timestamp.h
+-rw-r--r--   0        0        0     8155 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/kwargs_to_path_metadata.cpp
+-rw-r--r--   0        0        0     2315 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/kwargs_to_path_metadata.h
+-rw-r--r--   0        0        0     3178 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/kwargs_to_vector_construction.cpp
+-rw-r--r--   0        0        0     2549 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/kwargs_to_vector_construction.h
+-rw-r--r--   0        0        0     4247 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/numpy.cpp
+-rw-r--r--   0        0        0     2085 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/numpy.h
+-rw-r--r--   0        0        0    14003 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/parse_schema.cpp
+-rw-r--r--   0        0        0      786 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/args/parse_schema.h
+-rw-r--r--   0        0        0    10164 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/dlpack.h
+-rw-r--r--   0        0        0    11345 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/dlpack_LICENSE
+-rw-r--r--   0        0        0     1367 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/date_time_interval.cpp
+-rw-r--r--   0        0        0     2526 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/date_time_interval.h
+-rw-r--r--   0        0        0     3143 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/dyadic.cpp
+-rw-r--r--   0        0        0     1813 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/dyadic.h
+-rw-r--r--   0        0        0     3976 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/dyadic_interval.cpp
+-rw-r--r--   0        0        0     1849 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/dyadic_interval.h
+-rw-r--r--   0        0        0     4391 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/interval.cpp
+-rw-r--r--   0        0        0     2387 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/interval.h
+-rw-r--r--   0        0        0     2248 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/intervals.cpp
+-rw-r--r--   0        0        0     1825 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/intervals.h
+-rw-r--r--   0        0        0     2978 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/partition.cpp
+-rw-r--r--   0        0        0     1913 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/partition.h
+-rw-r--r--   0        0        0     2778 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/real_interval.cpp
+-rw-r--r--   0        0        0     1841 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/real_interval.h
+-rw-r--r--   0        0        0     1984 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/segmentation.cpp
+-rw-r--r--   0        0        0     1837 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/intervals/segmentation.h
+-rw-r--r--   0        0        0     3931 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/recombine.cpp
+-rw-r--r--   0        0        0     1798 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/recombine.h
+-rw-r--r--   0        0        0     2234 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/roughpy_module.cpp
+-rw-r--r--   0        0        0     2549 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/roughpy_module.h
+-rw-r--r--   0        0        0    53300 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/scalars/r_py_polynomial.cpp
+-rw-r--r--   0        0        0     2767 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/scalars/r_py_polynomial.h
+-rw-r--r--   0        0        0    14251 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/scalars/scalar_type.cpp
+-rw-r--r--   0        0        0     5932 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/scalars/scalar_type.h
+-rw-r--r--   0        0        0    20017 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/scalars/scalars.cpp
+-rw-r--r--   0        0        0     3487 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/scalars/scalars.h
+-rw-r--r--   0        0        0     3871 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/BaseStream.cpp
+-rw-r--r--   0        0        0     2937 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/BaseStream.h
+-rw-r--r--   0        0        0     3427 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/brownian_stream.cpp
+-rw-r--r--   0        0        0     1899 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/brownian_stream.h
+-rw-r--r--   0        0        0     2768 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/externally_sourced_stream.cpp
+-rw-r--r--   0        0        0      312 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/externally_sourced_stream.h
+-rw-r--r--   0        0        0     4425 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/function_stream.cpp
+-rw-r--r--   0        0        0     2584 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/function_stream.h
+-rw-r--r--   0        0        0     7325 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/lie_increment_stream.cpp
+-rw-r--r--   0        0        0     1863 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/lie_increment_stream.h
+-rw-r--r--   0        0        0     3510 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/piecewise_abelian_stream.cpp
+-rw-r--r--   0        0        0     1931 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/piecewise_abelian_stream.h
+-rw-r--r--   0        0        0     1270 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/py_schema_context.cpp
+-rw-r--r--   0        0        0     2540 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/py_schema_context.h
+-rw-r--r--   0        0        0     5107 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/r_py_tick_construction_helper.cpp
+-rw-r--r--   0        0        0     3919 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/r_py_tick_construction_helper.h
+-rw-r--r--   0        0        0     6517 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/schema.cpp
+-rw-r--r--   0        0        0     1867 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/schema.h
+-rw-r--r--   0        0        0    23321 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/stream.cpp
+-rw-r--r--   0        0        0     2024 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/stream.h
+-rw-r--r--   0        0        0     2271 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/streams.cpp
+-rw-r--r--   0        0        0     1811 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/streams.h
+-rw-r--r--   0        0        0    15603 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/tick_stream.cpp
+-rw-r--r--   0        0        0     1827 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/src/streams/tick_stream.h
+-rw-r--r--   0        0        0     1561 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/streams/__init__.py
+-rw-r--r--   0        0        0     6198 2022-11-09 12:37:21.000000 roughpy-0.0.4/roughpy/streams/tick_stream.py
+-rw-r--r--   0        0        0     3228 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/CMakeLists.txt
+-rw-r--r--   0        0        0      997 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/conversion.h
+-rw-r--r--   0        0        0     4783 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/key_scalar_array.h
+-rw-r--r--   0        0        0     2725 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/owned_scalar_array.h
+-rw-r--r--   0        0        0     2776 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/random.h
+-rw-r--r--   0        0        0     8620 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalar.h
+-rw-r--r--   0        0        0     3474 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_array.h
+-rw-r--r--   0        0        0     3142 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_blas.h
+-rw-r--r--   0        0        0     3004 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_interface.h
+-rw-r--r--   0        0        0     4213 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_matrix.h
+-rw-r--r--   0        0        0    13459 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_pointer.h
+-rw-r--r--   0        0        0     3012 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_stream.h
+-rw-r--r--   0        0        0     3109 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_traits.h
+-rw-r--r--   0        0        0    16541 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_type.h
+-rw-r--r--   0        0        0     6594 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars/scalars_fwd.h
+-rw-r--r--   0        0        0     2035 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/include/roughpy/scalars.h
+-rw-r--r--   0        0        0     1477 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/scalar_blas_defs.h.in
+-rw-r--r--   0        0        0    17500 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/RationalType.cpp
+-rw-r--r--   0        0        0     5477 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/RationalType.h
+-rw-r--r--   0        0        0     2117 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/ScalarTests.h
+-rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/b_float_16_type.cpp
+-rw-r--r--   0        0        0     1989 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/b_float_16_type.h
+-rw-r--r--   0        0        0     1848 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/bfloat16_random_generator.cpp
+-rw-r--r--   0        0        0     6106 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/bfloat16_random_generator.h
+-rw-r--r--   0        0        0     1736 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/double_type.cpp
+-rw-r--r--   0        0        0     1931 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/double_type.h
+-rw-r--r--   0        0        0    17637 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/float_blas.cpp
+-rw-r--r--   0        0        0     3803 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/float_blas.h
+-rw-r--r--   0        0        0     1732 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/float_type.cpp
+-rw-r--r--   0        0        0     1925 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/float_type.h
+-rw-r--r--   0        0        0     1836 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/half_random_generator.cpp
+-rw-r--r--   0        0        0     5999 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/half_random_generator.h
+-rw-r--r--   0        0        0     1790 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/half_type.cpp
+-rw-r--r--   0        0        0     1955 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/half_type.h
+-rw-r--r--   0        0        0     6399 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/key_scalar_array.cpp
+-rw-r--r--   0        0        0     4579 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/owned_scalar_array.cpp
+-rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/random_impl.cpp
+-rw-r--r--   0        0        0      496 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/random_impl.h
+-rw-r--r--   0        0        0    14466 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/rational_poly_scalar_type.cpp
+-rw-r--r--   0        0        0     5089 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/rational_poly_scalar_type.h
+-rw-r--r--   0        0        0    11521 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/scalar.cpp
+-rw-r--r--   0        0        0     3931 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/scalar_array.cpp
+-rw-r--r--   0        0        0     4835 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/scalar_blas.cpp
+-rw-r--r--   0        0        0     6889 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/scalar_blas_impl.h
+-rw-r--r--   0        0        0     1942 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/scalar_interface.cpp
+-rw-r--r--   0        0        0     8248 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/scalar_matrix.cpp
+-rw-r--r--   0        0        0     5961 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/scalar_pointer.cpp
+-rw-r--r--   0        0        0     4525 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/scalar_stream.cpp
+-rw-r--r--   0        0        0    16127 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/scalar_type.cpp
+-rw-r--r--   0        0        0     1991 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/standard_random_generator.cpp
+-rw-r--r--   0        0        0     6903 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/standard_random_generator.h
+-rw-r--r--   0        0        0    21578 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/standard_scalar_type.h
+-rw-r--r--   0        0        0     2731 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/test_float_blas.cpp
+-rw-r--r--   0        0        0     3307 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/test_key_scalar_array.cpp
+-rw-r--r--   0        0        0     2518 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/test_pcg_standard_random.cpp
+-rw-r--r--   0        0        0     6701 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/test_scalar.cpp
+-rw-r--r--   0        0        0     2590 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/test_scalar_array.cpp
+-rw-r--r--   0        0        0     2723 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/test_scalar_matrix.cpp
+-rw-r--r--   0        0        0     5404 2022-11-09 12:37:21.000000 roughpy-0.0.4/scalars/src/test_scalar_type.cpp
+-rw-r--r--   0        0        0     4201 2022-11-09 12:37:21.000000 roughpy-0.0.4/setup.py
+-rw-r--r--   0        0        0     1932 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/CMakeLists.txt
+-rw-r--r--   0        0        0     4501 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/brownian_stream.h
+-rw-r--r--   0        0        0     9020 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/channels.h
+-rw-r--r--   0        0        0     3945 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/dyadic_caching_layer.h
+-rw-r--r--   0        0        0     8489 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/dynamically_constructed_stream.h
+-rw-r--r--   0        0        0     4118 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/external_data_stream.h
+-rw-r--r--   0        0        0     3758 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/lie_increment_stream.h
+-rw-r--r--   0        0        0     4018 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/piecewise_abelian_stream.h
+-rw-r--r--   0        0        0     8084 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/schema.h
+-rw-r--r--   0        0        0      929 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/schema_context.h
+-rw-r--r--   0        0        0     6232 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/stream.h
+-rw-r--r--   0        0        0     7645 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/stream_base.h
+-rw-r--r--   0        0        0     4597 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/stream_construction_helper.h
+-rw-r--r--   0        0        0     6020 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/include/roughpy/streams/tick_stream.h
+-rw-r--r--   0        0        0     3595 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/brownian_stream.cpp
+-rw-r--r--   0        0        0    15358 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/channels.cpp
+-rw-r--r--   0        0        0     4949 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/dyadic_caching_layer.cpp
+-rw-r--r--   0        0        0    14792 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/dynamically_constructed_stream.cpp
+-rw-r--r--   0        0        0     1823 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/external_data_sources/csv_data_source.cpp
+-rw-r--r--   0        0        0     2273 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/external_data_sources/csv_data_source.h
+-rw-r--r--   0        0        0    10976 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/external_data_sources/sound_file_data_source.cpp
+-rw-r--r--   0        0        0     4278 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/external_data_sources/sound_file_data_source.h
+-rw-r--r--   0        0        0     7343 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/external_data_stream.cpp
+-rw-r--r--   0        0        0     5126 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/lie_increment_stream.cpp
+-rw-r--r--   0        0        0     7701 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/piecewise_abelian_stream.cpp
+-rw-r--r--   0        0        0     9413 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/schema.cpp
+-rw-r--r--   0        0        0     1981 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/schema_context.cpp
+-rw-r--r--   0        0        0    10523 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/stream.cpp
+-rw-r--r--   0        0        0     4131 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/stream_base.cpp
+-rw-r--r--   0        0        0     4749 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/stream_construction_helper.cpp
+-rw-r--r--   0        0        0     3902 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/test_brownian_stream.cpp
+-rw-r--r--   0        0        0     5285 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/test_lie_increment_stream.cpp
+-rw-r--r--   0        0        0     8105 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/test_schema.cpp
+-rw-r--r--   0        0        0    10348 2022-11-09 12:37:21.000000 roughpy-0.0.4/streams/src/tick_stream.cpp
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/algebra/__init__.py
+-rw-r--r--   0        0        0     3303 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/algebra/test_alg_poly_coeffs.py
+-rw-r--r--   0        0        0     1975 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/algebra/test_algebra_context.py
+-rw-r--r--   0        0        0    11886 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/algebra/test_free_tensor.py
+-rw-r--r--   0        0        0     4614 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/algebra/test_lie.py
+-rw-r--r--   0        0        0      614 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/algebra/test_lie_keys.py
+-rw-r--r--   0        0        0      835 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/algebra/test_tensor_iterator.py
+-rw-r--r--   0        0        0     2039 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/algebra/test_tensor_keys.py
+-rw-r--r--   0        0        0      685 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/intervals/__init__.py
+-rw-r--r--   0        0        0      458 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/intervals/test_dyadic.py
+-rw-r--r--   0        0        0     2507 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/intervals/test_intervals.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/scalars/__init__.py
+-rw-r--r--   0        0        0     1396 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/scalars/test_monomial.py
+-rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/scalars/test_polynomial.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/__init__.py
+-rw-r--r--   0        0        0   187338 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/audio/test.flac
+-rw-r--r--   0        0        0    44146 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/audio/test.mp3
+-rw-r--r--   0        0        0   311172 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/audio/test.wav
+-rw-r--r--   0        0        0     2291 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/test_brownian_stream.py
+-rw-r--r--   0        0        0     4341 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/test_function_path.py
+-rw-r--r--   0        0        0     7804 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/test_lie_increment_path.py
+-rw-r--r--   0        0        0     1482 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/test_piecewise_lie_path.py
+-rw-r--r--   0        0        0     6231 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/test_schema.py
+-rw-r--r--   0        0        0     2397 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/test_sound_path.py
+-rw-r--r--   0        0        0     4142 2022-11-09 12:37:21.000000 roughpy-0.0.4/tests/streams/test_tick_stream.py
+-rw-r--r--   0        0        0     2763 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/before-all-common.sh
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/triplets/arm-uwp.cmake
+-rw-r--r--   0        0        0      155 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/triplets/arm64-windows.cmake
+-rw-r--r--   0        0        0       30 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/triplets/common.cmake
+-rw-r--r--   0        0        0      184 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/triplets/x64-linux.cmake
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/triplets/x64-osx.cmake
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/triplets/x64-uwp.cmake
+-rw-r--r--   0        0        0      147 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/triplets/x64-windows-static.cmake
+-rw-r--r--   0        0        0      148 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/triplets/x64-windows.cmake
+-rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ci/triplets/x86-windows.cmake
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ports/libalgebra/portfile.cmake
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ports/libalgebra/vcpkg.json
+-rw-r--r--   0        0        0      204 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ports/libalgebra-lite/portfile.cmake
+-rw-r--r--   0        0        0      356 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/ports/libalgebra-lite/vcpkg.json
+-rw-r--r--   0        0        0     4396 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/python-get-binary-obj-path.py
+-rw-r--r--   0        0        0     2511 2022-11-09 12:37:21.000000 roughpy-0.0.4/tools/version_from_file.py
+-rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 roughpy-0.0.4/vcpkg.json
+-rw-r--r--   0        0        0     6248 2022-11-09 12:37:21.000000 roughpy-0.0.4/PKG-INFO
```

### Comparing `roughpy-0.0.3/.clang-format` & `roughpy-0.0.4/external/libalgebra/.clang-format`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # Generated from CLion C/C++ Code Style settings
 BasedOnStyle: LLVM
 AccessModifierOffset: -4
-AlignAfterOpenBracket: BlockIndent
-AlignArrayOfStructures: Right
-
+AlignAfterOpenBracket: Align
 AlignConsecutiveAssignments: None
 AlignOperands: DontAlign
 AllowAllArgumentsOnNextLine: false
 AllowAllConstructorInitializersOnNextLine: false
 AllowAllParametersOfDeclarationOnNextLine: false
 AllowShortBlocksOnASingleLine: Always
 AllowShortCaseLabelsOnASingleLine: true
@@ -22,40 +20,39 @@
   AfterCaseLabel: false
   AfterClass: true
   AfterControlStatement: Never
   AfterEnum: true
   AfterFunction: true
   AfterNamespace: false
   AfterUnion: true
-  BeforeCatch: false
-  BeforeElse: false
+  BeforeCatch: true
+  BeforeElse: true
   IndentBraces: false
   SplitEmptyFunction: false
   SplitEmptyRecord: true
-BreakBeforeBinaryOperators: All
+BreakBeforeBinaryOperators: NonAssignment
 BreakBeforeTernaryOperators: true
 BreakConstructorInitializers: BeforeColon
 BreakInheritanceList: BeforeColon
-ColumnLimit: 80
+ColumnLimit: 0
 CompactNamespaces: false
 ContinuationIndentWidth: 8
-IndentCaseLabels: true
-PPIndentWidth: 2
-IndentPPDirectives: AfterHash
+IndentCaseLabels: false
+IndentPPDirectives: None
 IndentWidth: 4
 KeepEmptyLinesAtTheStartOfBlocks: true
 MaxEmptyLinesToKeep: 1
 NamespaceIndentation: None
 ObjCSpaceAfterProperty: false
-ObjCSpaceBeforeProtocolList: true
+ObjCSpaceBeforeProtocolList: false
 PointerAlignment: Left
-ReflowComments: true
-SpaceAfterCStyleCast: true
+ReflowComments: false
+SpaceAfterCStyleCast: false
 SpaceAfterLogicalNot: false
-SpaceAfterTemplateKeyword: true
+SpaceAfterTemplateKeyword: false
 SpaceBeforeAssignmentOperators: true
 SpaceBeforeCpp11BracedList: false
 SpaceBeforeCtorInitializerColon: true
 SpaceBeforeInheritanceColon: true
 SpaceBeforeParens: ControlStatements
 SpaceBeforeRangeBasedForLoopColon: true
 SpaceInEmptyParentheses: false
```

### Comparing `roughpy-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md` & `roughpy-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md` & `roughpy-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/.github/workflows/build_wheels.yml` & `roughpy-0.0.4/.github/workflows/build_wheels.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 name: Build Wheels
 
 on:
-#  push:
-#    branches: [ "main" ]
+  push:
+    branches: [ "main" ]
+    paths-ignore:
+      - "examples/**"
+      - "doc/**"
+      - "README.md"
+      - "*.txt"
+      - "CHANGELOG"
   pull_request:
     branches: [ "main" ]
+    types:
+      - opened
+      - reopened
+      - synchronize
+    paths-ignore:
+      - "examples/**"
+      - "doc/**"
+      - "README.md"
+      - "*.txt"
+      - "CHANGELOG"
 
 
 env:
   BUILD_TYPE: Release
   VERBOSE: 1
 #  VCPKG_BINARY_SOURCES: 'clear;x-gha,readwrite;nuget,GitHub,readwrite'
   VCPKG_BINARY_SOURCES: 'clear;x-gha,readwrite'
@@ -96,17 +112,18 @@
 
 
 
   publish:
     runs-on: ubuntu-latest
     needs: [ build_wheels, build_sdist ]
     if: |
+      github.event_name == 'push' || (
       github.event.pull_request.action == 'closed' &&
-      github.event.pull_request.merged == true &&
-      startsWith(github.head_ref, 'release/')
+      ${{ github.event.pull_request.merged }} &&
+      startsWith(github.head_ref, 'release/'))
 
     steps:
       - name: Setup Python
         uses: actions/setup-python@v3
         with:
           python-version: "3.11"
```

### Comparing `roughpy-0.0.3/.github/workflows/manage_version.yml` & `roughpy-0.0.4/.github/workflows/manage_version.yml`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/.github/workflows/tests.yml` & `roughpy-0.0.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/.gitignore` & `roughpy-0.0.4/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -333,7 +333,8 @@
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 
 roughpy/version.py
+/my_todo.txt
```

### Comparing `roughpy-0.0.3/CMakeLists.txt` & `roughpy-0.0.4/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,18 @@
     file(READ "VERSION.txt" _rpy_version)
     message(STATUS "Repository version ${_rpy_version}")
     string(REGEX MATCH "[0-9]+\\.[0-9]+\\.[0-9]+" _rpy_version "${_rpy_version}")
 else ()
     set(_rpy_version 0.0.1)
 endif ()
 
-
 project(RoughPy VERSION ${_rpy_version})
 
+set_property(GLOBAL PROPERTY USE_FOLDERS ON)
+
 set(CMAKE_INSTALL_LIBDIR "roughpy" CACHE STRING "install library dir")
 set(CMAKE_INSTALL_BINDIR "roughpy" CACHE STRING "install binary dir")
 
 set(CMAKE_CXX_STANDARD 17)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 if (LINUX)
     set(CMAKE_INSTALL_RPATH "$ORIGIN")
```

### Comparing `roughpy-0.0.3/LICENSE.txt` & `roughpy-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/THANKS.txt` & `roughpy-0.0.4/THANKS.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/CMakeLists.txt` & `roughpy-0.0.4/algebra/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_base.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_base.h`

 * *Files 0% similar despite different names*

```diff
@@ -39,27 +39,31 @@
 #include <roughpy/scalars/scalar.h>
 #include <roughpy/scalars/scalar_array.h>
 
 #include "algebra_iterator.h"
 #include "basis.h"
 #include "fallback_operations.h"
 
+
+RPY_WARNING_PUSH
+RPY_MSVC_DISABLE_WARNING(4661)
+
 namespace rpy {
 namespace algebra {
 
 namespace dtl {
 
 /**
  * @brief Tag for all algebra interfaces
  *
  * Used to identify whether a class is an algebra interface or not in
  * various places. If you define an algebra interface, it should derive
  * from the base AlgebraInterface, which publicly derives from this tag.
  */
-class RPY_EXPORT AlgebraInterfaceBase
+class AlgebraInterfaceBase
 {
 protected:
     context_pointer p_ctx;
     const scalars::ScalarType* p_coeff_type;
     VectorType m_vector_type;
     ImplementationType m_impl_type;
 
@@ -525,8 +529,10 @@
         const context_pointer& ref, const context_pointer& other
 );
 }// namespace dtl
 
 }// namespace algebra
 }// namespace rpy
 
+RPY_WARNING_POP
+
 #endif// ROUGHPY_ALGEBRA_ALGEBRA_BASE_H_
```

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_base_impl.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_base_impl.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_bundle.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_bundle.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,22 @@
 #define ROUGHPY_ALGEBRA_ALGEBRA_BUNDLE_H_
 
 #include "algebra_base.h"
 #include "algebra_fwd.h"
 
 #include <roughpy/platform/serialization.h>
 
+RPY_WARNING_PUSH
+RPY_MSVC_DISABLE_WARNING(4661)
+
 namespace rpy {
 namespace algebra {
 
 template <typename Bundle, typename Base, typename Fibre>
-class RPY_EXPORT BundleInterface
+class  BundleInterface
     : public dtl::algebra_base_resolution<
               Bundle, typename Base::basis_type, dtl::AlgebraArithmetic,
               dtl::AlgebraElementAccess>::type
 {
 public:
     using base_alg_t = Base;
     using fibre_alg_t = Fibre;
@@ -225,8 +228,11 @@
 
     RPY_SERIAL_LOAD_FN();
     RPY_SERIAL_SAVE_FN();
 };
 
 }// namespace algebra
 }// namespace rpy
+
+RPY_WARNING_POP
+
 #endif// ROUGHPY_ALGEBRA_ALGEBRA_BUNDLE_H_
```

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_bundle_base_impl.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_bundle_base_impl.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_bundle_impl.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_bundle_impl.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_fwd.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_fwd.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_impl.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_impl.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_info.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_iterator.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_iterator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/algebra_iterator_impl.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/algebra_iterator_impl.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/basis.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/basis_impl.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/basis_impl.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/basis_info.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/basis_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/context.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/context.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/context_fwd.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/context_fwd.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/fallback_operations.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/fallback_operations.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/free_tensor.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/free_tensor.h`

 * *Files 9% similar despite different names*

```diff
@@ -34,26 +34,31 @@
 #include "algebra_base_impl.h"
 #include "algebra_bundle_base_impl.h"
 #include "context.h"
 
 namespace rpy {
 namespace algebra {
 
+RPY_WARNING_PUSH
+RPY_GCC_DISABLE_WARNING(-Wattributes)
+
 RPY_TEMPLATE_EXTERN template class RPY_EXPORT_TEMPLATE
         AlgebraInterface<FreeTensor, TensorBasis>;
 
 RPY_TEMPLATE_EXTERN template class RPY_EXPORT_TEMPLATE
         AlgebraBase<FreeTensorInterface, FreeTensorImplementation>;
 
 RPY_TEMPLATE_EXTERN template class RPY_EXPORT_TEMPLATE
         BundleInterface<FreeTensorBundle, FreeTensor, FreeTensor>;
 
 RPY_TEMPLATE_EXTERN template class RPY_EXPORT_TEMPLATE AlgebraBundleBase<
         FreeTensorBundleInterface, FreeTensorBundleImplementation>;
 
+RPY_WARNING_POP
+
 template <>
 RPY_EXPORT typename FreeTensor::basis_type
 basis_setup_helper<FreeTensor>::get(const context_pointer& ctx);
 
 template <>
 RPY_EXPORT typename FreeTensorBundle::basis_type
 basis_setup_helper<FreeTensorBundle>::get(const context_pointer& ctx);
```

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/free_tensor_fwd.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/free_tensor_fwd.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/free_tensor_impl.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/free_tensor_impl.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/lie.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/lie.h`

 * *Files 6% similar despite different names*

```diff
@@ -36,26 +36,30 @@
 #include "algebra_base_impl.h"
 #include "algebra_bundle_base_impl.h"
 #include "context.h"
 
 namespace rpy {
 namespace algebra {
 
+RPY_WARNING_PUSH
+RPY_GCC_DISABLE_WARNING(-Wattributes)
 RPY_TEMPLATE_EXTERN template class RPY_EXPORT_TEMPLATE
         AlgebraInterface<Lie, LieBasis>;
 
 RPY_TEMPLATE_EXTERN template class RPY_EXPORT_TEMPLATE
         AlgebraBase<LieInterface>;
 
 RPY_TEMPLATE_EXTERN template class RPY_EXPORT_TEMPLATE
         BundleInterface<LieBundle, Lie, Lie>;
 
 RPY_TEMPLATE_EXTERN template class RPY_EXPORT_TEMPLATE
         AlgebraBundleBase<LieBundleInterface>;
 
+RPY_WARNING_POP
+
 RPY_SERIAL_SERIALIZE_FN_IMPL(Lie) { RPY_SERIAL_SERIALIZE_BASE(base_t); }
 
 RPY_SERIAL_SERIALIZE_FN_IMPL(LieBundle) { RPY_SERIAL_SERIALIZE_BASE(base_t); }
 
 template <>
 RPY_EXPORT typename Lie::basis_type
 basis_setup_helper<Lie>::get(const context_pointer& ctx);
```

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/lie_basis.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/lie_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/lie_fwd.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/lie_fwd.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/linear_operator.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/linear_operator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/shuffle_tensor.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/shuffle_tensor.h`

 * *Files 3% similar despite different names*

```diff
@@ -34,26 +34,32 @@
 #include "algebra_base_impl.h"
 #include "algebra_bundle_base_impl.h"
 #include "context.h"
 
 namespace rpy {
 namespace algebra {
 
+RPY_WARNING_PUSH
+RPY_GCC_DISABLE_WARNING(-Wattributes)
+
 RPY_TEMPLATE_EXTERN template class RPY_EXPORT_TEMPLATE
         AlgebraInterface<ShuffleTensor, TensorBasis>;
 
 RPY_TEMPLATE_EXTERN template class RPY_EXPORT_TEMPLATE
         AlgebraBase<ShuffleTensorInterface>;
 
 RPY_TEMPLATE_EXTERN template class RPY_EXPORT_TEMPLATE
         BundleInterface<ShuffleTensorBundle, ShuffleTensor, ShuffleTensor>;
 
 RPY_TEMPLATE_EXTERN template class RPY_EXPORT_TEMPLATE
         AlgebraBundleBase<ShuffleTensorBundleInterface>;
 
+RPY_WARNING_POP
+
+
 RPY_SERIAL_SERIALIZE_FN_IMPL(ShuffleTensor)
 {
     RPY_SERIAL_SERIALIZE_BASE(base_t);
 }
 
 RPY_SERIAL_SERIALIZE_FN_IMPL(ShuffleTensorBundle)
 {
```

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/shuffle_tensor_fwd.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/shuffle_tensor_fwd.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/include/roughpy/algebra/tensor_basis.h` & `roughpy-0.0.4/algebra/include/roughpy/algebra/tensor_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/ContextFixture.cpp` & `roughpy-0.0.4/algebra/src/ContextFixture.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/ContextFixture.h` & `roughpy-0.0.4/algebra/src/ContextFixture.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/algebra_base.cpp` & `roughpy-0.0.4/algebra/src/algebra_base.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/algebra_iterator.cpp` & `roughpy-0.0.4/algebra/src/algebra_iterator.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/basis.cpp` & `roughpy-0.0.4/algebra/src/basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/context.cpp` & `roughpy-0.0.4/algebra/src/context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/double_lite_context.cpp` & `roughpy-0.0.4/algebra/src/double_lite_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/float_lite_context.cpp` & `roughpy-0.0.4/algebra/src/float_lite_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/free_tensor.cpp` & `roughpy-0.0.4/algebra/src/free_tensor.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/hall_set_size.cpp` & `roughpy-0.0.4/algebra/src/hall_set_size.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/hall_set_size.h` & `roughpy-0.0.4/algebra/src/hall_set_size.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/libalgebra_lite_internal/dense_vector_iterator.h` & `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/dense_vector_iterator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/libalgebra_lite_internal/free_tensor_info.h` & `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/free_tensor_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/libalgebra_lite_internal/lie_basis_info.h` & `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/lie_basis_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/libalgebra_lite_internal/lie_info.h` & `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/lie_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/libalgebra_lite_internal/lite_vector_selector.h` & `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/lite_vector_selector.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/libalgebra_lite_internal/shuffle_tensor_info.h` & `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/shuffle_tensor_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/libalgebra_lite_internal/sparse_mutable_ref_scalar_trait.h` & `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/sparse_mutable_ref_scalar_trait.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/libalgebra_lite_internal/sparse_vector_iterator.h` & `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/sparse_vector_iterator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/libalgebra_lite_internal/tensor_basis_info.h` & `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/tensor_basis_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/libalgebra_lite_internal/vector_type_helper.h` & `roughpy-0.0.4/algebra/src/libalgebra_lite_internal/vector_type_helper.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/lie.cpp` & `roughpy-0.0.4/algebra/src/lie.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/lie_basis.cpp` & `roughpy-0.0.4/algebra/src/lie_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/lite_context.cpp` & `roughpy-0.0.4/algebra/src/lite_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/lite_context.h` & `roughpy-0.0.4/algebra/src/lite_context.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/rational_lite_context.cpp` & `roughpy-0.0.4/algebra/src/rational_lite_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/rational_poly_lite_context.cpp` & `roughpy-0.0.4/algebra/src/rational_poly_lite_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/shuffle_tensor.cpp` & `roughpy-0.0.4/algebra/src/shuffle_tensor.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/tensor_basis.cpp` & `roughpy-0.0.4/algebra/src/tensor_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/test_lie.cpp` & `roughpy-0.0.4/algebra/src/test_lie.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/testing/mock_context.cpp` & `roughpy-0.0.4/algebra/src/testing/mock_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/algebra/src/testing/mock_context.h` & `roughpy-0.0.4/algebra/src/testing/mock_context.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/branding/logo/logo_square_white.jpg` & `roughpy-0.0.4/branding/logo/logo_square_white.jpg`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/cmake/roughpy_helpers.cmake` & `roughpy-0.0.4/cmake/roughpy_helpers.cmake`

 * *Files 0% similar despite different names*

```diff
@@ -242,16 +242,16 @@
     if (_runtime_deps)
         set_target_properties(${_real_name} PROPERTIES RUNTIME_DEPENDENCIES ${_runtime_deps})
     endif ()
 
     set_target_properties(${_real_name} PROPERTIES
             PUBLIC_HEADER "${ARGS_PUBLIC_HEADERS}"
             LINKER_LANGUAGE CXX
-            #            CXX_DEFAULT_VISIBILITY hidden
-            #            VISIBILITY_INLINES_HIDDEN ON
+            CXX_DEFAULT_VISIBILITY hidden
+            VISIBILITY_INLINES_HIDDEN ON
             VERSION "${PROJECT_VERSION}"
             )
     #    if (_lib_type STREQUAL SHARED)
     #        set_target_properties(${_real_name} PROPERTIES
     #                SOVERSION ${PROJECT_VERSION_MAJOR})
     #    endif ()
```

### Comparing `roughpy-0.0.3/core/include/roughpy/core/alloc.h` & `roughpy-0.0.4/core/include/roughpy/core/alloc.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/core/include/roughpy/core/helpers.h` & `roughpy-0.0.4/core/include/roughpy/core/helpers.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/core/include/roughpy/core/macros.h` & `roughpy-0.0.4/core/include/roughpy/core/macros.h`

 * *Files 20% similar despite different names*

```diff
@@ -31,25 +31,44 @@
 //
 
 #ifndef ROUGHPY_CORE_MACROS_H
 #define ROUGHPY_CORE_MACROS_H
 
 #include <cassert>
 #include <stdexcept>
+#include <string>
+
+#ifdef __has_builtin
+#  define RPY_HAS_BUILTIN(x) __has_builtin(x)
+#else
+#  define RPY_HAS_BUILTIN(x) 0
+#endif
 
 #ifdef __has_feature
 #  define RPY_HAS_FEATURE(FEAT) __has_feature(FEAT)
 #else
 #  define RPY_HAS_FEATURE(FEAT) 0
 #endif
 
+#ifdef __has_cpp_attribute
+#  define RPY_HAS_CPP_ATTRIBUTE(x) __has_cpp_attribute(x)
+#else
+#  define RPY_HAS_CPP_ATTRIBUTE(x) 0
+#endif
+
+#ifdef __has_include
+#  define RPY_HAS_INCLUDE(x) __has_include(x)
+#else
+#  define RPY_HAS_INCLUDE(x) 0
+#endif
+
 #define RPY_STRINGIFY_IMPL(ARG) #ARG
 #define RPY_STRINGIFY(ARG) RPY_STRINGIFY_IMPL(ARG)
 
-#define RPY_JOIN_IMPL_IMPL(LHS, RHS) X##Y
+#define RPY_JOIN_IMPL_IMPL(LHS, RHS) LHS##RHS
 #define RPY_JOIN_IMPL(LHS, RHS) RPY_JOIN_IMPL_IMPL(LHS, RHS)
 #define RPY_JOIN(LHS, RHS) RPY_JOIN_IMPL(LHS, RHS)
 
 #define RPY_IDENTITY(ARG) ARG
 
 #if (defined(_DEBUG) || !defined(NDEBUG) || !defined(__OPTIMIZE__))            \
         && !defined(RPY_DEBUG)
@@ -168,24 +187,32 @@
 #else
 #  define RPY_UNREACHABLE() abort()
 #  define RPY_UNREACHABLE_RETURN(...)                                          \
       RPY_UNREACHABLE();                                                       \
       return __VA_ARGS__
 #endif
 
+#ifdef RPY_MSVC
+#  define RPY_PRAGMA(ARG) __pragma(ARG)
+#else
+#  define RPY_PRAGMA(ARG) _Pragma(RPY_STRINGIFY(ARG))
+#endif
+
 // Macros that control optimisations
 
 #if defined(__OPTIMIZE__) || !defined(RPY_DEBUG)
 #  if defined(_WIN32) || defined(_WIN64)
 #    define RPY_INLINE_ALWAYS __forceinline
 #  elif defined(__GNUC__) || defined(__clang__)
 #    define RPY_INLINE_ALWAYS inline __attribute__((always_inline))
 #  else
 #    define RPY_INLINE_ALWAYS inline
 #  endif
+#else
+#  define RPY_INLINE_ALWAYS inline
 #endif
 
 #ifdef RPY_MSVC
 #  define RPY_INLINE_NEVER __declspec(noinline)
 #elif defined(RPY_GCC) || defined(RPY_CLANG)
 #  define RPY_INLINE_NEVER __attribute__((never_inline))
 #else
@@ -204,41 +231,14 @@
 #  define RPY_LIKELY(COND) (__builtin_expect(static_cast<bool>(COND), 1))
 #  define RPY_UNLIKELY(COND) (__builtin_expect(static_cast<bool>(COND), 0))
 #else
 #  define RPY_LIKELY(COND) (COND)
 #  define RPY_UNLIKELY(COND) (COND)
 #endif
 
-#define RPY_CHECK(EXPR)                                                        \
-    do {                                                                       \
-        if (RPY_UNLIKELY(!(EXPR))) {                                           \
-            throw std::runtime_error(                                          \
-                    std::string("failed check \"") + #EXPR + "\""              \
-            );                                                                 \
-        }                                                                      \
-    } while (0)
-
-#ifdef RPY_DEBUG
-#  ifdef RPY_DBG_ASSERT_USE_EXCEPTIONS
-#    define RPY_DBG_ASSERT(ARG)                                                \
-        do {                                                                   \
-            if (RPY_UNLIKEY(!(EXPR))) {                                        \
-                throw std::runtime_error(                                      \
-                        std::string("failed debug assertion \"") + #EXPR       \
-                        + "\""                                                 \
-                );                                                             \
-            }                                                                  \
-        } while (0)
-#  else
-#    define RPY_DBG_ASSERT(ARG) assert(ARG)
-#  endif
-#else
-#  define RPY_DBG_ASSERT(ARG) (void) 0
-#endif
-
 #define RPY_FALLTHROUGH (void) 0
 
 #if defined(RPY_PLATFORM_WINDOWS)
 #  if RPY_BUILDING_LIBRARY
 #    define RPY_TEMPLATE_EXTERN
 #    define RPY_EXPORT_TEMPLATE
 #    define RPY_EXPORT_INSTANTIATION RPY_EXPORT
@@ -262,8 +262,106 @@
 
 #if RPY_HAS_FEATURE(address_sanitizer)
 #  define RPY_NO_ASAN __attribute__((no_sanitize("address")))
 #else
 #  define RPY_NO_ASAN
 #endif
 
+// Warning and error control
+#if defined(RPY_MSVC)
+#  define RPY_WARNING_PUSH RPY_PRAGMA(warning(push))
+#  define RPY_WARNING_POP RPY_PRAGMA(warning(pop))
+#elif defined(RPY_GCC)
+#  define RPY_WARNING_PUSH RPY_PRAGMA(GCC diagnostic push)
+#  define RPY_WARNING_POP RPY_PRAGMA(GCC diagnostic pop)
+#elif defined(RPY_CLANG)
+#  define RPY_WARNING_PUSH RPY_PRAGMA(clang diagnostic push)
+#  define RPY_WARNING_POP RPY_PRAGMA(clang diagnostic pop)
+#else
+#  define RPY_WARNING_PUSH
+#  define RPY_WARNING_POP
+#endif
+
+#ifdef RPY_MSVC
+#  define RPY_MSVC_DISABLE_WARNING(ARG) RPY_PRAGMA(warning(disable : ARG))
+#else
+#  define RPY_MSVC_DISABLE_WARNING(ARG)
+#endif
+
+#ifdef RPY_GCC
+#  define RPY_GCC_DISABLE_WARNING(ARG)                                         \
+      RPY_PRAGMA(GCC diagnostic ignored RPY_STRINGIFY(ARG))
+#else
+#  define RPY_GCC_DISABLE_WARNING(ARG)
+#endif
+
+#ifdef RPY_CLANG
+#  define RPY_CLANG_DISABLE_WARNING(ARG)                                       \
+      RPY_PRAGMA(clang diagnostic ignored RPY_STRINGIFY(ARG))
+#else
+#  define RPY_CLANG_DISABLE_WARNING(ARG)
+#endif
+
+#if defined(RPY_GCC)
+#  define RPY_FUNC_NAME __PRETTY_FUNCTION__
+#elif defined(RPY_CLANG)
+#  define RPY_FUNC_NAME __builtin_FUNCTION()
+#elif defined(RPY_MSVC)
+#  define RPY_FUNC_NAME __FUNCTION__
+#else
+#  define RPY_FUNC_NAME static_cast<const char*>(0)
+#endif
+
+/*
+ * Check macro definition.
+ *
+ * This macro checks that the given expression evaluates to true (under the
+ * assumption that it will usually be true), and throws an error if this
+ * evaluates to false.
+ *
+ * Optionally, one can provide a message string literal that will be used
+ * instead of the default, and an optional error type. The default error type
+ * is a std::runtime_error.
+ */
+namespace rpy {
+namespace errors {
+template <typename E>
+RPY_NO_RETURN RPY_INLINE_ALWAYS void
+check_fail(const char* msg, const char* filename, int lineno, const char* func)
+{
+    throw E(std::string(msg) + " at lineno " + std::to_string(lineno) + " in "
+            + filename + " in function " + func);
+}
+}// namespace errors
+}// namespace rpy
+
+// Dispatch the check macro on the number of arguments
+// See: https://stackoverflow.com/a/16683147/9225581
+#define RPY_CHECK_3(EXPR, MSG, TYPE)                                           \
+    do {                                                                       \
+        if (RPY_UNLIKELY(!(EXPR))) {                                           \
+            ::rpy::errors::check_fail<TYPE>(                                   \
+                    MSG, __FILE__, __LINE__, RPY_FUNC_NAME                     \
+            );                                                                 \
+        }                                                                      \
+    } while (0)
+
+#define RPY_CHECK_2(EXPR, MSG) RPY_CHECK_3(EXPR, MSG, std::runtime_error)
+
+#define RPY_CHECK_1(EXPR) RPY_CHECK_2(EXPR, "failed check \"" #EXPR "\"")
+
+#define RPY_CHECK_CNT_IMPL(_1, _2, _3, COUNT, ...) COUNT
+// Always pass one more argument than expected, so clang doesn't complain about
+// empty parameter packs.
+#define RPY_CHECK_CNT(...) RPY_CHECK_CNT_IMPL(__VA_ARGS__, 3, 2, 1, 0)
+#define RPY_CHECK_SEL(NUM) RPY_JOIN(RPY_CHECK_, NUM)
+
+#define RPY_CHECK(...) RPY_CHECK_SEL(RPY_CHECK_CNT(__VA_ARGS__))(__VA_ARGS__)
+
+#ifdef RPY_DEBUG
+#  define RPY_DBG_ASSERT(ARG) assert(ARG)
+#else
+#  define RPY_DBG_ASSERT(ARG) (void) 0
+#endif
+
+
 #endif// ROUGHPY_CORE_MACROS_H
```

### Comparing `roughpy-0.0.3/core/include/roughpy/core/slice.h` & `roughpy-0.0.4/core/include/roughpy/core/slice.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/core/include/roughpy/core/traits.h` & `roughpy-0.0.4/core/include/roughpy/core/traits.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/core/include/roughpy/core/types.h` & `roughpy-0.0.4/core/include/roughpy/core/types.h`

 * *Files 4% similar despite different names*

```diff
@@ -32,24 +32,16 @@
 #include "macros.h"
 
 #include <cstdint>
 #include <string>
 #include <utility>
 
 #ifdef RPY_CPP_17
-#  ifndef RPY_APPLE
-
-#    include <optional>
-
-#  else
-#    include <boost/optional.hpp>
-#  endif
-
+#  include <optional>
 #  include <string_view>
-
 #else
 #  include <boost/optional.hpp>
 #  include <boost/utility/string_view.hpp>
 #endif
 
 namespace rpy {
```

### Comparing `roughpy-0.0.3/device/CMakeLists.txt` & `roughpy-0.0.4/device/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/device/cuda/CudaDeviceContext.cuh` & `roughpy-0.0.4/device/cuda/CudaDeviceContext.cuh`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/device/cuda/scalars/src/CUDAFloatType.cuh` & `roughpy-0.0.4/device/cuda/scalars/src/CUDAFloatType.cuh`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/device/cuda/scalars/src/CUDA_standard_scalar.cuh` & `roughpy-0.0.4/device/cuda/scalars/src/CUDA_standard_scalar.cuh`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/device/include/roughpy/device/core.h` & `roughpy-0.0.4/device/include/roughpy/device/core.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/device/include/roughpy/device/device_algebra_base.h` & `roughpy-0.0.4/device/include/roughpy/device/device_algebra_base.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/device/include/roughpy/device/device_context.h` & `roughpy-0.0.4/device/include/roughpy/device/device_context.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/device/kernels/binary_kernel.cuh` & `roughpy-0.0.4/device/kernels/binary_kernel.cuh`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/device/kernels/functors.h` & `roughpy-0.0.4/device/kernels/functors.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/device/kernels/tmp.cu` & `roughpy-0.0.4/device/kernels/tmp.cu`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/device/kernels/unary_kernel.cuh` & `roughpy-0.0.4/device/kernels/unary_kernel.cuh`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/device/src/device_algebra_base.cpp` & `roughpy-0.0.4/device/src/device_algebra_base.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/device/src/device_context.cpp` & `roughpy-0.0.4/device/src/device_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/device/src/device_free_tensor.cpp` & `roughpy-0.0.4/device/src/device_free_tensor.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/device/src/device_free_tensor.h` & `roughpy-0.0.4/device/src/device_free_tensor.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/docs/make.bat` & `roughpy-0.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/docs/source/conf.py` & `roughpy-0.0.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/examples/lie_to_tensor_formulae.py` & `roughpy-0.0.4/examples/lie_to_tensor_formulae.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/.gitignore` & `roughpy-0.0.4/external/libalgebra/.gitignore`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/CMakeLists.txt` & `roughpy-0.0.4/external/libalgebra/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/Dockerfile` & `roughpy-0.0.4/external/libalgebra/Dockerfile`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/Dockerfile.remote-cpp-env` & `roughpy-0.0.4/external/libalgebra/Dockerfile.remote-cpp-env`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/README.md` & `roughpy-0.0.4/external/libalgebra/README.md`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/benchmarks/antipode/antipode_bm.cpp` & `roughpy-0.0.4/external/libalgebra/benchmarks/antipode/antipode_bm.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/benchmarks/multiplication/CMakeLists.txt` & `roughpy-0.0.4/external/libalgebra/benchmarks/multiplication/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/benchmarks/multiplication/multiplication_bm.cpp` & `roughpy-0.0.4/external/libalgebra/benchmarks/multiplication/multiplication_bm.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/benchmarks/multiplication/multiplication_single.cpp` & `roughpy-0.0.4/external/libalgebra/benchmarks/multiplication/multiplication_single.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/cmake/Modules/FindBignum.cmake` & `roughpy-0.0.4/external/libalgebra/cmake/Modules/FindBignum.cmake`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/cmake/Modules/UnitTestPP.cmake` & `roughpy-0.0.4/external/libalgebra/cmake/Modules/UnitTestPP.cmake`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/cmake/Modules/UnitTestPP_DiscoverTests.cmake` & `roughpy-0.0.4/external/libalgebra/cmake/Modules/UnitTestPP_DiscoverTests.cmake`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/cmake/libalgebra_test_helper.cmake` & `roughpy-0.0.4/external/libalgebra/cmake/libalgebra_test_helper.cmake`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/_tensor_basis.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/_tensor_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/alg_types.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/alg_types.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/algebra.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/algebra.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/alternative_multiplications.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/alternative_multiplications.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/area_tensor_basis.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/area_tensor_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/area_tensor_multiplication.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/area_tensor_multiplication.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/base_basis.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/base_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/base_vector.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/base_vector.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/basis.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/coefficients/gmp_ser.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/coefficients/gmp_ser.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/coefficients.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/coefficients.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/composition_operator.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/composition_operator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/constlog2.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/constlog2.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/constpower.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/constpower.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/dense_storage.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/dense_storage.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/dense_vector.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/dense_vector.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/detail/caching_tags.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/detail/caching_tags.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/detail/function_extension_cache_base.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/detail/function_extension_cache_base.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/detail/integer_maths.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/detail/integer_maths.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/detail/level_walkers.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/detail/level_walkers.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/detail/meta.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/detail/meta.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/detail/platform.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/detail/platform.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/detail/reversing_permutation.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/detail/reversing_permutation.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/detail/smallest_int_type.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/detail/smallest_int_type.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/detail/unpacked_tensor_word.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/detail/unpacked_tensor_word.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/dot_product_implementations.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/dot_product_implementations.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/free_extension.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/free_extension.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/functionals.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/functionals.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/half_shuffle_tensor_basis.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/half_shuffle_tensor_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/half_shuffle_tensor_multiplication.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/half_shuffle_tensor_multiplication.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/hall_set.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/hall_set.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/hybrid_vector.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/hybrid_vector.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/implementation_types.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/implementation_types.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/iterators.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/iterators.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/key_iterators.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/key_iterators.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/libalgebra.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/libalgebra.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/lie.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/lie.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/lie_basis.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/lie_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/lie_inner_product.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/lie_inner_product.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/monomial_basis.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/monomial_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/mpfloat_coefficients.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/mpfloat_coefficients.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/multi_linear_operators.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/multi_linear_operators.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/multi_polynomial.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/multi_polynomial.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/multiplication_helpers.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/multiplication_helpers.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/operators.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/operators.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/poly_basis.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/poly_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/poly_lie.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/poly_lie.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/poly_lie_basis.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/poly_lie_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/polynomial_coefficients.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/polynomial_coefficients.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/polynomials.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/polynomials.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/rational_coefficients.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/rational_coefficients.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/reconfigure_operator.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/reconfigure_operator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/scalar_bundle.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/scalar_bundle.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/scalar_multiply_operator.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/scalar_multiply_operator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/sparse_vector.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/sparse_vector.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/sum_operator.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/sum_operator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/tags.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/tags.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/tensor.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/tensor.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/tensor_basis.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/tensor_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/tensor_operator.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/tensor_operator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/utils.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/utils.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/vector.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/vector.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/vector_bundle.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/vector_bundle.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/libalgebra/vectors.h` & `roughpy-0.0.4/external/libalgebra/libalgebra/vectors.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/CMakeLists.txt` & `roughpy-0.0.4/external/libalgebra/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/common/CMakeLists.txt` & `roughpy-0.0.4/external/libalgebra/tests/common/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/common/SHOW.h` & `roughpy-0.0.4/external/libalgebra/tests/common/SHOW.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/common/compat.h` & `roughpy-0.0.4/external/libalgebra/tests/common/compat.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/common/helpers.h` & `roughpy-0.0.4/external/libalgebra/tests/common/helpers.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/common/memfile.cpp` & `roughpy-0.0.4/external/libalgebra/tests/common/memfile.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/common/memfile.h` & `roughpy-0.0.4/external/libalgebra/tests/common/memfile.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/common/multi_test.h` & `roughpy-0.0.4/external/libalgebra/tests/common/multi_test.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/common/random_coeffs.h` & `roughpy-0.0.4/external/libalgebra/tests/common/random_coeffs.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/common/random_vector_generator.h` & `roughpy-0.0.4/external/libalgebra/tests/common/random_vector_generator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/common/reporter.cpp` & `roughpy-0.0.4/external/libalgebra/tests/common/reporter.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/common/reporter.h` & `roughpy-0.0.4/external/libalgebra/tests/common/reporter.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/common/rng.h` & `roughpy-0.0.4/external/libalgebra/tests/common/rng.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/common/run_tests.cpp` & `roughpy-0.0.4/external/libalgebra/tests/common/run_tests.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/common/simple_basis.h` & `roughpy-0.0.4/external/libalgebra/tests/common/simple_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/common/time_and_details.h` & `roughpy-0.0.4/external/libalgebra/tests/common/time_and_details.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/AlgebraFunctionsTests.cpp` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/AlgebraFunctionsTests.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/HallSetTests.cpp` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/HallSetTests.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/LatticePathTests.cpp` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/LatticePathTests.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/MemoryMappedFilesDocumentation.htm` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/MemoryMappedFilesDocumentation.htm`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/OMPSigsTests.cpp` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/OMPSigsTests.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/SigHelpers.h` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/SigHelpers.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/TreeBufferHelper.h` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/TreeBufferHelper.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/brown_path_increments.h` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/brown_path_increments.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/categorical_path.h` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/categorical_path.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/makebm.cpp` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/makebm.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/accuracy_suite.ins` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/accuracy_suite.ins`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/coefficient_path_suite.ins` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/coefficient_path_suite.ins`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/double_path_suite.ins` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/double_path_suite.ins`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/float_path_suite.ins` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/float_path_suite.ins`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/generic_coefficient.h` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/generic_coefficient.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/generic_lie_increment.h` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/generic_lie_increment.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/generic_path.h` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/generic_path.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/rational_path_suite.ins` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/rational_path_suite.ins`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/test_brownian_path.cpp` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/test_brownian_path.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/signature_tests/test_innovative_path.cpp` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/signature_tests/test_innovative_path.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/speed_tests.cpp` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/speed_tests.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/tests_TENSOR_LIE_CBH_MAPS.cpp` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/tests_TENSOR_LIE_CBH_MAPS.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/tests_libalgebra-demo.cpp` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/tests_libalgebra-demo.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/integration_tests/x64sigs.cpp` & `roughpy-0.0.4/external/libalgebra/tests/integration_tests/x64sigs.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/adjoint/test_adjoint.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/adjoint/test_adjoint.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/algebra/CMakeLists.txt` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/algebra/alg_mul_suite.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/alg_mul_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/algebra/framework_fixture.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/framework_fixture.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/algebra/simple_algebra_basis.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/simple_algebra_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/algebra/test_algebra_product.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/algebra/test_algebra_product.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/antipode/test_antipode.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/antipode/test_antipode.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/basis/basis_iteration_suite.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/basis/basis_iteration_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/basis/test_basis_iteration.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/basis/test_basis_iteration.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/basis/test_lie_basis_iteration.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/basis/test_lie_basis_iteration.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/coefficients/polynomial_coeff_ring.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/polynomial_coeff_ring.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/coefficients/standard_coefficient_test_suite.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/standard_coefficient_test_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/coefficients/test_mpfloat_fallback_field.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/test_mpfloat_fallback_field.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/coefficients/test_rational_fallback_field.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/test_rational_fallback_field.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/coefficients/unital_coefficient_test_suite.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/coefficients/unital_coefficient_test_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/half-shuffle-tests/half_shuffle_fixture.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/half-shuffle-tests/half_shuffle_fixture.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/half-shuffle-tests/test_half_shuffle.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/half-shuffle-tests/test_half_shuffle.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/hall_set/test_hall_set.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/hall_set/test_hall_set.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/lie/test_basis.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/lie/test_dense_lie_multiplication.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_dense_lie_multiplication.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/lie/test_function_extension.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_function_extension.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/lie/test_hall_basis.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_hall_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/lie/test_lie_multiplication.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/lie/test_lie_multiplication.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/operators/test_free_extension.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_free_extension.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/operators/test_lie_inner_product.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_lie_inner_product.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/operators/test_operator_composition.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_operator_composition.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/operators/test_operator_sum.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_operator_sum.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/operators/test_operators_smul.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_operators_smul.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/operators/test_recalibrate_operator.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_recalibrate_operator.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/operators/test_shuffle_functional.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_shuffle_functional.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/operators/test_tensor_defined_operator.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_tensor_defined_operator.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/operators/test_tensor_multiplication_operator.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/operators/test_tensor_multiplication_operator.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/CMakeLists.txt` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/dense_vec_serialization.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/dense_vec_serialization.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/fixture.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/fixture.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/hybrid_vector_serialization.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/hybrid_vector_serialization.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/sparse_vector_serialization.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/sparse_vector_serialization.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/temporary_directory.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/temporary_directory.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/test_dense_storage.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/test_dense_storage.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/test_hall_set_serialize.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/test_hall_set_serialize.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/serialization/test_higher_classes.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/serialization/test_higher_classes.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/shuffle-tensor-tests/test_shuffle_tensor.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/shuffle-tensor-tests/test_shuffle_tensor.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/tangents/CMakeLists.txt` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tangents/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/tangents/test_tangents.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tangents/test_tangents.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/CMakeLists.txt` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/tensor_exp_suite.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/tensor_exp_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/tensor_inverse_suite.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/tensor_inverse_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/tensor_log_suite.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/tensor_log_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/tensor_roundtrip_suite.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/tensor_roundtrip_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_basis.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_dense_tensor_functions.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_dense_tensor_functions.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_dense_tensor_multiplication.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_dense_tensor_multiplication.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_hybrid_tensor_functions.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_hybrid_tensor_functions.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_hybrid_tensor_multiplication.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_hybrid_tensor_multiplication.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_signature_calc.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_signature_calc.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_sparse_tensor_functions.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_sparse_tensor_functions.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_sparse_tensor_multiplication.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_sparse_tensor_multiplication.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_tensor_creation.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_tensor_creation.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_tensor_functions.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_tensor_functions.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_tensor_multiplication.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_tensor_multiplication.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/tensor/test_tensor_size_info.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/tensor/test_tensor_size_info.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/utils/test_integer_maths.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/utils/test_integer_maths.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/framework_fixture.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/framework_fixture.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/test_dense.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/test_dense.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/test_dense_storage.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/test_dense_storage.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/test_hybrid.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/test_hybrid.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/test_sparse.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/test_sparse.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/vector_arithmetic_suite.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_arithmetic_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/vector_binary_transform_suite.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_binary_transform_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/vector_comparison_suite.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_comparison_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/vector_element_access_suite.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_element_access_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/vector_iterator_suite.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_iterator_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/vector_norm_suite.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_norm_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/vector/vector_properties_suite.h` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/vector/vector_properties_suite.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra/tests/unit_tests/width1_tests/width1_tensors.cpp` & `roughpy-0.0.4/external/libalgebra/tests/unit_tests/width1_tests/width1_tensors.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/CMakeLists.txt` & `roughpy-0.0.4/external/libalgebra_lite/CMakeLists.txt`

 * *Files 26% similar despite different names*

```diff
@@ -8,41 +8,58 @@
 include(GenerateExportHeader)
 include(GNUInstallDirs)
 
 
 find_package(Boost REQUIRED)
 
 add_library(Libalgebra_lite SHARED
-        src/basis/hall_set.cpp
-        src/basis/tensor_basis.cpp
-        src/basis/monomial.cpp
-        src/basis/polynomial_basis.cpp
-        src/basis/unpacked_tensor_word.cpp
         src/algebra/lie_multiplier.cpp
         src/algebra/polynomial_multiplier.cpp
         src/algebra/polynomial.cpp
         src/algebra/half_shuffle_multiplier.cpp
         src/algebra/free_tensor_multiplier.cpp
         src/algebra/shuffle_multiplier.cpp
         src/algebra/polynomial_ring.cpp
+        src/basis/hall_set.cpp
+        src/basis/tensor_basis.cpp
+        src/basis/monomial.cpp
+        src/basis/polynomial_basis.cpp
+        src/basis/unpacked_tensor_word.cpp
+        src/coefficients/floating_fields.cpp
+        src/coefficients/rational_field.cpp
         src/maps.cpp
+        include/libalgebra_lite/detail/integer_maths.h
+        include/libalgebra_lite/detail/macros.h
+        include/libalgebra_lite/detail/notnull.h
+        include/libalgebra_lite/detail/traits.h
+        include/libalgebra_lite/algebra.h
+        include/libalgebra_lite/basis.h
+        include/libalgebra_lite/basis_traits.h
+        include/libalgebra_lite/coefficients.h
+        include/libalgebra_lite/dense_vector.h
         include/libalgebra_lite/free_tensor.h
+        include/libalgebra_lite/hall_set.h
+        include/libalgebra_lite/implementation_types.h
+        include/libalgebra_lite/index_key.h
+        include/libalgebra_lite/key_range.h
         include/libalgebra_lite/lie.h
         include/libalgebra_lite/maps.h
-        include/libalgebra_lite/vector_bundle.h
+        include/libalgebra_lite/operators.h
         include/libalgebra_lite/packed_integer.h
-        include/libalgebra_lite/polynomial_basis.h
         include/libalgebra_lite/polynomial.h
+        include/libalgebra_lite/polynomial_basis.h
         include/libalgebra_lite/registry.h
-        include/libalgebra_lite/unpacked_tensor_word.h
         include/libalgebra_lite/shuffle_tensor.h
-        include/libalgebra_lite/operators.h
-        include/libalgebra_lite/basis.h
+        include/libalgebra_lite/sparse_vector.h
+        include/libalgebra_lite/tensor_basis.h
+        include/libalgebra_lite/unpacked_tensor_word.h
+        include/libalgebra_lite/vector.h
         include/libalgebra_lite/vector_base.h
-        include/libalgebra_lite/detail/notnull.h
+        include/libalgebra_lite/vector_bundle.h
+        include/libalgebra_lite/vector_traits.h
         )
 
 add_library(Libalgebra_lite::Libalgebra_lite ALIAS Libalgebra_lite)
 generate_export_header(Libalgebra_lite)
 
 find_package(Bignum QUIET)
 if (NOT TARGET Bignum::Bignum)
```

### Comparing `roughpy-0.0.3/external/libalgebra_lite/cmake/lalhelpers.cmake` & `roughpy-0.0.4/external/libalgebra_lite/cmake/lalhelpers.cmake`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/cmake/rationals.h.in` & `roughpy-0.0.4/external/libalgebra_lite/cmake/rationals.h.in`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/algebra.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/algebra.h`

 * *Files 7% similar despite different names*

```diff
@@ -7,831 +7,946 @@
 
 #include "implementation_types.h"
 #include "libalgebra_lite_export.h"
 
 #include <algorithm>
 #include <map>
 #include <memory>
-#include <type_traits>
 #include <utility>
 #include <vector>
 
 #include <boost/container/small_vector.hpp>
-#include <boost/mpl/vector.hpp>
-#include <boost/mpl/contains.hpp>
 
 #include "basis_traits.h"
 #include "coefficients.h"
-#include "vector_traits.h"
 #include "vector.h"
+#include "vector_traits.h"
+
+#include "detail/traits.h"
 
 namespace lal {
 
 template <typename Multiplication>
 struct multiplication_traits {
 
     using mult_ptr = std::shared_ptr<const Multiplication>;
 
 private:
-
     template <typename, typename, typename, typename, typename = void>
-    struct has_fma_inplace : std::false_type {};
+    struct has_fma_inplace : false_type {
+    };
 
     template <typename L, typename R, typename F, typename M>
-    struct has_fma_inplace<L, R, F, M,
-                           std::void_t<decltype(M::template fma_inplace(std::declval<L &>(),
-                                                                        std::declval<const R &>(),
-                                                                        std::declval<F>()))>>
-        : std::true_type {
+    struct has_fma_inplace<
+            L, R, F, M,
+            void_t<decltype(M::template fma_inplace(
+                    declval<L&>(), declval<const R&>(), declval<F>()
+            ))>> : true_type {
     };
 
-    template <typename, typename, typename, typename, typename=void>
-    struct has_fma_inplace_with_deg : std::false_type {};
+    template <typename, typename, typename, typename, typename = void>
+    struct has_fma_inplace_with_deg : false_type {
+    };
 
     template <typename L, typename R, typename F, typename M>
-    struct has_fma_inplace_with_deg<L, R, F, M,
-                                    std::void_t<decltype(M::template fma_inplace(std::declval<L &>(),
-                                                                                 std::declval<const R &>(),
-                                                                                 std::declval<F>()), std::declval<deg_t>())>>
-        : std::true_type {
+    struct has_fma_inplace_with_deg<
+            L, R, F, M,
+            void_t<decltype(M::template fma_inplace(declval<L&>(), declval<const R&>(), declval<F>()), declval<deg_t>())>>
+        : true_type {
     };
 
     template <typename V>
-    using has_degree_t = std::is_same<typename basis_trait<typename V::basis_type>::degree_tag, with_degree_tag>;
-
-public:
-
-    template <typename Result,
-        typename Vector1,
-        typename Vector2,
-        typename Fn>
-    static std::enable_if_t<!has_degree_t<Result>::value>
-    multiply_and_add(
-        const Multiplication &mult,
-        Result &result,
-        const Vector1 &lhs,
-        const Vector2 &rhs,
-        Fn fn) {
-        if (lhs.empty() || rhs.empty()) {
-            return;
-        }
-
-        mult.fma(result.base_vector(),
-                 lhs.base_vector(),
-                 rhs.base_vector(),
-                 fn);
-    }
-
-    template <typename Result,
-        typename Vector1,
-        typename Vector2>
-    static std::enable_if_t<!has_degree_t<Result>::value>
-    multiply_and_add(const Multiplication &mult,
-                     Result &result,
-                     const Vector1 &lhs,
-                     const Vector2 &rhs) {
+    using has_degree_t = is_same<
+            typename basis_trait<typename V::basis_type>::degree_tag,
+            with_degree_tag>;
+
+public:
+    template <typename Result, typename Vector1, typename Vector2, typename Fn>
+    static enable_if_t<!has_degree_t<Result>::value> multiply_and_add(
+            const Multiplication& mult, Result& result, const Vector1& lhs,
+            const Vector2& rhs, Fn fn
+    )
+    {
+        if (lhs.empty() || rhs.empty()) { return; }
+
+        mult.fma(
+                result.base_vector(), lhs.base_vector(), rhs.base_vector(), fn
+        );
+    }
+
+    template <typename Result, typename Vector1, typename Vector2>
+    static enable_if_t<!has_degree_t<Result>::value> multiply_and_add(
+            const Multiplication& mult, Result& result, const Vector1& lhs,
+            const Vector2& rhs
+    )
+    {
         using scalar_type = typename Result::scalar_type;
-        mult.fma(result.base_vector(),
-                 lhs.base_vector(),
-                 rhs.base_vector(),
-                 [](scalar_type s) { return s; });
-    }
-
-    template <typename Result,
-        typename Vector1,
-        typename Vector2,
-        typename Fn>
-    static std::enable_if_t<has_degree_t<Result>::value>
-    multiply_and_add(
-        const Multiplication &mult,
-        Result &result,
-        const Vector1 &lhs,
-        const Vector2 &rhs,
-        Fn fn) {
+        mult.fma(
+                result.base_vector(), lhs.base_vector(), rhs.base_vector(),
+                [](scalar_type s) { return s; }
+        );
+    }
+
+    template <typename Result, typename Vector1, typename Vector2, typename Fn>
+    static enable_if_t<has_degree_t<Result>::value> multiply_and_add(
+            const Multiplication& mult, Result& result, const Vector1& lhs,
+            const Vector2& rhs, Fn fn
+    )
+    {
         using traits = basis_trait<typename Result::basis_type>;
-        mult.fma(result.base_vector(),
-                 lhs.base_vector(),
-                 rhs.base_vector(),
-                 fn,
-                 traits::max_degree(result.basis()));
+        mult.fma(
+                result.base_vector(), lhs.base_vector(), rhs.base_vector(), fn,
+                traits::max_degree(result.basis())
+        );
     }
 
-    template <typename Result,
-        typename Vector1,
-        typename Vector2>
-    static std::enable_if_t<has_degree_t<Result>::value>
-    multiply_and_add(const Multiplication &mult,
-                     Result &result,
-                     const Vector1 &lhs,
-                     const Vector2 &rhs) {
+    template <typename Result, typename Vector1, typename Vector2>
+    static enable_if_t<has_degree_t<Result>::value> multiply_and_add(
+            const Multiplication& mult, Result& result, const Vector1& lhs,
+            const Vector2& rhs
+    )
+    {
         using scalar_type = typename Result::scalar_type;
         using traits = basis_trait<typename Result::basis_type>;
-        mult.fma(result.base_vector(),
-                 lhs.base_vector(),
-                 rhs.base_vector(),
-                 [](scalar_type s) { return s; },
-                 traits::max_degree(result.basis()));
-    }
-//
-//    template <typename Left, typename Right, typename Fn, typename Mult=Multiplication>
-//    static std::enable_if_t<!has_degree_t<Left>::value && has_fma_inplace<Left, Right, Fn, Mult>::value>
-//    multiply_and_add_inplace(const Multiplication &mult, Left &lhs, const Right &rhs, Fn fn) {
-//        mult.fma_inplace(lhs.vector_type(), rhs.vector_type(), fn);
-//    }
-//
-//    template <typename Left, typename Right, typename Fn, typename Mult=Multiplication>
-//    static std::enable_if_t<has_degree_t<Left>::value && has_fma_inplace<Left, Right, Fn, Mult>::value>
-//    multiply_and_add_inplace(const Multiplication& mult, Left& lhs, const Right& rhs, Fn fn)
-//    {
-//        using traits = basis_trait<typename Left::basis_type>;
-//        mult.fma_inplace(lhs.base_vector(), rhs.base_vector(), fn,
-//                traits::max_degree(lhs.basis()));
-//    }
-//
-//    template <typename Left, typename Right, typename Fn, typename Mult=Multiplication>
-//    static std::enable_if_t<has_degree_t<Left>::value && has_fma_inplace<Left, Right, Fn, Mult>::value>
-//    multiply_and_add_inplace(const Multiplication &mult, Left &lhs, const Right &rhs, Fn fn, deg_t max_deg) {
-//        mult.fma_inplace(lhs.base_vector(), rhs.base_vector(), fn, max_deg);
-//    }
+        mult.fma(
+                result.base_vector(), lhs.base_vector(), rhs.base_vector(),
+                [](scalar_type s) { return s; },
+                traits::max_degree(result.basis())
+        );
+    }
+    //
+    //    template <typename Left, typename Right, typename Fn, typename
+    //    Mult=Multiplication> static enable_if_t<!has_degree_t<Left>::value &&
+    //    has_fma_inplace<Left, Right, Fn, Mult>::value>
+    //    multiply_and_add_inplace(const Multiplication &mult, Left &lhs, const
+    //    Right &rhs, Fn fn) {
+    //        mult.fma_inplace(lhs.vector_type(), rhs.vector_type(), fn);
+    //    }
+    //
+    //    template <typename Left, typename Right, typename Fn, typename
+    //    Mult=Multiplication> static enable_if_t<has_degree_t<Left>::value &&
+    //    has_fma_inplace<Left, Right, Fn, Mult>::value>
+    //    multiply_and_add_inplace(const Multiplication& mult, Left& lhs, const
+    //    Right& rhs, Fn fn)
+    //    {
+    //        using traits = basis_trait<typename Left::basis_type>;
+    //        mult.fma_inplace(lhs.base_vector(), rhs.base_vector(), fn,
+    //                traits::max_degree(lhs.basis()));
+    //    }
+    //
+    //    template <typename Left, typename Right, typename Fn, typename
+    //    Mult=Multiplication> static enable_if_t<has_degree_t<Left>::value &&
+    //    has_fma_inplace<Left, Right, Fn, Mult>::value>
+    //    multiply_and_add_inplace(const Multiplication &mult, Left &lhs, const
+    //    Right &rhs, Fn fn, deg_t max_deg) {
+    //        mult.fma_inplace(lhs.base_vector(), rhs.base_vector(), fn,
+    //        max_deg);
+    //    }
 
     template <typename Left, typename Right, typename Fn>
-    static std::enable_if_t<!has_degree_t<Left>::value>
-    multiply_inplace(const Multiplication &mult, Left &lhs, const Right &rhs, Fn fn) {
-//        Left tmp(lhs.get_basis());
-//        mult.fma(tmp.base_vector(), lhs.base_vector(), rhs.base_vector(), fn);
-//        lhs.swap(tmp);
+    static enable_if_t<!has_degree_t<Left>::value> multiply_inplace(
+            const Multiplication& mult, Left& lhs, const Right& rhs, Fn fn
+    )
+    {
+        //        Left tmp(lhs.get_basis());
+        //        mult.fma(tmp.base_vector(), lhs.base_vector(),
+        //        rhs.base_vector(), fn); lhs.swap(tmp);
         mult.multiply_inplace(lhs.base_vector(), rhs.base_vector(), fn);
     }
 
     template <typename Left, typename Right, typename Fn>
-    static std::enable_if_t<has_degree_t<Left>::value>
-    multiply_inplace(const Multiplication &mult, Left &lhs, const Right &rhs, Fn fn, deg_t max_deg) {
-//        Left tmp(lhs.get_basis());
-//        mult.fma(tmp.base_vector(), lhs.base_vector(), rhs.base_vector(), fn, max_deg);
-//        std::swap(lhs, tmp);
-//        lhs.swap(tmp);
-        mult.multiply_inplace(lhs.base_vector(), rhs.base_vector(), fn, max_deg);
+    static enable_if_t<has_degree_t<Left>::value> multiply_inplace(
+            const Multiplication& mult, Left& lhs, const Right& rhs, Fn fn,
+            deg_t max_deg
+    )
+    {
+        //        Left tmp(lhs.get_basis());
+        //        mult.fma(tmp.base_vector(), lhs.base_vector(),
+        //        rhs.base_vector(), fn, max_deg); std::swap(lhs, tmp);
+        //        lhs.swap(tmp);
+        mult.multiply_inplace(
+                lhs.base_vector(), rhs.base_vector(), fn, max_deg
+        );
     }
 
-
     template <typename Left, typename Right, typename Fn>
-    static std::enable_if_t<!has_degree_t<Left>::value>
-    multiply_inplace(const Multiplication &mult, Left &lhs, const Right &rhs, Fn fn, deg_t) {
-//        Left tmp(lhs.get_basis());
-//        mult.fma(tmp.base_vector(), lhs.base_vector(), rhs.base_vector(), fn, max_deg);
-//        std::swap(lhs, tmp);
-//        lhs.swap(tmp);
+    static enable_if_t<!has_degree_t<Left>::value> multiply_inplace(
+            const Multiplication& mult, Left& lhs, const Right& rhs, Fn fn,
+            deg_t
+    )
+    {
+        //        Left tmp(lhs.get_basis());
+        //        mult.fma(tmp.base_vector(), lhs.base_vector(),
+        //        rhs.base_vector(), fn, max_deg); std::swap(lhs, tmp);
+        //        lhs.swap(tmp);
         mult.multiply_inplace(lhs.base_vector(), rhs.base_vector(), fn);
     }
 
     template <typename Left, typename Right, typename Fn>
-    static std::enable_if_t<has_degree_t<Left>::value>
-    multiply_inplace(const Multiplication &mult, Left &lhs, const Right &rhs, Fn fn) {
-        auto max_deg = basis_trait<typename Left::basis_type>::max_degree(lhs.basis());
+    static enable_if_t<has_degree_t<Left>::value> multiply_inplace(
+            const Multiplication& mult, Left& lhs, const Right& rhs, Fn fn
+    )
+    {
+        auto max_deg
+                = basis_trait<typename Left::basis_type>::max_degree(lhs.basis()
+                );
         multiply_inplace(mult, lhs, rhs, fn, max_deg);
     }
-
-    template <typename Basis>
-    using compatible_with = boost::mpl::contains<typename Multiplication::compatible_bases, Basis>;
-
 };
 
 namespace dtl {
 
 template <typename Basis, typename Coefficients>
-class general_multiplication_helper {
+class general_multiplication_helper
+{
 protected:
     using basis_traits = basis_trait<Basis>;
     using key_type = typename basis_traits::key_type;
     using coeff_traits = coefficient_trait<Coefficients>;
     using scalar_type = typename coeff_traits::scalar_type;
 
-    using key_value = std::pair<key_type, scalar_type>;
+    using key_value = pair<key_type, scalar_type>;
     std::vector<key_value> right_buffer;
 
 public:
-
     using const_iterator = typename std::vector<key_value>::const_iterator;
 
     template <typename Vector>
-    explicit general_multiplication_helper(const Vector &rhs)
-        : right_buffer() {
+    explicit general_multiplication_helper(const Vector& rhs) : right_buffer()
+    {
         right_buffer.reserve(rhs.size());
         for (auto item : rhs) {
             right_buffer.emplace_back(item.key(), item.value());
         }
     }
 
     const_iterator begin() const noexcept { return right_buffer.begin(); }
     const_iterator end() const noexcept { return right_buffer.end(); }
-
 };
 
 template <typename It>
-class degree_range_iterator_helper {
+class degree_range_iterator_helper
+{
     It m_begin, m_end;
 
 public:
     using iterator = It;
 
-    degree_range_iterator_helper(It begin, It end)
-        : m_begin(begin), m_end(end) {}
+    degree_range_iterator_helper(It begin, It end) : m_begin(begin), m_end(end)
+    {}
 
     iterator begin() noexcept { return m_begin; }
     iterator end() noexcept { return m_end; }
 };
 
 template <typename Basis, typename Coefficients>
-class graded_multiplication_helper : protected general_multiplication_helper<Basis, Coefficients> {
+class graded_multiplication_helper
+    : protected general_multiplication_helper<Basis, Coefficients>
+{
     using base_type = general_multiplication_helper<Basis, Coefficients>;
     using ordering = typename base_type::basis_traits::kv_ordering;
 
+    using base_type::right_buffer;
     using typename base_type::basis_traits;
     using typename base_type::key_type;
-    using typename base_type::scalar_type;
     using typename base_type::key_value;
-    using base_type::right_buffer;
+    using typename base_type::scalar_type;
 
     using base_iter = typename std::vector<key_value>::const_iterator;
 
     std::vector<base_iter> degree_ranges;
     deg_t max_degree;
 
 public:
-
     using iterable = degree_range_iterator_helper<base_iter>;
 
     template <typename Vector>
-    explicit graded_multiplication_helper(const Vector &rhs)
-        : base_type(rhs) {
+    explicit graded_multiplication_helper(const Vector& rhs) : base_type(rhs)
+    {
         ordering order;
         std::sort(right_buffer.begin(), right_buffer.end(), order);
 
-        const auto &basis = rhs.basis();
+        const auto& basis = rhs.basis();
         max_degree = basis_traits::max_degree(basis);
         degree_ranges.reserve(max_degree + 1);
         auto it = right_buffer.cbegin();
         auto end = right_buffer.cend();
         degree_ranges.push_back(it);
         auto degree = 0;
 
         for (; it != end; ++it) {
             auto current = basis_traits::degree(basis, it->first);
-            for (; degree < current; ++degree) {
-                degree_ranges.push_back(it);
-            }
-        }
-        for (; degree <= max_degree; ++degree) {
-            degree_ranges.push_back(end);
+            for (; degree < current; ++degree) { degree_ranges.push_back(it); }
         }
+        for (; degree <= max_degree; ++degree) { degree_ranges.push_back(end); }
     }
 
-    iterable degree_range(deg_t degree) noexcept {
+    iterable degree_range(deg_t degree) noexcept
+    {
         if (degree < 0) {
             return iterable(right_buffer.begin(), right_buffer.begin());
         }
         if (degree > max_degree) {
             return iterable(right_buffer.end(), right_buffer.end());
         }
         return iterable(right_buffer.begin(), degree_ranges[degree + 1]);
     }
-
 };
 
-} // namespace dtl
+}// namespace dtl
 
-
-template <typename Multiplier, typename Basis, dimn_t SSO = 1, typename Scalar=int>
-class base_multiplier {
+template <
+        typename Multiplier, typename Basis, dimn_t SSO = 1,
+        typename Scalar = int>
+class base_multiplier
+{
     using basis_traits = basis_trait<Basis>;
 
 public:
     using key_type = typename basis_traits::key_type;
     using scalar_type = Scalar;
-    using pair_type = std::pair<key_type, scalar_type>;
+    using pair_type = pair<key_type, scalar_type>;
 
     using product_type = boost::container::small_vector<pair_type, SSO>;
-    using reference = const boost::container::small_vector_base<pair_type> &;
+    using reference = const boost::container::small_vector_base<pair_type>&;
 
-    static product_type uminus(reference arg) {
+    static product_type uminus(reference arg)
+    {
         product_type result;
         result.reserve(arg.size());
-        for (const auto &item : arg) {
+        for (const auto& item : arg) {
             result.emplace_back(item.first, -item.second);
         }
         return result;
     }
 
-    static product_type add(reference lhs, reference rhs) {
+    static product_type add(reference lhs, reference rhs)
+    {
         std::map<key_type, scalar_type> tmp;
         tmp.insert(lhs.begin(), lhs.end());
 
-        for (const auto &item : rhs) {
-            tmp[item.first] += item.second;
-        }
+        for (const auto& item : rhs) { tmp[item.first] += item.second; }
 
         return {tmp.begin(), tmp.end()};
     }
 
-    static product_type sub(reference lhs, reference rhs) {
+    static product_type sub(reference lhs, reference rhs)
+    {
         std::map<key_type, scalar_type> tmp;
         tmp.insert(lhs.begin(), lhs.end());
 
-        for (const auto &item : rhs) {
-            tmp[item.first] -= item.second;
-        }
+        for (const auto& item : rhs) { tmp[item.first] -= item.second; }
 
         return {tmp.begin(), tmp.end()};
     }
 
-    product_type mul(const Basis &basis, reference lhs, key_type rhs) const {
+    product_type mul(const Basis& basis, reference lhs, key_type rhs) const
+    {
         std::map<key_type, scalar_type> tmp;
 
-        const auto &mult = static_cast<const Multiplier &>(*this);
-        for (const auto &outer : lhs) {
-            for (const auto &inner : mult(basis, outer.first, rhs)) {
+        const auto& mult = static_cast<const Multiplier&>(*this);
+        for (const auto& outer : lhs) {
+            for (const auto& inner : mult(basis, outer.first, rhs)) {
                 tmp[inner.first] += outer.second * inner.second;
             }
         }
 
         return {tmp.begin(), tmp.end()};
     }
 
-    product_type mul(const Basis &basis, key_type lhs, reference rhs) const {
+    product_type mul(const Basis& basis, key_type lhs, reference rhs) const
+    {
         std::map<key_type, scalar_type> tmp;
 
-        const auto &mult = static_cast<const Multiplier &>(*this);
-        for (const auto &outer : rhs) {
-            for (const auto &inner : mult(basis, lhs, outer.first)) {
+        const auto& mult = static_cast<const Multiplier&>(*this);
+        for (const auto& outer : rhs) {
+            for (const auto& inner : mult(basis, lhs, outer.first)) {
                 tmp[inner.first] += inner.second * outer.second;
             }
         }
 
         return {tmp.begin(), tmp.end()};
     }
 
-    product_type mul(const Basis &basis, reference lhs, reference rhs) const {
+    product_type mul(const Basis& basis, reference lhs, reference rhs) const
+    {
         std::map<key_type, scalar_type> tmp;
 
-        const auto &mult = static_cast<const Multiplier &>(*this);
-        for (const auto &litem : lhs) {
-            for (const auto &ritem : rhs) {
-                for (const auto &inner : mult(basis, litem.first, ritem.first)) {
-                    tmp[inner.first] += inner.second * litem.second * ritem.second;
+        const auto& mult = static_cast<const Multiplier&>(*this);
+        for (const auto& litem : lhs) {
+            for (const auto& ritem : rhs) {
+                for (const auto& inner :
+                     mult(basis, litem.first, ritem.first)) {
+                    tmp[inner.first]
+                            += inner.second * litem.second * ritem.second;
                 }
             }
         }
 
         return {tmp.begin(), tmp.end()};
     }
-
 };
 
 namespace dtl {
 
 template <typename Derived>
 struct derived_or_this {
     template <typename Base>
-    static const Derived &cast(const Base &arg) noexcept {
-        return static_cast<const Derived &>(arg);
+    static const Derived& cast(const Base& arg) noexcept
+    {
+        return static_cast<const Derived&>(arg);
     }
 };
 
 template <>
 struct derived_or_this<void> {
     template <typename Base>
-    static const Base &cast(const Base &arg) noexcept {
+    static const Base& cast(const Base& arg) noexcept
+    {
         return arg;
     }
 };
 
-} // namespace dtl
-
+}// namespace dtl
 
-template <typename Multiplier, typename Derived=void>
-class base_multiplication {
+template <typename Multiplier, typename Derived = void>
+class base_multiplication
+{
 
     template <typename V>
     using basis_t = typename V::basis_type;
 
     template <typename V>
     using key_tp = typename basis_trait<basis_t<V>>::key_type;
 
     template <typename V>
     using scal_t = typename V::scalar_type;
 
     template <typename V, typename Sca>
     using key_vect = std::vector<
-        std::pair<typename basis_trait<typename V::basis_type>::key_type,
-                  Sca>>;
+            pair<typename basis_trait<typename V::basis_type>::key_type, Sca>>;
 
     template <typename V>
     using helper_type = dtl::general_multiplication_helper<
-        typename V::basis_type, typename V::coefficient_ring>;
+            typename V::basis_type, typename V::coefficient_ring>;
     template <typename V>
     using graded_helper_type = dtl::graded_multiplication_helper<
-        typename V::basis_type, typename V::coefficient_ring>;
+            typename V::basis_type, typename V::coefficient_ring>;
 
-//    template <typename OutVector, typename KeyProd, typename Sca>
-//    void asp_helper(OutVector& out, KeyProd&& key_prod, Sca&& scalar) const
-//    {
-//        using scalar_type = scal_t<OutVector>;
-//        scalar_type s(std::forward<Sca>(scalar));
-//        out.inplace_binary_op(std::forward<KeyProd>(key_prod), [s](scalar_type& lhs, const scalar_type& rhs) {
-//            return lhs += (rhs*s);
-//        });
-//    }
+    //    template <typename OutVector, typename KeyProd, typename Sca>
+    //    void asp_helper(OutVector& out, KeyProd&& key_prod, Sca&& scalar)
+    //    const
+    //    {
+    //        using scalar_type = scal_t<OutVector>;
+    //        scalar_type s(forward<Sca>(scalar));
+    //        out.inplace_binary_op(forward<KeyProd>(key_prod), [s](scalar_type&
+    //        lhs, const scalar_type& rhs) {
+    //            return lhs += (rhs*s);
+    //        });
+    //    }
 
     using caster = dtl::derived_or_this<Derived>;
 
     template <typename OutVector, typename ProductType, typename PSca>
-    void asp_helper(OutVector &out, ProductType &&key_prod, PSca &&scalar) const {
+    void asp_helper(OutVector& out, ProductType&& key_prod, PSca&& scalar) const
+    {
         using scalar_type = scal_t<OutVector>;
-        scalar_type s(std::forward<PSca>(scalar));
+        scalar_type s(forward<PSca>(scalar));
 
-        for (const auto &kv_pair : key_prod) {
+        for (const auto& kv_pair : key_prod) {
             out[kv_pair.first] += scalar_type(kv_pair.second) * s;
         }
     }
 
 protected:
     Multiplier m_mult;
 
 public:
-
     using basis_type = typename Multiplier::basis_type;
     using key_type = typename basis_trait<basis_type>::key_type;
-    using generic_ref = const boost::container::small_vector_base<std::pair<key_type, int>> &;
-
-    using compatible_bases = boost::mpl::vector<typename Multiplier::basis_type>;
+    using generic_ref
+            = const boost::container::small_vector_base<pair<key_type, int>>&;
 
-    template <typename... Args, typename=std::enable_if_t<std::is_constructible<Multiplier, Args...>::value>>
-    explicit base_multiplication(Args &&... args)
-        : m_mult(std::forward<Args>(args)...) {}
+    template <
+            typename... Args,
+            typename
+            = enable_if_t<is_constructible<Multiplier, Args...>::value>>
+    explicit base_multiplication(Args&&... args)
+        : m_mult(forward<Args>(args)...)
+    {}
 
     template <typename Basis, typename Key>
-    decltype(auto) multiply(const Basis &basis, Key lhs, Key rhs) const {
+    decltype(auto) multiply(const Basis& basis, Key lhs, Key rhs) const
+    {
         return m_mult(basis, lhs, rhs);
     }
 
     template <typename Basis>
-    decltype(auto) multiply_generic(const Basis &basis, generic_ref lhs, generic_ref rhs) const {
+    decltype(auto)
+    multiply_generic(const Basis& basis, generic_ref lhs, generic_ref rhs) const
+    {
         return m_mult.mul(basis, lhs, rhs);
     }
 
-    template <typename OutVector,
-        typename LeftVector,
-        typename RightVector,
-        typename Fn>
-    void fma(OutVector &out, const LeftVector &lhs, const RightVector &rhs, Fn fn) const {
+    template <
+            typename OutVector, typename LeftVector, typename RightVector,
+            typename Fn>
+    void
+    fma(OutVector& out, const LeftVector& lhs, const RightVector& rhs,
+        Fn fn) const
+    {
         // The helper makes a contiguous copy of rhs key-value pairs
         // so the inner loop is always contiguous, rather than potentially
         // a linked list or other cache unfriendly data structure.
         helper_type<RightVector> helper(rhs);
-        const auto &basis = out.basis();
+        const auto& basis = out.basis();
 
         for (auto litem : lhs) {
             for (auto ritem : helper) {
-                asp_helper(out, m_mult(basis, litem.key(), ritem.first),
-                           fn(litem.value() * ritem.second));
+                asp_helper(
+                        out, m_mult(basis, litem.key(), ritem.first),
+                        fn(litem.value() * ritem.second)
+                );
             }
         }
     }
 
-    template <typename OutVector,
-        typename LeftVector,
-        typename RightVector,
-        typename Fn>
-    void fma(OutVector &out, const LeftVector &lhs, const RightVector &rhs, Fn fn, deg_t max_deg) const {
+    template <
+            typename OutVector, typename LeftVector, typename RightVector,
+            typename Fn>
+    void
+    fma(OutVector& out, const LeftVector& lhs, const RightVector& rhs, Fn fn,
+        deg_t max_deg) const
+    {
         using out_basis_traits = basis_trait<typename OutVector::basis_type>;
         using lhs_basis_traits = basis_trait<typename LeftVector::basis_type>;
 
         // The helper makes a contiguous copy of rhs key-value pairs
         // so the inner loop is always contiguous, rather than potentially
         // a linked list or other cache unfriendly data structure.
         // The graded helper also sorts the keys and constructs a buffer
         // of degree ranges that we can use to truncate products that
         // would overflow the max degree.
         graded_helper_type<RightVector> helper(rhs);
-        const auto &basis = out.basis();
+        const auto& basis = out.basis();
 
-        auto out_deg = std::min(out_basis_traits::max_degree(basis), lhs.degree() + rhs.degree());
+        auto out_deg = std::min(
+                out_basis_traits::max_degree(basis), lhs.degree() + rhs.degree()
+        );
         out.update_degree(out_deg);
-        const auto &lhs_basis = lhs.basis();
+        const auto& lhs_basis = lhs.basis();
         for (auto litem : lhs) {
             auto lkey = litem.key();
             auto lhs_degree = lhs_basis_traits::degree(lhs_basis, lkey);
             auto rhs_degree = out_deg - lhs_degree;
             for (auto ritem : helper.degree_range(rhs_degree)) {
-                asp_helper(out, m_mult(basis, lkey, ritem.first),
-                           fn(litem.value() * ritem.second));
+                asp_helper(
+                        out, m_mult(basis, lkey, ritem.first),
+                        fn(litem.value() * ritem.second)
+                );
             }
         }
     }
 
     template <typename LeftVector, typename RightVector, typename Fn>
-    void multiply_inplace(LeftVector &left, const RightVector &right, Fn op) const {
+    void
+    multiply_inplace(LeftVector& left, const RightVector& right, Fn op) const
+    {
         if (!left.empty() && !right.empty()) {
             LeftVector tmp(left.get_basis());
             caster::cast(*this).fma(tmp, left, right, op);
-            left = std::move(tmp);
+            left = move(tmp);
         } else {
             left.clear();
         }
     }
     template <typename LeftVector, typename RightVector, typename Fn>
-    void multiply_inplace(LeftVector &left, const RightVector &right, Fn op, deg_t max_deg) const {
+    void multiply_inplace(
+            LeftVector& left, const RightVector& right, Fn op, deg_t max_deg
+    ) const
+    {
         if (!left.empty() && !right.empty()) {
             LeftVector tmp(left.get_basis());
-            tmp.update_degree(std::min(left.degree() + right.degree(), max_deg));
+            tmp.update_degree(std::min(left.degree() + right.degree(), max_deg)
+            );
             caster::cast(*this).fma(tmp, left, right, op, max_deg);
-            left = std::move(tmp);
+            left = move(tmp);
         } else {
             left.clear();
         }
     }
-
 };
 
-template <typename Basis,
-    typename Coefficients,
-    typename Multiplication,
-    template <typename, typename> class VectorType,
-    template <typename> class StorageModel,
-    template <typename,
-    typename,
-    template <typename, typename> class,
-    template <typename> class,
-    typename...> class Base=vector,
-    typename... BaseArgs>
-class algebra : public Base<Basis, Coefficients, VectorType, StorageModel, BaseArgs...> {
-    using base_type = Base<Basis, Coefficients, VectorType, StorageModel, BaseArgs...>;
+template <
+        typename Basis, typename Coefficients, typename Multiplication,
+        template <typename, typename> class VectorType,
+        template <typename> class StorageModel,
+        template <
+                typename, typename, template <typename, typename> class,
+                template <typename> class, typename...>
+        class Base
+        = vector,
+        typename... BaseArgs>
+class algebra
+    : public Base<Basis, Coefficients, VectorType, StorageModel, BaseArgs...>
+{
+    using base_type
+            = Base<Basis, Coefficients, VectorType, StorageModel, BaseArgs...>;
 
 public:
-
     using vector_type = vector<Basis, Coefficients, VectorType, StorageModel>;
-    static_assert(std::is_same<base_type, vector_type>::value || std::is_base_of<vector_type, base_type>::value,
-                  "algebra must derive from vector");
+    static_assert(
+            is_same<base_type, vector_type>::value
+                    || is_base_of<vector_type, base_type>::value,
+            "algebra must derive from vector"
+    );
 
     using multiplication_type = Multiplication;
 
     using typename vector_type::basis_pointer;
     using multiplication_pointer = std::shared_ptr<const multiplication_type>;
 
     using typename vector_type::basis_type;
-    using typename vector_type::key_type;
     using typename vector_type::coefficient_ring;
-    using typename vector_type::scalar_type;
+    using typename vector_type::key_type;
     using typename vector_type::rational_type;
+    using typename vector_type::scalar_type;
 
 private:
     multiplication_pointer p_mult;
 
 public:
+    //    using vector_type::vector_type;
 
-//    using vector_type::vector_type;
-
-    algebra() : vector_type(),
-                p_mult(multiplication_registry<Multiplication>::get(vector_type::basis())) {}
-
-    explicit algebra(basis_pointer basis) : vector_type(std::move(basis)),
-                                            p_mult(multiplication_registry<Multiplication>::get(
-                                                vector_type::basis())) {}
-
-    explicit algebra(vector_type &&arg) : vector_type(std::move(arg)),
-                                          p_mult(multiplication_registry<Multiplication>::get(vector_type::basis())) {}
+    algebra()
+        : vector_type(), p_mult(multiplication_registry<Multiplication>::get(
+                                 vector_type::basis()
+                         ))
+    {}
+
+    explicit algebra(basis_pointer basis)
+        : vector_type(move(basis)),
+          p_mult(multiplication_registry<Multiplication>::get(
+                  vector_type::basis()
+          ))
+    {}
+
+    explicit algebra(vector_type&& arg)
+        : vector_type(move(arg)),
+          p_mult(multiplication_registry<Multiplication>::get(
+                  vector_type::basis()
+          ))
+    {}
 
     template <typename Scalar>
     algebra(basis_pointer basis, std::shared_ptr<const Multiplication> mul,
             std::initializer_list<Scalar> args)
-        : vector_type(std::move(basis), args), p_mult(std::move(mul)) {}
+        : vector_type(move(basis), args), p_mult(move(mul))
+    {}
 
     algebra(basis_pointer basis, std::shared_ptr<const Multiplication> mult)
-        : vector_type(basis), p_mult(std::move(mult)) {}
-
-    algebra(const vector_type &base, std::shared_ptr<const Multiplication> mult)
-        : vector_type(base), p_mult(std::move(mult)) {}
-
-    template <typename... Args, typename=std::enable_if_t<std::is_constructible<vector_type, Args...>::value>>
-    explicit algebra(basis_pointer basis, Args... args) : vector_type(std::move(basis),
-                                                                      std::forward<Args>(args)...),
-                                                          p_mult(multiplication_registry<
-                                                              Multiplication>::get(vector_type::basis())) {}
-
-    template <typename... Args, typename=std::enable_if_t<std::is_constructible<vector_type, Args...>::value>>
-    explicit algebra(basis_pointer basis, std::shared_ptr<const Multiplication> mul,
-                     Args &&... args) : vector_type(std::move(basis), std::forward<Args>(args)...),
-                                        p_mult(std::move(mul)) {}
+        : vector_type(basis), p_mult(move(mult))
+    {}
 
-    template <template <typename, typename> class OtherVectorType,
-        template <typename> class OtherStorageModel>
-    explicit algebra(const algebra<Basis, Coefficients, Multiplication, OtherVectorType, OtherStorageModel> &other)
-        : vector_type((other)), p_mult(other.p_mult) {}
+    algebra(const vector_type& base, std::shared_ptr<const Multiplication> mult)
+        : vector_type(base), p_mult(move(mult))
+    {}
+
+    template <
+            typename... Args,
+            typename
+            = enable_if_t<is_constructible<vector_type, Args...>::value>>
+    explicit algebra(basis_pointer basis, Args... args)
+        : vector_type(move(basis), forward<Args>(args)...),
+          p_mult(multiplication_registry<Multiplication>::get(
+                  vector_type::basis()
+          ))
+    {}
+
+    template <
+            typename... Args,
+            typename
+            = enable_if_t<is_constructible<vector_type, Args...>::value>>
+    explicit algebra(
+            basis_pointer basis, std::shared_ptr<const Multiplication> mul,
+            Args&&... args
+    )
+        : vector_type(move(basis), forward<Args>(args)...), p_mult(move(mul))
+    {}
+
+    template <
+            template <typename, typename> class OtherVectorType,
+            template <typename> class OtherStorageModel>
+    explicit algebra(const algebra<
+                     Basis, Coefficients, Multiplication, OtherVectorType,
+                     OtherStorageModel>& other)
+        : vector_type((other)), p_mult(other.p_mult)
+    {}
+
+    algebra(const algebra& other) : vector_type(other), p_mult(other.p_mult) {}
+
+    algebra(algebra&& other) noexcept
+        : vector_type(static_cast<vector_type&&>(other)),
+          p_mult(move(other.p_mult))
+    {}
 
-    algebra(const algebra &other) : vector_type(other), p_mult(other.p_mult) {}
-
-    algebra(algebra &&other) noexcept
-        : vector_type(static_cast<vector_type &&>(other)), p_mult(std::move(other.p_mult)) {}
-
-    algebra &operator=(const algebra &other) {
+    algebra& operator=(const algebra& other)
+    {
         if (&other != this) {
             vector_type::operator=(other);
             p_mult = other.p_mult;
         }
         return *this;
     }
 
-    algebra &operator=(algebra &&other) noexcept {
+    algebra& operator=(algebra&& other) noexcept
+    {
         if (&other != this) {
-            p_mult = std::move(other.p_mult);
-            vector_type::operator=(static_cast<vector_type &&>(other));
+            p_mult = move(other.p_mult);
+            vector_type::operator=(static_cast<vector_type&&>(other));
         }
         return *this;
     }
 
-    std::shared_ptr<const multiplication_type> multiplication() const noexcept { return p_mult; }
+    std::shared_ptr<const multiplication_type> multiplication() const noexcept
+    {
+        return p_mult;
+    }
 
-    algebra &add_mul(const algebra &lhs, const algebra &rhs) {
+    algebra& add_mul(const algebra& lhs, const algebra& rhs)
+    {
         using traits = multiplication_traits<Multiplication>;
-        traits::multiply_and_add(*multiplication(), *this, lhs, rhs, [](scalar_type s) { return s; });
+        traits::multiply_and_add(
+                *multiplication(), *this, lhs, rhs,
+                [](scalar_type s) { return s; }
+        );
         return *this;
     }
-    algebra &sub_mul(const algebra &lhs, const algebra &rhs) {
+    algebra& sub_mul(const algebra& lhs, const algebra& rhs)
+    {
         using traits = multiplication_traits<Multiplication>;
-        traits::multiply_and_add(*multiplication(), *this, lhs, rhs, [](scalar_type s) { return -s; });
+        traits::multiply_and_add(
+                *multiplication(), *this, lhs, rhs,
+                [](scalar_type s) { return -s; }
+        );
         return *this;
     }
 
-    algebra &mul_scal_prod(const algebra &rhs, const scalar_type &scal) {
+    algebra& mul_scal_prod(const algebra& rhs, const scalar_type& scal)
+    {
         using traits = multiplication_traits<Multiplication>;
-        traits::multiply_inplace(*multiplication(), *this, rhs, [scal](scalar_type s) { return s * scal; });
+        traits::multiply_inplace(
+                *multiplication(), *this, rhs,
+                [scal](scalar_type s) { return s * scal; }
+        );
         return *this;
     }
-    algebra &mul_scal_div(const algebra &rhs, const rational_type &scal) {
+    algebra& mul_scal_div(const algebra& rhs, const rational_type& scal)
+    {
         using traits = multiplication_traits<Multiplication>;
-        traits::multiply_inplace(*multiplication(), *this, rhs, [scal](scalar_type s) { return s / scal; });
+        traits::multiply_inplace(
+                *multiplication(), *this, rhs,
+                [scal](scalar_type s) { return s / scal; }
+        );
         return *this;
     }
 
-    algebra &mul_scal_div(const algebra &rhs, const rational_type &scal, deg_t degree) {
+    algebra&
+    mul_scal_div(const algebra& rhs, const rational_type& scal, deg_t degree)
+    {
         using traits = multiplication_traits<Multiplication>;
-        traits::multiply_inplace(*multiplication(), *this, rhs, [scal](scalar_type s) { return s / scal; }, degree);
+        traits::multiply_inplace(
+                *multiplication(), *this, rhs,
+                [scal](scalar_type s) { return s / scal; }, degree
+        );
         return *this;
     }
 };
 
-template <typename Basis, typename Coefficients, typename Multiplication,
-    template <typename, typename> class VectorType,
-    template <typename> class StorageModel,
-    typename Base=algebra<Basis, Coefficients, Multiplication, VectorType, StorageModel>>
-class unital_algebra : public Base {
-    using algebra_base = algebra<Basis, Coefficients, Multiplication, VectorType, StorageModel>;
-
-    static_assert(std::is_same<Base, algebra_base>::value || std::is_base_of<algebra_base, Base>::value,
-                  "algebra types must derive from algebra"
+template <
+        typename Basis, typename Coefficients, typename Multiplication,
+        template <typename, typename> class VectorType,
+        template <typename> class StorageModel,
+        typename Base = algebra<
+                Basis, Coefficients, Multiplication, VectorType, StorageModel>>
+class unital_algebra : public Base
+{
+    using algebra_base = algebra<
+            Basis, Coefficients, Multiplication, VectorType, StorageModel>;
+
+    static_assert(
+            is_same<Base, algebra_base>::value
+                    || is_base_of<algebra_base, Base>::value,
+            "algebra types must derive from algebra"
     );
+
 public:
     using typename algebra_base::basis_pointer;
     using typename algebra_base::scalar_type;
 
     using Base::Base;
 
-    template <typename Scalar, typename=std::enable_if_t<std::is_constructible<scalar_type, Scalar>::value>>
+    template <
+            typename Scalar,
+            typename
+            = enable_if_t<is_constructible<scalar_type, Scalar>::value>>
     explicit unital_algebra(basis_pointer basis, Scalar val)
-        : algebra_base(std::move(basis),
-                       basis_trait<Basis>::first_key(*algebra_base::p_basis),
-                       scalar_type(val)) {}
-
-    template <typename Scalar, typename=std::enable_if_t<std::is_constructible<scalar_type, Scalar>::value>>
+        : algebra_base(
+                move(basis),
+                basis_trait<Basis>::first_key(*algebra_base::p_basis),
+                scalar_type(val)
+        )
+    {}
+
+    template <
+            typename Scalar,
+            typename
+            = enable_if_t<is_constructible<scalar_type, Scalar>::value>>
     explicit unital_algebra(Scalar val)
-        : algebra_base(basis_trait<Basis>::first_key(*algebra_base::p_basis),
-                       scalar_type(val)) {}
-};
-
-template <typename Basis, typename Coefficients, typename Multiplication,
-    template <typename, typename> class VectorType,
-    template <typename> class StorageModel,
-    typename Base=algebra<Basis, Coefficients, Multiplication, VectorType, StorageModel>>
-class graded_algebra : public Base {
-
-    using algebra_base = algebra<Basis, Coefficients, Multiplication, VectorType, StorageModel>;
-
-    static_assert(std::is_same<Base, algebra_base>::value || std::is_base_of<algebra_base, Base>::value,
-                  "algebra types must derive from algebra"
+        : algebra_base(
+                basis_trait<Basis>::first_key(*algebra_base::p_basis),
+                scalar_type(val)
+        )
+    {}
+};
+
+template <
+        typename Basis, typename Coefficients, typename Multiplication,
+        template <typename, typename> class VectorType,
+        template <typename> class StorageModel,
+        typename Base = algebra<
+                Basis, Coefficients, Multiplication, VectorType, StorageModel>>
+class graded_algebra : public Base
+{
+
+    using algebra_base = algebra<
+            Basis, Coefficients, Multiplication, VectorType, StorageModel>;
+
+    static_assert(
+            is_same<Base, algebra_base>::value
+                    || is_base_of<algebra_base, Base>::value,
+            "algebra types must derive from algebra"
     );
 
 public:
     using Base::Base;
-
 };
 
-template <typename Basis, typename Coefficients, typename Multiplication,
-    template <typename, typename> class VectorType, template <typename> class StorageModel>
-using graded_unital_algebra = unital_algebra<Basis, Coefficients, Multiplication, VectorType, StorageModel,
-                                             graded_algebra<Basis, Coefficients, Multiplication, VectorType,
-                                                            StorageModel>>;
+template <
+        typename Basis, typename Coefficients, typename Multiplication,
+        template <typename, typename> class VectorType,
+        template <typename> class StorageModel>
+using graded_unital_algebra = unital_algebra<
+        Basis, Coefficients, Multiplication, VectorType, StorageModel,
+        graded_algebra<
+                Basis, Coefficients, Multiplication, VectorType, StorageModel>>;
 
 namespace dtl {
 
 template <typename Algebra>
-class is_algebra {
-    template <typename Basis,
-        typename Coefficients,
-        typename Multiplication,
-        template <typename, typename> class VType,
-        template <typename> class SModel>
-    static std::true_type test(algebra<Basis, Coefficients, Multiplication, VType, SModel> &);
+class is_algebra
+{
+    template <
+            typename Basis, typename Coefficients, typename Multiplication,
+            template <typename, typename> class VType,
+            template <typename> class SModel>
+    static true_type
+    test(algebra<Basis, Coefficients, Multiplication, VType, SModel>&);
 
-    static std::false_type test(...);
+    static false_type test(...);
 
 public:
-    static constexpr bool value = decltype(test(std::declval<Algebra &>()))::value;
+    static constexpr bool value = decltype(test(declval<Algebra&>()))::value;
 };
 
-} // namespace dtl
+}// namespace dtl
 
 template <typename Algebra>
-std::enable_if_t<dtl::is_algebra<Algebra>::value, Algebra>
-operator*(const Algebra &lhs, const Algebra &rhs) {
+enable_if_t<dtl::is_algebra<Algebra>::value, Algebra>
+operator*(const Algebra& lhs, const Algebra& rhs)
+{
     using traits = multiplication_traits<typename Algebra::multiplication_type>;
     using scalar_type = typename Algebra::scalar_type;
 
     auto multiplication = lhs.multiplication();
-    if (!multiplication) {
-        multiplication = rhs.multiplication();
-    }
+    if (!multiplication) { multiplication = rhs.multiplication(); }
     Algebra result(lhs.get_basis(), multiplication);
     if (multiplication && !lhs.empty() && !rhs.empty()) {
-        traits::multiply_and_add(*multiplication, result, lhs, rhs, [](scalar_type s) { return s; });
+        traits::multiply_and_add(
+                *multiplication, result, lhs, rhs,
+                [](scalar_type s) { return s; }
+        );
     }
     return result;
 }
 
 template <typename Algebra>
-std::enable_if_t<dtl::is_algebra<Algebra>::value, Algebra &>
-operator*=(Algebra &lhs, const Algebra &rhs) {
+enable_if_t<dtl::is_algebra<Algebra>::value, Algebra&>
+operator*=(Algebra& lhs, const Algebra& rhs)
+{
     using traits = multiplication_traits<typename Algebra::multiplication_type>;
     using scalar_type = typename Algebra::scalar_type;
     if (rhs.empty()) {
         lhs.clear();
         return lhs;
     }
     auto multiplication = lhs.multiplication();
-    if (!multiplication) {
-        multiplication = rhs.multiplication();
-    }
+    if (!multiplication) { multiplication = rhs.multiplication(); }
 
     if (multiplication && !lhs.empty()) {
-        traits::multiply_inplace(*multiplication, lhs, rhs, [](scalar_type arg) { return arg; });
+        traits::multiply_inplace(
+                *multiplication, lhs, rhs, [](scalar_type arg) { return arg; }
+        );
     }
     return lhs;
 }
 
 template <typename Algebra>
-std::enable_if_t<dtl::is_algebra<Algebra>::value, Algebra>
-commutator(const Algebra &lhs, const Algebra &rhs) {
+enable_if_t<dtl::is_algebra<Algebra>::value, Algebra>
+commutator(const Algebra& lhs, const Algebra& rhs)
+{
     using traits = multiplication_traits<typename Algebra::multiplication_type>;
     using cring = typename Algebra::coefficient_ring;
 
     auto multiplication = lhs.multiplication();
-    if (!multiplication) {
-        multiplication = rhs.multiplication();
-    }
+    if (!multiplication) { multiplication = rhs.multiplication(); }
 
     Algebra result(lhs.get_basis(), multiplication);
     if (multiplication && !lhs.empty() && !rhs.empty()) {
         traits::multiply_and_add(*multiplication, result, lhs, rhs);
-        traits::multiply_and_add(*multiplication, result, rhs, lhs, cring::uminus);
+        traits::multiply_and_add(
+                *multiplication, result, rhs, lhs, cring::uminus
+        );
     }
     return result;
 }
 
-template <typename Multiplication,
-    typename Coefficients,
-    typename LBasis,
-    template <typename, typename> class LVectorType,
-    template <typename> class LStorageModel,
-    typename RBasis,
-    template <typename, typename> class RVectorType,
-    template <typename> class RStorageModel
->
-std::enable_if_t<
-    multiplication_traits<Multiplication>::template
-    compatible_with<LBasis>::value &&
-        multiplication_traits<Multiplication>::template
-        compatible_with<RBasis>::value,
-    vector<LBasis, Coefficients, LVectorType, LStorageModel>
->
-multiply(const Multiplication &multiplication,
-         const vector<LBasis, Coefficients, LVectorType, LStorageModel> &lhs,
-         const vector<RBasis, Coefficients, RVectorType, RStorageModel> &rhs) {
+template <
+        typename Multiplication, typename Coefficients, typename LBasis,
+        template <typename, typename> class LVectorType,
+        template <typename> class LStorageModel, typename RBasis,
+        template <typename, typename> class RVectorType,
+        template <typename> class RStorageModel>
+enable_if_t<
+        multiplication_traits<Multiplication>::template compatible_with<
+                LBasis>::value
+                && multiplication_traits<Multiplication>::
+                        template compatible_with<RBasis>::value,
+        vector<LBasis, Coefficients, LVectorType, LStorageModel>>
+multiply(
+        const Multiplication& multiplication,
+        const vector<LBasis, Coefficients, LVectorType, LStorageModel>& lhs,
+        const vector<RBasis, Coefficients, RVectorType, RStorageModel>& rhs
+)
+{
     using traits = multiplication_traits<Multiplication>;
-    vector<LBasis, Coefficients, LVectorType, LStorageModel> result(lhs.basis());
+    vector<LBasis, Coefficients, LVectorType, LStorageModel> result(lhs.basis()
+    );
 
     traits::multiply_and_add(multiplication, result, lhs, rhs);
 
     return result;
 }
 
-} // namespace lal
+}// namespace lal
 
-#endif //LIBALGEBRA_LITE_ALGEBRA_H
+#endif// LIBALGEBRA_LITE_ALGEBRA_H
```

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/basis_traits.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/basis_traits.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/coefficients.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/coefficients.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/dense_vector.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/dense_vector.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/detail/notnull.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/detail/notnull.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/free_tensor.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/free_tensor.h`

 * *Files 17% similar despite different names*

```diff
@@ -8,49 +8,53 @@
 #include "implementation_types.h"
 #include "libalgebra_lite_export.h"
 
 #include <algorithm>
 #include <memory>
 #include <mutex>
 #include <unordered_map>
+#include <unordered_set>
 #include <utility>
 #include <vector>
 
 #include <boost/functional/hash.hpp>
 #include <boost/mpl/vector.hpp>
 
 #include "algebra.h"
 #include "basis_traits.h"
 #include "coefficients.h"
 #include "dense_vector.h"
+#include "detail/integer_maths.h"
 #include "registry.h"
 #include "tensor_basis.h"
+#include "unpacked_tensor_word.h"
 #include "vector_traits.h"
 
 namespace lal {
 
-template<typename, template<typename, typename> class,
-        template<typename> class>
+template <
+        typename, template <typename, typename> class,
+        template <typename> class>
 class free_tensor;
 
 namespace dtl {
 
-#define LAL_IS_TENSOR(V)                                                       \
-  std::is_same<typename V::basis_type, tensor_basis>::value
+#define LAL_IS_TENSOR(V) is_same<typename V::basis_type, tensor_basis>::value
 
 #define LAL_SAME_COEFFS(V1, V2)                                                \
-  std::is_same<typename V1::coefficient_ring,                                  \
-               typename V2::coefficient_ring>::value
+    is_same<typename V1::coefficient_ring, typename V2::coefficient_ring>::value
 
 #define LAL_TENSOR_COMPAT_RVV(R, V1, V2)                                       \
-  std::enable_if_t<LAL_IS_TENSOR(R) && LAL_IS_TENSOR(V1) &&                    \
-                   LAL_IS_TENSOR(V2) && LAL_SAME_COEFFS(R, V1) &&              \
-                   LAL_SAME_COEFFS(R, V2)>
-
-template<typename Coefficients> class dense_multiplication_helper {
+    enable_if_t<                                                               \
+            LAL_IS_TENSOR(R) && LAL_IS_TENSOR(V1) && LAL_IS_TENSOR(V2)         \
+            && LAL_SAME_COEFFS(R, V1) && LAL_SAME_COEFFS(R, V2)>
+
+template <typename Coefficients>
+class dense_multiplication_helper
+{
     using traits = coefficient_trait<Coefficients>;
     using scalar_type = typename traits::scalar_type;
 
     std::vector<scalar_type> left_read_buffer;
     std::vector<scalar_type> right_read_buffer;
     std::vector<scalar_type> write_buffer;
     std::vector<scalar_type> reverse_buffer;
@@ -66,36 +70,37 @@
     using tensor_type = dense_vector<tensor_basis, Coefficients>;
 
 public:
     dimn_t tile_width;
     dimn_t tile_size;
     deg_t tile_letters;
 
-    dense_multiplication_helper(tensor_type& out, const tensor_type& lhs,
-            const tensor_type& rhs)
-            :p_basis(&out.basis()), lhs_deg(lhs.degree()), rhs_deg(rhs.degree())
+    dense_multiplication_helper(
+            tensor_type& out, const tensor_type& lhs, const tensor_type& rhs
+    )
+        : p_basis(&out.basis()), lhs_deg(lhs.degree()), rhs_deg(rhs.degree())
     {
         const auto& powers = p_basis->powers();
 
         // TODO: replace with logic
         tile_letters = 1;
 
         left_ptr = lhs.as_ptr();
         right_ptr = rhs.as_ptr();
         out_ptr = out.as_mut_ptr();
 
         tile_width = powers[tile_letters];
-        tile_size = tile_width*tile_width;
+        tile_size = tile_width * tile_width;
 
         left_read_buffer.resize(tile_width);
         right_read_buffer.resize(tile_width);
         write_buffer.resize(tile_size);
 
-        if (lhs.degree()>1) {
-            reverse_buffer.resize(p_basis->size(lhs.degree()-1));
+        if (lhs.degree() > 1) {
+            reverse_buffer.resize(p_basis->size(lhs.degree() - 1));
         }
     }
 
     const scalar_type& left_unit() const noexcept { return *left_ptr; }
     const scalar_type& right_unit() const noexcept { return *right_ptr; }
 
     const scalar_type* left_tile() const noexcept
@@ -110,406 +115,660 @@
 
     deg_t lhs_degree() const noexcept { return lhs_deg; }
     deg_t rhs_degree() const noexcept { return rhs_deg; }
 
     const scalar_type* left_fwd_read(key_type k) const noexcept
     {
         auto offset = p_basis->start_of_degree(static_cast<deg_t>(k.degree()));
-        return left_ptr+k.index()*tile_width+offset;
+        return left_ptr + k.index() * tile_width + offset;
     }
     const scalar_type* right_fwd_read(key_type k) const noexcept
     {
         auto offset = p_basis->start_of_degree(static_cast<deg_t>(k.degree()));
-        return right_ptr+k.index()*tile_width+offset;
+        return right_ptr + k.index() * tile_width + offset;
     }
     scalar_type* fwd_write(key_type k) const noexcept
     {
         auto offset = p_basis->start_of_degree(static_cast<deg_t>(k.degree()));
-        return out_ptr+k.index()*tile_width+offset;
+        return out_ptr + k.index() * tile_width + offset;
     }
 
     void read_left_tile(key_type k) noexcept
     {
         auto offset = p_basis->start_of_degree(static_cast<deg_t>(k.degree()));
-        const auto* reverse_ptr =
-                reverse_buffer.data()+k.index()*tile_width+offset;
-        std::copy(reverse_ptr, reverse_ptr+tile_width, left_read_buffer.data());
+        const auto* reverse_ptr
+                = reverse_buffer.data() + k.index() * tile_width + offset;
+        std::copy(
+                reverse_ptr, reverse_ptr + tile_width, left_read_buffer.data()
+        );
     }
     void read_right_tile(key_type k)
     {
         auto offset = p_basis->start_of_degree(static_cast<deg_t>(k.degree()));
-        const auto* fwd_ptr = right_ptr+k.index()*tile_width+offset;
-        std::copy(fwd_ptr, fwd_ptr+tile_width, right_read_buffer.data());
+        const auto* fwd_ptr = right_ptr + k.index() * tile_width + offset;
+        std::copy(fwd_ptr, fwd_ptr + tile_width, right_read_buffer.data());
     }
     void write_tile_in(key_type k, key_type kr)
     {
-        const auto offset = p_basis->start_of_degree(k.degree()+2*tile_letters);
-        const auto* in_ptr = out_ptr+k.index()*tile_width+offset;
+        const auto offset
+                = p_basis->start_of_degree(k.degree() + 2 * tile_letters);
+        const auto* in_ptr = out_ptr + k.index() * tile_width + offset;
         auto* tile_ptr = write_tile();
-        const auto stride = p_basis->powers()[k.degree()+tile_letters];
+        const auto stride = p_basis->powers()[k.degree() + tile_letters];
 
-        for (dimn_t i = 0; i<tile_width; ++i) {
-            for (dimn_t j = 0; j<tile_width; ++j) {
-                tile_ptr[i*tile_width+j] = in_ptr[i*stride+j];
+        for (dimn_t i = 0; i < tile_width; ++i) {
+            for (dimn_t j = 0; j < tile_width; ++j) {
+                tile_ptr[i * tile_width + j] = in_ptr[i * stride + j];
             }
         }
     }
 
     void write_tile_out(key_type k, key_type kr)
     {
         const auto deg = k.degree();
-        const auto offset = p_basis->start_of_degree(deg+2*tile_letters);
-        const auto stride = p_basis->powers()[deg+tile_letters];
+        const auto offset = p_basis->start_of_degree(deg + 2 * tile_letters);
+        const auto stride = p_basis->powers()[deg + tile_letters];
 
-        auto* ptr = out_ptr+k.index()*tile_width+offset;
+        auto* ptr = out_ptr + k.index() * tile_width + offset;
         auto* tile_ptr = write_tile();
 
-        for (dimn_t i = 0; i<tile_width; ++i) {
-            for (dimn_t j = 0; j<tile_width; ++j) {
-                ptr[i*stride+j] = tile_ptr[i*tile_width+j];
+        for (dimn_t i = 0; i < tile_width; ++i) {
+            for (dimn_t j = 0; j < tile_width; ++j) {
+                ptr[i * stride + j] = tile_ptr[i * tile_width + j];
             }
         }
 
-        if (deg<p_basis->depth()) {
+        if (deg < p_basis->depth()) {
             // Write reverse data
         }
     }
 
     key_type reverse(key_type k) const noexcept
     {
         const auto width = p_basis->width();
         auto idx = k.index();
 
         typename key_type::index_type result_idx = 0;
         while (idx) {
             result_idx *= width;
-            result_idx += idx%width;
+            result_idx += idx % width;
             idx /= width;
         }
 
         return key_type{k.degree(), result_idx};
     }
-    std::pair<key_type, key_type> split_key(key_type k,
-            deg_t lhs_size) const noexcept
+    pair<key_type, key_type>
+    split_key(key_type k, deg_t lhs_size) const noexcept
     {
-        auto rhs_size = k.degree()-lhs_size;
+        auto rhs_size = k.degree() - lhs_size;
         auto split = p_basis->powers()[rhs_size];
-        return {key_type(lhs_size, k.index()/split),
-                key_type(rhs_size, k.index()%split)};
+        return {key_type(lhs_size, k.index() / split),
+                key_type(rhs_size, k.index() % split)};
     }
 
     dimn_t stride(deg_t deg) const noexcept
     {
-        return p_basis->powers()[deg-tile_letters];
+        return p_basis->powers()[deg - tile_letters];
     }
 
     key_type combine(key_type lhs, key_type rhs)
     {
         const auto rhs_deg = rhs.degree();
         const auto shift = p_basis->powers()[rhs_deg];
-        return key_type{lhs.degree()+rhs_deg, lhs.index()*shift+rhs.index()};
+        return key_type{
+                lhs.degree() + rhs_deg, lhs.index() * shift + rhs.index()};
     }
     dimn_t combine(dimn_t lhs, key_type rhs)
     {
         const auto rhs_deg = rhs.degree();
         const auto shift = p_basis->powers()[rhs_deg];
-        return lhs*shift+rhs.index();
+        return lhs * shift + rhs.index();
     }
 
-    std::pair<dimn_t, dimn_t> range_size(deg_t lhs, deg_t rhs) const noexcept
+    pair<dimn_t, dimn_t> range_size(deg_t lhs, deg_t rhs) const noexcept
     {
         const auto& powers = p_basis->powers();
         return {powers[lhs], powers[rhs]};
     }
 
-    dimn_t range_size(deg_t deg) const noexcept { return p_basis->powers()[deg]; }
+    dimn_t range_size(deg_t deg) const noexcept
+    {
+        return p_basis->powers()[deg];
+    }
 };
 
-} // namespace dtl
-
+}// namespace dtl
 
 class LIBALGEBRA_LITE_EXPORT free_tensor_multiplier
-    : public base_multiplier<free_tensor_multiplier, tensor_basis> {
+    : public base_multiplier<free_tensor_multiplier, tensor_basis>
+{
     deg_t m_width;
 
 public:
     using key_type = typename tensor_basis::key_type;
     using basis_type = tensor_basis;
 
-    explicit free_tensor_multiplier(deg_t width)
-        : m_width(width) {}
+    explicit free_tensor_multiplier(deg_t width) : m_width(width) {}
 
-    static key_type concat_product(const tensor_basis &basis, key_type lhs,
-                                   key_type rhs) {
+    static key_type
+    concat_product(const tensor_basis& basis, key_type lhs, key_type rhs)
+    {
         const auto lhs_deg = lhs.degree();
         const auto rhs_deg = rhs.degree();
         const auto shift = basis.powers()[rhs_deg];
 
         const auto idx = lhs.index() * shift + rhs.index();
         return key_type(lhs_deg + rhs_deg, idx);
     }
 
-    using product_type =
-        boost::container::small_vector<std::pair<key_type, int>, 1>;
+    using product_type = boost::container::small_vector<pair<key_type, int>, 1>;
 
-    product_type operator()(const tensor_basis &basis, key_type lhs,
-                            key_type rhs) const ;
+    product_type
+    operator()(const tensor_basis& basis, key_type lhs, key_type rhs) const;
 };
 
 class LIBALGEBRA_LITE_EXPORT free_tensor_multiplication
-        : public base_multiplication<free_tensor_multiplier, free_tensor_multiplication> {
-    using base_type = base_multiplication<free_tensor_multiplier, free_tensor_multiplication>;
-
-    template<typename C> using ctraits = coefficient_trait<C>;
-
-    template<typename C> using sca_ref = typename ctraits<C>::scalar_type&;
-    template<typename C>
+    : public base_multiplication<
+              free_tensor_multiplier, free_tensor_multiplication>
+{
+    using base_type = base_multiplication<
+            free_tensor_multiplier, free_tensor_multiplication>;
+
+    template <typename C>
+    using ctraits = coefficient_trait<C>;
+
+    template <typename C>
+    using sca_ref = typename ctraits<C>::scalar_type&;
+    template <typename C>
     using sca_cref = const typename ctraits<C>::scalar_type&;
-    template<typename C> using sca_ptr = typename ctraits<C>::scalar_type*;
-    template<typename C>
+    template <typename C>
+    using sca_ptr = typename ctraits<C>::scalar_type*;
+    template <typename C>
     using sca_rptr = typename ctraits<C>::scalar_type* LAL_RESTRICT;
-    template<typename C>
+    template <typename C>
     using sca_cptr = const typename ctraits<C>::scalar_type*;
-    template<typename C>
+    template <typename C>
     using sca_crptr = const typename ctraits<C>::scalar_type* LAL_RESTRICT;
 
     using key_type = typename tensor_basis::key_type;
 
-    template<typename Coefficients, typename Fn>
-    void
-    fma_dense_traditional(dtl::dense_multiplication_helper<Coefficients>& helper,
-            Fn fn, deg_t out_degree) const
+    template <typename Coefficients, typename Fn>
+    void fma_dense_traditional(
+            dtl::dense_multiplication_helper<Coefficients>& helper, Fn fn,
+            deg_t out_degree
+    ) const
     {
         auto lhs_deg = helper.lhs_degree();
         auto rhs_deg = helper.rhs_degree();
 
-        for (deg_t out_deg = out_degree; out_deg>=0; --out_deg) {
-            auto lhs_deg_min = std::max(0, out_deg-rhs_deg);
+        for (deg_t out_deg = out_degree; out_deg >= 0; --out_deg) {
+            auto lhs_deg_min = std::max(0, out_deg - rhs_deg);
             auto lhs_deg_max = std::min(out_deg, lhs_deg);
 
             auto* out_ptr = helper.fwd_write(key_type(out_deg, 0));
 
-            for (deg_t lh_deg = lhs_deg_max; lh_deg>=lhs_deg_min; --lh_deg) {
-                auto rh_deg = out_deg-lh_deg;
+            for (deg_t lh_deg = lhs_deg_max; lh_deg >= lhs_deg_min; --lh_deg) {
+                auto rh_deg = out_deg - lh_deg;
 
                 auto lhs_ptr = helper.left_fwd_read(key_type(lh_deg, 0));
                 auto rhs_ptr = helper.right_fwd_read(key_type(rh_deg, 0));
 
                 auto range_sizes = helper.range_size(lh_deg, rh_deg);
 
                 auto* p = out_ptr;
-                for (dimn_t i = 0; i<range_sizes.first; ++i) {
-                    for (dimn_t j = 0; j<range_sizes.second; ++j) {
-                        *(p++) += fn(lhs_ptr[i]*rhs_ptr[j]);
+                for (dimn_t i = 0; i < range_sizes.first; ++i) {
+                    for (dimn_t j = 0; j < range_sizes.second; ++j) {
+                        *(p++) += fn(lhs_ptr[i] * rhs_ptr[j]);
                     }
                 }
             }
         }
     }
 
-    template<typename C, typename Fn>
-    LAL_INLINE_ALWAYS static void impl_db0(sca_rptr<C> tile, sca_crptr<C> lhs_ptr,
-            sca_cref<C> rhs_unit, dimn_t stride,
-            dimn_t tile_width, Fn op) noexcept { }
-    template<typename C, typename Fn>
-    LAL_INLINE_ALWAYS static void impl_0bd(sca_rptr<C> tile, sca_cref<C> lhs_unit,
-            sca_crptr<C> rhs_ptr, dimn_t stride,
-            dimn_t tile_width, Fn op) noexcept { }
-
-    template<typename C, typename Fn>
-    LAL_INLINE_ALWAYS static void
-    impl_mid(sca_rptr<C> tile, sca_crptr<C> lhs_tile, sca_crptr<C> rhs_tile,
-            dimn_t stride, dimn_t tile_width, Fn op) noexcept { }
-
-    template<typename C, typename Fn>
-    LAL_INLINE_ALWAYS static void
-    impl_lb1(sca_rptr<C> tile, sca_cref<C> lhs_val, sca_crptr<C> rhs_tile,
-            dimn_t lhs_index, dimn_t tile_width, Fn op) noexcept { }
-
-    template<typename C, typename Fn>
-    LAL_INLINE_ALWAYS static void
-    impl_1br(sca_rptr<C> tile, sca_crptr<C> lhs_tile, sca_cref<C> rhs_val,
-            dimn_t index, dimn_t tile_width, Fn op) noexcept { }
-
-    template<typename Coefficients, typename Fn>
-    void fma_dense_tiled(dtl::dense_multiplication_helper<Coefficients>& helper,
-            Fn fn, deg_t out_degree) const
+    template <typename C, typename Fn>
+    LAL_INLINE_ALWAYS static void impl_db0(
+            sca_rptr<C> tile, sca_crptr<C> lhs_ptr, sca_cref<C> rhs_unit,
+            dimn_t stride, dimn_t tile_width, Fn op
+    ) noexcept
+    {}
+    template <typename C, typename Fn>
+    LAL_INLINE_ALWAYS static void impl_0bd(
+            sca_rptr<C> tile, sca_cref<C> lhs_unit, sca_crptr<C> rhs_ptr,
+            dimn_t stride, dimn_t tile_width, Fn op
+    ) noexcept
+    {}
+
+    template <typename C, typename Fn>
+    LAL_INLINE_ALWAYS static void impl_mid(
+            sca_rptr<C> tile, sca_crptr<C> lhs_tile, sca_crptr<C> rhs_tile,
+            dimn_t stride, dimn_t tile_width, Fn op
+    ) noexcept
+    {}
+
+    template <typename C, typename Fn>
+    LAL_INLINE_ALWAYS static void impl_lb1(
+            sca_rptr<C> tile, sca_cref<C> lhs_val, sca_crptr<C> rhs_tile,
+            dimn_t lhs_index, dimn_t tile_width, Fn op
+    ) noexcept
+    {}
+
+    template <typename C, typename Fn>
+    LAL_INLINE_ALWAYS static void impl_1br(
+            sca_rptr<C> tile, sca_crptr<C> lhs_tile, sca_cref<C> rhs_val,
+            dimn_t index, dimn_t tile_width, Fn op
+    ) noexcept
+    {}
+
+    template <typename Coefficients, typename Fn>
+    void fma_dense_tiled(
+            dtl::dense_multiplication_helper<Coefficients>& helper, Fn fn,
+            deg_t out_degree
+    ) const
     {
         using key_type = tensor_basis::key_type;
 
         auto lhs_deg = helper.lhs_degree();
         auto rhs_deg = helper.rhs_degree();
 
         auto* tile = helper.write_tile();
         const auto* left_rtile = helper.left_tile();
         const auto* right_rtile = helper.right_tile();
 
-        for (deg_t out_deg = out_degree; out_deg>2*helper.tile_letters;
+        for (deg_t out_deg = out_degree; out_deg > 2 * helper.tile_letters;
              --out_deg) {
             const auto stride = helper.stride(out_deg);
-            const auto adj_deg = out_deg-2*helper.tile_letters;
+            const auto adj_deg = out_deg - 2 * helper.tile_letters;
 
             // end is not actually a valid key, but it serves as a marker.
-            key_type start{adj_deg, 0}, end{adj_deg, helper.range_size(adj_deg)};
+            key_type start{adj_deg, 0},
+                    end{adj_deg, helper.range_size(adj_deg)};
 
-            for (auto k = start; k<end; ++k) {
+            for (auto k = start; k < end; ++k) {
                 auto k_reverse = helper.reverse(k);
 
                 helper.write_tile_in(k, k_reverse);
 
                 {
                     const auto& lhs_unit = helper.left_unit();
                     const auto* rhs_ptr = helper.right_fwd_read(k);
 
-                    for (dimn_t i = 0; i<helper.tile_width; ++i) {
-                        for (dimn_t j = 0; j<helper.tile_width; ++j) {
-                            tile[i*helper.tile_width+j] +=
-                                    fn(lhs_unit*rhs_ptr[i*stride+j]);
+                    for (dimn_t i = 0; i < helper.tile_width; ++i) {
+                        for (dimn_t j = 0; j < helper.tile_width; ++j) {
+                            tile[i * helper.tile_width + j]
+                                    += fn(lhs_unit * rhs_ptr[i * stride + j]);
                         }
                     }
                 }
 
                 {
                     const auto* lhs_ptr = helper.left_fwd_read(k);
                     const auto& rhs_unit = helper.right_unit();
-                    for (dimn_t i = 0; i<helper.tile_width; ++i) {
-                        for (dimn_t j = 0; j<helper.tile_width; ++j) {
-                            tile[i*helper.tile_width+j] +=
-                                    fn(lhs_ptr[i*stride+j]*rhs_unit);
+                    for (dimn_t i = 0; i < helper.tile_width; ++i) {
+                        for (dimn_t j = 0; j < helper.tile_width; ++j) {
+                            tile[i * helper.tile_width + j]
+                                    += fn(lhs_ptr[i * stride + j] * rhs_unit);
                         }
                     }
                 }
 
-                for (deg_t lh_deg = 1; lh_deg<helper.tile_letters; ++lh_deg) {
-                    auto rh_deg = adj_deg-lh_deg;
-                    for (dimn_t i = 0; i<helper.tile_width; ++i) {
+                for (deg_t lh_deg = 1; lh_deg < helper.tile_letters; ++lh_deg) {
+                    auto rh_deg = adj_deg - lh_deg;
+                    for (dimn_t i = 0; i < helper.tile_width; ++i) {
                         const auto split = helper.split_key(k, lh_deg);
-                        const auto& lhs_val = *helper.left_fwd_read(split.first);
+                        const auto& lhs_val
+                                = *helper.left_fwd_read(split.first);
                         helper.read_right_tile(helper.combine(split.first, k));
-                        for (dimn_t j = 0; j<helper.tile_width; ++j) {
-                            tile[i*helper.tile_width+j] += fn(lhs_val*right_rtile[j]);
+                        for (dimn_t j = 0; j < helper.tile_width; ++j) {
+                            tile[i * helper.tile_width + j]
+                                    += fn(lhs_val * right_rtile[j]);
                         }
                     }
                 }
 
-                for (deg_t lh_deg = 0; lh_deg<adj_deg; ++lh_deg) {
-                    const auto rh_deg = adj_deg-lh_deg;
+                for (deg_t lh_deg = 0; lh_deg < adj_deg; ++lh_deg) {
+                    const auto rh_deg = adj_deg - lh_deg;
                     auto split = helper.split_key(k, lh_deg);
                     helper.read_left_tile(helper.reverse(split.first));
                     helper.read_right_tile(split.second);
 
-                    for (dimn_t i = 0; i<helper.tile_width; ++i) {
-                        for (dimn_t j = 0; j<helper.tile_width; ++j) {
-                            tile[i*helper.tile_width+j] +=
-                                    fn(left_rtile[i]*right_rtile[j]);
+                    for (dimn_t i = 0; i < helper.tile_width; ++i) {
+                        for (dimn_t j = 0; j < helper.tile_width; ++j) {
+                            tile[i * helper.tile_width + j]
+                                    += fn(left_rtile[i] * right_rtile[j]);
                         }
                     }
                 }
 
-                for (deg_t rh_deg = 1; rh_deg<helper.tile_letters; ++rh_deg) {
-                    const auto lh_deg = adj_deg-rh_deg;
-                    for (dimn_t j = 0; j<helper.tile_width; ++j) {
-                        const auto split = helper.split_key(key_type(rh_deg, j), lh_deg);
-                        const auto& rhs_val = *helper.right_fwd_read(
-                                helper.combine(k_reverse, helper.reverse(split.first)));
+                for (deg_t rh_deg = 1; rh_deg < helper.tile_letters; ++rh_deg) {
+                    const auto lh_deg = adj_deg - rh_deg;
+                    for (dimn_t j = 0; j < helper.tile_width; ++j) {
+                        const auto split
+                                = helper.split_key(key_type(rh_deg, j), lh_deg);
+                        const auto& rhs_val
+                                = *helper.right_fwd_read(helper.combine(
+                                        k_reverse, helper.reverse(split.first)
+                                ));
                         helper.read_left_tile(split.second);
 
-                        for (dimn_t i = 0; i<helper.tile_width; ++i) {
-                            tile[i*helper.tile_width+j] += fn(left_rtile[i]*rhs_val);
+                        for (dimn_t i = 0; i < helper.tile_width; ++i) {
+                            tile[i * helper.tile_width + j]
+                                    += fn(left_rtile[i] * rhs_val);
                         }
                     }
                 }
 
                 helper.write_tile_out(k, k_reverse);
             }
         }
 
-        fma_dense_traditional(helper, fn, 2*helper.tile_letters);
+        fma_dense_traditional(helper, fn, 2 * helper.tile_letters);
     }
 
 public:
-    template<typename Coeff>
+    template <typename Coeff>
     using dense_tensor_vec = dense_vector<tensor_basis, Coeff>;
 
     using base_type::base_type;
 
     using base_type::fma;
     using base_type::multiply_inplace;
 
-    template<typename Coeff, typename Op>
-    void fma(dense_tensor_vec<Coeff>& out, const dense_tensor_vec<Coeff>& lhs,
-            const dense_tensor_vec<Coeff>& rhs, Op op) const
+    template <typename Coeff, typename Op>
+    void
+    fma(dense_tensor_vec<Coeff>& out, const dense_tensor_vec<Coeff>& lhs,
+        const dense_tensor_vec<Coeff>& rhs, Op op) const
     {
         fma(out, lhs, rhs, op, out.basis().depth());
     }
 
-    template<typename Coeff, typename Op>
-    void fma(dense_tensor_vec<Coeff>& out, const dense_tensor_vec<Coeff>& lhs,
-            const dense_tensor_vec<Coeff>& rhs, Op op, deg_t max_degree) const
+    template <typename Coeff, typename Op>
+    void
+    fma(dense_tensor_vec<Coeff>& out, const dense_tensor_vec<Coeff>& lhs,
+        const dense_tensor_vec<Coeff>& rhs, Op op, deg_t max_degree) const
     {
         const auto& basis = out.basis();
-        if (max_degree>=basis.depth()) {
-            max_degree = basis.depth();
-        }
+        if (max_degree >= basis.depth()) { max_degree = basis.depth(); }
 
-        deg_t out_degree = std::min(max_degree, lhs.degree()+rhs.degree());
+        deg_t out_degree = std::min(max_degree, lhs.degree() + rhs.degree());
 
         const auto out_size = basis.size(out_degree);
-        if (out.size()<out_size) {
+        if (out.size() < out_size) {
             /*
-             * The resize function will look for the smallest dimension larger than
-             * the requested dim, so if we give it size, it will look for the smallest
-             * dimension greater than size, not simply size. Thus, we subtract 1 to make
-             * sure the next smallest dimension is equal to size.
+             * The resize function will look for the smallest dimension larger
+             * than the requested dim, so if we give it size, it will look for
+             * the smallest dimension greater than size, not simply size. Thus,
+             * we subtract 1 to make sure the next smallest dimension is equal
+             * to size.
              */
-            out.resize(out_size-1);
+            out.resize(out_size - 1);
         }
 
         dtl::dense_multiplication_helper<Coeff> helper(out, lhs, rhs);
         //        if (out_degree > 2*helper.tile_letters) {
         //            fma_dense_tiled(helper, op, out_degree);
         //        } else {
         fma_dense_traditional(helper, op, out_degree);
         //        }
     }
-
-
 };
 
-
-
 #undef LAL_TENSOR_COMPAT_RVV
 #undef LAL_SAME_COEFFS
 #undef LAL_IS_TENSOR
 
-template<typename Coefficients, template<typename, typename> class VectorType,
-        template<typename> class StorageModel>
-class free_tensor
-        : public algebra<tensor_basis, Coefficients, free_tensor_multiplication,
-                         VectorType, StorageModel> {
-    using algebra_type =
-            algebra<tensor_basis, Coefficients, free_tensor_multiplication,
-                    VectorType, StorageModel>;
+namespace dtl {
+
+template <typename Coefficients>
+class antipode_helper
+{
+    using scalar_type = typename Coefficients::scalar_type;
+    using pointer = scalar_type*;
+    using const_pointer = const scalar_type*;
+
+    std::vector<pair<dimn_t, dimn_t>> permute;
+    pointer tile;
+
+    lal::basis_pointer<tensor_basis> p_basis;
+    deg_t tile_letters;
+    dimn_t tile_width;
+    dimn_t tile_size;
+    bool do_signing = true;
 
+    void read_tile(const_pointer src, dimn_t stride) const
+    {
+        for (dimn_t i = 0; i < tile_width; ++i) {
+            for (dimn_t j = 0; j < tile_width; ++j) {
+                tile[i * tile_width + j] = src[i * stride + j];
+            }
+        }
+    }
+
+    void write_tile(pointer dst, dimn_t stride) const
+    {
+        for (dimn_t i = 0; i < tile_width; ++i) {
+            for (dimn_t j = 0; j < tile_width; ++j) {
+                dst[i * stride + j] = move(tile[i * tile_width + j]);
+            }
+        }
+    }
 
-    static void resize_to_degree(free_tensor<Coefficients, dense_vector, StorageModel>& arg, deg_t degree) {
+    void handle_dense_untiled_level(
+            pointer LAL_RESTRICT dst, const_pointer LAL_RESTRICT src,
+            deg_t degree
+    ) const
+    {
+        if (degree == 0) {
+            // Degree 0 is easy, just copy the data from src to dst.
+            *dst = *src;
+        } else if (degree == 1) {
+            // Degree 1 is like degree 0, no permutation is needed so we only
+            // need to worry about signing
+            for (dimn_t i = 0; i < p_basis->width(); ++i) {
+                if (do_signing) {
+                    dst[i] = -src[i];
+                } else {
+                    dst[i] = src[i];
+                }
+            }
+        } else {
+            for (dimn_t i = 0; i < p_basis->powers()[degree]; ++i) {
+                auto ri = p_basis->reverse_idx(degree, i);
+                if (do_signing && !is_even(degree)) {
+                    dst[ri] = -src[i];
+                } else {
+                    dst[ri] = src[i];
+                }
+            }
+        }
+    }
+
+    void permute_tile() const
+    {
+        for (const auto& pids : permute) {
+            std::swap(tile[pids.first], tile[pids.second]);
+        }
+    }
+
+    void sign_tile() const
+    {
+        for (dimn_t i = 0; i < tile_size; ++i) { tile[i] = -tile[i]; }
+    }
+
+    void handle_dense_tiled_level(
+            pointer LAL_RESTRICT dst, const_pointer LAL_RESTRICT src,
+            deg_t degree
+    ) const
+    {
+        auto middle_degree = degree - 2 * tile_letters;
+        auto stride = p_basis->powers()[degree - tile_letters];
+        unpacked_tensor_word word(p_basis->width(), middle_degree);
+
+        for (dimn_t i = 0; i < p_basis->powers()[middle_degree]; ++i, ++word) {
+            auto ridx = word.to_reverse_index();
+//            auto ridx = p_basis->reverse_idx(middle_degree, i);
+
+            read_tile(src + i*tile_width, stride);
+            if (do_signing && !is_even(degree)) { sign_tile(); }
+            permute_tile();
+
+            write_tile(dst + ridx*tile_width, stride);
+        }
+    }
+
+    template <template <typename, typename> class VectorType>
+    void handle_antipode(
+            VectorType<tensor_basis, Coefficients>& result,
+            const VectorType<tensor_basis, Coefficients>& arg
+    ) const;
+
+    template <template <typename, typename...> class Storage>
+    void handle_antipode(
+            dense_vector_base<tensor_basis, Coefficients, Storage>& result,
+            const dense_vector_base<tensor_basis, Coefficients, Storage>& arg
+    ) const;
+
+public:
+    explicit antipode_helper(lal::basis_pointer<tensor_basis> basis)
+        : p_basis(basis)
+    {
+#if defined(LAL_MAX_TILE_LETTERS) && LAL_MAX_TILE_LETTERS == 0
+        tile_letters = 0;
+        tile_width = 0;
+#else
+#  if defined(LAL_MAX_TILE_LETTERS) && LAL_MAX_TILE_LETTERS > 0
+        constexpr deg_t max_letters = LAL_MAX_TILE_LETTERS;
+#  else
+        constexpr deg_t max_letters = 3;
+#  endif
+        tile_letters = std::min(max_letters, p_basis->depth() / 2);
+        tile_width = p_basis->powers()[tile_letters];
+#endif
+        tile_size = tile_width * tile_width;
+        if (tile_size > 0) {
+            tile = new scalar_type[tile_size]{};
+
+            std::unordered_set<dimn_t> seen;
+
+            for (dimn_t i = 0; i < tile_width; ++i) {
+                auto ri = p_basis->reverse_idx(tile_letters, i);
+                for (dimn_t j=0; j<tile_width; ++j) {
+                    auto rj = p_basis->reverse_idx(tile_letters, j);
+                    auto idx = i*tile_width + j;
+                    auto ridx = rj * tile_width + ri;
+                    if (ridx != idx && seen.find(idx) == seen.end()) {
+                        seen.insert(idx);
+                        seen.insert(ridx);
+                        permute.push_back({idx, ridx});
+                    }
+                }
+            }
+        } else {
+            tile = nullptr;
+        }
+    }
+    ~antipode_helper() { delete[] tile; }
+
+    template <typename Tensor>
+    enable_if_t<
+            is_same<Coefficients, typename Tensor::coefficient_ring>::value,
+            Tensor>
+    operator()(const Tensor& arg) const
+    {
+        Tensor result(p_basis, arg.multiplication());
+        handle_antipode(result.base_vector(), arg.base_vector());
+        return result;
+    }
+};
+
+template <typename Coefficients>
+template <template <typename, typename> class VectorType>
+void antipode_helper<Coefficients>::handle_antipode(
+        VectorType<tensor_basis, Coefficients>& result,
+        const VectorType<tensor_basis, Coefficients>& arg
+) const
+{
+    for (auto&& term : arg) {
+        auto key = p_basis->reverse_key(term.key());
+        if (do_signing && !is_even(key.degree())) {
+            result[key] = -term.value();
+        } else {
+            result[key] = term.value();
+        }
+    }
+}
+template <typename Coefficients>
+template <template <typename, typename...> class Storage>
+void antipode_helper<Coefficients>::handle_antipode(
+        dense_vector_base<tensor_basis, Coefficients, Storage>& result,
+        const dense_vector_base<tensor_basis, Coefficients, Storage>& arg
+) const
+{
+    result.resize_exact(arg.dimension());
+    auto* optr = result.as_mut_ptr();
+    const auto* iptr = arg.as_ptr();
+    const auto max_degree = arg.degree();
+    result.update_degree(max_degree);
+    deg_t deg = 0;
+
+    const auto untiled_levels = (tile_letters > 0)
+            ?  std::min(max_degree, 2 * tile_letters - 1)
+            : max_degree;
+
+    for (; deg <= untiled_levels; ++deg) {
+        handle_dense_untiled_level(optr, iptr, deg);
+        optr += p_basis->powers()[deg];
+        iptr += p_basis->powers()[deg];
+    }
+
+    // Handle the higher levels with tiling.
+    // Note this loop will do nothing if all the levels have already been done
+    for (; deg <= max_degree; ++deg) {
+        handle_dense_tiled_level(optr, iptr, deg);
+        optr += p_basis->powers()[deg];
+        iptr += p_basis->powers()[deg];
+    }
+
+}
+
+}// namespace dtl
+
+template <
+        typename Coefficients, template <typename, typename> class VectorType,
+        template <typename> class StorageModel>
+class free_tensor
+    : public algebra<
+              tensor_basis, Coefficients, free_tensor_multiplication,
+              VectorType, StorageModel>
+{
+    using algebra_type = algebra<
+            tensor_basis, Coefficients, free_tensor_multiplication, VectorType,
+            StorageModel>;
+
+    static void resize_to_degree(
+            free_tensor<Coefficients, dense_vector, StorageModel>& arg,
+            deg_t degree
+    )
+    {
         assert(degree <= basis_trait<tensor_basis>::max_degree(arg.basis()));
         auto size = arg.basis().size(degree);
         /*
          * The resize function will look for the smallest dimension larger than
-         * the requested dim, so if we give it size, it will look for the smallest
-         * dimension greater than size, not simply size. Thus, we subtract 1 to make
-         * sure the next smallest dimension is equal to size.
+         * the requested dim, so if we give it size, it will look for the
+         * smallest dimension greater than size, not simply size. Thus, we
+         * subtract 1 to make sure the next smallest dimension is equal to size.
          */
-        arg.base_vector().resize(size-1);
+        arg.base_vector().resize(size - 1);
         arg.base_vector().update_degree(degree);
     }
 
     template <template <typename, typename> class OVT>
-    static void resize_to_degree(free_tensor<Coefficients, OVT, StorageModel>& arg, deg_t degree) {
+    static void resize_to_degree(
+            free_tensor<Coefficients, OVT, StorageModel>& arg, deg_t degree
+    )
+    {
         arg.base_vector().update_degree(degree);
     }
 
 public:
     using typename algebra_type::basis_type;
     using typename algebra_type::coefficient_ring;
     using typename algebra_type::key_type;
@@ -517,67 +776,76 @@
     using typename algebra_type::scalar_type;
 
     using typename algebra_type::basis_pointer;
     using typename algebra_type::multiplication_pointer;
 
     using algebra_type::algebra_type;
 
-    free_tensor(basis_pointer basis, multiplication_pointer mul, scalar_type arg)
-            :algebra_type(basis, mul, key_type(0, 0), std::move(arg)) { }
+    free_tensor(
+            basis_pointer basis, multiplication_pointer mul, scalar_type arg
+    )
+        : algebra_type(basis, mul, key_type(0, 0), std::move(arg))
+    {}
 
     free_tensor(basis_pointer basis, scalar_type arg)
-            :algebra_type(basis, key_type(0, 0), std::move(arg)) { }
+        : algebra_type(basis, key_type(0, 0), std::move(arg))
+    {}
 
-
-    free_tensor& fmexp_inplace(const free_tensor& exp_arg) {
+    free_tensor& fmexp_inplace(const free_tensor& exp_arg)
+    {
         free_tensor original(*this), x(exp_arg);
 
         x[key_type(0, 0)] = scalar_type(0);
 
         auto degree = this->basis().depth();
         resize_to_degree(*this, degree);
-        for (deg_t i=degree; i >= 1; --i) {
+        for (deg_t i = degree; i >= 1; --i) {
             this->mul_scal_div(x, rational_type(i), degree - i + 1);
             *this += original;
         }
 
         return *this;
     }
 
-    free_tensor fmexp(const free_tensor& exp_arg) const {
+    free_tensor fmexp(const free_tensor& exp_arg) const
+    {
         free_tensor result(*this), x(exp_arg);
 
         x[key_type(0, 0)] = scalar_type(0);
 
         auto degree = this->basis().depth();
         resize_to_degree(result, degree);
 
-        for (deg_t i=degree; i>= 1; --i) {
+        for (deg_t i = degree; i >= 1; --i) {
             result.mul_scal_div(x, rational_type(i), degree - i + 1);
             result += *this;
         }
 
         return result;
     }
 
-    friend free_tensor exp(const free_tensor &arg) {
-        free_tensor result(arg.get_basis(), arg.multiplication(), scalar_type(1));
+    friend free_tensor exp(const free_tensor& arg)
+    {
+        free_tensor result(
+                arg.get_basis(), arg.multiplication(), scalar_type(1)
+        );
         free_tensor one(arg.get_basis(), arg.multiplication(), scalar_type(1));
 
         const auto degree = arg.basis().depth();
         resize_to_degree(result, degree);
         for (deg_t i = degree; i >= 1; --i) {
             result.mul_scal_div(arg, rational_type(i));
             result += one;
         }
 
         return result;
     }
 
-    friend free_tensor log(const free_tensor &arg) {
+    friend free_tensor log(const free_tensor& arg)
+    {
 
         auto x = arg;
         x[typename tensor_basis::key_type(0, 0)] = scalar_type(0);
 
         free_tensor result(arg.get_basis(), arg.multiplication());
         const auto degree = arg.basis().depth();
         resize_to_degree(result, degree);
@@ -591,41 +859,40 @@
             }
             result *= x;
         }
 
         return result;
     }
 
-    friend free_tensor inverse(const free_tensor &arg) {
+    friend free_tensor inverse(const free_tensor& arg)
+    {
 
-        const auto &a = arg[key_type(0, 0)];
+        const auto& a = arg[key_type(0, 0)];
         assert(a != Coefficients::zero());
         auto x = arg;
         x[key_type(0, 0)] = Coefficients::zero();
 
         const auto degree = arg.basis().depth();
-        free_tensor a_inverse(arg.get_basis(), arg.multiplication(), scalar_type(1) / a);
+        free_tensor a_inverse(
+                arg.get_basis(), arg.multiplication(), scalar_type(1) / a
+        );
         free_tensor result(a_inverse);
         resize_to_degree(result, degree);
 
         auto z = x / a;
-        for (deg_t d=0; d<degree; ++d) {
-            result = a_inverse + z*result;
-        }
+        for (deg_t d = 0; d < degree; ++d) { result = a_inverse + z * result; }
 
         return result;
     }
 
-    friend free_tensor antipode(const free_tensor& arg) {
-        // TODO: replace with implementation of antipode.
-//        return inverse(arg);
-        return arg;
+    friend free_tensor antipode(const free_tensor& arg)
+    {
+        dtl::antipode_helper<Coefficients> helper(arg.get_basis());
+        return helper(arg);
     }
-
 };
 
 LAL_EXPORT_TEMPLATE_CLASS(multiplication_registry, free_tensor_multiplication)
 
+}// namespace lal
 
-} // namespace lal
-
-#endif // LIBALGEBRA_LITE_FREE_TENSOR_H
+#endif// LIBALGEBRA_LITE_FREE_TENSOR_H
```

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/hall_set.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/hall_set.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/implementation_types.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/implementation_types.h`

 * *Files 23% similar despite different names*

```diff
@@ -3,56 +3,41 @@
 //
 
 #ifndef LIBALGEBRA_LITE_IMPLEMENTATION_TYPES_H
 #define LIBALGEBRA_LITE_IMPLEMENTATION_TYPES_H
 
 #include <cstddef>
 #include <cstdint>
+#include <utility>
 
-#include <boost/predef.h>
 
 #include "config.h"
+#include "detail/macros.h"
 
 #ifdef LAL_USE_LIBAGEBRA
 #include <libalgebra/libalgebra.h>
 #endif
 
 
 namespace lal {
 
 using dimn_t = std::size_t;
 using idimn_t = std::ptrdiff_t;
 using deg_t = std::int32_t;
 
 using let_t = std::size_t;
 
+using std::pair;
 
 
 } // namespace lal
 
 
-#if BOOST_COMP_MSVC
-#define LAL_INLINE_ALWAYS
-#define LAL_INLINE_NEVER
-#define LAL_RESTRICT
-#define LAL_UNUSED
-#elif BOOST_COMP_GNUC
-#define LAL_INLINE_ALWAYS __attribute__((always_inline))
-#define LAL_INLINE_NEVER __attribute__((noinline))
-#define LAL_RESTRICT __restrict
-#define LAL_UNUSED __attribute__((unused))
-#else
-#define LAL_INLINE_ALWAYS
-#define LAL_INLINE_NEVER
-#define LAL_RESTRICT
-#define LAL_UNUSED
-#endif
-
 
-#if WIN32
+#ifdef _WIN32
 #ifdef Libalgebra_Lite_EXPORTS
 #define LAL_EXPORT_TEMPLATE_CLASS(TMPL, ...) \
     extern template class TMPL<__VA_ARGS__>;
 #define LAL_EXPORT_TEMPLATE_STRUCT(TMPL, ...) \
     extern template struct TMPL<__VA_ARGS__>;
 #else
 #define LAL_EXPORT_TEMPLATE_CLASS(TMPL, ...) \
```

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/index_key.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/index_key.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/key_range.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/key_range.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/lie.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/lie.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/maps.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/maps.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/operators.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/operators.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/packed_integer.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/packed_integer.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/polynomial.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/polynomial.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/polynomial_basis.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/polynomial_basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/registry.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/registry.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/shuffle_tensor.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/shuffle_tensor.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/sparse_vector.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/sparse_vector.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/tensor_basis.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/tensor_basis.h`

 * *Files 10% similar despite different names*

```diff
@@ -93,14 +93,31 @@
     { return m_powers; }
 
     dimn_t key_to_index(key_type arg) const noexcept;
     key_type index_to_key(dimn_t arg) const noexcept;
 
     void advance_key(key_type& key) const noexcept;
 
+    dimn_t reverse_idx(deg_t degree, dimn_t idx) const noexcept {
+        dimn_t result = 0;
+        for (deg_t i = 0; i < degree; ++i) {
+            result *= m_width;
+            auto tmp = idx;
+            idx /= m_width;
+            result += tmp - idx * m_width;
+        }
+        return result;
+    }
+
+    key_type reverse_key(key_type arg) const noexcept {
+        auto degree = arg.degree();
+        auto idx = arg.index();
+        auto result_idx = reverse_idx(degree, idx);
+        return key_type{degree, result_idx};
+    }
 
 };
 
 LAL_EXPORT_TEMPLATE_CLASS(basis_registry, tensor_basis)
 
 } // namespace lal
```

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/unpacked_tensor_word.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/unpacked_tensor_word.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/vector.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/vector.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/vector_base.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/vector_base.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/vector_bundle.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/vector_bundle.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/include/libalgebra_lite/vector_traits.h` & `roughpy-0.0.4/external/libalgebra_lite/include/libalgebra_lite/vector_traits.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/src/algebra/free_tensor_multiplier.cpp` & `roughpy-0.0.4/external/libalgebra_lite/src/algebra/free_tensor_multiplier.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/src/algebra/half_shuffle_multiplier.cpp` & `roughpy-0.0.4/external/libalgebra_lite/src/algebra/half_shuffle_multiplier.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/src/algebra/lie_multiplier.cpp` & `roughpy-0.0.4/external/libalgebra_lite/src/algebra/lie_multiplier.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/src/algebra/polynomial_multiplier.cpp` & `roughpy-0.0.4/external/libalgebra_lite/src/algebra/polynomial_multiplier.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/src/algebra/shuffle_multiplier.cpp` & `roughpy-0.0.4/external/libalgebra_lite/src/algebra/shuffle_multiplier.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/src/basis/hall_set.cpp` & `roughpy-0.0.4/external/libalgebra_lite/src/basis/hall_set.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/src/basis/monomial.cpp` & `roughpy-0.0.4/external/libalgebra_lite/src/basis/monomial.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/src/basis/polynomial_basis.cpp` & `roughpy-0.0.4/external/libalgebra_lite/src/basis/polynomial_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/src/basis/tensor_basis.cpp` & `roughpy-0.0.4/external/libalgebra_lite/src/basis/tensor_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/src/basis/unpacked_tensor_word.cpp` & `roughpy-0.0.4/external/libalgebra_lite/src/basis/unpacked_tensor_word.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -48,29 +48,29 @@
 unpacked_tensor_word::unpacked_tensor_word(deg_t width, deg_t depth)
     : m_data(depth), m_width(width)
 {
 }
 
 void unpacked_tensor_word::advance(deg_t number)
 {
+    const auto degree = m_data.size();
+    if (degree == 0) { return; }
     assert(number < std::numeric_limits<letter_type>::max());
     dimn_t position = 0;
     do {
-        auto& let = m_data[position++];
+        auto& let = m_data[position];
         let += number;
+        number = 0;
         if (let >= m_width) {
-            number = let - m_width;
-            let = 0;
-            if (position == m_data.size()) {
-                m_data.push_back(0);
-            }
+            number = let / m_width;
+            let = let - number*m_width;
+            ++position;
         }
-
     }
-    while (number > 0);
+    while (number > 0 && position < degree);
 }
 
 
 unpacked_tensor_word& unpacked_tensor_word::operator++()
 {
     advance(1);
     return *this;
```

### Comparing `roughpy-0.0.3/external/libalgebra_lite/src/maps.cpp` & `roughpy-0.0.4/external/libalgebra_lite/src/maps.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/tests/lie/hall_basis.cpp` & `roughpy-0.0.4/external/libalgebra_lite/tests/lie/hall_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/tests/lie/lie_fixture.h` & `roughpy-0.0.4/external/libalgebra_lite/tests/lie/lie_fixture.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/tests/lie/lie_multiplier.cpp` & `roughpy-0.0.4/external/libalgebra_lite/tests/lie/lie_multiplier.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/tests/maps/maps.cpp` & `roughpy-0.0.4/external/libalgebra_lite/tests/maps/maps.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/tests/maps/maps_fixture.h` & `roughpy-0.0.4/external/libalgebra_lite/tests/maps/maps_fixture.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/tests/polynomial/polynomial_basis.cpp` & `roughpy-0.0.4/external/libalgebra_lite/tests/polynomial/polynomial_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/tests/polynomial/polynomial_fixture.h` & `roughpy-0.0.4/external/libalgebra_lite/tests/polynomial/polynomial_fixture.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/tests/tensors/CMakeLists.txt` & `roughpy-0.0.4/external/libalgebra_lite/tests/tensors/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/tests/tensors/dense_tensor.cpp` & `roughpy-0.0.4/external/libalgebra_lite/tests/tensors/dense_tensor.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/tests/tensors/free_tensor_multiplier.cpp` & `roughpy-0.0.4/external/libalgebra_lite/tests/tensors/free_tensor_multiplier.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/tests/tensors/half_shuffle_multiplier.cpp` & `roughpy-0.0.4/external/libalgebra_lite/tests/tensors/half_shuffle_multiplier.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/tests/tensors/shuffle_tensor_multiplier.cpp` & `roughpy-0.0.4/external/libalgebra_lite/tests/tensors/shuffle_tensor_multiplier.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/tests/tensors/sparse_tensor.cpp` & `roughpy-0.0.4/external/libalgebra_lite/tests/tensors/sparse_tensor.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/tests/tensors/tensor_basis.cpp` & `roughpy-0.0.4/external/libalgebra_lite/tests/tensors/tensor_basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/tests/tensors/tensor_fixture.h` & `roughpy-0.0.4/external/libalgebra_lite/tests/tensors/tensor_fixture.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/tests/tensors/tensor_multiplication.cpp` & `roughpy-0.0.4/external/libalgebra_lite/tests/tensors/tensor_multiplication.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/tests/utilities/packed_integer.cpp` & `roughpy-0.0.4/external/libalgebra_lite/tests/utilities/packed_integer.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/libalgebra_lite/vcpkg.json` & `roughpy-0.0.4/external/libalgebra_lite/vcpkg.json`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/CMakeLists.txt` & `roughpy-0.0.4/external/recombine/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/LICENSE.txt` & `roughpy-0.0.4/external/recombine/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/README.md` & `roughpy-0.0.4/external/recombine/README.md`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/recombine/CMakeLists.txt` & `roughpy-0.0.4/external/recombine/recombine/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/recombine/recombine/BufferConstructor.h` & `roughpy-0.0.4/external/recombine/recombine/recombine/BufferConstructor.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/recombine/recombine/Compare.cpp` & `roughpy-0.0.4/external/recombine/recombine/recombine/Compare.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/recombine/recombine/LinearAlgebraReductionTool.cpp` & `roughpy-0.0.4/external/recombine/recombine/recombine/LinearAlgebraReductionTool.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/recombine/recombine/LinearAlgebraReductionTool.h` & `roughpy-0.0.4/external/recombine/recombine/recombine/LinearAlgebraReductionTool.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/recombine/recombine/RdToPowers.cpp` & `roughpy-0.0.4/external/recombine/recombine/recombine/RdToPowers.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/recombine/recombine/SafeInt3.hpp` & `roughpy-0.0.4/external/recombine/recombine/recombine/SafeInt3.hpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/recombine/recombine/TreeBufferHelper.cpp` & `roughpy-0.0.4/external/recombine/recombine/recombine/TreeBufferHelper.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/recombine/recombine/TreeBufferHelper.h` & `roughpy-0.0.4/external/recombine/recombine/recombine/TreeBufferHelper.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/recombine/recombine/aligned_allocator.h` & `roughpy-0.0.4/external/recombine/recombine/recombine/aligned_allocator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/recombine/recombine/lapack_defns.h` & `roughpy-0.0.4/external/recombine/recombine/recombine/lapack_defns.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/recombine/recombine/lapack_fortran_definitions.h` & `roughpy-0.0.4/external/recombine/recombine/recombine/lapack_fortran_definitions.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/recombine/recombine/recombine.cpp` & `roughpy-0.0.4/external/recombine/recombine/recombine/recombine.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/recombine/recombine/recombine.h` & `roughpy-0.0.4/external/recombine/recombine/recombine/recombine.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/recombine/recombine/reweight.h` & `roughpy-0.0.4/external/recombine/recombine/recombine/reweight.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/recombine/recombine/stdafx.h` & `roughpy-0.0.4/external/recombine/recombine/recombine/stdafx.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/recombine/recombine/tjlUtilities.h` & `roughpy-0.0.4/external/recombine/recombine/recombine/tjlUtilities.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/test_recombine/CMakeLists.txt` & `roughpy-0.0.4/external/recombine/test_recombine/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/test_recombine/TestVec/EvaluateAllMonomials.h` & `roughpy-0.0.4/external/recombine/test_recombine/TestVec/EvaluateAllMonomials.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/test_recombine/TestVec/OstreamContainerOverloads.h` & `roughpy-0.0.4/external/recombine/test_recombine/TestVec/OstreamContainerOverloads.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/test_recombine/TestVec/ScopedWindowsPerformanceTimer.cpp` & `roughpy-0.0.4/external/recombine/test_recombine/TestVec/ScopedWindowsPerformanceTimer.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/test_recombine/TestVec/utils.h` & `roughpy-0.0.4/external/recombine/test_recombine/TestVec/utils.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/external/recombine/test_recombine/test_recombine.cpp` & `roughpy-0.0.4/external/recombine/test_recombine/test_recombine.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/CMakeLists.txt` & `roughpy-0.0.4/intervals/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/include/roughpy/intervals/dyadic.h` & `roughpy-0.0.4/intervals/include/roughpy/intervals/dyadic.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/include/roughpy/intervals/dyadic_interval.h` & `roughpy-0.0.4/intervals/include/roughpy/intervals/dyadic_interval.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/include/roughpy/intervals/interval.h` & `roughpy-0.0.4/intervals/include/roughpy/intervals/interval.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/include/roughpy/intervals/partition.h` & `roughpy-0.0.4/intervals/include/roughpy/intervals/partition.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/include/roughpy/intervals/real_interval.h` & `roughpy-0.0.4/intervals/include/roughpy/intervals/real_interval.h`

 * *Files 12% similar despite different names*

```diff
@@ -47,37 +47,55 @@
     RealInterval() = default;
     RealInterval(const RealInterval&) = default;
     RealInterval(RealInterval&&) noexcept = default;
 
     RealInterval& operator=(const RealInterval&) = default;
     RealInterval& operator=(RealInterval&&) noexcept = default;
 
-    RealInterval(param_t inf, param_t sup,
-                 IntervalType itype = IntervalType::Clopen)
+    RealInterval(
+            param_t inf, param_t sup, IntervalType itype = IntervalType::Clopen
+    )
         : Interval(itype), m_inf(inf), m_sup(sup)
     {
         if (m_inf > m_sup) { std::swap(m_inf, m_sup); }
     }
 
     explicit RealInterval(const Interval& interval)
         : Interval(interval.type()), m_inf(interval.inf()),
           m_sup(interval.sup())
     {}
 
     explicit RealInterval(const Interval& interval, IntervalType itype)
         : Interval(itype), m_inf(interval.inf()), m_sup(interval.sup())
     {}
 
-    RPY_NO_DISCARD
-    param_t inf() const override { return m_inf; }
-    RPY_NO_DISCARD
-    param_t sup() const override { return m_sup; }
+    static RealInterval unbounded() noexcept
+    {
+        return {-std::numeric_limits<param_t>::infinity(),
+                std::numeric_limits<param_t>::infinity()};
+    }
+
+    static RealInterval left_unbounded(
+            param_t sup = 0.0, IntervalType itype = IntervalType::Clopen
+    ) noexcept
+    {
+        return {-std::numeric_limits<param_t>::infinity(), sup, itype};
+    }
+
+    static RealInterval right_unbounded(
+            param_t inf = 0.0, IntervalType itype = IntervalType::Clopen
+    ) noexcept
+    {
+        return {inf, std::numeric_limits<param_t>::infinity(), itype};
+    }
+
+    RPY_NO_DISCARD param_t inf() const override { return m_inf; }
+    RPY_NO_DISCARD param_t sup() const override { return m_sup; }
 
-    RPY_NO_DISCARD
-    bool contains(const Interval& arg) const noexcept override;
+    RPY_NO_DISCARD bool contains(const Interval& arg) const noexcept override;
 
     RPY_SERIAL_SERIALIZE_FN();
 };
 
 RPY_SERIAL_SERIALIZE_FN_IMPL(RealInterval)
 {
     RPY_SERIAL_SERIALIZE_NVP("type", m_interval_type);
```

### Comparing `roughpy-0.0.3/intervals/include/roughpy/intervals/segmentation.h` & `roughpy-0.0.4/intervals/include/roughpy/intervals/segmentation.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/src/dyadic.cpp` & `roughpy-0.0.4/intervals/src/dyadic.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/src/dyadic_interval.cpp` & `roughpy-0.0.4/intervals/src/dyadic_interval.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/src/dyadic_searcher.cpp` & `roughpy-0.0.4/intervals/src/dyadic_searcher.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/src/dyadic_searcher.h` & `roughpy-0.0.4/intervals/src/dyadic_searcher.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/src/interval.cpp` & `roughpy-0.0.4/intervals/src/interval.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/src/partition.cpp` & `roughpy-0.0.4/intervals/src/partition.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/src/real_interval.cpp` & `roughpy-0.0.4/intervals/src/real_interval.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/src/scaled_predicate.cpp` & `roughpy-0.0.4/intervals/src/scaled_predicate.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/src/scaled_predicate.h` & `roughpy-0.0.4/intervals/src/scaled_predicate.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/src/segmentation.cpp` & `roughpy-0.0.4/intervals/src/segmentation.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/src/test_dyadic.cpp` & `roughpy-0.0.4/intervals/src/test_dyadic.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/src/test_dyadic_intervals.cpp` & `roughpy-0.0.4/intervals/src/test_dyadic_intervals.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/src/test_partition.cpp` & `roughpy-0.0.4/intervals/src/test_partition.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/intervals/src/test_real_interval.cpp` & `roughpy-0.0.4/intervals/src/test_real_interval.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/la_context/CMakeLists.txt` & `roughpy-0.0.4/la_context/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/la_context/include/roughpy/la_context/free_tensor_info.h` & `roughpy-0.0.4/la_context/include/roughpy/la_context/free_tensor_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/la_context/include/roughpy/la_context/lie_basis_info.h` & `roughpy-0.0.4/la_context/include/roughpy/la_context/lie_basis_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/la_context/include/roughpy/la_context/lie_info.h` & `roughpy-0.0.4/la_context/include/roughpy/la_context/lie_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/la_context/include/roughpy/la_context/shuffle_tensor_info.h` & `roughpy-0.0.4/la_context/include/roughpy/la_context/shuffle_tensor_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/la_context/include/roughpy/la_context/tensor_basis_info.h` & `roughpy-0.0.4/la_context/include/roughpy/la_context/tensor_basis_info.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/la_context/include/roughpy/la_context/vector_iterator.h` & `roughpy-0.0.4/la_context/include/roughpy/la_context/vector_iterator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/la_context/include/roughpy/la_context/vector_type_helper.h` & `roughpy-0.0.4/la_context/include/roughpy/la_context/vector_type_helper.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/la_context/include/roughpy/la_context/vector_type_selector.h` & `roughpy-0.0.4/la_context/include/roughpy/la_context/vector_type_selector.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/la_context/include/roughpy/la_context.h` & `roughpy-0.0.4/la_context/include/roughpy/la_context.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/la_context/src/la_context.cpp` & `roughpy-0.0.4/la_context/src/la_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/platform/CMakeLists.txt` & `roughpy-0.0.4/platform/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/platform/include/roughpy/platform/configuration.h` & `roughpy-0.0.4/platform/include/roughpy/platform/configuration.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/platform/include/roughpy/platform/filesystem.h` & `roughpy-0.0.4/platform/include/roughpy/platform/filesystem.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/platform/include/roughpy/platform/serialization.h` & `roughpy-0.0.4/platform/include/roughpy/platform/serialization.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/platform/include/roughpy/platform/serialization_instantiations.inl` & `roughpy-0.0.4/platform/include/roughpy/platform/serialization_instantiations.inl`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/platform/include/roughpy/platform.h` & `roughpy-0.0.4/platform/include/roughpy/platform.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/platform/src/configuration.cpp` & `roughpy-0.0.4/platform/src/configuration.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/pyproject.toml` & `roughpy-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -39,27 +39,29 @@
 
 [build-system]
 requires = [
     "scikit-build-core[pyproject]",
     "pybind11",
     "ninja; platform_system!='Windows'",
     "oldest-supported-numpy",
-    "mkl-devel",
-    "mkl-static",
-    "intel-openmp; platform_system!='Windows'"
+    "mkl-devel; platform_machine in 'x86_64 x86 AMD64'",
+    "mkl-static; platform_machine in 'x86_64 x86 AMD64'",
+    "intel-openmp; platform_machine in 'x86_64 x86' and platform_system!='Windows'"
 ]
 build-backend = "scikit_build_core.build"
 
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 
 [tool.scikit-build]
 wheel.packages = []
+cmake.verbose = true
+logging.level = "INFO"
 cmake.build-type = "Release"
 experimental=true
 metadata.readme.provider = "scikit_build_core.metadata.fancy_pypi_readme"
 
 [tool.scikit-build.metadata.version]
 provider = "version_from_file"
 provider-path = "tools"
@@ -78,15 +80,16 @@
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "CHANGELOG"
 
 # From the documentation
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.substitutions]]
 # Literal TOML strings (single quotes) need no escaping of backslashes.
 pattern = '\[(.+?)\]\(((?!https?://)\S+?)\)'
-replacement = '[\1](https://github.com/datasig-ac-uk/roughpy/tree/main\g<2>)'
+replacement = '[\1](https://github.com/datasig-ac-uk/roughpy/tree/main/\g<2>)'
+
 [tool.scikit-build.cmake.define]
 ROUGHPY_BUILD_TESTS = "OFF"
 
 [tool.setuptools_scm]
 write_to = "VERSION.txt"
 tag_regex = "^(?P<prefix>v)?(?P<version>[^\\+]+)(?P<suffix>.*)?$"
 version_scheme = "release-branch-semver"
```

### Comparing `roughpy-0.0.3/roughpy/CMakeLists.txt` & `roughpy-0.0.4/roughpy/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/__init__.py` & `roughpy-0.0.4/roughpy/__init__.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/algebra.cpp` & `roughpy-0.0.4/roughpy/src/algebra/algebra.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/algebra.h` & `roughpy-0.0.4/roughpy/src/algebra/algebra.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/algebra_iterator.cpp` & `roughpy-0.0.4/roughpy/src/algebra/algebra_iterator.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/algebra_iterator.h` & `roughpy-0.0.4/roughpy/src/algebra/algebra_iterator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/basis.cpp` & `roughpy-0.0.4/roughpy/src/algebra/basis.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/basis.h` & `roughpy-0.0.4/roughpy/src/algebra/basis.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/context.cpp` & `roughpy-0.0.4/roughpy/src/algebra/context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/context.h` & `roughpy-0.0.4/roughpy/src/algebra/context.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/free_tensor.cpp` & `roughpy-0.0.4/roughpy/src/algebra/free_tensor.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,15 @@
 
     klass.def("__getitem__", [](const FreeTensor& self, key_type key) {
         return self[key];
     });
 
     klass.def("exp", &FreeTensor::exp);
     klass.def("log", &FreeTensor::log);
+    klass.def("antipode", &FreeTensor::antipode);
 //    klass.def("inverse", &FreeTensor::inverse);
     klass.def("fmexp", &FreeTensor::fmexp, "other"_a);
 //
     klass.def("__repr__", [](const FreeTensor& self) {
         std::stringstream ss;
         ss << "FreeTensor(width=" << *self.width()
            << ", depth=" << *self.depth();
```

### Comparing `roughpy-0.0.3/roughpy/src/algebra/free_tensor.h` & `roughpy-0.0.4/roughpy/src/algebra/free_tensor.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/lie.cpp` & `roughpy-0.0.4/roughpy/src/algebra/lie.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/lie.h` & `roughpy-0.0.4/roughpy/src/algebra/lie.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/lie_key.cpp` & `roughpy-0.0.4/roughpy/src/algebra/lie_key.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/lie_key.h` & `roughpy-0.0.4/roughpy/src/algebra/lie_key.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/lie_key_iterator.cpp` & `roughpy-0.0.4/roughpy/src/algebra/lie_key_iterator.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/lie_key_iterator.h` & `roughpy-0.0.4/roughpy/src/algebra/lie_key_iterator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/lie_letter.cpp` & `roughpy-0.0.4/roughpy/src/algebra/lie_letter.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/lie_letter.h` & `roughpy-0.0.4/roughpy/src/algebra/lie_letter.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/setup_algebra_type.h` & `roughpy-0.0.4/roughpy/src/algebra/setup_algebra_type.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/shuffle_tensor.cpp` & `roughpy-0.0.4/roughpy/src/algebra/shuffle_tensor.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/shuffle_tensor.h` & `roughpy-0.0.4/roughpy/src/algebra/shuffle_tensor.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/tensor_key.cpp` & `roughpy-0.0.4/roughpy/src/algebra/tensor_key.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/tensor_key.h` & `roughpy-0.0.4/roughpy/src/algebra/tensor_key.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/tensor_key_iterator.cpp` & `roughpy-0.0.4/roughpy/src/algebra/tensor_key_iterator.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/algebra/tensor_key_iterator.h` & `roughpy-0.0.4/roughpy/src/algebra/tensor_key_iterator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/args/convert_timestamp.cpp` & `roughpy-0.0.4/roughpy/src/args/convert_timestamp.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/args/convert_timestamp.h` & `roughpy-0.0.4/roughpy/src/args/convert_timestamp.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/args/kwargs_to_path_metadata.cpp` & `roughpy-0.0.4/roughpy/src/args/kwargs_to_path_metadata.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/args/kwargs_to_path_metadata.h` & `roughpy-0.0.4/roughpy/src/args/kwargs_to_path_metadata.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/args/kwargs_to_vector_construction.cpp` & `roughpy-0.0.4/roughpy/src/args/kwargs_to_vector_construction.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/args/kwargs_to_vector_construction.h` & `roughpy-0.0.4/roughpy/src/args/kwargs_to_vector_construction.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/args/numpy.cpp` & `roughpy-0.0.4/roughpy/src/args/numpy.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/args/numpy.h` & `roughpy-0.0.4/roughpy/src/args/numpy.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/args/parse_schema.cpp` & `roughpy-0.0.4/roughpy/src/args/parse_schema.cpp`

 * *Files 27% similar despite different names*

```diff
@@ -202,183 +202,183 @@
             );
         } else {
             throw py::type_error("unsupported type in schema specification");
         }
     }
 }
 
-void handle_timestamp_pair(StreamSchema* schema, py::object data);
-
-RPY_NO_DISCARD
-pair<ChannelType, string>
-get_type_and_variant(StreamSchema* schema, py::object data)
-{
-    if (py::isinstance<py::dict>(data)) {
-        auto data_dict = py::reinterpret_borrow<py::dict>(data);
-        RPY_CHECK(data_dict.contains("data"));
-
-        if (data_dict.contains("type")) {
-            auto type = py_to_channel_type(data_dict["type"]);
-            if (type == ChannelType::Categorical) {
-                return {type, data_dict["data"].cast<string>()};
-            }
-            return {type, {}};
-        }
-
-        return get_type_and_variant(schema, data_dict["data"]);
-    }
-
-    if (py::isinstance<py::tuple>(data)) {
-        auto data_tuple = py::reinterpret_borrow<py::tuple>(data);
-        if (data_tuple.size() == 1) {
-            return get_type_and_variant(
-                    schema, py::reinterpret_borrow<py::object>(data_tuple[0])
-            );
-        }
-
-        // data is (type, data, ...)
-        auto type = py_to_channel_type(data_tuple[0]);
-        if (type == ChannelType::Categorical) {
-            return {type, data_tuple[1].cast<string>()};
-        }
-
-        return {type, {}};
-    }
-
-    // The data is a plain value, infer from type
-    if (py::isinstance<py::str>(data)) {
-        return {ChannelType::Categorical, data.cast<string>()};
-    }
-
-    // TODO: IN the future, use the schema to determine what should be
-    // returned here, but for now hard-code increment
-    return {ChannelType::Increment, {}};
-}
-
-inline void
-handle_labeled_data(StreamSchema* schema, string label, py::object data)
-{
-    auto [type, variant] = get_type_and_variant(schema, std::move(data));
-    auto found = schema->find(label);
-    if (found != schema->end()) {
-        RPY_CHECK(type == found->second.type());
-
-        if (type == ChannelType::Categorical) {
-            found->second.insert_variant(std::move(variant));
-        }
-        // TODO: add checks for other data types
-    } else {
-        switch (type) {
-            case ChannelType::Increment:
-                schema->insert_increment(std::move(label));
-                break;
-            case ChannelType::Value:
-                schema->insert_value(std::move(label));
-                break;
-            case ChannelType::Categorical:
-                schema->insert_categorical(std::move(label))
-                        .add_variant(std::move(variant));
-                break;
-            case ChannelType::Lie:
-                // TODO: Handle Lie case?
-                break;
-        }
-    }
-}
-
-/**
- * @brief Handle tuple of (label, *data)
- */
-inline void handle_data_tuple(StreamSchema* schema, const py::sequence& seq)
-{
-    auto length = py::len(seq);
-    RPY_CHECK(length > 1);
-
-    auto label = seq[0].cast<string>();
-    handle_labeled_data(schema, std::move(label), seq[py::slice(1, {}, {})]);
-}
-
-/**
- * @brief Handle dict of {label: value, ...}
- *
- */
-inline void handle_data_dict(StreamSchema* schema, const py::dict& data_dict)
-{
-    //    py::print(data_dict);
-    //    RPY_CHECK(data_dict.contains("label"));
-    //    RPY_CHECK(data_dict.contains("data"));
-    //    auto label = data_dict["label"].cast<string>();
-    //
-    //    if (data_dict.contains("type")) {
-    //        auto to_pass = py::make_tuple(data_dict["type"],
-    //        data_dict["data"]); handle_labeled_data(schema, std::move(label),
-    //        std::move(to_pass));
-    //    } else {
-    //        auto to_pass =
-    //        py::reinterpret_borrow<py::object>(data_dict["data"]);
-    //        handle_labeled_data(schema, std::move(label), std::move(to_pass));
-    //    }
-    for (auto&& [label, value] : data_dict) {
-        auto true_label = label.cast<string>();
-        handle_labeled_data(
-                schema, std::move(true_label),
-                py::reinterpret_borrow<py::object>(value)
-        );
-    }
-}
-
-void handle_timestamp_pair(StreamSchema* schema, py::object data)
-{
-    if (py::isinstance<py::dict>(data)) {
-        auto data_dict = py::reinterpret_borrow<py::dict>(data);
-        handle_data_dict(schema, data_dict);
-    } else if (py::isinstance<py::tuple>(data)) {
-        auto data_tuple = py::reinterpret_borrow<py::tuple>(data);
-        handle_data_tuple(schema, data_tuple);
-    } else if (py::isinstance<py::sequence>(data)) {
-        auto data_seq = py::reinterpret_borrow<py::sequence>(data);
-
-        for (auto&& it_data : data_seq) {
-            auto inner = py::reinterpret_borrow<py::object>(it_data);
-            handle_timestamp_pair(schema, std::move(inner));
-        }
-    } else {
-        throw py::value_error("expected dict, tuple, or other sequence");
-    }
-}
-
-inline void handle_dict_stream(StreamSchema* schema, const py::dict& data)
-{
-    for (auto&& [timestamp, tick_value] : data) {
-        handle_timestamp_pair(
-                schema, py::reinterpret_borrow<py::object>(tick_value)
-        );
-    }
-}
-
-inline void
-handle_tuple_sequence(StreamSchema* schema, const py::sequence& data)
-{
-    for (auto&& it_value : data) {
-        RPY_CHECK(py::isinstance<py::sequence>(it_value));
-        auto inner = py::reinterpret_borrow<py::sequence>(it_value);
-        auto len = py::len(inner);
-
-        RPY_CHECK(len > 1);
-        if (len == 2) {
-            handle_timestamp_pair(schema, inner[1]);
-        } else if (len <= 4) {
-            auto right = inner[py::slice(1, {}, {})];
-            handle_timestamp_pair(schema, right);
-        } else {
-            throw py::value_error("expected tuple with no more than 4 elements"
-            );
-        }
-    }
-}
+//void handle_timestamp_pair(StreamSchema* schema, py::object data);
+//
+//RPY_NO_DISCARD
+//pair<ChannelType, string>
+//get_type_and_variant(StreamSchema* schema, py::object data)
+//{
+//    if (py::isinstance<py::dict>(data)) {
+//        auto data_dict = py::reinterpret_borrow<py::dict>(data);
+//        RPY_CHECK(data_dict.contains("data"));
+//
+//        if (data_dict.contains("type")) {
+//            auto type = py_to_channel_type(data_dict["type"]);
+//            if (type == ChannelType::Categorical) {
+//                return {type, data_dict["data"].cast<string>()};
+//            }
+//            return {type, {}};
+//        }
+//
+//        return get_type_and_variant(schema, data_dict["data"]);
+//    }
+//
+//    if (py::isinstance<py::tuple>(data)) {
+//        auto data_tuple = py::reinterpret_borrow<py::tuple>(data);
+//        if (data_tuple.size() == 1) {
+//            return get_type_and_variant(
+//                    schema, py::reinterpret_borrow<py::object>(data_tuple[0])
+//            );
+//        }
+//
+//        // data is (type, data, ...)
+//        auto type = py_to_channel_type(data_tuple[0]);
+//        if (type == ChannelType::Categorical) {
+//            return {type, data_tuple[1].cast<string>()};
+//        }
+//
+//        return {type, {}};
+//    }
+//
+//    // The data is a plain value, infer from type
+//    if (py::isinstance<py::str>(data)) {
+//        return {ChannelType::Categorical, data.cast<string>()};
+//    }
+//
+//    // TODO: IN the future, use the schema to determine what should be
+//    // returned here, but for now hard-code increment
+//    return {ChannelType::Increment, {}};
+//}
+//
+//inline void
+//handle_labeled_data(StreamSchema* schema, string label, py::object data)
+//{
+//    auto [type, variant] = get_type_and_variant(schema, std::move(data));
+//    auto found = schema->find(label);
+//    if (found != schema->end()) {
+//        RPY_CHECK(type == found->second.type());
+//
+//        if (type == ChannelType::Categorical) {
+//            found->second.insert_variant(std::move(variant));
+//        }
+//        // TODO: add checks for other data types
+//    } else {
+//        switch (type) {
+//            case ChannelType::Increment:
+//                schema->insert_increment(std::move(label));
+//                break;
+//            case ChannelType::Value:
+//                schema->insert_value(std::move(label));
+//                break;
+//            case ChannelType::Categorical:
+//                schema->insert_categorical(std::move(label))
+//                        .add_variant(std::move(variant));
+//                break;
+//            case ChannelType::Lie:
+//                // TODO: Handle Lie case?
+//                break;
+//        }
+//    }
+//}
+//
+///**
+// * @brief Handle tuple of (label, *data)
+// */
+//inline void handle_data_tuple(StreamSchema* schema, const py::sequence& seq)
+//{
+//    auto length = py::len(seq);
+//    RPY_CHECK(length > 1);
+//
+//    auto label = seq[0].cast<string>();
+//    handle_labeled_data(schema, std::move(label), seq[py::slice(1, {}, {})]);
+//}
+//
+///**
+// * @brief Handle dict of {label: value, ...}
+// *
+// */
+//inline void handle_data_dict(StreamSchema* schema, const py::dict& data_dict)
+//{
+//    //    py::print(data_dict);
+//    //    RPY_CHECK(data_dict.contains("label"));
+//    //    RPY_CHECK(data_dict.contains("data"));
+//    //    auto label = data_dict["label"].cast<string>();
+//    //
+//    //    if (data_dict.contains("type")) {
+//    //        auto to_pass = py::make_tuple(data_dict["type"],
+//    //        data_dict["data"]); handle_labeled_data(schema, std::move(label),
+//    //        std::move(to_pass));
+//    //    } else {
+//    //        auto to_pass =
+//    //        py::reinterpret_borrow<py::object>(data_dict["data"]);
+//    //        handle_labeled_data(schema, std::move(label), std::move(to_pass));
+//    //    }
+//    for (auto&& [label, value] : data_dict) {
+//        auto true_label = label.cast<string>();
+//        handle_labeled_data(
+//                schema, std::move(true_label),
+//                py::reinterpret_borrow<py::object>(value)
+//        );
+//    }
+//}
+//
+//void handle_timestamp_pair(StreamSchema* schema, py::object data)
+//{
+//    if (py::isinstance<py::dict>(data)) {
+//        auto data_dict = py::reinterpret_borrow<py::dict>(data);
+//        handle_data_dict(schema, data_dict);
+//    } else if (py::isinstance<py::tuple>(data)) {
+//        auto data_tuple = py::reinterpret_borrow<py::tuple>(data);
+//        handle_data_tuple(schema, data_tuple);
+//    } else if (py::isinstance<py::sequence>(data)) {
+//        auto data_seq = py::reinterpret_borrow<py::sequence>(data);
+//
+//        for (auto&& it_data : data_seq) {
+//            auto inner = py::reinterpret_borrow<py::object>(it_data);
+//            handle_timestamp_pair(schema, std::move(inner));
+//        }
+//    } else {
+//        throw py::value_error("expected dict, tuple, or other sequence");
+//    }
+//}
+//
+//inline void handle_dict_stream(StreamSchema* schema, const py::dict& data)
+//{
+//    for (auto&& [timestamp, tick_value] : data) {
+//        handle_timestamp_pair(
+//                schema, py::reinterpret_borrow<py::object>(tick_value)
+//        );
+//    }
+//}
+//
+//inline void
+//handle_tuple_sequence(StreamSchema* schema, const py::sequence& data)
+//{
+//    for (auto&& it_value : data) {
+//        RPY_CHECK(py::isinstance<py::sequence>(it_value));
+//        auto inner = py::reinterpret_borrow<py::sequence>(it_value);
+//        auto len = py::len(inner);
+//
+//        RPY_CHECK(len > 1);
+//        if (len == 2) {
+//            handle_timestamp_pair(schema, inner[1]);
+//        } else if (len <= 4) {
+//            auto right = inner[py::slice(1, {}, {})];
+//            handle_timestamp_pair(schema, right);
+//        } else {
+//            throw py::value_error("expected tuple with no more than 4 elements"
+//            );
+//        }
+//    }
+//}
 
 }// namespace
 
 void python::parse_into_schema(
         std::shared_ptr<streams::StreamSchema> schema, const py::object& data
 )
 {
```

### Comparing `roughpy-0.0.3/roughpy/src/args/parse_schema.h` & `roughpy-0.0.4/roughpy/src/args/parse_schema.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/dlpack.h` & `roughpy-0.0.4/roughpy/src/dlpack.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/dlpack_LICENSE` & `roughpy-0.0.4/roughpy/src/dlpack_LICENSE`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/intervals/date_time_interval.cpp` & `roughpy-0.0.4/roughpy/src/intervals/date_time_interval.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/intervals/date_time_interval.h` & `roughpy-0.0.4/roughpy/src/intervals/date_time_interval.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/intervals/dyadic.cpp` & `roughpy-0.0.4/roughpy/src/intervals/dyadic.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/intervals/dyadic.h` & `roughpy-0.0.4/roughpy/src/intervals/dyadic.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/intervals/dyadic_interval.cpp` & `roughpy-0.0.4/roughpy/src/intervals/dyadic_interval.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/intervals/dyadic_interval.h` & `roughpy-0.0.4/roughpy/src/intervals/dyadic_interval.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/intervals/interval.cpp` & `roughpy-0.0.4/roughpy/src/intervals/interval.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/intervals/interval.h` & `roughpy-0.0.4/roughpy/src/intervals/interval.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/intervals/intervals.cpp` & `roughpy-0.0.4/roughpy/src/intervals/intervals.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/intervals/intervals.h` & `roughpy-0.0.4/roughpy/src/intervals/intervals.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/intervals/partition.cpp` & `roughpy-0.0.4/roughpy/src/intervals/partition.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/intervals/partition.h` & `roughpy-0.0.4/roughpy/src/intervals/partition.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/intervals/real_interval.cpp` & `roughpy-0.0.4/roughpy/src/intervals/real_interval.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/intervals/real_interval.h` & `roughpy-0.0.4/roughpy/src/intervals/real_interval.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/intervals/segmentation.cpp` & `roughpy-0.0.4/roughpy/src/intervals/segmentation.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/intervals/segmentation.h` & `roughpy-0.0.4/roughpy/src/intervals/segmentation.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/recombine.cpp` & `roughpy-0.0.4/roughpy/src/recombine.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/recombine.h` & `roughpy-0.0.4/roughpy/src/recombine.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/roughpy_module.cpp` & `roughpy-0.0.4/roughpy/src/roughpy_module.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/roughpy_module.h` & `roughpy-0.0.4/roughpy/src/roughpy_module.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/scalars/r_py_polynomial.cpp` & `roughpy-0.0.4/roughpy/src/scalars/r_py_polynomial.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/scalars/r_py_polynomial.h` & `roughpy-0.0.4/roughpy/src/scalars/r_py_polynomial.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/scalars/scalar_type.cpp` & `roughpy-0.0.4/roughpy/src/scalars/scalar_type.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/scalars/scalar_type.h` & `roughpy-0.0.4/roughpy/src/scalars/scalar_type.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/scalars/scalars.cpp` & `roughpy-0.0.4/roughpy/src/scalars/scalars.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,17 @@
 
     py::class_<Scalar> klass(m, "Scalar", SCALAR_DOC);
 
     klass.def("scalar_type", [](const Scalar& self) {
         return scalar_type_to_py_type(self.type());
     });
 
+    RPY_WARNING_PUSH
+    RPY_CLANG_DISABLE_WARNING(-Wself-assign-overloaded)
+
     klass.def(-py::self);
     klass.def(py::self + py::self);
     klass.def(py::self - py::self);
     klass.def(py::self * py::self);
     klass.def(py::self / py::self);
 
     klass.def(py::self += py::self);
@@ -112,14 +115,16 @@
     });
     klass.def("__repr__", [](const Scalar& self) {
         std::stringstream ss;
         ss << "Scalar(type=" << self.type()->info().name << ", value approx "
            << self.to_scalar_t() << ")";
         return ss.str();
     });
+
+    RPY_WARNING_POP
 }
 
 /*
  * Everything that follows is for the implementation of py_to_buffer,
  * which is our primary way of constructing RoughPy objects from python
  * objects.
  */
@@ -218,28 +223,35 @@
     // This function throws if no matching dtype is found
     const auto* tensor_stype
             = dlpack_dtype_to_scalar_type(dltensor.dtype, dltensor.device);
     if (options.type == nullptr) {
         options.type = tensor_stype;
         buffer = scalars::KeyScalarArray(options.type);
     }
+    RPY_DBG_ASSERT(options.type != nullptr);
 
     if (data == nullptr) {
         // The array is empty, empty result.
         return true;
     }
 
     RPY_CHECK(shape != nullptr);
     options.shape.assign(shape, shape + ndim);
 
     idimn_t size = 1;
     for (auto i = 0; i < ndim; ++i) { size *= static_cast<idimn_t>(shape[i]); }
 
     if (strides == nullptr) {
-        buffer = scalars::ScalarArray({options.type, data}, size);
+        if (options.type == tensor_stype) {
+            buffer = scalars::ScalarArray({options.type, data}, size);
+        } else {
+            buffer.allocate_scalars(size);
+            options.type->convert_copy(buffer,
+                                       {tensor_stype, data}, size);
+        }
     } else {
         buffer.allocate_scalars(size);
         scalars::ScalarPointer p(tensor_stype, data);
         dl_copy_strided(
                 ndim, shape, strides, p, buffer + static_cast<dimn_t>(0)
         );
     }
@@ -263,19 +275,16 @@
     UnSet,
     Scalars,
     KeyValuePairs
 };
 
 static inline bool is_scalar(py::handle arg)
 {
-    return (
-        py::isinstance<py::int_>(arg)
-        || py::isinstance<py::float_>(arg)
-        || RPyPolynomial_Check(arg.ptr())
-    );
+    return (py::isinstance<py::int_>(arg) || py::isinstance<py::float_>(arg)
+            || RPyPolynomial_Check(arg.ptr()));
 }
 
 static inline bool
 is_key(py::handle arg, python::AlternativeKeyType* alternative)
 {
     if (alternative != nullptr) {
         return py::isinstance<py::int_>(arg)
```

### Comparing `roughpy-0.0.3/roughpy/src/scalars/scalars.h` & `roughpy-0.0.4/roughpy/src/scalars/scalars.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/BaseStream.cpp` & `roughpy-0.0.4/roughpy/src/streams/BaseStream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/BaseStream.h` & `roughpy-0.0.4/roughpy/src/streams/BaseStream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/brownian_stream.cpp` & `roughpy-0.0.4/roughpy/src/streams/brownian_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/brownian_stream.h` & `roughpy-0.0.4/roughpy/src/streams/brownian_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/externally_sourced_stream.cpp` & `roughpy-0.0.4/roughpy/src/streams/externally_sourced_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/function_stream.cpp` & `roughpy-0.0.4/roughpy/src/streams/function_stream.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -89,17 +89,23 @@
         pmd.ctx = algebra::get_context(
                 pmd.width, pmd.depth, pmd.scalar_type, {}
         );
     }
 
     // TODO: Fix this up properly.
 
+    intervals::RealInterval effective_support =
+            intervals::RealInterval::unbounded();
+    if (pmd.support) {
+        effective_support = *pmd.support;
+    }
+
     streams::StreamMetadata md{
             pmd.width,
-            pmd.support ? *pmd.support : intervals::RealInterval(0, 1),
+            effective_support,
             pmd.ctx,
             pmd.scalar_type,
             pmd.vector_type ? *pmd.vector_type : algebra::VectorType::Dense,
             pmd.resolution};
 
     PyObject* stream = python::RPyStream_FromStream(
             streams::Stream(python::FunctionStream(
```

### Comparing `roughpy-0.0.3/roughpy/src/streams/function_stream.h` & `roughpy-0.0.4/roughpy/src/streams/function_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/lie_increment_stream.cpp` & `roughpy-0.0.4/roughpy/src/streams/lie_increment_stream.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -118,14 +118,17 @@
             throw py::value_error(
                     "either ctx or both width and depth must be specified"
             );
         }
         md.ctx = algebra::get_context(md.width, md.depth, md.scalar_type);
     }
 
+    auto effective_support
+            = intervals::RealInterval::right_unbounded(0.0, md.interval_type);
+
     if (kwargs.contains("indices")) {
         auto indices_arg = kwargs["indices"];
 
         if (py::isinstance<py::buffer>(indices_arg)) {
             auto info
                     = py::reinterpret_borrow<py::buffer>(indices_arg).request();
             buffer_to_indices(indices, info);
@@ -141,14 +144,24 @@
             for (idimn_t i = 0; i < num_increments; ++i) {
                 indices.push_back(static_cast<param_t>(
                         buffer[i * increment_size + icol].to_scalar_t()
                 ));
             }
         } else if (py::isinstance<py::sequence>(indices_arg)) {
             indices = indices_arg.cast<std::vector<param_t>>();
+        } else {
+            throw py::type_error("unexpected type provided to 'indices' "
+                                 "argument");
+        }
+
+        if (!indices.empty()) {
+            auto minmax = std::minmax_element(indices.begin(), indices.end());
+            effective_support = intervals::RealInterval(
+                    *minmax.first, *minmax.second + 1.0, md.interval_type
+            );
         }
     }
 
     if (indices.empty()) {
         indices.reserve(num_increments);
         for (idimn_t i = 0; i < num_increments; ++i) {
             indices.emplace_back(i);
@@ -156,29 +169,28 @@
     } else if (static_cast<idimn_t>(indices.size()) != num_increments) {
         throw py::value_error("mismatch between number of rows in data and "
                               "number of indices");
     }
 
     auto result = streams::Stream(streams::LieIncrementStream(
             std::move(buffer).copy_or_move(), indices,
-            {md.width, md.support ? *md.support : intervals::RealInterval(0, 1),
-             md.ctx, md.scalar_type,
+            {md.width, effective_support, md.ctx, md.scalar_type,
              md.vector_type ? *md.vector_type : algebra::VectorType::Dense,
              md.resolution}
     ));
+    if (md.support) { result.restrict_to(*md.support); }
 
     if (options.cleanup) { options.cleanup(); }
 
     return py::reinterpret_steal<py::object>(
             python::RPyStream_FromStream(std::move(result))
     );
 }
 
-RPY_UNUSED
-static streams::Stream
+RPY_UNUSED static streams::Stream
 lie_increment_path_from_values(const py::object& data, const py::kwargs& kwargs)
 {
     throw std::runtime_error("Not implemented");
 }
 
 void python::init_lie_increment_stream(py::module_& m)
 {
```

### Comparing `roughpy-0.0.3/roughpy/src/streams/lie_increment_stream.h` & `roughpy-0.0.4/roughpy/src/streams/lie_increment_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/piecewise_abelian_stream.cpp` & `roughpy-0.0.4/roughpy/src/streams/piecewise_abelian_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/piecewise_abelian_stream.h` & `roughpy-0.0.4/roughpy/src/streams/piecewise_abelian_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/py_schema_context.cpp` & `roughpy-0.0.4/roughpy/src/streams/py_schema_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/py_schema_context.h` & `roughpy-0.0.4/roughpy/src/streams/py_schema_context.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/r_py_tick_construction_helper.cpp` & `roughpy-0.0.4/roughpy/src/streams/r_py_tick_construction_helper.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/r_py_tick_construction_helper.h` & `roughpy-0.0.4/roughpy/src/streams/r_py_tick_construction_helper.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/schema.cpp` & `roughpy-0.0.4/roughpy/src/streams/schema.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/schema.h` & `roughpy-0.0.4/roughpy/src/streams/schema.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/stream.cpp` & `roughpy-0.0.4/roughpy/src/streams/stream.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -478,23 +478,48 @@
                 stream.simplify(partition, resolution, *ctx)
         );
     }
 
     return python::RPyStream_FromStream(stream.simplify(partition, resolution));
 }
 
+static const char RESTRICT_DOC[] = R"rpydoc(Create a new stream with the same
+ data but restricted to a given interval.)rpydoc";
+static PyObject* restrict(PyObject* self, PyObject* args, PyObject* kwargs)
+{
+    static const char* kwords[] = {"interval", nullptr};
+
+    PyObject* py_interval;
+
+    if (PyArg_ParseTupleAndKeywords(
+                args, kwargs, "O", const_cast<char**>(kwords), &py_interval
+        )
+        == 0) {
+        return nullptr;
+    }
+
+    intervals::RealInterval ivl(py::cast<const intervals::Interval&>(py_interval
+    ));
+
+    const auto& stream = reinterpret_cast<python::RPyStream*>(self)->m_data;
+
+    return python::RPyStream_FromStream(stream.restrict(ivl));
+}
+
 static PyMethodDef RPyStream_members[] = {
         {           "signature",       (PyCFunction) &signature,METH_VARARGS | METH_KEYWORDS,
          SIGNATURE_DOC                                                                                            },
         {       "log_signature",   (PyCFunction) &log_signature,
          METH_VARARGS | METH_KEYWORDS,    LOGSIGNATURE_DOC                                                        },
         {"signature_derivative",       (PyCFunction) &sig_deriv,
          METH_VARARGS | METH_KEYWORDS,       SIG_DERIV_DOC                                                        },
         {            "simplify", (PyCFunction) &simplify_stream,
          METH_VARARGS | METH_KEYWORDS, SIMPLIFY_STREAM_DOC                                                        },
+        {            "restrict",        (PyCFunction)& restrict, METH_VARARGS | METH_KEYWORDS,
+         RESTRICT_DOC                                                                                             },
         {               nullptr,                        nullptr,                            0,             nullptr}
 };
 
 static PyObject* width_getter(PyObject* self)
 {
     return PyLong_FromUnsignedLong(
             reinterpret_cast<python::RPyStream*>(self)->m_data.metadata().width
@@ -517,17 +542,16 @@
                     ->m_data.metadata()
                     .default_context
     );
 }
 
 static PyObject* support_getter(PyObject* self)
 {
-    return py::cast(reinterpret_cast<python::RPyStream*>(self)
-                            ->m_data.metadata()
-                            .effective_support)
+    return py::cast(reinterpret_cast<python::RPyStream*>(self)->m_data.support()
+    )
             .release()
             .ptr();
 }
 
 static PyGetSetDef RPyStream_getset[] = {
         {  "width",   (getter) width_getter, nullptr, nullptr, nullptr},
         {  "dtype",   (getter) ctype_getter, nullptr, nullptr, nullptr},
@@ -543,18 +567,19 @@
        << reinterpret_cast<python::RPyStream*>(self)->m_data.metadata().width
        << ')';
     return PyUnicode_FromString(ss.str().c_str());
 }
 static PyObject* RPyStream_str(PyObject* self) { return RPyStream_repr(self); }
 
 PyTypeObject rpy::python::RPyStream_Type = {
-        PyVarObject_HEAD_INIT(nullptr, 0) "_roughpy.Stream", /* tp_name */
-        sizeof(python::RPyStream),                           /* tp_basicsize */
-        0,                                                   /* tp_itemsize */
-        nullptr,                                             /* tp_dealloc */
+        PyVarObject_HEAD_INIT(nullptr, 0)         //
+        "_roughpy.Stream",                        /* tp_name */
+        sizeof(python::RPyStream),                /* tp_basicsize */
+        0,                                        /* tp_itemsize */
+        nullptr,                                  /* tp_dealloc */
         0,                                        /* tp_vectorcall_offset */
         (getattrfunc) nullptr,                    /* tp_getattr */
         (setattrfunc) nullptr,                    /* tp_setattr */
         nullptr,                                  /* tp_as_async */
         (reprfunc) RPyStream_repr,                /* tp_repr */
         nullptr,                                  /* tp_as_number */
         nullptr,                                  /* tp_as_sequence */
```

### Comparing `roughpy-0.0.3/roughpy/src/streams/stream.h` & `roughpy-0.0.4/roughpy/src/streams/stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/streams.cpp` & `roughpy-0.0.4/roughpy/src/streams/streams.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/streams.h` & `roughpy-0.0.4/roughpy/src/streams/streams.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/tick_stream.cpp` & `roughpy-0.0.4/roughpy/src/streams/tick_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/src/streams/tick_stream.h` & `roughpy-0.0.4/roughpy/src/streams/tick_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/streams/__init__.py` & `roughpy-0.0.4/roughpy/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/roughpy/streams/tick_stream.py` & `roughpy-0.0.4/roughpy/streams/tick_stream.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/CMakeLists.txt` & `roughpy-0.0.4/scalars/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/include/roughpy/scalars/conversion.h` & `roughpy-0.0.4/scalars/include/roughpy/scalars/conversion.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/include/roughpy/scalars/key_scalar_array.h` & `roughpy-0.0.4/scalars/include/roughpy/scalars/key_scalar_array.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/include/roughpy/scalars/owned_scalar_array.h` & `roughpy-0.0.4/scalars/include/roughpy/scalars/owned_scalar_array.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/include/roughpy/scalars/random.h` & `roughpy-0.0.4/scalars/include/roughpy/scalars/random.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/include/roughpy/scalars/scalar.h` & `roughpy-0.0.4/scalars/include/roughpy/scalars/scalar.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/include/roughpy/scalars/scalar_array.h` & `roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_array.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/include/roughpy/scalars/scalar_blas.h` & `roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_blas.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/include/roughpy/scalars/scalar_interface.h` & `roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_interface.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/include/roughpy/scalars/scalar_matrix.h` & `roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_matrix.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/include/roughpy/scalars/scalar_pointer.h` & `roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_pointer.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/include/roughpy/scalars/scalar_stream.h` & `roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/include/roughpy/scalars/scalar_traits.h` & `roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_traits.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/include/roughpy/scalars/scalar_type.h` & `roughpy-0.0.4/scalars/include/roughpy/scalars/scalar_type.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/include/roughpy/scalars/scalars_fwd.h` & `roughpy-0.0.4/scalars/include/roughpy/scalars/scalars_fwd.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/include/roughpy/scalars.h` & `roughpy-0.0.4/scalars/include/roughpy/scalars.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/scalar_blas_defs.h.in` & `roughpy-0.0.4/scalars/scalar_blas_defs.h.in`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/RationalType.cpp` & `roughpy-0.0.4/scalars/src/RationalType.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/RationalType.h` & `roughpy-0.0.4/scalars/src/RationalType.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/ScalarTests.h` & `roughpy-0.0.4/scalars/src/ScalarTests.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/b_float_16_type.h` & `roughpy-0.0.4/scalars/src/b_float_16_type.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/bfloat16_random_generator.cpp` & `roughpy-0.0.4/scalars/src/bfloat16_random_generator.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/bfloat16_random_generator.h` & `roughpy-0.0.4/scalars/src/bfloat16_random_generator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/double_type.cpp` & `roughpy-0.0.4/scalars/src/double_type.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/double_type.h` & `roughpy-0.0.4/scalars/src/double_type.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/float_blas.cpp` & `roughpy-0.0.4/scalars/src/float_blas.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/float_blas.h` & `roughpy-0.0.4/scalars/src/float_blas.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/float_type.cpp` & `roughpy-0.0.4/scalars/src/float_type.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/float_type.h` & `roughpy-0.0.4/scalars/src/float_type.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/half_random_generator.cpp` & `roughpy-0.0.4/scalars/src/half_random_generator.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/half_random_generator.h` & `roughpy-0.0.4/scalars/src/half_random_generator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/half_type.cpp` & `roughpy-0.0.4/scalars/src/half_type.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/half_type.h` & `roughpy-0.0.4/scalars/src/half_type.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/key_scalar_array.cpp` & `roughpy-0.0.4/scalars/src/key_scalar_array.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/owned_scalar_array.cpp` & `roughpy-0.0.4/scalars/src/owned_scalar_array.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/rational_poly_scalar_type.cpp` & `roughpy-0.0.4/scalars/src/rational_poly_scalar_type.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/rational_poly_scalar_type.h` & `roughpy-0.0.4/scalars/src/rational_poly_scalar_type.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/scalar.cpp` & `roughpy-0.0.4/scalars/src/scalar.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/scalar_array.cpp` & `roughpy-0.0.4/scalars/src/scalar_array.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/scalar_blas.cpp` & `roughpy-0.0.4/scalars/src/scalar_blas.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/scalar_blas_impl.h` & `roughpy-0.0.4/scalars/src/scalar_blas_impl.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/scalar_interface.cpp` & `roughpy-0.0.4/scalars/src/scalar_interface.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/scalar_matrix.cpp` & `roughpy-0.0.4/scalars/src/scalar_matrix.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/scalar_pointer.cpp` & `roughpy-0.0.4/scalars/src/scalar_pointer.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/scalar_stream.cpp` & `roughpy-0.0.4/scalars/src/scalar_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/scalar_type.cpp` & `roughpy-0.0.4/scalars/src/scalar_type.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/standard_random_generator.cpp` & `roughpy-0.0.4/scalars/src/standard_random_generator.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/standard_random_generator.h` & `roughpy-0.0.4/scalars/src/standard_random_generator.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/standard_scalar_type.h` & `roughpy-0.0.4/scalars/src/standard_scalar_type.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/test_float_blas.cpp` & `roughpy-0.0.4/scalars/src/test_float_blas.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/test_key_scalar_array.cpp` & `roughpy-0.0.4/scalars/src/test_key_scalar_array.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/test_pcg_standard_random.cpp` & `roughpy-0.0.4/scalars/src/test_pcg_standard_random.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/test_scalar.cpp` & `roughpy-0.0.4/scalars/src/test_scalar.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/test_scalar_array.cpp` & `roughpy-0.0.4/scalars/src/test_scalar_array.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/test_scalar_matrix.cpp` & `roughpy-0.0.4/scalars/src/test_scalar_matrix.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/scalars/src/test_scalar_type.cpp` & `roughpy-0.0.4/scalars/src/test_scalar_type.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/setup.py` & `roughpy-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/CMakeLists.txt` & `roughpy-0.0.4/streams/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/include/roughpy/streams/brownian_stream.h` & `roughpy-0.0.4/streams/include/roughpy/streams/brownian_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/include/roughpy/streams/channels.h` & `roughpy-0.0.4/streams/include/roughpy/streams/channels.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/include/roughpy/streams/dyadic_caching_layer.h` & `roughpy-0.0.4/streams/include/roughpy/streams/dyadic_caching_layer.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/include/roughpy/streams/dynamically_constructed_stream.h` & `roughpy-0.0.4/streams/include/roughpy/streams/dynamically_constructed_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/include/roughpy/streams/external_data_stream.h` & `roughpy-0.0.4/streams/include/roughpy/streams/external_data_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/include/roughpy/streams/lie_increment_stream.h` & `roughpy-0.0.4/streams/include/roughpy/streams/lie_increment_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/include/roughpy/streams/piecewise_abelian_stream.h` & `roughpy-0.0.4/streams/include/roughpy/streams/piecewise_abelian_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/include/roughpy/streams/schema.h` & `roughpy-0.0.4/streams/include/roughpy/streams/schema.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/include/roughpy/streams/schema_context.h` & `roughpy-0.0.4/streams/include/roughpy/streams/schema_context.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/include/roughpy/streams/stream.h` & `roughpy-0.0.4/streams/include/roughpy/streams/stream.h`

 * *Files 15% similar despite different names*

```diff
@@ -27,126 +27,150 @@
 // POSSIBILITY OF SUCH DAMAGE.
 
 #ifndef ROUGHPY_STREAMS_STREAM_H_
 #define ROUGHPY_STREAMS_STREAM_H_
 
 #include "stream_base.h"
 
-#include <roughpy/platform/serialization.h>
 #include <roughpy/intervals/interval.h>
 #include <roughpy/intervals/partition.h>
+#include <roughpy/platform/serialization.h>
 
 #include <memory>
 
 namespace rpy {
 namespace streams {
 
 class RPY_EXPORT Stream
 {
-    std::unique_ptr<const StreamInterface> p_impl;
-
 public:
     using FreeTensor = algebra::FreeTensor;
     using Lie = algebra::Lie;
     using Context = algebra::Context;
     using Interval = intervals::Interval;
     using RealInterval = intervals::RealInterval;
 
     using perturbation_t = std::pair<RealInterval, Lie>;
     using perturbation_list_t = std::vector<perturbation_t>;
 
+private:
+    std::shared_ptr<const StreamInterface> p_impl;
+    RealInterval m_support;
+
+    RPY_NO_DISCARD FreeTensor unit_tensor(const Context& ctx) const
+    {
+        auto result = ctx.zero_free_tensor(metadata().cached_vector_type);
+        result[0] = scalars::Scalar(1);
+        return result;
+    }
+
+    RPY_NO_DISCARD Lie zero_lie(const Context& ctx) const
+    {
+        return ctx.zero_lie(metadata().cached_vector_type);
+    }
+
+    RPY_NO_DISCARD bool check_support_and_trim(RealInterval& domain
+    ) const noexcept;
+
+    Stream(const std::shared_ptr<const StreamInterface>& impl,
+           RealInterval support)
+        : p_impl(impl), m_support(support)
+    {}
+
+public:
     template <typename Impl>
     explicit Stream(Impl&& impl);
 
-    RPY_NO_DISCARD
-    const StreamMetadata& metadata() const;
+    void restrict_to(const Interval& interval);
+
+    Stream restrict(const Interval& interval) const;
+
+    RPY_NO_DISCARD const RealInterval& support() const noexcept
+    {
+        return m_support;
+    }
 
-    RPY_NO_DISCARD
-    const Context& get_default_context() const;
+    RPY_NO_DISCARD const StreamMetadata& metadata() const;
 
-    RPY_NO_DISCARD
-    const StreamSchema& schema() const;
+    RPY_NO_DISCARD const Context& get_default_context() const;
 
-    RPY_NO_DISCARD
-    Lie log_signature() const;
-    RPY_NO_DISCARD
-    Lie log_signature(const Context& ctx) const;
-    RPY_NO_DISCARD
-    Lie log_signature(resolution_t resolution);
-    RPY_NO_DISCARD
-    Lie log_signature(resolution_t resolution, const Context& ctx) const;
-    RPY_NO_DISCARD
-    Lie log_signature(const Interval& interval) const;
-    RPY_NO_DISCARD
-    Lie log_signature(const Interval& interval, resolution_t resolution) const;
-    RPY_NO_DISCARD
-    Lie log_signature(const Interval& interval, resolution_t resolution,
-                      const Context& ctx) const;
-
-    RPY_NO_DISCARD
-    FreeTensor signature() const;
-    RPY_NO_DISCARD
-    FreeTensor signature(const Context& ctx) const;
-    RPY_NO_DISCARD
-    FreeTensor signature(resolution_t resolution);
-    RPY_NO_DISCARD
-    FreeTensor signature(resolution_t resolution, const Context& ctx) const;
-    RPY_NO_DISCARD
-    FreeTensor signature(const Interval& interval) const;
-    RPY_NO_DISCARD
-    FreeTensor signature(const Interval& interval,
-                         resolution_t resolution) const;
-    RPY_NO_DISCARD
-    FreeTensor signature(const Interval& interval, resolution_t resolution,
-                         const Context& ctx) const;
-
-    RPY_NO_DISCARD
-    FreeTensor signature_derivative(const Interval& domain,
-                                    const Lie& perturbation) const;
-    RPY_NO_DISCARD
-    FreeTensor signature_derivative(const Interval& domain,
-                                    const Lie& perturbation,
-                                    const Context& ctx) const;
-    RPY_NO_DISCARD
-    FreeTensor signature_derivative(const Interval& domain,
-                                    const Lie& perturbation,
-                                    resolution_t resolution) const;
-    RPY_NO_DISCARD
-    FreeTensor signature_derivative(const Interval& domain,
-                                    const Lie& perturbation,
-                                    resolution_t resolution,
-                                    const Context& ctx) const;
-    RPY_NO_DISCARD
-    FreeTensor signature_derivative(const perturbation_list_t& perturbations,
-                                    resolution_t resolution) const;
-    RPY_NO_DISCARD
-    FreeTensor signature_derivative(const perturbation_list_t& perturbations,
-                                    resolution_t resolution,
-                                    const Context& ctx) const;
+    RPY_NO_DISCARD const StreamSchema& schema() const;
 
-    Stream simplify(const intervals::Partition& partition,
-                    resolution_t resolution) const
+    RPY_NO_DISCARD Lie log_signature() const;
+    RPY_NO_DISCARD Lie log_signature(const Context& ctx) const;
+    RPY_NO_DISCARD Lie log_signature(resolution_t resolution);
+    RPY_NO_DISCARD Lie
+    log_signature(resolution_t resolution, const Context& ctx) const;
+    RPY_NO_DISCARD Lie log_signature(const Interval& interval) const;
+    RPY_NO_DISCARD Lie
+    log_signature(const Interval& interval, resolution_t resolution) const;
+    RPY_NO_DISCARD Lie log_signature(
+            const Interval& interval, resolution_t resolution,
+            const Context& ctx
+    ) const;
+
+    RPY_NO_DISCARD FreeTensor signature() const;
+    RPY_NO_DISCARD FreeTensor signature(const Context& ctx) const;
+    RPY_NO_DISCARD FreeTensor signature(resolution_t resolution);
+    RPY_NO_DISCARD FreeTensor
+    signature(resolution_t resolution, const Context& ctx) const;
+    RPY_NO_DISCARD FreeTensor signature(const Interval& interval) const;
+    RPY_NO_DISCARD FreeTensor
+    signature(const Interval& interval, resolution_t resolution) const;
+    RPY_NO_DISCARD FreeTensor signature(
+            const Interval& interval, resolution_t resolution,
+            const Context& ctx
+    ) const;
+
+    RPY_NO_DISCARD FreeTensor
+    signature_derivative(const Interval& domain, const Lie& perturbation) const;
+    RPY_NO_DISCARD FreeTensor signature_derivative(
+            const Interval& domain, const Lie& perturbation, const Context& ctx
+    ) const;
+    RPY_NO_DISCARD FreeTensor signature_derivative(
+            const Interval& domain, const Lie& perturbation,
+            resolution_t resolution
+    ) const;
+    RPY_NO_DISCARD FreeTensor signature_derivative(
+            const Interval& domain, const Lie& perturbation,
+            resolution_t resolution, const Context& ctx
+    ) const;
+    RPY_NO_DISCARD FreeTensor signature_derivative(
+            const perturbation_list_t& perturbations, resolution_t resolution
+    ) const;
+    RPY_NO_DISCARD FreeTensor signature_derivative(
+            const perturbation_list_t& perturbations, resolution_t resolution,
+            const Context& ctx
+    ) const;
+
+    Stream simplify(
+            const intervals::Partition& partition, resolution_t resolution
+    ) const
     {
         const auto& md = metadata();
         return simplify(partition, resolution, *md.default_context);
     }
 
-    Stream simplify(const intervals::Partition& partition,
-                    resolution_t resolution, const Context& ctx) const;
+    Stream simplify(
+            const intervals::Partition& partition, resolution_t resolution,
+            const Context& ctx
+    ) const;
 
     RPY_SERIAL_SERIALIZE_FN();
 };
 
 template <typename Impl>
 Stream::Stream(Impl&& impl)
-    : p_impl(new remove_cv_t<Impl>(std::forward<Impl>(impl)))
+    : p_impl(new remove_cv_t<Impl>(std::forward<Impl>(impl))),
+      m_support(p_impl->metadata().effective_support)
 {}
 
 RPY_SERIAL_SERIALIZE_FN_IMPL(Stream)
 {
     RPY_SERIAL_SERIALIZE_NVP("impl", p_impl);
+    RPY_SERIAL_SERIALIZE_NVP("support", m_support);
 }
 
 }// namespace streams
 }// namespace rpy
 
 #endif// ROUGHPY_STREAMS_STREAM_H_
```

### Comparing `roughpy-0.0.3/streams/include/roughpy/streams/stream_base.h` & `roughpy-0.0.4/streams/include/roughpy/streams/stream_base.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/include/roughpy/streams/stream_construction_helper.h` & `roughpy-0.0.4/streams/include/roughpy/streams/stream_construction_helper.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/include/roughpy/streams/tick_stream.h` & `roughpy-0.0.4/streams/include/roughpy/streams/tick_stream.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/src/brownian_stream.cpp` & `roughpy-0.0.4/streams/src/brownian_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/src/channels.cpp` & `roughpy-0.0.4/streams/src/channels.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/src/dyadic_caching_layer.cpp` & `roughpy-0.0.4/streams/src/dyadic_caching_layer.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/src/dynamically_constructed_stream.cpp` & `roughpy-0.0.4/streams/src/dynamically_constructed_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/src/external_data_sources/csv_data_source.cpp` & `roughpy-0.0.4/streams/src/external_data_sources/csv_data_source.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/src/external_data_sources/csv_data_source.h` & `roughpy-0.0.4/streams/src/external_data_sources/csv_data_source.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/src/external_data_sources/sound_file_data_source.cpp` & `roughpy-0.0.4/streams/src/external_data_sources/sound_file_data_source.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/src/external_data_sources/sound_file_data_source.h` & `roughpy-0.0.4/streams/src/external_data_sources/sound_file_data_source.h`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/src/external_data_stream.cpp` & `roughpy-0.0.4/streams/src/external_data_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/src/lie_increment_stream.cpp` & `roughpy-0.0.4/streams/src/lie_increment_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/src/piecewise_abelian_stream.cpp` & `roughpy-0.0.4/streams/src/piecewise_abelian_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/src/schema.cpp` & `roughpy-0.0.4/streams/src/schema.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/src/schema_context.cpp` & `roughpy-0.0.4/streams/src/schema_context.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/src/stream.cpp` & `roughpy-0.0.4/streams/src/stream.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,48 @@
 
 #include <roughpy/intervals/partition.h>
 #include <roughpy/streams/piecewise_abelian_stream.h>
 
 using namespace rpy;
 using namespace streams;
 
+bool Stream::check_support_and_trim(Stream::RealInterval& domain) const noexcept
+{
+    if (domain.sup() < m_support.inf() || domain.inf() > m_support.sup()) {
+        // The intervals don't intersect, return false
+        return false;
+    }
+
+    // Intervals do intersect, trim domain so it is a subset of m_support
+    domain = RealInterval(
+            std::max(domain.inf(), m_support.inf()),
+            std::min(domain.sup(), m_support.sup()), domain.type()
+    );
+
+    return true;
+}
+
+void Stream::restrict_to(const Stream::Interval& interval) {
+    if (p_impl) {
+        m_support = p_impl->schema().adjust_interval(interval);
+    } else {
+        m_support = RealInterval(interval);
+    }
+}
+
+Stream Stream::restrict(const Stream::Interval& interval) const
+{
+    RealInterval support(interval);
+    if (p_impl) {
+        support = p_impl->schema().adjust_interval(interval);
+    }
+
+    return { p_impl, support };
+}
+
 const algebra::Context& rpy::streams::Stream::get_default_context() const
 {
     RPY_CHECK(p_impl);
     return *p_impl->metadata().default_context;
 }
 const rpy::streams::StreamMetadata& rpy::streams::Stream::metadata() const
 {
@@ -52,94 +86,93 @@
 }
 
 rpy::streams::Stream::Lie rpy::streams::Stream::log_signature() const
 {
     const auto& md = metadata();
 
     return p_impl->log_signature(
-            md.effective_support, md.default_resolution, *md.default_context
+            m_support, md.default_resolution, *md.default_context
     );
 }
 rpy::streams::Stream::Lie
 rpy::streams::Stream::log_signature(const rpy::streams::Stream::Context& ctx
 ) const
 {
     const auto& md = metadata();
-    return p_impl->log_signature(
-            md.effective_support, md.default_resolution, ctx
-    );
+    return p_impl->log_signature(m_support, md.default_resolution, ctx);
 }
 rpy::streams::Stream::Lie
 rpy::streams::Stream::log_signature(rpy::resolution_t resolution)
 {
     const auto& md = metadata();
-    return p_impl->log_signature(
-            md.effective_support, resolution, *md.default_context
-    );
+    return p_impl->log_signature(m_support, resolution, *md.default_context);
 }
 rpy::streams::Stream::Lie rpy::streams::Stream::log_signature(
         rpy::resolution_t resolution, const rpy::streams::Stream::Context& ctx
 ) const
 {
     const auto& md = metadata();
-    return p_impl->log_signature(md.effective_support, resolution, ctx);
+    return p_impl->log_signature(m_support, resolution, ctx);
 }
 rpy::streams::Stream::Lie rpy::streams::Stream::log_signature(
         const rpy::streams::Stream::Interval& interval
 ) const
 {
     const auto& md = metadata();
+
     return log_signature(interval, md.default_resolution, *md.default_context);
 }
 rpy::streams::Stream::Lie rpy::streams::Stream::log_signature(
         const rpy::streams::Stream::Interval& interval,
         rpy::resolution_t resolution
 ) const
 {
     const auto& md = metadata();
+
     return log_signature(interval, resolution, *md.default_context);
 }
 rpy::streams::Stream::Lie rpy::streams::Stream::log_signature(
         const rpy::streams::Stream::Interval& interval,
         rpy::resolution_t resolution, const rpy::streams::Stream::Context& ctx
 ) const
 {
+    const auto& md = metadata();
     const auto& schema = p_impl->schema();
 
-    return p_impl->log_signature(
-            schema.adjust_interval(interval), resolution, ctx
-    );
+    RealInterval query_interval(schema.adjust_interval(interval));
+    if (!check_support_and_trim(query_interval)) {
+        return ctx.zero_lie(md.cached_vector_type);
+    }
+
+    return p_impl->log_signature(query_interval, resolution, ctx);
 }
 rpy::streams::Stream::FreeTensor rpy::streams::Stream::signature() const
 {
     const auto& md = metadata();
     return p_impl->signature(
-            md.effective_support, md.default_resolution, *md.default_context
+            m_support, md.default_resolution, *md.default_context
     );
 }
 rpy::streams::Stream::FreeTensor
 rpy::streams::Stream::signature(const rpy::streams::Stream::Context& ctx) const
 {
     const auto& md = metadata();
-    return p_impl->signature(md.effective_support, md.default_resolution, ctx);
+    return p_impl->signature(m_support, md.default_resolution, ctx);
 }
 rpy::streams::Stream::FreeTensor
 rpy::streams::Stream::signature(rpy::resolution_t resolution)
 {
     const auto& md = metadata();
-    return p_impl->signature(
-            md.effective_support, resolution, *md.default_context
-    );
+    return p_impl->signature(m_support, resolution, *md.default_context);
 }
 rpy::streams::Stream::FreeTensor rpy::streams::Stream::signature(
         rpy::resolution_t resolution, const rpy::streams::Stream::Context& ctx
 ) const
 {
-    const auto& md = metadata();
-    return p_impl->signature(md.effective_support, resolution, ctx);
+    return p_impl->signature(m_support, resolution, ctx);
 }
 rpy::streams::Stream::FreeTensor
 rpy::streams::Stream::signature(const rpy::streams::Stream::Interval& interval
 ) const
 {
     const auto& md = metadata();
     return signature(interval, md.default_resolution, *md.default_context);
@@ -154,15 +187,19 @@
 }
 rpy::streams::Stream::FreeTensor rpy::streams::Stream::signature(
         const rpy::streams::Stream::Interval& interval,
         rpy::resolution_t resolution, const rpy::streams::Stream::Context& ctx
 ) const
 {
     const auto& schema = p_impl->schema();
-    return p_impl->signature(schema.adjust_interval(interval), resolution, ctx);
+
+    RealInterval query_interval(schema.adjust_interval(interval));
+    if (!check_support_and_trim(query_interval)) { return unit_tensor(ctx); }
+
+    return p_impl->signature(query_interval, resolution, ctx);
 }
 rpy::streams::Stream::FreeTensor rpy::streams::Stream::signature_derivative(
         const rpy::streams::Stream::Interval& domain,
         const rpy::streams::Stream::Lie& perturbation
 ) const
 {
     const auto& md = metadata();
```

### Comparing `roughpy-0.0.3/streams/src/stream_base.cpp` & `roughpy-0.0.4/streams/src/stream_base.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/src/stream_construction_helper.cpp` & `roughpy-0.0.4/streams/src/stream_construction_helper.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/src/test_brownian_stream.cpp` & `roughpy-0.0.4/streams/src/test_brownian_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/src/test_lie_increment_stream.cpp` & `roughpy-0.0.4/streams/src/test_lie_increment_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/src/test_schema.cpp` & `roughpy-0.0.4/streams/src/test_schema.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/streams/src/tick_stream.cpp` & `roughpy-0.0.4/streams/src/tick_stream.cpp`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tests/algebra/test_alg_poly_coeffs.py` & `roughpy-0.0.4/tests/algebra/test_alg_poly_coeffs.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tests/algebra/test_algebra_context.py` & `roughpy-0.0.4/tests/algebra/test_algebra_context.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tests/algebra/test_free_tensor.py` & `roughpy-0.0.4/tests/algebra/test_free_tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -422,7 +422,15 @@
 
 def test_coeff_and_vec_type(width, depth, data1, coeff_type, vec_type):
     t = FreeTensor(data1, width=width, depth=depth, dtype=coeff_type,
                    vector_type=vec_type)
 
     assert t.storage_type == vec_type
     assert t.dtype == coeff_type
+
+
+def test_antipode(width, depth, data1, coeff_type, vec_type):
+    t = FreeTensor(data1, width=width, depth=depth, dtype=coeff_type,
+                   vector_type=vec_type)
+
+    result = t.antipode().antipode()
+    assert result == t, f"{result} {t} {result - t}"
```

### Comparing `roughpy-0.0.3/tests/algebra/test_lie.py` & `roughpy-0.0.4/tests/algebra/test_lie.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tests/algebra/test_lie_keys.py` & `roughpy-0.0.4/tests/algebra/test_lie_keys.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tests/algebra/test_tensor_iterator.py` & `roughpy-0.0.4/tests/algebra/test_tensor_iterator.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tests/algebra/test_tensor_keys.py` & `roughpy-0.0.4/tests/algebra/test_tensor_keys.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tests/conftest.py` & `roughpy-0.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tests/intervals/test_intervals.py` & `roughpy-0.0.4/tests/intervals/test_intervals.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tests/scalars/test_monomial.py` & `roughpy-0.0.4/tests/scalars/test_monomial.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tests/streams/audio/test.flac` & `roughpy-0.0.4/tests/streams/audio/test.flac`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tests/streams/audio/test.mp3` & `roughpy-0.0.4/tests/streams/audio/test.mp3`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tests/streams/audio/test.wav` & `roughpy-0.0.4/tests/streams/audio/test.wav`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tests/streams/test_brownian_stream.py` & `roughpy-0.0.4/tests/streams/test_brownian_stream.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tests/streams/test_function_path.py` & `roughpy-0.0.4/tests/streams/test_function_path.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tests/streams/test_lie_increment_path.py` & `roughpy-0.0.4/tests/streams/test_lie_increment_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 #         pytest.skip("empty array not valid data.")
 #     p = path(tick_data_w_indices, include_time=True)
 #
 #     assert p.width == width + 1
 #     assert p.depth == 2
 
 
-@pytest.fixture(params=[2, 5, 10, 25, 100, 1000])
+@pytest.fixture(params=[2, 5, 10, 25, 100])
 def t_values(request):
     return np.arange(0.0, 2.0, 2.0 / request.param) + 2.0 / request.param
 
 
 @pytest.fixture
 def known_path_data(t_values, width):
     t = np.arange(1.0, width + 1) * (2.0 / len(t_values))
```

### Comparing `roughpy-0.0.3/tests/streams/test_piecewise_lie_path.py` & `roughpy-0.0.4/tests/streams/test_piecewise_lie_path.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tests/streams/test_schema.py` & `roughpy-0.0.4/tests/streams/test_schema.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tests/streams/test_sound_path.py` & `roughpy-0.0.4/tests/streams/test_sound_path.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tests/streams/test_tick_stream.py` & `roughpy-0.0.4/tests/streams/test_tick_stream.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tools/ci/before-all-common.sh` & `roughpy-0.0.4/tools/ci/before-all-common.sh`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tools/python-get-binary-obj-path.py` & `roughpy-0.0.4/tools/python-get-binary-obj-path.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/tools/version_from_file.py` & `roughpy-0.0.4/tools/version_from_file.py`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/vcpkg.json` & `roughpy-0.0.4/vcpkg.json`

 * *Files identical despite different names*

### Comparing `roughpy-0.0.3/PKG-INFO` & `roughpy-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roughpy
-Version: 0.0.3
+Version: 0.0.4
 Keywords: data streams rough paths signatures
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: BSD License
@@ -16,35 +16,45 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Description-Content-Type: text/markdown
 
-![RoughPy Logo](https://github.com/datasig-ac-uk/roughpy/tree/mainbranding/logo/logo_square_white.jpg)
+![RoughPy Logo](https://github.com/datasig-ac-uk/roughpy/tree/main/branding/logo/logo_square_white.jpg)
 # RoughPy
 RoughPy is a package for working with streaming data as rough paths, and working with algebraic objects such as free tensors, shuffle tensors, and elements of the free Lie algebra.
 
 This library is currently in an alpha stage, and as such many features are still incomplete or not fully implemented. Please bear this in mind when looking at the source code.
 
 
 ## Installation
-Currently, RoughPy is only available as a source distribution. It should still be installable via pip, provided you have all the dependencies set up.
-Use 
+RoughPy can be installed from PyPI using `pip` on Windows, Linux, and MacOS (Intel based Mac only, sorry not Apple Silicon support yet). Simply run
 ```
-pip install https://github.com/datasig-ac-uk/roughpy
+pip install roughpy
 ```
-The compilation process is quite long - there is a lot to build. For the full release, we will add prebuilt binaries for major platforms.
-The following packages are required to build RoughPy:
- - Boost (at least version 1.81, components system threads filesystem serialization)
- - libsndfile
- - Eigen3
- - (More to be added)
+to get the latest version.
 
-Microsoft vcpkg can be used to install these dependencies - see the vcpkg.json file for the requirements.
+Alternatively, the wheel files can be downloaded from the [Releases](https://github.com/datasig-ac-uk/RoughPy/releases) page.
+
+### Installing from source
+RoughPy can be installed from source, although this is not the recommended way to install.
+The build system requires [vcpkg](https://github.com/Microsoft/vcpkg) in order to obtain the necessary dependencies (except for MKL on x86 platforms, which is installed via pip).
+You will need to make sure that vcpkg is available on your system before attempting to build RoughPy.
+The following commands should be sufficient to set up the environment for building RoughPy:
+```bash
+git clone https://github.com/Microsoft/vcpkg.git tools/vcpkg
+tools/vcpkg/bootstrap-vcpkg.sh
+export CMAKE_TOOLCHAIN_FILE=$(pwd)/tools/vcpkg/scripts/buildsystems/vcpkg.cmake
+```
+With this environment variable set, you should now be able to pip install either using the PyPI source distribution (using the `--no-binary :all:` flag), or directly from GitHub:
+```bash
+pip install https://github.com/datasig-ac-uk/RoughPy.git
+```
+It will take some time to build.
 
 ## Usage
 Following the NumPy (and related) convention, we import RoughPy under the alias `rp` as follows:
 ```python
 import roughpy as rp
 ```
 The main object(s) that you will interact with are `Stream` objects or the family of factory classes such as `LieIncrementStream`. For example, we can create a `LieIncrementStream` using the following commands:
@@ -82,14 +92,25 @@
 ## Contributors
 The full list of contributors is listed in `THANKS` alongside this readme. The people mentioned in this document constitute `The RoughPy Developers`.
 
 ## License
 RoughPy is licensed under a BSD-3-Clause license. This was chosen specifically to match the license of NumPy.
 # Changelog
 
+Version 0.0.4:
+  - Overhauled the RPY_CHECK macro so it now gives much better contextual
+  information.
+  - Readme updated to reflect PyPI installation with wheels.
+  - Antipode is now implemented in libalgebra_lite, and exposed to Python for
+  Free tensors.
+  - Streams now carry a support interval, outside of which the signature will be
+   return trivial.
+  - Build requirements fixed for non x86 platforms.
+  - Expanded coverage of pytype stub file.
+
 Version 0.0.3:
   - Added datetime interval support.
   - Integrated schema reparametrisation into stream signature methods.
   - Fixed bug in names of scalar types, names now display correctly.
   - Fixed bfloat16 given wrong scalar type code.
   - Added half precision float and bfloat16 to py module
   - Added real partition class and Python interface.
```

