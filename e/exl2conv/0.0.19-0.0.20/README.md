# Comparing `tmp/exl2conv-0.0.19.tar.gz` & `tmp/exl2conv-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exl2conv-0.0.19.tar", last modified: Fri Apr 26 11:14:48 2024, max compression
+gzip compressed data, was "exl2conv-0.0.20.tar", last modified: Mon Apr 29 15:19:05 2024, max compression
```

## Comparing `exl2conv-0.0.19.tar` & `exl2conv-0.0.20.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.690673 exl2conv-0.0.19/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-26 11:14:22.000000 exl2conv-0.0.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-26 11:14:22.000000 exl2conv-0.0.19/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-26 11:14:48.690673 exl2conv-0.0.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-26 11:14:22.000000 exl2conv-0.0.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.678673 exl2conv-0.0.19/exl2conv/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17069 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/architecture.py
--rw-r--r--   0 runner    (1001) docker     (127)    32609 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/attn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14232 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.678673 exl2conv-0.0.19/exl2conv/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)    21674 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/adaptivegptq.py
--rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    24398 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/qparams.py
--rw-r--r--   0 runner    (1001) docker     (127)    18875 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/quantize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.678673 exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/
--rw-r--r--   0 runner    (1001) docker     (127)   332173 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/c4.utf8
--rw-r--r--   0 runner    (1001) docker     (127)   248834 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/code.utf8
--rw-r--r--   0 runner    (1001) docker     (127)   222555 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/multilingual.utf8
--rw-r--r--   0 runner    (1001) docker     (127)   196701 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/technical.utf8
--rw-r--r--   0 runner    (1001) docker     (127)   261693 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/tiny.utf8
--rw-r--r--   0 runner    (1001) docker     (127)  2093275 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/wiki.utf8
--rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/conversion/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.682673 exl2conv-0.0.19/exl2conv/exl2conv_ext/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.682673 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/avx2_target.h
--rw-r--r--   0 runner    (1001) docker     (127)    24414 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/avx_mathfun.h
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/profiling.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/profiling.h
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/quantize_func.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/quantize_func.h
--rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/safetensors.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/safetensors.h
--rw-r--r--   0 runner    (1001) docker     (127)    20254 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/sampling.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/sampling.h
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/sampling_avx2.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/sampling_avx2.h
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/util.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.686673 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/
--rw-r--r--   0 runner    (1001) docker     (127)    10058 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/cache.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/cache.cuh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.686673 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cu
--rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cuh
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1a.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1b.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2a.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2b.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3a.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3b.cu
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_1.cu
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_2.cu
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_3.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/compat.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/h_add.cu
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/h_add.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/h_gemm.cu
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/h_gemm.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/head_norm.cu
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/head_norm.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/layer_norm.cu
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/layer_norm.cuh
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/lora.cu
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/lora.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/matrix_view.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/pack_tensor.cu
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/pack_tensor.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_attn.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_attn.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm.cu
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm_autotune.cuh
--rw-r--r--   0 runner    (1001) docker     (127)    19672 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm_kernel_gptq.cuh
--rw-r--r--   0 runner    (1001) docker     (127)    21853 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_matrix.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_matrix.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_mlp.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_mlp.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_mlp_activation.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_mlp_softmax.cuh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.686673 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_2.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_3.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_4.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_5.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_6.cuh
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_8.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_util.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     9812 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quantize.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quantize.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/rms_norm.cu
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/rms_norm.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/rope.cu
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/rope.cuh
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/util.cu
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/util.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_cache.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_cache.h
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_gemm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_gemm.h
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_hadamard.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_hadamard.h
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_norm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_norm.h
--rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qattn.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qattn.h
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qmatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qmatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qmlp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qmlp.h
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_quant.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_quant.h
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_rope.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_rope.h
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_safetensors.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_safetensors.h
--rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_sampling.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_sampling.h
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/fasttensors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.686673 exl2conv-0.0.19/exl2conv/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12746 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.686673 exl2conv-0.0.19/exl2conv/generator/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/filters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/filters/prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/filters/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/ngram.py
--rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    33047 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/generator/streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.686673 exl2conv-0.0.19/exl2conv/hadamard/
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_100.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13571 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_116.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24491 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_156.txt
--rw-r--r--   0 runner    (1001) docker     (127)    29755 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_172.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35531 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_188.txt
--rw-r--r--   0 runner    (1001) docker     (127)    55931 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_236.txt
--rw-r--r--   0 runner    (1001) docker     (127)    59779 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_244.txt
--rw-r--r--   0 runner    (1001) docker     (127)   183612 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_428.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_52.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/hadamard_92.txt
--rw-r--r--   0 runner    (1001) docker     (127)    58982 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/hadamard/primes.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/headnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    28424 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/model_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/moe_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/parallel_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/rmsnorm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.686673 exl2conv-0.0.19/exl2conv/server/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/server/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/server/websocket_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.686673 exl2conv-0.0.19/exl2conv/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/tokenizer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/tokenizer/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/tokenizer/spm.py
--rw-r--r--   0 runner    (1001) docker     (127)    22712 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/tokenizer/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    22386 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-26 11:14:22.000000 exl2conv-0.0.19/exl2conv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:14:48.678673 exl2conv-0.0.19/exl2conv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-26 11:14:48.000000 exl2conv-0.0.19/exl2conv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5953 2024-04-26 11:14:48.000000 exl2conv-0.0.19/exl2conv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:14:48.000000 exl2conv-0.0.19/exl2conv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-26 11:14:48.000000 exl2conv-0.0.19/exl2conv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 11:14:48.000000 exl2conv-0.0.19/exl2conv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 11:14:48.690673 exl2conv-0.0.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-26 11:14:22.000000 exl2conv-0.0.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.039785 exl2conv-0.0.20/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-29 15:18:33.000000 exl2conv-0.0.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-29 15:18:33.000000 exl2conv-0.0.20/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-29 15:19:05.039785 exl2conv-0.0.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-29 15:18:33.000000 exl2conv-0.0.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.023785 exl2conv-0.0.20/exl2conv/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18758 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/architecture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32609 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/attn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14232 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.027785 exl2conv-0.0.20/exl2conv/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)    22378 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/adaptivegptq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24398 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/qparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18875 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/quantize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.027785 exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   332173 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/c4.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)   248834 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/code.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)   222555 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/multilingual.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)   196701 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/technical.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)   261693 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/tiny.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)  2093275 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/wiki.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/conversion/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.031785 exl2conv-0.0.20/exl2conv/exl2conv_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/config.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.031785 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/avx2_target.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24414 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/avx_mathfun.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/profiling.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/profiling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/quantize_func.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/quantize_func.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/safetensors.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/safetensors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20254 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/sampling.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/sampling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/sampling_avx2.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/sampling_avx2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/util.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.035785 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/
+-rw-r--r--   0 runner    (1001) docker     (127)    10058 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/cache.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/cache.cuh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.035785 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1a.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1b.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2a.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2b.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3a.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3b.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_1.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_2.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_3.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/compat.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/h_add.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/h_add.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/h_gemm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/h_gemm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/head_norm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/head_norm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/layer_norm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/layer_norm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/lora.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/lora.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/matrix_view.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/pack_tensor.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/pack_tensor.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_attn.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_attn.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm_autotune.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    19672 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm_kernel_gptq.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    21853 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_matrix.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_matrix.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_mlp.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_mlp.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_mlp_activation.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_mlp_softmax.cuh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.035785 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_2.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_3.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_4.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_5.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_6.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_8.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_util.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     9812 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quantize.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quantize.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/rms_norm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/rms_norm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/rope.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/rope.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/util.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/util.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_cache.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_cache.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_gemm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_gemm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_hadamard.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_hadamard.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_norm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_norm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qattn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qattn.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qmatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qmatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qmlp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qmlp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_quant.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_quant.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_rope.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_rope.h
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_safetensors.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_safetensors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_sampling.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_sampling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/fasttensors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.035785 exl2conv-0.0.20/exl2conv/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12746 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.035785 exl2conv-0.0.20/exl2conv/generator/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/filters/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/filters/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/ngram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33700 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/generator/streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.035785 exl2conv-0.0.20/exl2conv/hadamard/
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_100.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13571 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_116.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24491 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_156.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    29755 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_172.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35531 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_188.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    55931 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_236.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    59779 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_244.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   183612 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_428.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_52.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/hadamard_92.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    58982 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/hadamard/primes.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/headnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29232 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/model_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/moe_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/parallel_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/rmsnorm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.035785 exl2conv-0.0.20/exl2conv/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/server/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/server/websocket_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.039785 exl2conv-0.0.20/exl2conv/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/tokenizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/tokenizer/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/tokenizer/spm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23253 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/tokenizer/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22386 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 15:18:33.000000 exl2conv-0.0.20/exl2conv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:19:05.027785 exl2conv-0.0.20/exl2conv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-29 15:19:05.000000 exl2conv-0.0.20/exl2conv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5953 2024-04-29 15:19:05.000000 exl2conv-0.0.20/exl2conv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:19:05.000000 exl2conv-0.0.20/exl2conv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-29 15:19:05.000000 exl2conv-0.0.20/exl2conv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 15:19:05.000000 exl2conv-0.0.20/exl2conv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:19:05.039785 exl2conv-0.0.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-29 15:18:33.000000 exl2conv-0.0.20/setup.py
```

### Comparing `exl2conv-0.0.19/LICENSE` & `exl2conv-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/README.md` & `exl2conv-0.0.20/README.md`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/architecture.py` & `exl2conv-0.0.20/exl2conv/architecture.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,24 @@
                          ["self_attn.k_proj"],
                          ["self_attn.v_proj"],
                          ["self_attn.o_proj"]]
 layer_keys_dbrx_attn = [["self_attn.Wqkv", "self_attn.q_proj"],
                         ["self_attn.Wqkv", "self_attn.k_proj"],
                         ["self_attn.Wqkv", "self_attn.v_proj"],
                         ["self_attn.o_proj"]]
+layer_keys_phi3_attn = [["self_attn.qkv_proj", "self_attn.q_proj"],
+                        ["self_attn.qkv_proj", "self_attn.k_proj"],
+                        ["self_attn.qkv_proj", "self_attn.v_proj"],
+                        ["self_attn.o_proj"]]
 layer_keys_llama_mlp = [["mlp.down_proj"],
                         ["mlp.gate_proj"],
                         ["mlp.up_proj"]]
+layer_keys_phi3_mlp = [["mlp.down_proj"],
+                       ["mlp.gate_up_proj", "mlp.gate_proj"],
+                       ["mlp.gate_up_proj", "mlp.up_proj"]]
 layer_keys_mixtral_mlp = [["block_sparse_moe.experts.*.w1"],
                           ["block_sparse_moe.experts.*.w2"],
                           ["block_sparse_moe.experts.*.w3"],
                           ["block_sparse_moe.gate"]]
 layer_keys_dbrx_mlp = [["block_sparse_moe.experts.*.v1", "block_sparse_moe.experts.v1"],
                        ["block_sparse_moe.experts.*.w1", "block_sparse_moe.experts.w1"],
                        ["block_sparse_moe.experts.*.w2", "block_sparse_moe.experts.w2"],
@@ -384,14 +391,47 @@
             self.requires_bos = False
             self.rope_neox_style = True
             self.keymap = dbrx_keymap
             self.fused_qkv_key = "Wqkv"
 
         # Llama (default + fallback)
 
+        if arch_string == "Phi3ForCausalLM":
+            arch_recognized = True
+            self.layer_keys += \
+                layer_keys_llama_norms + \
+                layer_keys_phi3_attn + \
+                layer_keys_phi3_mlp
+            self.expect_keys += \
+                expect_keys_llama
+            self.norm_eps_key = "rms_norm_eps"
+            self.attention_bias_qkv = False
+            self.attention_bias_o = False
+            self.mlp_bias = False
+            self.mlp_gate = True
+            self.mlp_key_gate = ".mlp.gate_proj"
+            self.mlp_key_up = ".mlp.up_proj"
+            self.mlp_key_down = ".mlp.down_proj"
+            self.mlp_act_func = "silu"
+            self.is_moe = False
+            self.norm = "rmsnorm"
+            self.lm_head_key = "lm_head"
+            self.normalize_embeddings = False
+            self.norm_key_1 = ".input_layernorm"
+            self.norm_key_2 = ".post_attention_layernorm"
+            self.norm_constant_bias = 0
+            self.parallel_decoder_blocks = False
+            self.requires_bos = False
+            self.rope_neox_style = True
+            self.keymap = None
+            self.fused_qkv_key = "qkv_proj"
+            self.fused_mlp_key_12 = "gate_up_proj"
+
+        # Llama (default + fallback)
+
         if arch_string != "LlamaForCausalLM" and not arch_recognized:
             print(f" !! Warning, unknown architecture: {arch_string}")
             print(f" !! Loading as LlamaForCausalLM")
             self.arch_string = "LlamaForCausalLM"
         if not arch_recognized:
             self.layer_keys += \
                 layer_keys_llama_norms + \
```

### Comparing `exl2conv-0.0.19/exl2conv/attn.py` & `exl2conv-0.0.20/exl2conv/attn.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/cache.py` & `exl2conv-0.0.20/exl2conv/cache.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/compat.py` & `exl2conv-0.0.20/exl2conv/compat.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/config.py` & `exl2conv-0.0.20/exl2conv/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,14 +81,18 @@
     num_attention_heads: int
     num_key_value_heads: int
     num_key_value_groups: int
     num_hidden_layers: int
     norm_eps: float | None
     vocab_size: int
     rotary_embedding_base: float
+    scale_long_factor: list[float] | None
+    scale_short_factor: list[float] | None
+    alt_rope_method: str | None
+    original_max_seq_len: int
     head_dim: int
     num_experts: int | None
     num_experts_per_token: int | None
     logit_scale: float
     use_qk_norm: bool
 
     checkpoint_fused_mlp: bool
@@ -103,27 +107,31 @@
 
         self.max_batch_size = 1
         self.max_input_len = 2048
         self.max_attention_size = 2048**2
         self.max_output_len = None
         self.scale_pos_emb = 1.0
         self.scale_alpha_value = 1.0
+        self.scale_long_factor = None
+        self.scale_short_factor = None
+        self.alt_rope_method = None
 
         self.no_flash_attn = False
         self.fasttensors = False
         self.load_in_q4 = False
 
         if model_dir is not None:
             self.model_dir = model_dir
             self.prepare()
         else:
             self.model_dir = None
 
         self.max_dq_size = 512*(1024**2)
 
+
     # Set low-mem options
 
     def set_low_mem(self):
 
         self.max_input_len = 1024
         self.max_attention_size = 1024 ** 2
         self.max_output_len = 1024
@@ -196,22 +204,32 @@
 
         self.rotary_embedding_base = read(read_config, float, ["rope_theta", "attn_config->rope_theta"], 10000.0)
 
         self.max_seq_len = read(read_config, int,["max_sequence_length",
                                                   "model_max_length",
                                                   "max_position_embeddings",
                                                   "max_seq_len"], 2048)
+        self.original_max_seq_len = self.max_seq_len
 
         rs = read(read_config, dict, "rope_scaling", None)
-        if rs and "factor" in rs:
-            factor = rs["factor"]
+        if rs:
             scaling_type = rs.get("type", None)
             if scaling_type == "linear":
-                self.scale_pos_emb = factor
-            # elif scaling_type == "yarn":
+                assert "factor" in rs, "'factor' missing from 'rope_scaling' config"
+                self.scale_pos_emb = rs.get("factor", 1.0)
+            if scaling_type == "su":
+                assert "long_factor" in rs, "'long_factor' missing from 'rope_scaling' config"
+                assert "short_factor" in rs, "'short_factor' missing from 'rope_scaling' config"
+                assert "original_max_position_embeddings" in read_config, \
+                    "'original_max_position_embeddings' required for 'su' scaling"
+                self.scale_long_factor = rs["long_factor"]
+                self.scale_short_factor = rs["short_factor"]
+                self.original_max_seq_len = read_config["original_max_position_embeddings"]
+                self.alt_rope_method = "su"
+            # if scaling_type == "yarn":
             #     self.scale_alpha_value = factor
 
         # Create map of model tensors
 
         if no_tensors: return
 
         self.tensor_file_map = {}
```

### Comparing `exl2conv-0.0.19/exl2conv/conversion/adaptivegptq.py` & `exl2conv-0.0.20/exl2conv/conversion/adaptivegptq.py`

 * *Files 5% similar despite different names*

```diff
@@ -194,23 +194,39 @@
         self.total_groups = groups
 
 
     def add_batch(self, inputs):
 
         with torch.inference_mode():
 
+            # dim = inputs.shape[-1]
+            # inputs = inputs.view((-1, dim)).float().T.to("cuda:0")
+            # ns = 1
+            #
+            # if self.hessian is None:
+            #     self.hessian = torch.zeros((dim, dim), device = self.device, dtype = torch.float)
+            # else:
+            #     self.hessian.mul_(self.num_samples / (self.num_samples + ns))
+            # self.num_samples += ns
+            # inputs.mul_(math.sqrt(2 / self.num_samples))
+            # self.hessian.addmm_(inputs, inputs.T)
+
+            # self.num_batches += 1
+            # num_samples = len(inputs)
+            # # inputs = torch.cat(inputs, dim = 0)
+            # inputs = inputs.view((-1, inputs.shape[-1])).float().T.to("cuda:0")
+            # inputs *= math.sqrt(2 / num_samples)
+            # self.hessian += inputs.matmul(inputs.T)
+
             if self.hessian is None:
                 self.hessian = torch.zeros((self.rows, self.rows), device=self.device, dtype=torch.float)
 
             self.num_batches += 1
-            num_samples = len(inputs)
-            # inputs = torch.cat(inputs, dim = 0)
-            inputs = inputs.view((-1, inputs.shape[-1])).float().T.to("cuda:0")
-            inputs *= math.sqrt(2 / num_samples)
-            self.hessian += inputs.matmul(inputs.T)
+            inputs = inputs.view((-1, inputs.shape[-1])).float().to("cuda:0")
+            self.hessian.addmm_(inputs.T, inputs)
 
 
     def prepare(self, no_h_inv = False):
 
         with torch.inference_mode():
 
             self.hessian /= self.num_batches
```

### Comparing `exl2conv-0.0.19/exl2conv/conversion/compile.py` & `exl2conv-0.0.20/exl2conv/conversion/compile.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/conversion/convert.py` & `exl2conv-0.0.20/exl2conv/conversion/convert.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/conversion/measure.py` & `exl2conv-0.0.20/exl2conv/conversion/measure.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/conversion/optimize.py` & `exl2conv-0.0.20/exl2conv/conversion/optimize.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/conversion/qparams.py` & `exl2conv-0.0.20/exl2conv/conversion/qparams.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/conversion/quantize.py` & `exl2conv-0.0.20/exl2conv/conversion/quantize.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/c4.utf8` & `exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/c4.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/code.utf8` & `exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/code.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/multilingual.utf8` & `exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/multilingual.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/technical.utf8` & `exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/technical.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/tiny.utf8` & `exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/tiny.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/conversion/standard_cal_data/wiki.utf8` & `exl2conv-0.0.20/exl2conv/conversion/standard_cal_data/wiki.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/conversion/tokenize.py` & `exl2conv-0.0.20/exl2conv/conversion/tokenize.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/embedding.py` & `exl2conv-0.0.20/exl2conv/embedding.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/avx2_target.h` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/avx2_target.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/avx_mathfun.h` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/avx_mathfun.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/profiling.cpp` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/profiling.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/quantize_func.cpp` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/quantize_func.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/quantize_func.h` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/quantize_func.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/safetensors.cpp` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/safetensors.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/safetensors.h` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/safetensors.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/sampling.cpp` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/sampling.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/sampling.h` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/sampling.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/sampling_avx2.cpp` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/sampling_avx2.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cpp/util.h` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cpp/util.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/cache.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/cache.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/cache.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/cache.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1a.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1a.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1b.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1b.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2a.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2a.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2b.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2b.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3a.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3a.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3b.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3b.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_1.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_1.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_2.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_2.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_3.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_3.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/compat.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/compat.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/h_add.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/h_add.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/h_gemm.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/h_gemm.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/h_gemm.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/h_gemm.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/head_norm.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/head_norm.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/layer_norm.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/layer_norm.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/lora.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/lora.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/matrix_view.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/matrix_view.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/pack_tensor.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/pack_tensor.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/pack_tensor.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/pack_tensor.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_attn.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_attn.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_attn.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_attn.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm_autotune.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm_autotune.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm_kernel.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm_kernel.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_gemm_kernel_gptq.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_gemm_kernel_gptq.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_matrix.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_matrix.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_matrix.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_matrix.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_mlp.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_mlp.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_mlp.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_mlp.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_mlp_activation.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_mlp_activation.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/q_mlp_softmax.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/q_mlp_softmax.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_2.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_2.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_3.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_3.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_4.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_4.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_5.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_5.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_6.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_6.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_8.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_8.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quant/qdq_util.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quant/qdq_util.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quantize.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quantize.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/quantize.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/quantize.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/rms_norm.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/rms_norm.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/rope.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/rope.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/rope.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/rope.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/util.cu` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/util.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/cuda/util.cuh` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/cuda/util.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_bindings.cpp` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_bindings.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_cache.cpp` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_cache.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_cache.h` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_cache.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_gemm.cpp` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_gemm.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_hadamard.cpp` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_hadamard.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_norm.cpp` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_norm.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_norm.h` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_norm.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qattn.cpp` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qattn.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qattn.h` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qattn.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qmatrix.cpp` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qmatrix.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qmatrix.h` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qmatrix.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qmlp.cpp` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qmlp.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_qmlp.h` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_qmlp.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_quant.cpp` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_quant.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_quant.h` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_quant.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_rope.cpp` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_rope.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_sampling.cpp` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_sampling.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/exl2conv_ext/ext_sampling.h` & `exl2conv-0.0.20/exl2conv/exl2conv_ext/ext_sampling.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/ext.py` & `exl2conv-0.0.20/exl2conv/ext.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/fasttensors.py` & `exl2conv-0.0.20/exl2conv/fasttensors.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/generator/base.py` & `exl2conv-0.0.20/exl2conv/generator/base.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/generator/filters/base.py` & `exl2conv-0.0.20/exl2conv/generator/filters/base.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/generator/filters/prefix.py` & `exl2conv-0.0.20/exl2conv/generator/filters/prefix.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/generator/filters/select.py` & `exl2conv-0.0.20/exl2conv/generator/filters/select.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/generator/ngram.py` & `exl2conv-0.0.20/exl2conv/generator/ngram.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/generator/sampler.py` & `exl2conv-0.0.20/exl2conv/generator/sampler.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/generator/streaming.py` & `exl2conv-0.0.20/exl2conv/generator/streaming.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,18 @@
     first_token: bool
     heal_next_token: bool
 
     # LoRAs
 
     active_loras: list[ExLlamaV2Lora]
 
+    # Extra decoding options
+
+    decode_special_tokens: bool
+
 
     def __init__(self, model, cache, tokenizer, draft_model = None, draft_cache = None, num_speculative_tokens = 5):
         super().__init__(model, cache, tokenizer)
 
         # Stop conditions
 
         self.stop_strings = set()
@@ -212,15 +216,16 @@
                         token_healing: bool = False,
                         loras: ExLlamaV2Lora | list[ExLlamaV2Lora] = None,
                         input_mask: torch.Tensor | None = None,
                         position_offsets: torch.Tensor | None = None,
                         return_probabilities: bool = False,
                         return_top_tokens: int = 0,
                         return_logits: bool = False,
-                        abort_event: threading.Event = None):
+                        abort_event: threading.Event = None,
+                        decode_special_tokens: bool = False):
         """
         Resets the generator and starts a new completion of the supplied input_ids. Reuses the existing
         cache for any token IDs matching the previous sequence.
 
         :param input_ids:
             Input token ID sequence, as produced by ExLlamaV2Tokenizer. Streaming generator does not
             currently support batch size > 1 except when performing CFG, in which case batch size
@@ -250,22 +255,27 @@
             probabilities.
 
         :param return_logits:
             Return the raw logits output by the model for each streamed token
 
         :param abort_event:
             Forwarded to the model during generation. Will abort prefill/context ingestion if triggered.
+
+        :param decode_special_tokens:
+            Also decode special tokens into output text stream
         """
 
         self.return_probabilities = return_probabilities
         self.return_top_tokens = return_top_tokens
         self.return_logits = return_logits
 
         self.abort_event = abort_event
 
+        self.decode_special_tokens = decode_special_tokens
+
         assert input_ids.shape[0] <= 2, "Streaming generator does not support batch size > 1"
         if input_ids.shape[0] == 2:
             assert gen_settings.cfg_scale is not None, "No CFG scale set"
 
         self.position_offsets = position_offsets
         self.input_mask = input_mask
 
@@ -390,30 +400,32 @@
 
         # Token healing
 
         if self.heal_next_token:
 
             # Pop the last token
 
-            old_tail = self.tokenizer.decode(self.sequence_ids[:, -self.tail_decode_tokens:])[0]
+            old_tail = self.tokenizer.decode(self.sequence_ids[:, -self.tail_decode_tokens:],
+                                             decode_special_tokens = self.decode_special_tokens)[0]
             last_token = self.sequence_ids[:, -1:]
             self.sequence_ids = self.sequence_ids[:, :-1]
             self.cache.current_seq_len -= 1
 
             # Start filters
 
             if self.first_token:
 
-                self.settings.begin_filters(self.tokenizer.get_id_to_piece_list()[last_token])
+                self.settings.begin_filters(self.tokenizer.get_id_to_piece_list(self.decode_special_tokens)[last_token])
                 self.first_token = False
 
             # Regenerate the last token again, with prefix
 
             healed_token, _, _, _, eos, logits = self._gen_single_token(self.settings, prefix_token = last_token)
-            new_tail = self.tokenizer.decode(self.sequence_ids[:, -self.tail_decode_tokens:])[0]
+            new_tail = self.tokenizer.decode(self.sequence_ids[:, -self.tail_decode_tokens:],
+                                             decode_special_tokens = self.decode_special_tokens)[0]
             self.held_text += new_tail[len(old_tail):]
 
             self.heal_next_token = False
 
             # In case we only needed the healed token
 
             if eos: return self.held_text, True, self.no_tokens, self.no_probs, self.no_ptokens, self.no_pprobs, self.no_logits
@@ -432,15 +444,15 @@
         next_token, next_ptokens, next_pprobs, next_prob, eos, next_logits = self._gen_single_token(self.settings)
 
         # End immediately if it was a stop token
 
         if next_token.item() in self.stop_tokens:
             return self.held_text, True, self.no_tokens, self.no_probs, self.no_ptokens, self.no_pprobs, self.no_logits
 
-        id_to_piece = self.tokenizer.get_id_to_piece_list()
+        id_to_piece = self.tokenizer.get_id_to_piece_list(self.decode_special_tokens)
         new_text = id_to_piece[next_token]
 
         next_token, new_text = self._catch_utf8(next_token, new_text)
         next_token, new_text = self._catch_fallback(next_token, new_text)
 
         self.held_text += new_text
         self.held_tokens = torch.cat([self.held_tokens, next_token], dim = -1)
@@ -503,29 +515,30 @@
         if self.held_utf8_tokens.shape[-1] == 0: return self.no_tokens, ""
 
         try:
             id_to_ord = self.tokenizer.get_id_to_ord_list()
             b = [id_to_ord[x] for x in self.held_utf8_tokens[0].tolist()]
             c = bytes(b).decode('utf-8')
         except ValueError or UnicodeDecodeError:
-            id_to_piece = self.tokenizer.get_id_to_piece_list()
+            id_to_piece = self.tokenizer.get_id_to_piece_list(self.decode_special_tokens)
             c = "".join(id_to_piece[x] for x in self.held_utf8_tokens[0].tolist())
 
         pre_t = self.held_utf8_tokens
         self.held_utf8_tokens = self.no_tokens
         return pre_t, c
 
 
     def _catch_fallback(self, next_token, new_text):
 
         if self.held_fallback_tokens.shape[-1] == 0:
             if "�" not in new_text: return next_token, new_text
 
         self.held_fallback_tokens = torch.cat((self.held_fallback_tokens, next_token), dim = -1)
-        new_decode = self.tokenizer.decode(self.held_fallback_tokens)[0]
+        new_decode = self.tokenizer.decode(self.held_fallback_tokens,
+                                           decode_special_tokens = self.decode_special_tokens)[0]
 
         if "�" not in new_decode or self.held_fallback_tokens.shape[-1] >= self.max_fallback_tokens:
             r_tokens = self.held_fallback_tokens
             self.held_fallback_tokens = self.no_tokens
             return r_tokens, new_decode
 
         return self.no_tokens, ""
```

### Comparing `exl2conv-0.0.19/exl2conv/hadamard/hadamard.py` & `exl2conv-0.0.20/exl2conv/hadamard/hadamard.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/hadamard/primes.txt` & `exl2conv-0.0.20/exl2conv/hadamard/primes.txt`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/headnorm.py` & `exl2conv-0.0.20/exl2conv/headnorm.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/layernorm.py` & `exl2conv-0.0.20/exl2conv/layernorm.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/linear.py` & `exl2conv-0.0.20/exl2conv/linear.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/lora.py` & `exl2conv-0.0.20/exl2conv/lora.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/mlp.py` & `exl2conv-0.0.20/exl2conv/mlp.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,43 +35,46 @@
                  model: ExLlamaV2,
                  key: str,
                  layer_idx: int,
                  has_norm: bool = True,
                  has_residual: bool = True):
 
         super().__init__(model, key)
+        cfg = self.model.config
 
         self.layer_idx = layer_idx
         self.has_norm = has_norm
         self.has_residual = has_residual
 
         self.q_handle = None
         self.temp_lora_size = 0
 
-        hidden_size = self.model.config.hidden_size
-        intermediate_size = self.model.config.intermediate_size
+        f_a = 0
+        f_b = cfg.intermediate_size
+        f_c = f_b + cfg.intermediate_size
+        f_key = (key + ".mlp." + cfg.arch.fused_mlp_key_12) if cfg.arch.fused_mlp_key_12 else None
 
         if self.has_norm:
-            if self.model.config.arch.norm == "layernorm":
-                self.post_attention_layernorm = ExLlamaV2LayerNorm(model, key + self.model.config.arch.norm_key_2)
-            elif self.model.config.arch.norm == "rmsnorm":
-                self.post_attention_layernorm = ExLlamaV2RMSNorm(model, key + self.model.config.arch.norm_key_2)
+            if cfg.arch.norm == "layernorm":
+                self.post_attention_layernorm = ExLlamaV2LayerNorm(model, key + cfg.arch.norm_key_2)
+            elif cfg.arch.norm == "rmsnorm":
+                self.post_attention_layernorm = ExLlamaV2RMSNorm(model, key + cfg.arch.norm_key_2)
         else:
             self.post_attention_layernorm = None
 
-        self.up_proj = ExLlamaV2Linear(model, key + self.model.config.arch.mlp_key_up, hidden_size, intermediate_size, self.model.config.arch.mlp_bias)
-        self.down_proj = ExLlamaV2Linear(model, key + self.model.config.arch.mlp_key_down, intermediate_size, hidden_size, self.model.config.arch.mlp_bias)
+        self.up_proj = ExLlamaV2Linear(model, key + cfg.arch.mlp_key_up, cfg.hidden_size, cfg.intermediate_size, self.model.config.arch.mlp_bias, f_key = f_key, f_beg = f_b, f_end = f_c)
+        self.down_proj = ExLlamaV2Linear(model, key + cfg.arch.mlp_key_down, cfg.intermediate_size, cfg.hidden_size, self.model.config.arch.mlp_bias)
 
         self.submodules = [self.up_proj,
                            self.down_proj]
         if self.has_norm:
             self.submodules += [self.post_attention_layernorm]
 
-        if self.model.config.arch.mlp_gate:
-            self.gate_proj = ExLlamaV2Linear(model, key + self.model.config.arch.mlp_key_gate, hidden_size, intermediate_size, self.model.config.arch.mlp_bias)
+        if cfg.arch.mlp_gate:
+            self.gate_proj = ExLlamaV2Linear(model, key + cfg.arch.mlp_key_gate, cfg.hidden_size, cfg.intermediate_size, self.model.config.arch.mlp_bias, f_key = f_key, f_beg = f_a, f_end = f_b)
             self.submodules += [self.gate_proj]
         else:
             self.gate_proj = None
 
 
     def numel(self) -> int:
 
@@ -85,22 +88,24 @@
             numel += self.post_attention_layernorm.numel()
 
         return numel
 
 
     def load(self):
 
+        cfg = self.model.config
+
         if self.post_attention_layernorm is not None:
             self.post_attention_layernorm.load()
 
-        if self.model.config.checkpoint_fused_mlp:
-            w12 = self.load_weight(self.key + self.model.config.arch.fused_mlp_key_12)
-            w1 = nn.Parameter(w12[:self.model.config.intermediate_size, :].contiguous())
-            w2 = nn.Parameter(w12[self.model.config.intermediate_size:, :].contiguous())
-            w3 = self.load_weight(self.key + self.model.config.arch.fused_mlp_key_3)
+        if cfg.checkpoint_fused_mlp:
+            w12 = self.load_weight(self.key + cfg.arch.fused_mlp_key_12)
+            w1 = nn.Parameter(w12[:cfg.intermediate_size, :].contiguous())
+            w2 = nn.Parameter(w12[cfg.intermediate_size:, :].contiguous())
+            w3 = self.load_weight(self.key + cfg.arch.fused_mlp_key_3)
             self.gate_proj.load(w1)
             self.up_proj.load(w2)
             self.down_proj.load(w3)
         else:
             if self.gate_proj is not None: self.gate_proj.load()
             self.up_proj.load()
             self.down_proj.load()
@@ -129,16 +134,16 @@
                                              0 if self.gate_proj is None else self.gate_proj.q_handle,
                                              self.up_proj.q_handle,
                                              self.down_proj.q_handle,
                                              device_tensors.get_scratch_slice(self.temp_state_size()),
                                              device_tensors.get_scratch_slice(self.temp_a_size()),
                                              device_tensors.get_scratch_slice(self.temp_b_size()),
                                              device_tensors.get_scratch_slice(self.temp_dq_size()),
-                                             self.model.config.max_input_len * self.model.config.max_batch_size,
-                                             self.model.config.arch.mlp_act_func == "gelu",
+                                             cfg.max_input_len * cfg.max_batch_size,
+                                             cfg.arch.mlp_act_func == "gelu",
                                              self.has_residual)
 
 
     def unload(self):
 
         if self.q_handle is not None:
             ext_c.free_q_mlp(self.q_handle)
```

### Comparing `exl2conv-0.0.19/exl2conv/model.py` & `exl2conv-0.0.20/exl2conv/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,35 +109,65 @@
         scratch_slice = self.scratch.narrow(0, self.scratch_idx, size_half)
         self.scratch_idx += size_half
         return scratch_slice
 
 
     def prepare_sincos(self):
 
-        base = self.model.config.rotary_embedding_base
-        alpha = self.model.config.scale_alpha_value or 1.0
-        scale = self.model.config.scale_pos_emb or 1.0
-        head_dim = self.model.config.head_dim
+        cfg = self.model.config
+
+        base = cfg.rotary_embedding_base
+        alpha = cfg.scale_alpha_value or 1.0
+        scale = cfg.scale_pos_emb or 1.0
+        head_dim = cfg.head_dim
         device = _torch_device(self.device_idx)
+        scaling_factor = 1.0
+
+        # Alpha scaling for any rope_scaling type
+
+        if alpha != 1.0: base *= alpha ** (cfg.head_dim / (cfg.head_dim - 2))
+
+        # "su"
+
+        if cfg.alt_rope_method == "su":
+
+            a = cfg.max_seq_len
+            b = cfg.original_max_seq_len
+            if a > b:
+                ext_factors = torch.tensor(cfg.scale_long_factor, dtype = torch.float32, device = device)
+                scaling_factor = math.sqrt(1 + math.log(a / b) / math.log(b))
+            else:
+                ext_factors = torch.tensor(cfg.scale_short_factor, dtype = torch.float32, device = device)
+
+            inv_freq = 1.0 / (ext_factors * base ** (torch.arange(0, head_dim, 2, device = device).float() / head_dim))
+
+        # Regular
+
+        else:
 
-        if alpha != 1.0: base *= alpha ** (self.model.config.head_dim / (self.model.config.head_dim - 2))
+            inv_freq = 1.0 / (base ** (torch.arange(0, head_dim, 2, device = device).float() / head_dim))
 
-        inv_freq = 1.0 / (base ** (torch.arange(0, head_dim, 2, device = device).float() / head_dim))
-        t = torch.arange(self.model.config.max_seq_len, device = device, dtype = torch.float32)
+        # Common
 
+        t = torch.arange(cfg.max_seq_len, device = device, dtype = torch.float32)
         if scale != 1.0: t /= scale
 
         freqs = torch.einsum("i,j->ij", t, inv_freq)
-        if self.model.config.arch.rope_neox_style:
+        if cfg.arch.rope_neox_style:
             emb = torch.cat((freqs, freqs), dim=-1)
         else:
             emb = torch.repeat_interleave(freqs, 2, dim=-1)
 
-        self.sin = emb.sin()[None, None, :, :].half()
-        self.cos = emb.cos()[None, None, :, :].half()
+        self.sin = emb.sin()[None, None, :, :]
+        self.cos = emb.cos()[None, None, :, :]
+        if scaling_factor != 1.0:
+            self.sin *= scaling_factor
+            self.cos *= scaling_factor
+        self.sin = self.sin.half()
+        self.cos = self.cos.half()
 
 
 class ExLlamaV2:
 
     config: ExLlamaV2Config
     modules: list[ExLlamaV2Module]
     modules_dict: dict[str: ExLlamaV2Module]
```

### Comparing `exl2conv-0.0.19/exl2conv/model_init.py` & `exl2conv-0.0.20/exl2conv/model_init.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/module.py` & `exl2conv-0.0.20/exl2conv/module.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/moe_mlp.py` & `exl2conv-0.0.20/exl2conv/moe_mlp.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/parallel_decoder.py` & `exl2conv-0.0.20/exl2conv/parallel_decoder.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/rmsnorm.py` & `exl2conv-0.0.20/exl2conv/rmsnorm.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/server/websocket.py` & `exl2conv-0.0.20/exl2conv/server/websocket.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/server/websocket_actions.py` & `exl2conv-0.0.20/exl2conv/server/websocket_actions.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/tokenizer/base.py` & `exl2conv-0.0.20/exl2conv/tokenizer/base.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/tokenizer/hf.py` & `exl2conv-0.0.20/exl2conv/tokenizer/hf.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/tokenizer/spm.py` & `exl2conv-0.0.20/exl2conv/tokenizer/spm.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv/tokenizer/tokenizer.py` & `exl2conv-0.0.20/exl2conv/tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,29 +273,14 @@
         :return:
             LongTensor of shape (1, 1) of token ID
         """
 
         return torch.tensor([[token_id]], dtype = torch.long)
 
 
-    def single_id(self, token: str) -> torch.Tensor:
-        """
-        Get the ID of a single token from exact string match
-
-        :param token:
-            Token
-
-        :return:
-            int
-        """
-
-        tid = self.extended_piece_to_id.get(token, self.get_piece_to_id_dict().get(token))
-        return tid
-
-
     # Encode string with added, unspecial tokens
 
     def encode_unspecial(self, text: str) -> list[int]:
 
         if not self.unspecial_piece_to_id:
             return self.tokenizer_model.encode(text)
```

### Comparing `exl2conv-0.0.19/exl2conv/tokenizer.py` & `exl2conv-0.0.20/exl2conv/tokenizer/tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     eos_token_id: int
     pad_token_id: int
     newline_token_id: int | None
     space_token_id: int | None
 
     id_to_ord: list | None
     id_to_piece: list | None
+    id_to_piece_with_special: list | None
     piece_to_id: dict | None
     prefix_to_ids: dict | None
     prefix_id_to_ids: dict | None
     char_trie: Trie | None
     char_trie_ci: Trie | None
 
     unspecial_piece_to_id: dict[str: int]
@@ -159,15 +160,15 @@
         self.unk_token_id = self.tokenizer_model.unk_id()
         self.eos_token_id = config.eos_token_id
         self.bos_token_id = config.bos_token_id
         self.pad_token_id = config.pad_token_id
 
         # If model config doesn't specify BOS and EOS tokens, try to load from tokenizer config
 
-        def get_default_token_id(config_key: str, current: int | None, default: int):
+        def get_default_token_id(config_key: str, current: int | None, default: int | None):
             if current is not None: return current
             if self.tokenizer_config_dict is not None and config_key in self.tokenizer_config_dict:
                 st = self.tokenizer_config_dict[config_key]
                 if st is None: return None
                 if isinstance(st, dict):
                     stc: str | None = st.get("content", None)
                     if stc is None:
@@ -177,29 +178,29 @@
                 elif isinstance(st, str):
                     return self.tokenizer_model.piece_to_id(st)
                 else:
                     return None
             else:
                 return default
 
-        self.pad_token_id = get_default_token_id("pad_token", self.pad_token_id, 0)
+        self.pad_token_id = get_default_token_id("pad_token", self.pad_token_id, None)
         self.bos_token_id = get_default_token_id("bos_token", self.bos_token_id, 1)
         self.eos_token_id = get_default_token_id("eos_token", self.eos_token_id, 2)
 
         # Get control token strings
 
         self.unk_token = (self.tokenizer_model.unk_token() or self.extended_id_to_piece.get(self.unk_token_id, None)) or self.tokenizer_model.id_to_piece(self.unk_token_id)
         self.bos_token = (self.tokenizer_model.bos_token() or self.extended_id_to_piece.get(self.bos_token_id, None)) or self.tokenizer_model.id_to_piece(self.bos_token_id)
         self.eos_token = (self.tokenizer_model.eos_token() or self.extended_id_to_piece.get(self.eos_token_id, None)) or self.tokenizer_model.id_to_piece(self.eos_token_id)
 
-        # Use "<pad>" or EOS token as fallback for padding token
+        # Use "<pad>" or BOS token as fallback for padding token
 
         if self.pad_token_id is None:
             pad_test = self.tokenizer_model.piece_to_id("<pad>")
-            self.pad_token_id = pad_test or self.eos_token_id
+            self.pad_token_id = pad_test or self.bos_token_id
 
         # Special case if <unk> and <pad> have the same ID
 
         if self.unk_token_id == self.pad_token_id:
             self.unk_token = self.pad_token
 
         # Make sure extended vocab contains control tokens, but avoid empty pieces
@@ -227,14 +228,15 @@
         try: self.space_token_id = self.tokenizer_model.encode(self.space_token)[-1]
         except: self.space_token_id = None
 
         # Optionally create dictionaries on init
 
         self.id_to_ord = None
         self.id_to_piece = None
+        self.id_to_piece_with_special = None
         self.piece_to_id = None
         self.prefix_to_ids = None
         self.prefix_id_to_ids = None
         self.char_trie = None
         self.char_trie_ci = None
 
         if not lazy_init:
@@ -273,14 +275,29 @@
         :return:
             LongTensor of shape (1, 1) of token ID
         """
 
         return torch.tensor([[token_id]], dtype = torch.long)
 
 
+    def single_id(self, token: str) -> int:
+        """
+        Get the ID of a single token from exact string match
+
+        :param token:
+            Token
+
+        :return:
+            int
+        """
+
+        tid = self.extended_piece_to_id.get(token, self.get_piece_to_id_dict().get(token))
+        return tid
+
+
     # Encode string with added, unspecial tokens
 
     def encode_unspecial(self, text: str) -> list[int]:
 
         if not self.unspecial_piece_to_id:
             return self.tokenizer_model.encode(text)
 
@@ -550,15 +567,26 @@
             i += 1
 
         return self.id_to_ord
 
 
     # Copy vocabulary from model
 
-    def get_id_to_piece_list(self):
+    def get_id_to_piece_list(self, include_special_tokens = False):
+
+        if include_special_tokens:
+            if self.id_to_piece_with_special is not None: return self.id_to_piece_with_special
+
+            id_to_piece_extended = self.get_id_to_piece_list().copy()
+            for k, v in self.extended_id_to_piece.items():
+                id_to_piece_extended[k] = v
+
+            self.id_to_piece_with_special = id_to_piece_extended
+            return self.id_to_piece_with_special
+
 
         if self.id_to_piece is not None: return self.id_to_piece
         id_to_ord = self.get_id_to_ord_list()
 
         self.id_to_piece = [""] * self.tokenizer_model.vocab_size()
         for idx, p in self.tokenizer_model.enumerate_tokens():
             # if id_to_ord[idx] != -1:
```

### Comparing `exl2conv-0.0.19/exl2conv/util.py` & `exl2conv-0.0.20/exl2conv/util.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/exl2conv.egg-info/SOURCES.txt` & `exl2conv-0.0.20/exl2conv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.19/setup.py` & `exl2conv-0.0.20/setup.py`

 * *Files identical despite different names*

