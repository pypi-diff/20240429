# Comparing `tmp/triton_xpu-0.0.2-py3-none-any.whl.zip` & `tmp/triton_xpu-0.0.3a1-cp39-cp39-manylinux_2_31_x86_64.manylinux_2_35_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,151 @@
-Zip file size: 1648 bytes, number of entries: 5
--rw-r--r--  2.0 unx      331 b- defN 24-Mar-22 16:39 triton/__init__.py
--rw-r--r--  2.0 unx      704 b- defN 24-Mar-22 16:39 triton_xpu-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-22 16:39 triton_xpu-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Mar-22 16:39 triton_xpu-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      382 b- defN 24-Mar-22 16:39 triton_xpu-0.0.2.dist-info/RECORD
-5 files, 1516 bytes uncompressed, 930 bytes compressed:  38.7%
+Zip file size: 3332314 bytes, number of entries: 149
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton_xpu-0.0.3a1.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton_xpu.libs/
+-rw-r--r--  2.0 unx      219 b- defN 24-Apr-29 17:52 triton_xpu-0.0.3a1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      149 b- defN 24-Apr-29 17:52 triton_xpu-0.0.3a1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx    12800 b- defN 24-Apr-29 17:52 triton_xpu-0.0.3a1.dist-info/RECORD
+-rw-r--r--  2.0 unx     1426 b- defN 24-Apr-29 17:52 triton_xpu-0.0.3a1.dist-info/METADATA
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton/compiler/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton/language/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton/backends/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton/_C/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton/ops/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton/runtime/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton/tools/
+-rw-r--r--  2.0 unx    18449 b- defN 24-Apr-29 17:52 triton/testing.py
+-rw-r--r--  2.0 unx       89 b- defN 24-Apr-29 17:52 triton/errors.py
+-rw-r--r--  2.0 unx     1349 b- defN 24-Apr-29 17:52 triton/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 17:52 triton/compiler/make_launcher.py
+-rw-r--r--  2.0 unx    55248 b- defN 24-Apr-29 17:52 triton/compiler/code_generator.py
+-rw-r--r--  2.0 unx    16434 b- defN 24-Apr-29 17:52 triton/compiler/compiler.py
+-rw-r--r--  2.0 unx     1732 b- defN 24-Apr-29 17:52 triton/compiler/errors.py
+-rw-r--r--  2.0 unx      256 b- defN 24-Apr-29 17:52 triton/compiler/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton/language/extra/
+-rw-r--r--  2.0 unx     6736 b- defN 24-Apr-29 17:52 triton/language/random.py
+-rw-r--r--  2.0 unx    72243 b- defN 24-Apr-29 17:52 triton/language/semantic.py
+-rw-r--r--  2.0 unx    13132 b- defN 24-Apr-29 17:52 triton/language/standard.py
+-rw-r--r--  2.0 unx    88021 b- defN 24-Apr-29 17:52 triton/language/core.py
+-rw-r--r--  2.0 unx     4613 b- defN 24-Apr-29 17:52 triton/language/__init__.py
+-rw-r--r--  2.0 unx     7094 b- defN 24-Apr-29 17:52 triton/language/math.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton/language/extra/intel/
+-rw-r--r--  2.0 unx       41 b- defN 24-Apr-29 17:52 triton/language/extra/__init__.py
+-rw-r--r--  2.0 unx     1674 b- defN 24-Apr-29 17:52 triton/language/extra/intel/utils.py
+-rw-r--r--  2.0 unx    44326 b- defN 24-Apr-29 17:52 triton/language/extra/intel/libdevice.py
+-rw-r--r--  2.0 unx      212 b- defN 24-Apr-29 17:52 triton/language/extra/intel/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton/backends/amd/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton/backends/intel/
+-rw-r--r--  2.0 unx      977 b- defN 24-Apr-29 17:52 triton/backends/driver.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-Apr-29 17:52 triton/backends/compiler.py
+-rw-r--r--  2.0 unx     1600 b- defN 24-Apr-29 17:52 triton/backends/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton/backends/amd/include/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton/backends/amd/lib/
+-rw-r--r--  2.0 unx    15959 b- defN 24-Apr-29 17:52 triton/backends/amd/driver.py
+-rw-r--r--  2.0 unx     9845 b- defN 24-Apr-29 17:52 triton/backends/amd/compiler.py
+-rw-r--r--  2.0 unx     8061 b- defN 24-Apr-29 17:52 triton/backends/amd/driver.c
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton/backends/amd/include/hip/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/
+-rw-r--r--  2.0 unx     6687 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/texture_types.h
+-rw-r--r--  2.0 unx     1307 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/hip_hcc.h
+-rw-r--r--  2.0 unx     1523 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/hip_fp16.h
+-rw-r--r--  2.0 unx     1594 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/hip_complex.h
+-rw-r--r--  2.0 unx     1878 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/hip_cooperative_groups.h
+-rw-r--r--  2.0 unx     1630 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/hip_vector_types.h
+-rw-r--r--  2.0 unx     1438 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/hip_gl_interop.h
+-rw-r--r--  2.0 unx     1815 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/math_functions.h
+-rw-r--r--  2.0 unx     1237 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/hip_texture_types.h
+-rw-r--r--  2.0 unx     8514 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/hip_ext.h
+-rw-r--r--  2.0 unx     1755 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/hip_bfloat16.h
+-rw-r--r--  2.0 unx     3058 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/hip_runtime.h
+-rw-r--r--  2.0 unx     6339 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/hip_deprecated.h
+-rw-r--r--  2.0 unx     1304 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/hip_profile.h
+-rw-r--r--  2.0 unx   373379 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/hip_runtime_api.h
+-rw-r--r--  2.0 unx     1588 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/hip_math_constants.h
+-rw-r--r--  2.0 unx     1959 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/surface_types.h
+-rw-r--r--  2.0 unx    18816 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/driver_types.h
+-rw-r--r--  2.0 unx     1571 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/hip_bf16.h
+-rw-r--r--  2.0 unx     2370 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/library_types.h
+-rw-r--r--  2.0 unx     3450 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/hip_common.h
+-rw-r--r--  2.0 unx     1589 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/device_functions.h
+-rw-r--r--  2.0 unx    14764 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/hiprtc.h
+-rw-r--r--  2.0 unx     1773 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/channel_descriptor.h
+-rw-r--r--  2.0 unx      407 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/hip_version.h
+-rw-r--r--  2.0 unx     3151 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/amd_math_functions.h
+-rw-r--r--  2.0 unx     1252 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/concepts.hpp
+-rw-r--r--  2.0 unx     3652 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/hip_ldg.h
+-rw-r--r--  2.0 unx     1830 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/grid_launch.h
+-rw-r--r--  2.0 unx    30346 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/amd_hip_bf16.h
+-rw-r--r--  2.0 unx     8129 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/functional_grid_launch.hpp
+-rw-r--r--  2.0 unx    57854 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/amd_hip_fp16.h
+-rw-r--r--  2.0 unx     1370 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/amd_hip_common.h
+-rw-r--r--  2.0 unx     3232 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/hsa_helpers.hpp
+-rw-r--r--  2.0 unx    14679 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/amd_hip_complex.h
+-rw-r--r--  2.0 unx    67925 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/macro_based_grid_launch.hpp
+-rw-r--r--  2.0 unx    33980 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/amd_device_functions.h
+-rw-r--r--  2.0 unx     5890 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/amd_hip_math_constants.h
+-rw-r--r--  2.0 unx     9484 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/amd_hip_bfloat16.h
+-rw-r--r--  2.0 unx     7038 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/host_defines.h
+-rw-r--r--  2.0 unx    11062 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/amd_surface_functions.h
+-rw-r--r--  2.0 unx    32159 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/amd_hip_cooperative_groups.h
+-rw-r--r--  2.0 unx     3154 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/program_state.hpp
+-rw-r--r--  2.0 unx     5134 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/hip_fp16_math_fwd.h
+-rw-r--r--  2.0 unx     9986 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/amd_hip_runtime_pt_api.h
+-rw-r--r--  2.0 unx     2715 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/hip_runtime_prof.h
+-rw-r--r--  2.0 unx     3860 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/amd_hip_gl_interop.h
+-rw-r--r--  2.0 unx     7957 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/hip_cooperative_groups_helper.h
+-rw-r--r--  2.0 unx   618543 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/hip_prof_str.h
+-rw-r--r--  2.0 unx     1370 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/grid_launch.hpp
+-rw-r--r--  2.0 unx    50307 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/amd_hip_atomic.h
+-rw-r--r--  2.0 unx     6660 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/hip_fp16_gcc.h
+-rw-r--r--  2.0 unx    18966 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/amd_warp_functions.h
+-rw-r--r--  2.0 unx    55689 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/amd_hip_vector_types.h
+-rw-r--r--  2.0 unx    17787 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/texture_fetch_functions.h
+-rw-r--r--  2.0 unx    17000 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/math_fwd.h
+-rw-r--r--  2.0 unx    10538 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/ockl_image.h
+-rw-r--r--  2.0 unx     5707 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/helpers.hpp
+-rw-r--r--  2.0 unx    11708 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/amd_channel_descriptor.h
+-rw-r--r--  2.0 unx    18447 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/texture_indirect_functions.h
+-rw-r--r--  2.0 unx    14891 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/amd_hip_runtime.h
+-rw-r--r--  2.0 unx     1219 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/grid_launch_GGL.hpp
+-rw-r--r--  2.0 unx    24202 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/amd_hip_unsafe_atomics.h
+-rw-r--r--  2.0 unx     7457 b- defN 24-Apr-29 17:52 triton/backends/amd/include/hip/amd_detail/device_library_decls.h
+-rw-r--r--  2.0 unx  2700232 b- defN 24-Apr-29 17:52 triton/backends/amd/lib/opencl.bc
+-rw-r--r--  2.0 unx    41568 b- defN 24-Apr-29 17:52 triton/backends/amd/lib/cuda2gcn.bc
+-rw-r--r--  2.0 unx   246124 b- defN 24-Apr-29 17:52 triton/backends/amd/lib/ockl.bc
+-rw-r--r--  2.0 unx   205964 b- defN 24-Apr-29 17:52 triton/backends/amd/lib/ocml.bc
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton/backends/intel/bin/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton/backends/intel/lib/
+-rw-r--r--  2.0 unx     2634 b- defN 24-Apr-29 17:52 triton/backends/intel/arch_parser.c
+-rw-r--r--  2.0 unx    15137 b- defN 24-Apr-29 17:52 triton/backends/intel/driver.py
+-rw-r--r--  2.0 unx     9075 b- defN 24-Apr-29 17:52 triton/backends/intel/compiler.py
+-rw-r--r--  2.0 unx    13891 b- defN 24-Apr-29 17:52 triton/backends/intel/driver.c
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 17:52 triton/backends/intel/__init__.py
+-rwxr-xr-x  2.0 unx  5104880 b- defN 24-Apr-29 17:52 triton/backends/intel/bin/spirv-dis
+-rw-r--r--  2.0 unx  1703916 b- defN 24-Apr-29 17:52 triton/backends/intel/lib/libsycl-spir64-unknown-unknown.bc
+-rwxr-xr-x  2.0 unx        0 b- defN 24-Apr-29 17:52 triton/_C/libtriton.so
+-rw-r--r--  2.0 unx     1943 b- defN 24-Apr-29 17:52 triton/_C/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 17:52 triton/ops/blocksparse/
+-rw-r--r--  2.0 unx     9278 b- defN 24-Apr-29 17:52 triton/ops/matmul.py
+-rw-r--r--  2.0 unx     6697 b- defN 24-Apr-29 17:52 triton/ops/matmul_perf_model.py
+-rw-r--r--  2.0 unx     3451 b- defN 24-Apr-29 17:52 triton/ops/cross_entropy.py
+-rw-r--r--  2.0 unx    18201 b- defN 24-Apr-29 17:52 triton/ops/flash_attention.py
+-rw-r--r--  2.0 unx      324 b- defN 24-Apr-29 17:52 triton/ops/__init__.py
+-rw-r--r--  2.0 unx     8243 b- defN 24-Apr-29 17:52 triton/ops/blocksparse/softmax.py
+-rw-r--r--  2.0 unx    15920 b- defN 24-Apr-29 17:52 triton/ops/blocksparse/matmul.py
+-rw-r--r--  2.0 unx      100 b- defN 24-Apr-29 17:52 triton/ops/blocksparse/__init__.py
+-rw-r--r--  2.0 unx     9759 b- defN 24-Apr-29 17:52 triton/runtime/cache.py
+-rw-r--r--  2.0 unx     3292 b- defN 24-Apr-29 17:52 triton/runtime/build.py
+-rw-r--r--  2.0 unx    27693 b- defN 24-Apr-29 17:52 triton/runtime/jit.py
+-rw-r--r--  2.0 unx     1509 b- defN 24-Apr-29 17:52 triton/runtime/driver.py
+-rw-r--r--  2.0 unx    47640 b- defN 24-Apr-29 17:52 triton/runtime/interpreter.py
+-rw-r--r--  2.0 unx      787 b- defN 24-Apr-29 17:52 triton/runtime/errors.py
+-rw-r--r--  2.0 unx    13556 b- defN 24-Apr-29 17:52 triton/runtime/autotuner.py
+-rw-r--r--  2.0 unx      621 b- defN 24-Apr-29 17:52 triton/runtime/__init__.py
+-rw-r--r--  2.0 unx     5080 b- defN 24-Apr-29 17:52 triton/tools/disasm.py
+-rw-r--r--  2.0 unx    13673 b- defN 24-Apr-29 17:52 triton/tools/build_extern.py
+-rw-r--r--  2.0 unx      332 b- defN 24-Apr-29 17:52 triton/tools/compile.h
+-rw-r--r--  2.0 unx     6467 b- defN 24-Apr-29 17:52 triton/tools/compile.py
+-rw-r--r--  2.0 unx    11871 b- defN 24-Apr-29 17:52 triton/tools/link.py
+-rw-r--r--  2.0 unx     2090 b- defN 24-Apr-29 17:52 triton/tools/compile.c
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 17:52 triton/tools/__init__.py
+149 files, 12305434 bytes uncompressed, 3309276 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -1,16 +1,448 @@
+Filename: triton_xpu-0.0.3a1.dist-info/
+Comment: 
+
+Filename: triton/
+Comment: 
+
+Filename: triton_xpu.libs/
+Comment: 
+
+Filename: triton_xpu-0.0.3a1.dist-info/top_level.txt
+Comment: 
+
+Filename: triton_xpu-0.0.3a1.dist-info/WHEEL
+Comment: 
+
+Filename: triton_xpu-0.0.3a1.dist-info/RECORD
+Comment: 
+
+Filename: triton_xpu-0.0.3a1.dist-info/METADATA
+Comment: 
+
+Filename: triton/compiler/
+Comment: 
+
+Filename: triton/language/
+Comment: 
+
+Filename: triton/backends/
+Comment: 
+
+Filename: triton/_C/
+Comment: 
+
+Filename: triton/ops/
+Comment: 
+
+Filename: triton/runtime/
+Comment: 
+
+Filename: triton/tools/
+Comment: 
+
+Filename: triton/testing.py
+Comment: 
+
+Filename: triton/errors.py
+Comment: 
+
 Filename: triton/__init__.py
 Comment: 
 
-Filename: triton_xpu-0.0.2.dist-info/METADATA
+Filename: triton/compiler/make_launcher.py
+Comment: 
+
+Filename: triton/compiler/code_generator.py
+Comment: 
+
+Filename: triton/compiler/compiler.py
+Comment: 
+
+Filename: triton/compiler/errors.py
+Comment: 
+
+Filename: triton/compiler/__init__.py
+Comment: 
+
+Filename: triton/language/extra/
+Comment: 
+
+Filename: triton/language/random.py
+Comment: 
+
+Filename: triton/language/semantic.py
+Comment: 
+
+Filename: triton/language/standard.py
+Comment: 
+
+Filename: triton/language/core.py
+Comment: 
+
+Filename: triton/language/__init__.py
+Comment: 
+
+Filename: triton/language/math.py
+Comment: 
+
+Filename: triton/language/extra/intel/
+Comment: 
+
+Filename: triton/language/extra/__init__.py
+Comment: 
+
+Filename: triton/language/extra/intel/utils.py
+Comment: 
+
+Filename: triton/language/extra/intel/libdevice.py
+Comment: 
+
+Filename: triton/language/extra/intel/__init__.py
+Comment: 
+
+Filename: triton/backends/amd/
+Comment: 
+
+Filename: triton/backends/intel/
+Comment: 
+
+Filename: triton/backends/driver.py
+Comment: 
+
+Filename: triton/backends/compiler.py
+Comment: 
+
+Filename: triton/backends/__init__.py
+Comment: 
+
+Filename: triton/backends/amd/include/
+Comment: 
+
+Filename: triton/backends/amd/lib/
+Comment: 
+
+Filename: triton/backends/amd/driver.py
+Comment: 
+
+Filename: triton/backends/amd/compiler.py
+Comment: 
+
+Filename: triton/backends/amd/driver.c
+Comment: 
+
+Filename: triton/backends/amd/include/hip/
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/
+Comment: 
+
+Filename: triton/backends/amd/include/hip/texture_types.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/hip_hcc.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/hip_fp16.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/hip_complex.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/hip_cooperative_groups.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/hip_vector_types.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/hip_gl_interop.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/math_functions.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/hip_texture_types.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/hip_ext.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/hip_bfloat16.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/hip_runtime.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/hip_deprecated.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/hip_profile.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/hip_runtime_api.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/hip_math_constants.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/surface_types.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/driver_types.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/hip_bf16.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/library_types.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/hip_common.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/device_functions.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/hiprtc.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/channel_descriptor.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/hip_version.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/amd_math_functions.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/concepts.hpp
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/hip_ldg.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/grid_launch.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/amd_hip_bf16.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/functional_grid_launch.hpp
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/amd_hip_fp16.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/amd_hip_common.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/hsa_helpers.hpp
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/amd_hip_complex.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/macro_based_grid_launch.hpp
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/amd_device_functions.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/amd_hip_math_constants.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/amd_hip_bfloat16.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/host_defines.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/amd_surface_functions.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/amd_hip_cooperative_groups.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/program_state.hpp
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/hip_fp16_math_fwd.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/amd_hip_runtime_pt_api.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/hip_runtime_prof.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/amd_hip_gl_interop.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/hip_cooperative_groups_helper.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/hip_prof_str.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/grid_launch.hpp
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/amd_hip_atomic.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/hip_fp16_gcc.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/amd_warp_functions.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/amd_hip_vector_types.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/texture_fetch_functions.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/math_fwd.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/ockl_image.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/helpers.hpp
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/amd_channel_descriptor.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/texture_indirect_functions.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/amd_hip_runtime.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/grid_launch_GGL.hpp
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/amd_hip_unsafe_atomics.h
+Comment: 
+
+Filename: triton/backends/amd/include/hip/amd_detail/device_library_decls.h
+Comment: 
+
+Filename: triton/backends/amd/lib/opencl.bc
+Comment: 
+
+Filename: triton/backends/amd/lib/cuda2gcn.bc
+Comment: 
+
+Filename: triton/backends/amd/lib/ockl.bc
+Comment: 
+
+Filename: triton/backends/amd/lib/ocml.bc
+Comment: 
+
+Filename: triton/backends/intel/bin/
+Comment: 
+
+Filename: triton/backends/intel/lib/
+Comment: 
+
+Filename: triton/backends/intel/arch_parser.c
+Comment: 
+
+Filename: triton/backends/intel/driver.py
+Comment: 
+
+Filename: triton/backends/intel/compiler.py
+Comment: 
+
+Filename: triton/backends/intel/driver.c
+Comment: 
+
+Filename: triton/backends/intel/__init__.py
+Comment: 
+
+Filename: triton/backends/intel/bin/spirv-dis
+Comment: 
+
+Filename: triton/backends/intel/lib/libsycl-spir64-unknown-unknown.bc
+Comment: 
+
+Filename: triton/_C/libtriton.so
+Comment: 
+
+Filename: triton/_C/__init__.py
+Comment: 
+
+Filename: triton/ops/blocksparse/
+Comment: 
+
+Filename: triton/ops/matmul.py
+Comment: 
+
+Filename: triton/ops/matmul_perf_model.py
+Comment: 
+
+Filename: triton/ops/cross_entropy.py
+Comment: 
+
+Filename: triton/ops/flash_attention.py
+Comment: 
+
+Filename: triton/ops/__init__.py
+Comment: 
+
+Filename: triton/ops/blocksparse/softmax.py
+Comment: 
+
+Filename: triton/ops/blocksparse/matmul.py
+Comment: 
+
+Filename: triton/ops/blocksparse/__init__.py
+Comment: 
+
+Filename: triton/runtime/cache.py
+Comment: 
+
+Filename: triton/runtime/build.py
+Comment: 
+
+Filename: triton/runtime/jit.py
+Comment: 
+
+Filename: triton/runtime/driver.py
+Comment: 
+
+Filename: triton/runtime/interpreter.py
+Comment: 
+
+Filename: triton/runtime/errors.py
+Comment: 
+
+Filename: triton/runtime/autotuner.py
+Comment: 
+
+Filename: triton/runtime/__init__.py
+Comment: 
+
+Filename: triton/tools/disasm.py
+Comment: 
+
+Filename: triton/tools/build_extern.py
+Comment: 
+
+Filename: triton/tools/compile.h
+Comment: 
+
+Filename: triton/tools/compile.py
 Comment: 
 
-Filename: triton_xpu-0.0.2.dist-info/WHEEL
+Filename: triton/tools/link.py
 Comment: 
 
-Filename: triton_xpu-0.0.2.dist-info/top_level.txt
+Filename: triton/tools/compile.c
 Comment: 
 
-Filename: triton_xpu-0.0.2.dist-info/RECORD
+Filename: triton/tools/__init__.py
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## triton/__init__.py

```diff
@@ -1,9 +1,64 @@
 """isort:skip_file"""
-__version__ = '0.0.2'
+__version__ = '0.0.3a1'
+
+# ---------------------------------------
+# Note: import order is significant here.
+
+# submodules
+from .runtime import (
+    autotune,
+    Config,
+    heuristics,
+    JITFunction,
+    KernelInterface,
+    reinterpret,
+    TensorWrapper,
+    OutOfResources,
+    InterpreterError,
+    MockTensor,
+)
+from .runtime.jit import jit
+from .compiler import compile, CompilationError
+from .errors import TritonError
+
+from . import language
+from . import testing
+from . import tools
+
+__all__ = [
+    "autotune",
+    "cdiv",
+    "CompilationError",
+    "compile",
+    "Config",
+    "heuristics",
+    "impl",
+    "InterpreterError",
+    "jit",
+    "JITFunction",
+    "KernelInterface",
+    "language",
+    "MockTensor",
+    "next_power_of_2",
+    "ops",
+    "OutOfResources",
+    "reinterpret",
+    "runtime",
+    "TensorWrapper",
+    "TritonError",
+    "testing",
+    "tools",
+]
+
+# -------------------------------------
+# misc. utilities that  don't fit well
+# into any specific module
+# -------------------------------------
+
 
 def cdiv(x: int, y: int):
     return (x + y - 1) // y
 
 
 def next_power_of_2(n: int):
     """Return the smallest power of 2 greater than or equal to n"""
```

