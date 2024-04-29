# Comparing `tmp/paibox-1.0.0b1.tar.gz` & `tmp/paibox-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paibox-1.0.0b1.tar", max compression
+gzip compressed data, was "paibox-1.0.0rc1.tar", max compression
```

## Comparing `paibox-1.0.0b1.tar` & `paibox-1.0.0rc1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0     1065 2024-04-03 02:23:11.626351 paibox-1.0.0b1/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-04-03 02:23:11.626351 paibox-1.0.0b1/LICENSE
--rw-r--r--   0        0        0     1004 2024-04-03 02:23:11.626351 paibox-1.0.0b1/README.md
--rw-r--r--   0        0        0    26509 2024-04-03 02:23:11.626351 paibox-1.0.0b1/docs/Guide-of-PAIBox.md
--rw-r--r--   0        0        0     2352 2024-04-03 02:23:11.626351 paibox-1.0.0b1/docs/Guide-of-Test.md
--rw-r--r--   0        0        0    19453 2024-04-03 02:23:11.626351 paibox-1.0.0b1/docs/images/Guide-基础网络搭建-全连接网络示例.png
--rw-r--r--   0        0        0     1545 2024-04-03 02:23:11.630351 paibox-1.0.0b1/paibox/__init__.py
--rw-r--r--   0        0        0      131 2024-04-03 02:23:11.630351 paibox-1.0.0b1/paibox/backend/__init__.py
--rw-r--r--   0        0        0      394 2024-04-03 02:23:11.630351 paibox-1.0.0b1/paibox/backend/checker.py
--rw-r--r--   0        0        0    12743 2024-04-03 02:23:11.630351 paibox-1.0.0b1/paibox/backend/conf_template.py
--rw-r--r--   0        0        0     2079 2024-04-03 02:23:11.630351 paibox-1.0.0b1/paibox/backend/constrs.py
--rw-r--r--   0        0        0     1672 2024-04-03 02:23:11.630351 paibox-1.0.0b1/paibox/backend/context.py
--rw-r--r--   0        0        0    17822 2024-04-03 02:23:11.630351 paibox-1.0.0b1/paibox/backend/graphs.py
--rw-r--r--   0        0        0     1044 2024-04-03 02:23:11.630351 paibox-1.0.0b1/paibox/backend/graphs_types.py
--rw-r--r--   0        0        0    19027 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/backend/mapper.py
--rw-r--r--   0        0        0    23458 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/backend/placement.py
--rw-r--r--   0        0        0    18234 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/backend/routing.py
--rw-r--r--   0        0        0    11780 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/backend/segment_utils.py
--rw-r--r--   0        0        0    10082 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/base.py
--rw-r--r--   0        0        0     5192 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/collector.py
--rw-r--r--   0        0        0     1826 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/context.py
--rw-r--r--   0        0        0     1212 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/exceptions.py
--rw-r--r--   0        0        0     7015 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/mixin.py
--rw-r--r--   0        0        0     1116 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/naming.py
--rw-r--r--   0        0        0    10079 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/network.py
--rw-r--r--   0        0        0      316 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/neuron/__init__.py
--rw-r--r--   0        0        0    18461 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/neuron/base.py
--rw-r--r--   0        0        0     5469 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/neuron/neurons.py
--rw-r--r--   0        0        0      775 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/neuron/utils.py
--rw-r--r--   0        0        0      894 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/node.py
--rw-r--r--   0        0        0     5204 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/projection.py
--rw-r--r--   0        0        0      244 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/simulator/__init__.py
--rw-r--r--   0        0        0     3699 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/simulator/encoder.py
--rw-r--r--   0        0        0     1097 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/simulator/probe.py
--rw-r--r--   0        0        0     6794 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/simulator/simulator.py
--rw-r--r--   0        0        0      348 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/synapses/__init__.py
--rw-r--r--   0        0        0     8069 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/synapses/base.py
--rw-r--r--   0        0        0     7179 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/synapses/conv_utils.py
--rw-r--r--   0        0        0     4274 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/synapses/synapses.py
--rw-r--r--   0        0        0    11275 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/synapses/transforms.py
--rw-r--r--   0        0        0      400 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/tools.py
--rw-r--r--   0        0        0     2165 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/types.py
--rw-r--r--   0        0        0     5195 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/utils.py
--rw-r--r--   0        0        0     1936 2024-04-03 02:23:11.634351 paibox-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 paibox-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1218 2024-04-22 15:46:57.687398 paibox-1.0.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-04-22 15:46:57.687398 paibox-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     1005 2024-04-22 15:46:57.687398 paibox-1.0.0rc1/README.md
+-rw-r--r--   0        0        0    31292 2024-04-22 15:46:57.687398 paibox-1.0.0rc1/docs/Guide-of-PAIBox.md
+-rw-r--r--   0        0        0     2352 2024-04-22 15:46:57.687398 paibox-1.0.0rc1/docs/Guide-of-Test.md
+-rw-r--r--   0        0        0    19453 2024-04-22 15:46:57.687398 paibox-1.0.0rc1/docs/images/Guide-基础网络搭建-全连接网络示例.png
+-rw-r--r--   0        0        0     1659 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/__init__.py
+-rw-r--r--   0        0        0      131 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/__init__.py
+-rw-r--r--   0        0        0      394 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/checker.py
+-rw-r--r--   0        0        0    13672 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/conf_template.py
+-rw-r--r--   0        0        0     2079 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/constrs.py
+-rw-r--r--   0        0        0     1899 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/context.py
+-rw-r--r--   0        0        0    19312 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/graphs.py
+-rw-r--r--   0        0        0     1044 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/graphs_types.py
+-rw-r--r--   0        0        0    23915 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/mapper.py
+-rw-r--r--   0        0        0    25561 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/placement.py
+-rw-r--r--   0        0        0    19149 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/routing.py
+-rw-r--r--   0        0        0    11780 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/backend/segment_utils.py
+-rw-r--r--   0        0        0    10082 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/base.py
+-rw-r--r--   0        0        0     5192 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/collector.py
+-rw-r--r--   0        0        0     1826 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/context.py
+-rw-r--r--   0        0        0     1212 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/exceptions.py
+-rw-r--r--   0        0        0     7015 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/mixin.py
+-rw-r--r--   0        0        0     1116 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/naming.py
+-rw-r--r--   0        0        0    10079 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/network.py
+-rw-r--r--   0        0        0      316 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/neuron/__init__.py
+-rw-r--r--   0        0        0    18461 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/neuron/base.py
+-rw-r--r--   0        0        0     5469 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/neuron/neurons.py
+-rw-r--r--   0        0        0      775 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/neuron/utils.py
+-rw-r--r--   0        0        0      894 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/node.py
+-rw-r--r--   0        0        0     5202 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/projection.py
+-rw-r--r--   0        0        0      103 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/simulator/__init__.py
+-rw-r--r--   0        0        0     7733 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/simulator/encoder.py
+-rw-r--r--   0        0        0     1097 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/simulator/probe.py
+-rw-r--r--   0        0        0     6794 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/simulator/simulator.py
+-rw-r--r--   0        0        0     1571 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/simulator/utils.py
+-rw-r--r--   0        0        0      531 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/synapses/__init__.py
+-rw-r--r--   0        0        0    10565 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/synapses/base.py
+-rw-r--r--   0        0        0    18094 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/synapses/conv_utils.py
+-rw-r--r--   0        0        0     8643 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/synapses/synapses.py
+-rw-r--r--   0        0        0    13881 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/synapses/transforms.py
+-rw-r--r--   0        0        0      400 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/tools.py
+-rw-r--r--   0        0        0     2165 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/types.py
+-rw-r--r--   0        0        0     5195 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/paibox/utils.py
+-rw-r--r--   0        0        0     2077 2024-04-22 15:46:57.691398 paibox-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2371 1970-01-01 00:00:00.000000 paibox-1.0.0rc1/PKG-INFO
```

### Comparing `paibox-1.0.0b1/CHANGELOG.md` & `paibox-1.0.0rc1/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -23,13 +23,19 @@
 
 - 新增 `Always1Neuron` 神经元，该神经元将在工作期间持续输出1，不得单独存在，需存在前向突触与其连接。
 
 ## v1.0.0a7
 
 - 支持全展开1D卷积算子构建与部署（`padding` 不支持）
 
-## v1.0.0a8
+## v1.0.0b1
 
 - 提高 `numpy` 依赖版本至 `^1.24.0`
 - 修复神经元输入累加错误
 - 修复当权重为 `np.bool_` 且关闭权重精度优化选项( `weight_bit_optimization` )后，仍视为 `np.int8` 的错误
 - 支持混合精度权重的部署
+
+## v1.0.0rc1
+
+- 支持全展开1D/2D转置卷积算子。所有的卷积算子均支持 `padding`
+- 新增直接编码器
+- 修复后端的一些错误
```

### Comparing `paibox-1.0.0b1/LICENSE` & `paibox-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/README.md` & `paibox-1.0.0rc1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 </div>
 
 <p align="center">
     <a href="https://github.com/PAICookers/PAIBox/blob/master/pyproject.toml">
         <img src="https://img.shields.io/pypi/pyversions/paibox">
     </a>
-    <a href="https://github.com/PAICookers/PAIBox/releases/tag/v1.0.0b1">
+    <a href="https://github.com/PAICookers/PAIBox/releases/tag/v1.0.0rc1">
         <img src="https://img.shields.io/github/v/release/PAICookers/PAIBox?include_prereleases&color=orange">
     </a>
     <a href="https://www.codefactor.io/repository/github/PAICookers/PAIBox">
       <img src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIBox/master?color=red">
     </a>
     <a href="https://results.pre-commit.ci/latest/github/PAICookers/PAIBox/master">
 	   <img src="https://results.pre-commit.ci/badge/github/PAICookers/PAIBox/master.svg" alt="pre-commit.ci status">
```

### Comparing `paibox-1.0.0b1/docs/Guide-of-PAIBox.md` & `paibox-1.0.0rc1/docs/Guide-of-PAIBox.md`

 * *Files 16% similar despite different names*

```diff
@@ -252,56 +252,100 @@
 
 ##### MatConn 一般连接
 
 普通的神经元连接类型，仅可以通过矩阵设置其权重 `weights`。
 
 #### 1D卷积
 
-全展开形式1D卷积为全连接突触的一种特殊表达。对于卷积形式的突触，需**严格指定**前后神经元的尺寸、神经元维度顺序、卷积核权重、卷积核维度顺序与步长。
+全展开形式1D卷积为全连接突触的一种特殊表达。需**严格指定**输入神经元的尺寸与维度、卷积核权重、卷积核维度顺序与步长。对于输出神经元的具体尺寸不做严格要求。
 
 - `kernel`：卷积核权重。
 - `stride`：步长，标量。
-- `fm_order` 指定神经元维度顺序为 `CL` 或 `LC` 排列。
+- `padding`：填充，标量。
 - `kernel_order`：指定卷积核维度顺序为 `OIL` 或 `IOL` 排列。
+- 神经元维度顺序仅支持 `CL`。
 
 ```python
 n1 = pb.IF(shape=(8, 28), threshold=1)      # Input feature map: (8, 28)
 n2 = pb.IF(shape=(16, 26), threshold=1)     # Output feature map: (16, 26)
 kernel = np.random.randint(-128, 128, size=(16, 8, 3), dtype=np.int8) # OIl
 
-conv2d = pb.Conv1d(n1, n2, kernel=kernel, stride=1, fm_order="CL", kernel_order="OIL", name="conv1d_1")
+conv1d = pb.Conv1d(n1, n2, kernel=kernel, stride=1, padding=0, kernel_order="OIL", name="conv1d_1")
 ```
 
 #### 2D卷积
 
-全展开形式2D卷积为全连接突触的一种特殊表达。对于卷积形式的突触，需**严格指定**前后神经元的尺寸、神经元维度顺序、卷积核权重、卷积核维度顺序与步长。
+全展开形式2D卷积为全连接突触的一种特殊表达。需**严格指定**输入神经元的尺寸与维度、卷积核权重、卷积核维度顺序与步长。对于输出神经元的具体尺寸不做严格要求。
 
 - `kernel`：卷积核权重。
 - `stride`：步长，可以为标量或元组。当为标量时，对应为 `(x, x)`；当为元组时，则对应为 `(x, y)`。
-- `fm_order` 指定神经元维度顺序为 `CHW` 或 `HWC` 排列。
+- `padding`：填充，可以为标量或元组。当为标量时，对应为 `(x, x)`；当为元组时，则对应为 `(x, y)`。
 - `kernel_order`：指定卷积核维度顺序为 `OIHW` 或 `IOHW` 排列。
+- 神经元维度顺序仅支持 `CHW`。
 
 ```python
 n1 = pb.IF(shape=(8, 28, 28), threshold=1)      # Input feature map: (8, 28, 28)
 n2 = pb.IF(shape=(16, 26, 26), threshold=1)     # Output feature map: (16, 26, 26)
 kernel = np.random.randint(-128, 128, size=(16, 8, 3, 3), dtype=np.int8) # OIHW
 
-conv2d = pb.Conv2d(n1, n2, kernel=kernel, stride=1, fm_order="CHW", kernel_order="OIHW", name="conv2d_1")
+conv2d = pb.Conv2d(n1, n2, kernel=kernel, stride=(1, 2), padding=1, kernel_order="OIHW", name="conv2d_1")
 ```
 
-⚠️ `padding` 不支持，默认为0。
+#### 1D转置卷积
 
-### 编码器
+全展开形式1D转置卷积为全连接突触的一种特殊表达。需**严格指定**输入神经元的尺寸与维度、卷积核权重、卷积核维度顺序与步长。对于输出神经元的具体尺寸不做严格要求。
+
+对于 `Conv1d`：
+
+- `kernel`：卷积核权重。
+- `stride`：步长，标量。
+- `padding`：填充，标量。
+- `output_padding`：对输出特征图的一侧进行额外的填充，标量。
+- `kernel_order`：指定卷积核维度顺序为 `OIL` 或 `IOL` 排列。
+- 神经元维度顺序仅支持 `CL`。
+- 参数详细含义参见：[pytorch/ConvTranspose1d](https://pytorch.org/docs/stable/generated/torch.nn.ConvTranspose1d.html#torch.nn.ConvTranspose1d)
+
+```python
+n1 = pb.IF(shape=(8, 28), threshold=1)      # Input feature map: (8, 28)
+n2 = pb.IF(shape=(16, 26), threshold=1)     # Output feature map: (16, 26)
+kernel = np.random.randint(-128, 128, size=(16, 8, 3), dtype=np.int8) # OIl
+
+convt1d = pb.ConvTranspose1d(n1, n2, kernel=kernel, stride=1, padding=0, output_padding=1, kernel_order="OIL", name="convt1d_1")
+```
+
+#### 2D转置卷积
+
+全展开形式2D转置卷积为全连接突触的一种特殊表达。需**严格指定**输入神经元的尺寸与维度、卷积核权重、卷积核维度顺序与步长。对于输出神经元的具体尺寸不做严格要求。
+
+- `kernel`：卷积核权重。
+- `stride`：步长，可以为标量或元组。当为标量时，对应为 `(x, x)`；当为元组时，则对应为 `(x, y)`。
+- `padding`：填充，可以为标量或元组。当为标量时，对应为 `(x, x)`；当为元组时，则对应为 `(x, y)`。
+- `output_padding`：对输出特征图的一侧进行额外的填充，可以为标量或元组。当为标量时，对应为 `(x, x)`；当为元组时，则对应为 `(x, y)`。
+- `kernel_order`：指定卷积核维度顺序为 `OIHW` 或 `IOHW` 排列。
+- 神经元维度顺序仅支持 `CHW`。
+- 参数详细含义参见：[pytorch/ConvTranspose2d](https://pytorch.org/docs/stable/generated/torch.nn.ConvTranspose2d.html#torch.nn.ConvTranspose2d)
 
-对于非脉冲数据，我们需要将其进行脉冲编码，然后输入网络中进行计算。
+```python
+n1 = pb.IF(shape=(8, 28, 28), threshold=1)      # Input feature map: (8, 28, 28)
+n2 = pb.IF(shape=(16, 26, 26), threshold=1)     # Output feature map: (16, 26, 26)
+kernel = np.random.randint(-128, 128, size=(16, 8, 3, 3), dtype=np.int8) # OIHW
+
+convt2d = pb.ConvTranspose2d(n1, n2, kernel=kernel, stride=2, padding=1, output_padding=0, kernel_order="OIHW", name="convt2d_1")
+```
+
+### 编码器
 
 PAIBox提供了有状态与无状态编码器。其中，有状态编码器是指编码过程与时间有关，将输入数据编码到一段时间窗口内。而无状态编码器是指编码过程与时间无关，每个时间步，都可以根据输入数据进行编码。
 
+⚠️ 请注意，我们只提供较为简单的编码器，以便用户在不依赖外部库的条件下实现基本编码操作；如果需要更复杂的编码，请直接使用它们。
+
 #### 无状态编码器
 
+##### 泊松编码
+
 泊松编码是一种常用的无状态编码。以下为一个简单实例：
 
 ```python
 seed = 1
 rng = np.random.RandomState(seed=seed)
 x = rng.rand(10, 10).astype(np.float32)
 pe = pb.simulator.PoissonEncoder(seed=seed)
@@ -309,14 +353,52 @@
 
 for t in range(20):
     out_spike[t] = pe(x)
 ```
 
 通过调用该编码器，将需编码数据传入，即可得到编码后结果。
 
+##### 直接编码
+
+直接编码使用2D卷积进行特征提取，经过LIF神经元进行编码 。`Conv2dEncoder` 使用示例如下：
+
+```python
+kernel = np.random.uniform(-1, 1, size=(1, 3, 3, 3)).astype(np.float32) # OIHW
+stride = (1, 1)
+padding = (1, 1)
+de = pb.simulator.Conv2dEncoder(
+    kernel,
+    stride,
+    padding,
+    "OIHW",
+    tau=2,
+    decay_input=True,
+    v_threshold=1,
+    v_reset=0.2,
+)
+x = np.random.uniform(-1, 1, size=(3, 28, 28)).astype(np.float32) # CHW
+
+for t in range(20):
+    out_spike = de(x)
+```
+
+其中，
+
+- `kernel`：卷积核权重。
+- `stride`：步长，可以为标量或元组。当为标量时，对应为 `(x, x)`；当为元组时，则对应为 `(x, y)`。
+- `padding`：对输入进行填充，可以为标量或元组。当为标量时，对应为 `(x, x)`；当为元组时，则对应为 `(x, y)`。
+- `kernel_order`：指定卷积核维度顺序为 `OIHW` 或 `IOHW` 排列。
+- `tau`：膜电位时间常数。
+- `decay_input`：输入是否也会参与衰减。
+- `v_threshold`：阈值电平。
+- `v_reset`：复位电平。
+- 待编码数据维度顺序仅支持 `CHW`。
+
+其中，所使用的LIF为SpikingJelly内的 `SimpleLIFNode`。具体原理参见：[SpikingJelly/SimpleLIFNode](https://spikingjelly.readthedocs.io/zh-cn/latest/sub_module/spikingjelly.activation_based.neuron.html#spikingjelly.activation_based.neuron.SimpleLIFNode)。如果需要使用更复杂的编码，请直接使用它们。
+
 #### 有状态编码器
 
 有状态编码器类别较多。PAIBox提供了几种有状态编码器：周期编码器 `PeriodicEncoder`、延迟编码器 `LatencyEncoder` 。
 
 ##### 周期编码器
 
 它以一段脉冲序列为输入，将其循环地在每一个时间步输出。以下为一个简单实例：
@@ -693,15 +775,15 @@
 
 例化 `Mapper`，传入所构建的网络模型，进行编译，最后导出帧即可。
 
 ```python
 mapper = pb.Mapper()
 mapper.build(fcnet)
 graph_info = mapper.compile(weight_bit_optimization=True, grouping_optim_target="both")
-mapper.export(write_to_file=True, fp="./debug/", format="npy", split_by_coordinate=False, local_chip_addr=(0, 0), export_core_params=False)
+mapper.export(write_to_file=True, fp="./debug/", format="bin", split_by_coordinate=False, local_chip_addr=(0, 0), export_core_params=False)
 
 # Clear all the results
 mapper.clear()
 ```
 
 其中，编译时有如下参数可指定：
 
@@ -725,24 +807,56 @@
 - `memebers`：中间层所在物理核的配置项字典。
 - `inherent_timestep`：网络模型的最长时间步。
 - `n_core_required`：网络模型需要的物理核数目。
 - `extras`：其他额外的网络信息字典，例如，编译后的网络名称。
 
 ### 后端配置项
 
-与后端相关的配置项由 `BACKEND_CONFIG` 统一保存与访问，例如上述**编译选项**、`build_directory`、`local_chip_addr` 等。常用的配置项有如下：
-
-```python
-BACKEND_CONFIG.local_chip_addr # 本地芯片坐标
->>> Coord(0, 0)
+与后端相关的配置项由 `BACKEND_CONFIG` 统一保存与访问，例如上述**编译选项**、`build_directory`、`local_chip_addr` 等。如下所示，对常用的配置项进行读取与修改：
 
-BACKEND_CONFIG.test_chip_addr # 测试芯片坐标（一般是FPGA）
->>> Coord(1, 0)
+1. 本地芯片地址 `local_chip_addr`
 
-# Set output directory
-BACKEND_CONFIG.output_dir = "./output"
-
-# Set cflag for enabling weight precision optimization
-set_cflag(enable_wp_opt=True, cflag="This is a cflag.")
-BACKEND_CONFIG.cflag
->>> {"enable_wp_opt": True, "cflag": "This is a cflag."}
-```
+   ```python
+   # Read
+   BACKEND_CONFIG.local_chip_addr
+   >>> Coord(0, 0)
+
+   # Modify
+   BACKEND_CONFIG.local_chip_addr = (1, 1)
+   ```
+
+2. 输出芯片地址（测试芯片地址） `output_chip_addr`
+
+   ```python
+   # Read
+   BACKEND_CONFIG.output_chip_addr
+   # or
+   BACKEND_CONFIG.test_chip_addr
+   >>> Coord(1, 0)
+
+   # Modify
+   BACKEND_CONFIG.output_chip_addr = (2, 0)
+   # or
+   BACKEND_CONFIG.test_chip_addr = (2, 0)
+   ```
+
+3. 编译后配置信息等文件输出目录路径 `output_dir`，默认为用户当前工作目录
+
+   ```python
+   # Read
+   BACKEND_CONFIG.output_dir
+   >>> Path.cwd() # Default is your current working directory
+
+   # Modify
+   BACKEND_CONFIG.output_dir = "path/to/myoutput"
+   ```
+
+4. 编译选项
+
+   ```python
+   # Set cflag for enabling weight precision optimization
+   set_cflag(enable_wp_opt=True, cflag="This is a cflag.")
+
+   # Read
+   BACKEND_CONFIG.cflag
+   >>> {"enable_wp_opt": True, "cflag": "This is a cflag."}
+   ```
```

### Comparing `paibox-1.0.0b1/docs/Guide-of-Test.md` & `paibox-1.0.0rc1/docs/Guide-of-Test.md`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/docs/images/Guide-基础网络搭建-全连接网络示例.png` & `paibox-1.0.0rc1/docs/images/Guide-基础网络搭建-全连接网络示例.png`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/paibox/__init__.py` & `paibox-1.0.0rc1/paibox/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from .node import NodeDict as NodeDict
 from .node import NodeList as NodeList
 from .projection import InputProj as InputProj
 from .simulator import Probe as Probe
 from .simulator import Simulator as Simulator
 from .synapses import Conv1d as Conv1d
 from .synapses import Conv2d as Conv2d
+from .synapses import ConvTranspose1d as ConvTranspose1d
+from .synapses import ConvTranspose2d as ConvTranspose2d
 from .synapses import FullConn as FullConn
 from .synapses import GeneralConnType as SynConnType
 from .synapses import NoDecay as NoDecay
 
 try:
     __version__ = version("paibox")
 except Exception:
```

### Comparing `paibox-1.0.0b1/paibox/backend/conf_template.py` & `paibox-1.0.0rc1/paibox/backend/conf_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import json
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
-from typing import Any, Dict, List, Literal, NamedTuple, TypedDict
+from typing import Any, ClassVar, Dict, List, Literal, NamedTuple, TypedDict
 
 import numpy as np
 from numpy.typing import NDArray
 from paicorelib import (
     LCN_EX,
     AxonCoord,
     Coord,
+    HwConfig,
     InputWidthFormat,
     MaxPoolingEnable,
     NeuronAttrs,
     NeuronDestInfo,
     ParamsReg,
 )
 from paicorelib import ReplicationId as RId
@@ -26,15 +27,14 @@
 from paicorelib.framelib import types
 from paicorelib.framelib.frame_gen import OfflineFrameGen
 from paicorelib.framelib.utils import np2bin, np2npy, np2txt
 from typing_extensions import NotRequired, TypeAlias
 
 from paibox.base import NeuDyn
 
-from .context import _BACKEND_CONTEXT
 from .graphs_types import NodeName
 
 # Prevent import errors caused by changes in type definitions in paicorelib.
 if hasattr(types, "FRAME_DTYPE"):
     FRAME_DTYPE = types.FRAME_DTYPE
 else:
     FRAME_DTYPE = np.uint64
@@ -151,26 +151,25 @@
         cls,
         neuron: NeuDyn,
         n_neuron: int,
         addr_ram: List[int],
         addr_offset: int,
         axon_coords: List[AxonCoord],
         dest_core_coords: List[Coord],
-        dest_chip_coord: Coord = _BACKEND_CONTEXT["output_chip_addr"],
+        dest_chip_coord: Coord,
     ):
         """Build the `NeuronConfig`.
 
         Args:
             - neuron: the target `NeuDyn`.
             - addr_ram: assigned RAM address of the target neuron.
             - addr_offset: offset of the RAM address.
             - axon_segs: the destination axon segments.
             - dest_core_coords: coordinates of the core of the destination axons.
-            - dest_chip_coord: coordinate of the chip of the destination axons. Default is \
-                `output_chip_addr` in the backend context.
+            - dest_chip_coord: coordinate of the chip of the destination axons.
         """
         attrs = NeuronAttrs.model_validate(neuron.export_params(), strict=True)
         dest_rid = get_replication_id(dest_core_coords)
 
         dest_info = NeuronDest(
             [coord.tick_relative for coord in axon_coords],
             [coord.addr_axon for coord in axon_coords],
@@ -250,14 +249,30 @@
 
         for var in self._extra_params:
             dict_[var] = getattr(self, var)
 
         return dict_
 
 
+class EmptyCorePlacementConfig(CorePlacementConfig):
+    _default_seed: ClassVar[int] = 0
+    _default_zero_wram: ClassVar[NDArray[np.uint64]] = np.zeros(
+        (HwConfig.ADDR_RAM_MAX, 18), dtype=np.uint64
+    )
+
+    @classmethod
+    def encapsulate(cls, core_config: CoreConfig):
+        return cls(
+            cls._default_seed,
+            cls._default_zero_wram,
+            ParamsReg.model_validate(core_config._asdict(), strict=True),
+            {},
+        )
+
+
 InputNodeInfo: TypeAlias = Dict[NodeName, NeuronDest]
 OutputDestInfo: TypeAlias = Dict[NodeName, Dict[int, NeuronDestInfo]]
 CorePlacementInfo: TypeAlias = Dict[Coord, CorePlacementConfig]
 
 
 class GraphInfo(TypedDict):
     """Information of compiled graph.
@@ -267,16 +282,16 @@
 
     input: InputNodeInfo
     output: OutputDestInfo
     members: CorePlacementInfo
     inherent_timestep: int
     n_core_required: int
     """The actual used cores."""
-    # n_core_occupied: int
-    # """The occupied cores, including used & wasted."""
+    n_core_occupied: int
+    """The occupied cores, including used & wasted."""
     extras: NotRequired[Dict[str, Any]]
 
 
 def gen_config_frames_by_coreconf(
     config_dict: Dict[Coord, CorePlacementConfig],
     target_chip_coord: Coord,
     write_to_file: bool,
@@ -288,15 +303,15 @@
 
     Args:
         - config_dict: the dictionary of configurations.
         - target_chip_coord: local chip coordinate.
         - write_to_file: whether to write frames to file.
         - fp: If `write_to_file` is `True`, specify the path.
         - split_by_coord: whether to split the generated frames file by the core coordinates.
-        - format: `txt`, `bin`, or `npy`. `bin` & `npy` are recommended.
+        - format: `txt`, `bin`, or `npy`.
     """
 
     def _write_to_f(name: str, array: FrameArrayType) -> None:
         nonlocal fp, format
 
         _fp = fp / (name + f".{format}")
         if format == "npy":
@@ -323,15 +338,15 @@
         config_frame_type2 = OfflineFrameGen.gen_config_frame2(
             target_chip_coord,
             core_coord,
             _default_rid,
             v.params_reg,
         )
 
-        # 3. Iterate all the neuron segments in the function inside
+        # 3. Iterate all the neuron segments inside the physical core.
         config_frame_type3 = []
         for neu_conf in v.neuron_configs.values():
             config_frame_type3.append(
                 OfflineFrameGen.gen_config_frame3(
                     target_chip_coord,
                     core_coord,
                     _default_rid,
@@ -340,53 +355,69 @@
                     neu_conf.neuron_attrs,
                     neu_conf.neuron_dest_info,
                     lcn_ex=v.params_reg.lcn_extension,
                     weight_precision=v.params_reg.weight_precision,
                 )
             )
 
-        frame3 = np.concatenate(
-            [f.value for f in config_frame_type3], dtype=FRAME_DTYPE
-        )
+        if config_frame_type3:
+            frame3 = np.concatenate(
+                [f.value for f in config_frame_type3], dtype=FRAME_DTYPE, casting="no"
+            )
+        else:
+            frame3 = np.asarray([], dtype=FRAME_DTYPE)
 
         # 4. Only one config frame type IV for each physical core.
         n_addr_write = v.params_reg.num_dendrite  # The number of address to write
-        config_frame_type4 = OfflineFrameGen.gen_config_frame4(
-            target_chip_coord,
-            core_coord,
-            _default_rid,
-            0,
-            18 * n_addr_write,
-            v.weight_ram[:n_addr_write],
-        )
+        if n_addr_write > 0:
+            config_frame_type4 = OfflineFrameGen.gen_config_frame4(
+                target_chip_coord,
+                core_coord,
+                _default_rid,
+                0,
+                18 * n_addr_write,
+                v.weight_ram[:n_addr_write],
+            )
+        else:
+            config_frame_type4 = None
 
         _debug_dict[core_coord] = {
             "config1": config_frame_type1,
             "config2": config_frame_type2,
             "config3": config_frame_type3,
             "config4": config_frame_type4,
         }
 
-        frame_arrays_on_core[core_coord] = np.concatenate(
-            [
-                config_frame_type1.value,
-                config_frame_type2.value,
-                frame3,
-                config_frame_type4.value,
-            ],
-            dtype=FRAME_DTYPE,
-        )
+        if config_frame_type4:
+            frame_arrays_on_core[core_coord] = np.concatenate(
+                [
+                    config_frame_type1.value,
+                    config_frame_type2.value,
+                    frame3,
+                    config_frame_type4.value,
+                ],
+                dtype=FRAME_DTYPE,
+                casting="no",
+            )
+        else:
+            frame_arrays_on_core[core_coord] = np.concatenate(
+                [config_frame_type1.value, config_frame_type2.value, frame3],
+                dtype=FRAME_DTYPE,
+                casting="no",
+            )
 
     if write_to_file:
         if split_by_coord:
             for core_coord, f in frame_arrays_on_core.items():
                 addr = core_coord.address
                 _write_to_f(f"config_core{addr}", f)
         else:
-            _f = np.concatenate(list(frame_arrays_on_core.values()), dtype=FRAME_DTYPE)
+            _f = np.concatenate(
+                list(frame_arrays_on_core.values()), dtype=FRAME_DTYPE, casting="no"
+            )
             _write_to_f(f"config_cores_all", _f)
 
     return frame_arrays_on_core
 
 
 class PAIConfigJsonEncoder(json.JSONEncoder):
     def default(self, o: Any) -> Any:
```

### Comparing `paibox-1.0.0b1/paibox/backend/constrs.py` & `paibox-1.0.0rc1/paibox/backend/constrs.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/paibox/backend/context.py` & `paibox-1.0.0rc1/paibox/backend/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,20 +26,28 @@
         return self["local_chip_addr"]
 
     @local_chip_addr.setter
     def local_chip_addr(self, addr: CoordLike) -> None:
         self["local_chip_addr"] = to_coord(addr)
 
     @property
-    def test_chip_addr(self) -> Coord:
+    def output_chip_addr(self) -> Coord:
         return self["output_chip_addr"]
 
+    @output_chip_addr.setter
+    def output_chip_addr(self, addr: CoordLike) -> None:
+        self["output_chip_addr"] = to_coord(addr)
+
+    @property
+    def test_chip_addr(self) -> Coord:
+        return self.output_chip_addr
+
     @test_chip_addr.setter
     def test_chip_addr(self, addr: CoordLike) -> None:
-        self["output_chip_addr"] = to_coord(addr)
+        self.output_chip_addr = to_coord(addr)
 
     @property
     def output_dir(self) -> Path:
         return self["build_directory"]
 
     @output_dir.setter
     def output_dir(self, p: Union[str, Path]) -> None:
```

### Comparing `paibox-1.0.0b1/paibox/backend/graphs.py` & `paibox-1.0.0rc1/paibox/backend/graphs.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,32 +188,36 @@
         else:
             return NodePosition.MEMBER
 
     def build_check(self) -> None:
         if not self.has_built:
             raise BuildError(f"the graph hasn't been built yet.")
 
-    def group_edges(self) -> List[FrozenSet[EdgeType]]:
+    def group_edges(self) -> Tuple[List[FrozenSet[EdgeType]], List[int]]:
         """Group all edges according to a certain rule.
 
-        Return: a list of set of grouped edges.
+        Return: a list of set of grouped edges and a list of routing groups id.
         """
         self.build_check()
 
+        rgid = 0  # routing group id
+        routing_groups_id: List[int] = []
         gathered: List[FrozenSet[EdgeType]] = []
         seen_edges: Set[EdgeType] = set()  # Check if all edges are traversed
 
         for node in self.ordered_nodes:
             """Process the predecessor nodes of nodes first, then process the successor nodes."""
             if self.degree_of_nodes[node].in_degree > 1:
                 edge_group = self._find_pred_edges(self.succ_dg, node)
                 # Get the edges traversed for the first time
                 comming_edges = edge_group.difference(seen_edges)
 
                 seen_edges.update(comming_edges)
+                routing_groups_id.append(rgid)
+                rgid += 1
                 gathered.append(frozenset(comming_edges))
 
             if self.degree_of_nodes[node].out_degree > 1:
                 """Consider the constraints to the nodes."""
                 succ_edges = [e.edge for e in self.succ_dg[node].values()]
                 succ_nodes = [self.nodes[n].node for n in self.succ_dg[node]]
 
@@ -221,41 +225,47 @@
                 idx_of_sg = GraphNodeConstrs.tick_wait_attr_constr(succ_nodes)
 
                 if len(idx_of_sg) > 0:
                     for idx in idx_of_sg:
                         succ_edges_sg = frozenset([succ_edges[i] for i in idx])
                         if succ_edges_sg not in gathered:
                             seen_edges.update(succ_edges_sg)
+                            routing_groups_id.append(rgid)
                             gathered.append(succ_edges_sg)
                         else:
                             # FIXME Will this happen?
                             raise NotSupportedError
                 else:
                     succ_edges_sg = frozenset(succ_edges)
                     if succ_edges_sg not in gathered:
                         seen_edges.update(succ_edges_sg)
+                        routing_groups_id.append(rgid)
                         gathered.append(succ_edges_sg)
                     else:
                         # FIXME Will this happen?
                         raise NotSupportedError
 
+                rgid += 1
+
             elif self.degree_of_nodes[node].out_degree == 1:
                 succ_node = list(self.succ_dg[node].keys())[0]
                 # Check the in-degree of the only following node.
                 if self.degree_of_nodes[succ_node].in_degree == 1:
                     gathered.append(frozenset({self.succ_dg[node][succ_node].edge}))
+                    routing_groups_id.append(rgid)
+                    rgid += 1
                 else:
                     # This edge is waiting to be processed when
                     # traversing the following node `succ_node`.
                     pass
             else:
                 # out-degree = 0, do nothing.
                 continue
 
-        return gathered
+        return gathered, routing_groups_id
 
     @staticmethod
     def _find_pred_edges(
         succ_edges: Dict[NodeName, Dict[NodeName, EdgeAttr]], target_node: NodeName
     ) -> Set[EdgeType]:
         pred = set()
 
@@ -283,41 +293,63 @@
 
 
 def _degree_check(
     degree_of_nodes: Mapping[_NT, NodeDegree], succ_dg: Mapping[_NT, Iterable[_NT]]
 ) -> None:
     """Filter out such network structure, which is currently not supported."""
     for node in filter(lambda node: degree_of_nodes[node].out_degree > 1, succ_dg):
-        if any(degree_of_nodes[succ_node].in_degree > 1 for succ_node in succ_dg[node]):
-            raise NotSupportedError(
-                "If out-degree of a node is greater than 1, the in-degree of its sucessors must be 1."
-            )
+        for succ_node in succ_dg[node]:
+            if degree_of_nodes[succ_node].in_degree > 1:
+                _node_repr = (
+                    succ_node.name if isinstance(succ_node, CoreBlock) else succ_node
+                )
+                raise NotSupportedError(
+                    f"If out-degree of a node is greater than 1, the in-degree of its sucessors must be 1. "
+                    f"However, in-degree of {_node_repr} is {degree_of_nodes[succ_node].in_degree}."
+                )
 
 
 def convert2routing_groups(
     succ_dg_of_cb: Dict[CoreBlock, List[CoreBlock]],
     degrees_of_cb: Dict[CoreBlock, NodeDegree],
+    input_core_blocks: Dict[SourceNodeType, List[CoreBlock]],
 ) -> List[RoutingGroup]:
     ordered_core_blocks = toposort(succ_dg_of_cb)
     seen_cb = set()
     routing_groups = []
+    succ_cb_gid_dict = defaultdict(list)
 
     _degree_check(degrees_of_cb, succ_dg_of_cb)
 
+    # After that, all input core blocks have been traversed.
+    for input_cbs in input_core_blocks.values():
+        seen_cb.update(input_cbs)
+        routing_groups.append(RoutingGroup(*input_cbs))
+
     for cb in ordered_core_blocks:
-        # Check whether it has been traversed
+        # Check whether the core block has been traversed. This judgment condition is for
+        # core blocks with out-degree = 1 & output core blocks (out-degree = 0).
         if cb not in seen_cb:
             seen_cb.add(cb)
             routing_groups.append(RoutingGroup(cb))
 
-        # If the out-degree > 1, treat the following core blocks as one routing group.
+        # If out-degree > 1, group successor core blocks according to their routing id.
         if degrees_of_cb[cb].out_degree > 1:
             succ_cbs = succ_dg_of_cb[cb]
             seen_cb.update(succ_cbs)
-            routing_groups.append(RoutingGroup(*succ_cbs))
+
+            succ_cb_gid_dict.clear()
+            for succ_cb in succ_cbs:
+                if succ_cb._routing_id in succ_cb_gid_dict:
+                    succ_cb_gid_dict[succ_cb._routing_id].append(succ_cb)
+                else:
+                    succ_cb_gid_dict[succ_cb._routing_id] = [succ_cb]
+
+            for succ_cb in succ_cb_gid_dict.values():
+                routing_groups.append(RoutingGroup(*succ_cb))
 
     return routing_groups
 
 
 def toposort(directed_edges: Mapping[_NT, Iterable[_NT]]) -> List[_NT]:
     """
     Topological sort algorithm by Kahn [1]_.
```

### Comparing `paibox-1.0.0b1/paibox/backend/graphs_types.py` & `paibox-1.0.0rc1/paibox/backend/graphs_types.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/paibox/backend/mapper.py` & `paibox-1.0.0rc1/paibox/backend/mapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 from collections import defaultdict
 from copy import copy
 from pathlib import Path
 from typing import Any, Dict, List, Literal, Optional, Union
 
 from paicorelib import (
     Coord,
@@ -26,15 +27,15 @@
     export_core_params_json,
     export_inp_nodes_conf_json,
     export_outp_dests_conf_json,
     gen_config_frames_by_coreconf,
 )
 from .context import _BACKEND_CONTEXT, set_cflag
 from .graphs import PAIGraph, convert2routing_groups, get_node_degrees
-from .graphs_types import NodeDegree
+from .graphs_types import NodeDegree, SourceNodeType
 from .placement import CoreBlock, aligned_coords, max_lcn_of_cb
 from .routing import RoutingGroup, RoutingRoot
 
 __all__ = ["Mapper"]
 
 
 class Mapper:
@@ -46,53 +47,48 @@
 
     routing_tree = RoutingRoot(tag="L5")
     """The routing tree root."""
     graph = PAIGraph()
 
     def __init__(self) -> None:
         self.core_blocks: List[CoreBlock] = []
-        """A list for core blocks in topological order."""
-
+        """List for core blocks in the network."""
         self.succ_core_blocks: Dict[CoreBlock, List[CoreBlock]] = defaultdict(list)
-        """Grouped post-synapses of nodes. Structure:
-        {
-            node1.name: {
-                post-node1.name: grouped post-syn1,
-                post-node2.name: grouped post-syn2
-            }
-        }
-        """
-        self.degrees_of_cb: Dict[CoreBlock, NodeDegree] = defaultdict(NodeDegree)
+        self.input_core_blocks: Dict[SourceNodeType, List[CoreBlock]] = defaultdict(
+            list
+        )
+        """List of input core blocks for each input node."""
 
-        self.core_params: Dict[Coord, CoreConfig] = dict()
-        """The dictionary of core parameters. Structure:
-        {
-            address of core: {
-                parameters...
-            }
-        }
-        """
+        self.degrees_of_cb: Dict[CoreBlock, NodeDegree] = defaultdict(NodeDegree)
         self.routing_groups: List[RoutingGroup] = []
 
         self.core_plm_config: CorePlacementInfo = dict()
+        self.core_params: Dict[Coord, CoreConfig] = dict()
+        """The dictionary of core parameters."""
+
         self.graph_info: GraphInfo
         self.n_core_required = 0
+        self.n_core_occupied = 0
 
         self.clear()
 
     def clear(self) -> None:
         self.routing_tree.clear()
         self.graph.clear()
 
         self.core_blocks.clear()
         self.succ_core_blocks.clear()
+        self.input_core_blocks.clear()
 
         self.core_params.clear()
         self.core_plm_config.clear()
 
+        self.n_core_required = 0
+        self.n_core_occupied = 0
+
         # Set default cflags
         _BACKEND_CONTEXT.cflags.clear()
         set_cflag(enable_wp_opt=True)
         set_cflag(grouping_optim_target="both")
 
     def build(
         self,
@@ -162,32 +158,62 @@
         return self.config_export()
 
     def build_core_blocks(self) -> None:
         """Build core blocks based on grouped edges.
 
         Description: Group all edges & build `CoreBlock` based on the grouped edges.
         """
-        grouped_edges = self.graph.group_edges()
+        grouped_edges, routing_groups_id = self.graph.group_edges()
+
+        if sys.version_info >= (3, 10):
+            for syns, routing_id in zip(grouped_edges, routing_groups_id, strict=True):
+                self.core_blocks.append(
+                    CoreBlock.build(*syns, seed=0, routing_id=routing_id)
+                )
+        else:
+            if len(grouped_edges) != len(routing_groups_id):
+                raise ValueError(
+                    f"the length of grouped edges & routing groups id are not equal, "
+                    f"{len(grouped_edges)} != {len(routing_groups_id)}"
+                )
 
-        for syns in grouped_edges:
-            self.core_blocks.append(CoreBlock.build(*syns, seed=0))
+            for syns, routing_id in zip(grouped_edges, routing_groups_id):
+                self.core_blocks.append(CoreBlock.build(*syns, routing_id=routing_id))
 
         for cb in self.core_blocks:
             succ_cbs = list(
                 filter(
                     lambda succ_cb: any(d for d in cb.dest if d in succ_cb.source),
                     self.core_blocks,
                 )
             )
             self.succ_core_blocks[cb].extend(succ_cbs)
 
+        for inode in self.graph.inodes.values():
+            # TODO How to prevent this situation: there is input node & predecessor nodes
+            # in a certain core blocks.
+
+            # Disconnected input nodes will not be recorded.
+            succ_cb = [cb for cb in self.core_blocks if inode in cb.source]
+            if len(succ_cb) > 0:
+                self.input_core_blocks[inode] = succ_cb
+
         self.degrees_of_cb = get_node_degrees(self.succ_core_blocks)
 
     def lcn_ex_adjustment(self) -> None:
         """Adjust the LCN extension of each core block."""
+        # In the absence of the above complex situations, the following judgment is useless.
+        # But it'd be better to add this lcn adjustment.
+        for input_cbs in self.input_core_blocks.values():
+            if len(input_cbs) > 1:
+                max_lcn_ex = max_lcn_of_cb(input_cbs)
+                # Adjust the `lcn_ex` of the input core blocks for each input node
+                for g in input_cbs:
+                    g.lcn_ex = max_lcn_ex
+
         for cb in self.core_blocks:
             succ_cb = self.succ_core_blocks[cb]
 
             if len(succ_cb) > 1:
                 max_lcn_ex = max_lcn_of_cb(succ_cb)
                 # Adjust the `lcn_ex` of the following core blocks
                 for g in succ_cb:
@@ -212,42 +238,50 @@
         """
         for cb in self.core_blocks:
             # Group the neurons, get the #N of cores required.
             cb.group_neurons(
                 optim_target=_BACKEND_CONTEXT.cflags["grouping_optim_target"]
             )
 
-        # Calculate the consumption of physical cores required.
+        # Calculate the consumption of required physical cores.
         if (
             n_core_required := sum(cb.n_core_required for cb in self.core_blocks)
         ) > HwConfig.N_CORE_OFFLINE:
             raise ResourceError(
                 f"the number of required cores is out of range {HwConfig.N_CORE_OFFLINE} ({n_core_required})."
             )
 
         self.n_core_required = n_core_required
 
         # Generate routing groups by given the list of core blocks.
         routing_groups = convert2routing_groups(
-            self.succ_core_blocks, self.degrees_of_cb
+            self.succ_core_blocks, self.degrees_of_cb, self.input_core_blocks
         )
         for rg in routing_groups:
             if not self.routing_tree.insert_routing_group(rg):
                 raise RuntimeError(
                     f"insert routing group {rg} into the routing tree failed."
                 )
 
         self.routing_groups = routing_groups
 
+        # Calculate the consumption of occupied physical cores.
+        if (
+            n_core_occupied := sum(rg.get_n_core_occupied() for rg in routing_groups)
+        ) > HwConfig.N_CORE_OFFLINE:
+            raise ResourceError(
+                f"the number of occupied cores is out of range {HwConfig.N_CORE_OFFLINE} ({n_core_occupied})."
+            )
+
+        self.n_core_occupied = n_core_occupied
+
     def core_allocation(self) -> None:
-        """Allocate the core blocks to the physical cores. \
-            The order of `core_plms` is the same as `core_blocks`.
-        """
-        for cb in self.core_blocks:
-            cb.core_plm_alloc()
+        """Allocate the routing groups to core placements level."""
+        for rg in self.routing_groups:
+            rg.core_block_alloc()
 
     def config_export(self) -> GraphInfo:
         """Export parameters of cores & neurons inside.
 
         Steps:
             - 1. Export the parameters(PARAMETER_REG, including RANDOM_SEED \
                 & Weight RAM) of cores.
@@ -258,15 +292,15 @@
 
         _graph_info = GraphInfo(
             input=input_nodes_info,
             output=output_dest_info,
             members=self.core_plm_config,  # The configuration of physical cores is in `core_plm_config`
             inherent_timestep=self.graph.inherent_timestep,
             n_core_required=self.n_core_required,
-            # n_core_occupied=self.n_core_occupied,
+            n_core_occupied=self.n_core_occupied,
             extras={"name": self.graph.graph_name_repr},
         )
 
         self.graph_info = _graph_info
 
         return _graph_info
 
@@ -289,56 +323,54 @@
                 "addr_axon": [...]
             },
             "inp2_1": {...} # as input node #2
         }
         """
         input_nodes_info = dict()
 
-        # Traverse input core blocks where input nodes are
-        for input_cb in filter(
-            lambda cb: any(s for s in cb.source if s in self.graph.inodes.values()),
-            self.core_blocks,
-        ):
-            dest_coords = input_cb.core_coords
+        # Traverse input core blocks
+        for inode, input_cbs in self.input_core_blocks.items():
+            dest_coords: List[Coord] = []
+            for cb in input_cbs:  # Do not use iterative generation.
+                dest_coords.extend(cb.core_coords)
+
             dest_rid = get_replication_id(dest_coords)
 
-            # Traverse input nodes in the input core block only, in case that
-            # "other source nodes" are grouped with the input nodes.
-            for inode in filter(
-                lambda s: s in self.graph.inodes.values(), input_cb.source
-            ):
-                axon_coords = aligned_coords(
-                    slice(0, input_cb.n_axon_of(input_cb.source.index(inode)), 1),
-                    input_cb.axon_segments[inode],
-                    1,
-                    input_cb.n_timeslot,
-                )
+            # The arrangement of axons is the same for the rest of `input_cbs`.
+            # LCN of `input_cbs` are the same.
+            input_cb = input_cbs[0]
+            axon_coords = aligned_coords(
+                slice(0, input_cb.n_axon_of(input_cb.source.index(inode)), 1),
+                input_cb.axon_segments[inode],
+                1,
+                input_cb.n_timeslot,
+            )
 
-                neuron_dest = NeuronDest(
-                    [coord.tick_relative for coord in axon_coords],
-                    [coord.addr_axon for coord in axon_coords],
-                    dest_coords[0].x,
-                    dest_coords[0].y,
-                    dest_rid.x,
-                    dest_rid.y,
-                    _BACKEND_CONTEXT["local_chip_addr"].x,
-                    _BACKEND_CONTEXT["local_chip_addr"].y,
-                )
+            neuron_dest = NeuronDest(
+                [coord.tick_relative for coord in axon_coords],
+                [coord.addr_axon for coord in axon_coords],
+                dest_coords[0].x,
+                dest_coords[0].y,
+                dest_rid.x,
+                dest_rid.y,
+                _BACKEND_CONTEXT["local_chip_addr"].x,
+                _BACKEND_CONTEXT["local_chip_addr"].y,
+            )
 
-                input_nodes_info[inode.name] = neuron_dest
+            input_nodes_info[inode.name] = neuron_dest
 
         return input_nodes_info
 
     def _member_cb_and_onode_config_export(self) -> OutputDestInfo:
-        """Export the configuration of member core blocks & output destinations.
+        """Export configuration & output destinations inormation for core blocks.
 
         Description:
             Traverse core placements in core blocks, find the following core    \
             blocks where the axons at. Get the coordinate of the core placement \
-            & coordinates of axons(for broadcasting).
+            & coordinates of axons(for multicasting).
 
         Json exchange file format for output nodes:
         {
             "n3": { # as output node #1 & required two physical cores
                 "4": { # as output core #1 of node #1
                     "tick_relative": [0, 0, 0, 0, 0],
                     "addr_axon": [0, 1, 2, 3, 4, 5],
@@ -354,53 +386,128 @@
             "n4": {...} # as output node #2
         }
         """
         output_dest_info = defaultdict(dict)
         # Shallow copy
         ocoord = copy(_BACKEND_CONTEXT["output_core_addr_start"])
 
-        for member_cb in self.core_blocks:
-            self.core_params.update(
-                CoreBlock.export_core_plm_config(member_cb)
-            )  # compatible for py3.8
-
-            output_axon_offset = 0
-            for core_plm in member_cb.core_placements.values():
-                for neu_seg in core_plm.neu_segs_of_cplm:
-                    # Find the axon destinations
-                    dest_cb = [
-                        cb for cb in self.core_blocks if neu_seg.parent in cb.source
-                    ]
-
-                    # FIXME It is necessary to ensure that when there are both output nodes
-                    # & member nodes in the same `CoreBlock`, they need to be allocated on
-                    # different physical cores, otherwise routing problem will occur.
-                    if dest_cb:  # `neu_seg` is memeber neurons
-                        # Should not happen
-                        assert _cb_routable(self.routing_groups, dest_cb)
-                        core_plm.export_neu_config(neu_seg, dest_cb)
-                    else:
-                        # `neu_seg` is output neurons. Every neuron segment is a output node.
-                        # Update the offset of axon
-                        output_axon_offset = core_plm.export_neu_config(
-                            neu_seg,
-                            output_core_coord=ocoord,
-                            axon_addr_offset=output_axon_offset,
-                        )
-                        output_dest_info[neu_seg.parent.name][
-                            core_plm.coord.address
-                        ] = core_plm.neu_configs[neu_seg.parent].neuron_dest_info
+        for rg in self.routing_groups:
+            for member_cb in rg:
+                self.core_params.update(
+                    CoreBlock.export_core_plm_config(member_cb)
+                )  # compatible for py3.8
+
+                if self.degrees_of_cb[member_cb].out_degree == 0:
+                    # member_cb is a pure output core block. All neu_segs inside are output neurons.
+                    ocoord = self._onode_cb_config_export(
+                        member_cb, output_dest_info, ocoord
+                    )
+                elif any(d in self.graph.onodes.values() for d in member_cb.dest):
+                    # member_cb is both a member & output core block.
+                    ocoord = self._member_onode_cb_config_export(
+                        member_cb, output_dest_info, ocoord
+                    )
+                else:
+                    # member_cb is a pure member.
+                    self._member_cb_config_export(member_cb)
 
-                        # Coord.x += 1 for the destination of the next output node
-                        ocoord += CoordOffset(1, 0)
+                for coord, core_plm in member_cb.core_placements.items():
+                    self.core_plm_config[coord] = core_plm.export_core_plm_config()
 
-                self.core_plm_config[core_plm.coord] = core_plm.export_core_plm_config()
+            # Generate default configurations for wasted core placements of the routing group
+            self.core_plm_config.update(rg.get_wasted_cplm_config())
 
         return output_dest_info
 
+    def _member_cb_config_export(self, member_cb: CoreBlock) -> None:
+        """Export configuration information for core blocks that are pure members."""
+        succ_cbs = self.succ_core_blocks[member_cb]
+
+        for core_plm in member_cb.core_placements.values():
+            for neu_seg in core_plm.neu_segs_of_cplm:
+                # Find the axon destinations of neu_seg, not the successor core blocks.
+                dest_cb_of_nseg = [cb for cb in succ_cbs if neu_seg.parent in cb.source]
+
+                assert _cb_routable(self.routing_groups, dest_cb_of_nseg)
+                core_plm.export_neu_config(neu_seg, dest_cb_of_nseg)
+
+    def _member_onode_cb_config_export(
+        self,
+        member_onode_cb: CoreBlock,
+        output_dest_info: OutputDestInfo,
+        ocoord: Coord,
+    ) -> Coord:
+        """Export configuration information for core blocks that are both members & output."""
+        cur_ocoord = ocoord
+        output_axon_offset = 0
+        o_nodes = [d for d in member_onode_cb.dest if d in self.graph.onodes.values()]
+        succ_cbs = self.succ_core_blocks[member_onode_cb]
+
+        for core_plm in member_onode_cb.core_placements.values():
+            for neu_seg in core_plm.neu_segs_of_cplm:
+                dest_cb_of_nseg = [cb for cb in succ_cbs if neu_seg.parent in cb.source]
+
+                if len(dest_cb_of_nseg) > 0:
+                    assert _cb_routable(self.routing_groups, dest_cb_of_nseg)
+                    core_plm.export_neu_config(neu_seg, dest_cb_of_nseg)
+                else:
+                    offset_idx = o_nodes.index(neu_seg.parent)
+
+                    if hasattr(CoordOffset, "from_offset"):
+                        # For paicorelib > 0.0.13
+                        raise NotImplementedError
+                    else:
+                        # For paicorelib <= 0.0.13
+                        cur_ocoord = ocoord + CoordOffset(
+                            offset_idx % 32, offset_idx // 32
+                        )
+
+                    output_axon_offset = core_plm.export_neu_config(
+                        neu_seg,
+                        output_core_coord=cur_ocoord,
+                        axon_addr_offset=output_axon_offset,
+                    )
+                    output_dest_info[neu_seg.parent.name][core_plm.coord.address] = (
+                        core_plm.neu_configs[neu_seg.parent].neuron_dest_info
+                    )
+
+        # Add the offset as the starting coordinate of the next output node
+        return cur_ocoord + CoordOffset(1, 0)
+
+    def _onode_cb_config_export(
+        self, onode_cb: CoreBlock, output_dest_info: OutputDestInfo, ocoord: Coord
+    ) -> Coord:
+        """Export configuration information for core blocks that are pure output."""
+        cur_ocoord = ocoord
+        output_axon_offset = 0
+        o_nodes = [d for d in onode_cb.dest if d in self.graph.onodes.values()]
+
+        for core_plm in onode_cb.core_placements.values():
+            for neu_seg in core_plm.neu_segs_of_cplm:
+                # Get the output coordinate of this neu_seg
+                offset_idx = o_nodes.index(neu_seg.parent)
+
+                if hasattr(CoordOffset, "from_offset"):
+                    # For paicorelib > 0.0.13
+                    raise NotImplementedError
+                else:
+                    # For paicorelib <= 0.0.13
+                    cur_ocoord = ocoord + CoordOffset(offset_idx % 32, offset_idx // 32)
+
+                output_axon_offset = core_plm.export_neu_config(
+                    neu_seg,
+                    output_core_coord=cur_ocoord,
+                    axon_addr_offset=output_axon_offset,
+                )
+                output_dest_info[neu_seg.parent.name][core_plm.coord.address] = (
+                    core_plm.neu_configs[neu_seg.parent].neuron_dest_info
+                )
+
+        return cur_ocoord
+
     def export(
         self,
         write_to_file: bool = True,
         *,
         fp: Optional[Union[str, Path]] = None,
         format: Literal["txt", "bin", "npy"] = "bin",
         split_by_coordinate: bool = False,
@@ -408,19 +515,18 @@
         export_core_params: bool = False,
     ) -> Dict[Coord, Any]:
         """Generate configuration frames & export to file.
 
         Args:
             - write_to_file: whether to write frames into file.
             - fp: If `write_to_file` is `True`, specify the output path.
-            - format: `txt`, `bin`, or `npy`.`bin` & `npy` are recommended.
-            - split_by_coordinate: whether to split the generated frames file by the    \
-                core coordinates.
-            - local_chip_addr: the address of the local chip. If not specified, the     \
-                default value in `_BACKEND_CONTEXT` will be used.
+            - format: `txt`, `bin`, or `npy`. `bin` is recommended.
+            - split_by_coordinate: whether to split the generated frames file by the core coordinates.
+            - local_chip_addr: the address of the local chip. If not specified, the default value in    \
+                `_BACKEND_CONTEXT` will be used.
             - export_core_params: whether to export the parameters of occupied cores.
 
         Return: a dictionary of configurations.
         """
         if format not in ("bin", "npy", "txt"):
             raise ValueError(f"format {format} is not supported.")
```

### Comparing `paibox-1.0.0b1/paibox/backend/placement.py` & `paibox-1.0.0rc1/paibox/backend/placement.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,15 +27,20 @@
 
 from paibox.base import NeuDyn, PAIBoxObject
 from paibox.exceptions import BuildError, ResourceError, TruncationWarning
 from paibox.synapses import SynSys
 from paibox.types import WeightType
 from paibox.utils import check_attr_same, count_unique_elem
 
-from .conf_template import CoreConfig, CorePlacementConfig, NeuronConfig
+from .conf_template import (
+    CoreConfig,
+    CorePlacementConfig,
+    EmptyCorePlacementConfig,
+    NeuronConfig,
+)
 from .context import _BACKEND_CONTEXT
 from .graphs_types import DestNodeType, SourceNodeType
 from .segment_utils import (
     NeuSeg,
     NeuSegOfCoreBlock,
     NeuSegOfCorePlm,
     aligned_coords,
@@ -52,26 +57,30 @@
 
 
 class CoreBlock(CoreAbstract):
     """Core Block for `MODE_SNN` ONLY."""
 
     RUNTIME_MODE: ClassVar[CoreMode] = CoreMode.MODE_SNN
 
-    def __init__(self, *parents: SynSys, seed: int, name: Optional[str] = None) -> None:
+    def __init__(
+        self, *parents: SynSys, routing_id: int, seed: int, name: Optional[str] = None
+    ) -> None:
         """Core blocks in SNN mode.
 
         Args:
             - parents: the parent synapses.
+            - routing_id: id of routing group.
             - seed: random seed. Default value is 0.
             - name: name of the core block. Optional.
         """
         super().__init__(name)
         self._parents = parents
         self._lcn_ex = self._n_axon2lcn_ex()
         self._wp = WP.WEIGHT_WIDTH_8BIT  # Default value
+        self._routing_id = routing_id
 
         self.seed = seed
         """Random seed, legal integer, no more than uint64."""
 
         self.target_lcn = LCN_EX.LCN_1X
         """The target(destination core block) LCN."""
 
@@ -112,17 +121,15 @@
     def core_plm_alloc(self) -> None:
         """Allocate `CoreBlock` to physical cores."""
         if not self.lcn_locked:
             raise BuildError("Allocate core placements after lcn_ex is locked.")
 
         for i, coord in enumerate(self.core_coords):
             # assert self.get_raw_weight_of_coord(i)[0].shape[0] == self.n_axon
-            self.core_placements[coord] = CorePlacement.build(
-                self, i, self.get_raw_weight_of_coord(i)
-            )
+            self.core_placements[coord] = CorePlacement.build(self, i)
 
     def _get_syn_of(self, src: SourceNodeType, dest: DestNodeType) -> Optional[SynSys]:
         for syn in self.obj:
             if syn.source == src and syn.dest == dest:
                 return syn
 
         return None
@@ -273,16 +280,16 @@
         )
 
     @property
     def n_neuron(self) -> int:
         return sum(d.num_in for d in self.dest)
 
     @property
-    def unroll_factor(self) -> List[int]:
-        return [d.unroll_factor for d in self.dest]
+    def unrolling_factor(self) -> List[int]:
+        return [d.unrolling_factor for d in self.dest]
 
     @property
     def n_neuron_of_plm(self) -> List[int]:
         """A list of the #N of neurons on each `CorePlacement`.
 
         FIXME Different in SNN/ANN RUNTIME_MODE.
         """
@@ -348,24 +355,24 @@
         return f"<{self.name} of target '{self.obj}'>"
 
     def _obj_repr(self) -> str:
         """The representation of the names of target objects."""
         return ", ".join(n.name for n in self.obj)
 
     @classmethod
-    def build(cls, *synapses: SynSys, seed: int = 0):
+    def build(cls, *synapses: SynSys, routing_id: int, seed: int = 0):
         """Group synapses & build `CoreBlock`."""
         # FIXME where does the parameter check do?
         if seed > (1 << 64) - 1:
             warnings.warn(
                 f"random seed {seed} is too large, truncated into 64 bits.",
                 TruncationWarning,
             )
 
-        return cls(*synapses, seed=seed)
+        return cls(*synapses, routing_id=routing_id, seed=seed)
 
     @classmethod
     def export_core_plm_config(cls, cb: "CoreBlock") -> Dict[Coord, CoreConfig]:
         """Export the parameters of the core into a dictionary."""
         cb_config = dict()
 
         for coord, core_plm in cb.core_placements.items():
@@ -384,15 +391,14 @@
     """SNN mode ONLY."""
 
     def __init__(
         self,
         parent: CoreBlock,
         routing_coord: Coord,
         n_neuron: int,
-        *,
         raw_weights: List[WeightType],
         neu_segs_of_cplm: NeuSegOfCorePlm,
         name: Optional[str] = None,
     ) -> None:
         """
         Arguments:
             - parent: the parent core block.
@@ -412,26 +418,21 @@
         self._weights_folded = self._fold_raw_weights(raw_weights)
         """The folded weights."""
 
         self.neu_segs_of_cplm = neu_segs_of_cplm
         self.neu_configs: Dict[NeuDyn, NeuronConfig] = dict()
 
     @classmethod
-    def build(cls, parent: CoreBlock, idx: int, raw_weights: List[WeightType]):
+    def build(cls, parent: CoreBlock, idx: int):
         coord = parent.core_coords[idx]
         n_neuron = parent.n_neuron_of_plm[idx]
         neu_segs_of_cplm = parent.neuron_segs_of_cb[idx]
+        raw_weights = parent.get_raw_weight_of_coord(idx)
 
-        return cls(
-            parent,
-            coord,
-            n_neuron,
-            raw_weights=raw_weights,
-            neu_segs_of_cplm=neu_segs_of_cplm,
-        )
+        return cls(parent, coord, n_neuron, raw_weights, neu_segs_of_cplm)
 
     def _fold_raw_weights(self, raw_weights: List[WeightType]) -> WeightType:
         """Fold the weights into LCN-sized blocks."""
         w_folded_list = []
         w_folded_of_axon_segs = []
         n_fold = self.n_timeslot
 
@@ -468,15 +469,15 @@
     def _weight_ram_mapping(self) -> WeightRamType:
         row, col = self._weights_folded.shape
         w_unpacked = np.zeros(self.WEIGHT_RAM_SHAPE, dtype=np.uint8)
 
         if self.n_weight_bits == 1:
             w_unpacked[:row, :col] = self._weights_folded
         else:
-            # [N*M] -> [M*N*1]
+            # (N, M) -> (M*N, 1)
             w_folded_3d = np.expand_dims(self._weights_folded.T, axis=2).astype(
                 np.uint8
             )
 
             for i in range(col):
                 # For every column, unpack the array [N*1] -> [N*n_weight_bits]
                 unpacked = np.unpackbits(
@@ -486,27 +487,28 @@
                     bitorder=HwConfig.WEIGHT_BITORDER,
                 )
 
                 w_unpacked[
                     :row, self.n_weight_bits * i : self.n_weight_bits * (i + 1)
                 ] = unpacked
 
-        assert np.max(w_unpacked, axis=None) <= 1
-        assert np.min(w_unpacked, axis=None) >= 0
+        assert np.max(w_unpacked, axis=None) <= np.uint8(1)
+        assert np.min(w_unpacked, axis=None) >= np.uint8(0)
 
         # Convert the unpacked weights into a mapping format,
         # corresponding to the RAM address, each address contains 18 uint64.
-        # [512 * 1152] -> [(512*18) * 64](uint8). Reshape to 64 columns to avoid contiguous problem.
+        # (1152, 512) -> (512, 1152) -> (512*18, 64)(uint8).
+        # Reshape to 64 columns to avoid contiguous problem.
         w_unpacked_T_rehaped = w_unpacked.T.reshape(-1, 64)
 
-        # [(512*18) * 64](uint8) -> [(512*18) * 8](uint8)
+        # (512*18, 64)(uint8) -> (512*18, 8)(uint8)
         w_packed_u8 = np.packbits(
             w_unpacked_T_rehaped, axis=1, bitorder=HwConfig.WEIGHT_BITORDER
         )
-        # [(512*18) * 8](uint8) -> [(512*18) * 1](uint64) -> [512 * 18](uint64)
+        # (512*18, 8)(uint8) -> (512*18, 1)(uint64) -> (512, 18)(uint64)
         w_packed_u64 = w_packed_u8.view(np.uint64).reshape(-1, 18)
         w_packed_u64.setflags(write=False)
 
         return w_packed_u64
 
     @staticmethod
     def _nfold_weight(
@@ -607,15 +609,16 @@
             config = NeuronConfig.encapsulate(
                 neu_seg.parent,
                 neu_seg.n_neuron,
                 neu_seg.segment.addr_ram,
                 neu_seg.segment.addr_offset,
                 axon_coords,
                 dest_core_coords,
-                _BACKEND_CONTEXT["local_chip_addr"],  # Here is local chip coordinate
+                # local chip coordinate for member nodes
+                _BACKEND_CONTEXT["local_chip_addr"],
             )
 
             self.neu_configs[neu_seg.parent] = config
         else:
             assert isinstance(output_core_coord, Coord)
             assert isinstance(axon_addr_offset, int)
 
@@ -627,14 +630,16 @@
             config = NeuronConfig.encapsulate(
                 neu_seg.parent,
                 neu_seg.n_neuron,
                 neu_seg.segment.addr_ram,
                 neu_seg.segment.addr_offset,
                 axon_coords,
                 [output_core_coord],
+                # output chip coordinate for output node
+                _BACKEND_CONTEXT["output_chip_addr"],
             )
 
             self.neu_configs[neu_seg.parent] = config
 
             return axon_addr_offset + neu_seg.n_neuron
 
     def export_core_plm_config(self) -> CorePlacementConfig:
@@ -711,14 +716,65 @@
     def n_core_required(self):
         return 1
 
     def __len__(self) -> int:
         return self.n_core_required
 
 
+class EmptyCorePlacement(CoreAbstract):
+    """Empty core placement."""
+
+    _default_wp: ClassVar[WP] = WP.WEIGHT_WIDTH_1BIT
+    _default_lcn_ex: ClassVar[LCN_EX] = LCN_EX.LCN_1X
+    _default_n_dendrite: ClassVar[int] = 0
+    _default_tws: ClassVar[int] = 0
+    _default_twe: ClassVar[int] = 0
+    _default_target_lcn: ClassVar[LCN_EX] = LCN_EX.LCN_1X
+
+    def __init__(self, coord: Coord, name: Optional[str] = None) -> None:
+        super().__init__(name)
+        self.coord = coord
+
+    def export_param_config(self) -> CoreConfig:
+        _mode_params = CoreModeDict[CoreMode.MODE_SNN]
+        # fmt: off
+        cb_config = CoreConfig(
+            self.name,                          # name of the core
+            self._default_wp,                   # weight_precision
+            self._default_lcn_ex,               # lcn_extension
+            _mode_params[0],                    # input_width_format
+            _mode_params[1],                    # spike_width_format
+            self._default_n_dendrite,           # num_dendrite
+            MaxPoolingEnable.DISABLE,           # max_pooling_en
+            self._default_tws,                  # tick_wait_start
+            self._default_twe,                  # tick_wait_end
+            _mode_params[2],                    # snn_mode_en
+            self._default_target_lcn,           # target_lcn
+            _BACKEND_CONTEXT.test_chip_addr,    # test_chip_addr
+        )
+        # fmt: on
+        return cb_config
+
+    def export_core_plm_config(self) -> EmptyCorePlacementConfig:
+        core_param = self.export_param_config()
+        return EmptyCorePlacementConfig.encapsulate(core_param)
+
+    @classmethod
+    def build(cls, coord: Coord):
+        return cls(coord)
+
+    @property
+    def n_core_required(self):
+        return 1
+
+    @property
+    def shape(self) -> Tuple[int, int]:
+        return (0, 0)
+
+
 def max_lcn_of_cb(cb: List[CoreBlock]) -> LCN_EX:
     """Find the max LCN extenion of previous grouped synapses"""
     return max(cb, key=lambda cb: cb.lcn_ex).lcn_ex
 
 
 def _neuron_repl_prop(nbits: int, ntimeslot: int) -> int:
     """Get the proportion of neuron replication.
```

### Comparing `paibox-1.0.0b1/paibox/backend/routing.py` & `paibox-1.0.0rc1/paibox/backend/routing.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from paicorelib.routing_defs import RoutingDirection as Direction
 from paicorelib.routing_defs import RoutingLevel as Level
 from paicorelib.routing_defs import RoutingStatus as Status
 from paicorelib.routing_defs import get_routing_consumption
 
 from paibox.exceptions import NotSupportedError
 
-from .placement import CoreBlock, CorePlacement
+from .conf_template import CorePlacementInfo
+from .placement import CoreBlock, CorePlacement, EmptyCorePlacement
 
 __all__ = ["RoutingGroup", "RoutingRoot"]
 
 
 class RoutingCluster:
     def __init__(
         self,
@@ -413,46 +414,67 @@
 class RoutingGroup(List[CoreBlock]):
     """Core blocks located within a routing group are routable.
 
     NOTE: Axon groups within a routing group are the same.
     """
 
     def __init__(self, *cb: CoreBlock) -> None:
-        self.cb = list(cb)
-
+        self.core_blocks = list(cb)
         self.assigned_coords: List[Coord] = []
-        """Assigned core coordinates for the routing group."""
+        """Assigned core coordinates in the routing group"""
         self.wasted_coords: List[Coord] = []
-        """Wasted core coordinates for the routing group."""
+        """Wasted core coordinates in routing group"""
+        self.wasted_core_plm: Dict[Coord, EmptyCorePlacement] = {}
+        """Wasted core placements"""
 
     def assign(self, assigned: List[Coord], wasted: List[Coord]) -> None:
         self.assigned_coords = assigned
         self.wasted_coords = wasted
 
         # Assign the coordinates to each core block inside the routing group.
         cur_i = 0
         for cb in self:
             n = cb.n_core_required
             cb.core_coords = assigned[cur_i : cur_i + n]
             cur_i += n
 
+    def core_block_alloc(self) -> None:
+        for cb in self:
+            cb.core_plm_alloc()
+
+        # Allocate blank core placements for the wasted coordinates.
+        for coord in self.wasted_coords:
+            self.wasted_core_plm[coord] = EmptyCorePlacement.build(coord)
+
+    def get_wasted_cplm_config(self) -> CorePlacementInfo:
+        return {
+            coord: core_plm.export_core_plm_config()
+            for coord, core_plm in self.wasted_core_plm.items()
+        }
+
+    def get_n_core_occupied(self) -> int:
+        """Get the #N of cores occupied by the routing group."""
+        return len(self.assigned_coords) + len(self.wasted_coords)
+
     def __getitem__(self, idx: int) -> CoreBlock:
-        if idx >= len(self.cb) or idx < 0:
-            raise IndexError(f"index out of range [0, {len(self.cb)}) ({idx}).")
+        if idx >= len(self.core_blocks) or idx < 0:
+            raise IndexError(
+                f"index out of range [0, {len(self.core_blocks)}), ({idx})."
+            )
 
-        return self.cb[idx]
+        return self.core_blocks[idx]
 
     def __len__(self) -> int:
-        return len(self.cb)
+        return len(self.core_blocks)
 
     def __iter__(self) -> Iterator[CoreBlock]:
-        return self.cb.__iter__()
+        return self.core_blocks.__iter__()
 
     def __contains__(self, key: CoreBlock) -> bool:
-        return key in self.cb
+        return key in self.core_blocks
 
     @property
     def n_core_required(self) -> int:
         return sum(cb.n_core_required for cb in self)
 
     @property
     def routing_cost(self) -> RoutingCost:
```

### Comparing `paibox-1.0.0b1/paibox/backend/segment_utils.py` & `paibox-1.0.0rc1/paibox/backend/segment_utils.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/paibox/base.py` & `paibox-1.0.0rc1/paibox/base.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/paibox/collector.py` & `paibox-1.0.0rc1/paibox/collector.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/paibox/context.py` & `paibox-1.0.0rc1/paibox/context.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/paibox/exceptions.py` & `paibox-1.0.0rc1/paibox/exceptions.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/paibox/mixin.py` & `paibox-1.0.0rc1/paibox/mixin.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/paibox/naming.py` & `paibox-1.0.0rc1/paibox/naming.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/paibox/network.py` & `paibox-1.0.0rc1/paibox/network.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/paibox/neuron/base.py` & `paibox-1.0.0rc1/paibox/neuron/base.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/paibox/neuron/neurons.py` & `paibox-1.0.0rc1/paibox/neuron/neurons.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/paibox/neuron/utils.py` & `paibox-1.0.0rc1/paibox/neuron/utils.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/paibox/node.py` & `paibox-1.0.0rc1/paibox/node.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/paibox/projection.py` & `paibox-1.0.0rc1/paibox/projection.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         if isinstance(_spike, (int, np.bool_, np.integer)):
             self._inner_spike = np.full((self.num_out,), _spike, dtype=np.bool_)
         elif isinstance(_spike, np.ndarray):
             if shape2num(_spike.shape) != self.num_out:
                 raise ShapeError(
                     f"cannot reshape output value from {_spike.shape} to ({self.num_out},)."
                 )
-            self._inner_spike = _spike.flatten().astype(np.bool_)
+            self._inner_spike = _spike.ravel().astype(np.bool_)
         else:
             # should never be reached
             raise TypeError(
                 f"expected type int, np.bool_, np.integer or np.ndarray, "
                 f"but got {_spike}, type {type(_spike)}."
             )
```

### Comparing `paibox-1.0.0b1/paibox/simulator/probe.py` & `paibox-1.0.0rc1/paibox/simulator/probe.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/paibox/simulator/simulator.py` & `paibox-1.0.0rc1/paibox/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/paibox/synapses/base.py` & `paibox-1.0.0rc1/paibox/synapses/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 
 from paibox.base import NeuDyn, SynSys
 from paibox.exceptions import ShapeError
 from paibox.neuron import Neuron
 from paibox.projection import InputProj
 from paibox.types import DataArrayType, SynOutType, WeightType
 
-from .conv_utils import (
-    _fm_ndim1_check,
-    _fm_ndim2_check,
-    _KOrder3d,
-    _KOrder4d,
-    _Order2d,
-    _Order3d,
+from .conv_utils import _fm_ndim1_check, _fm_ndim2_check, _KOrder3d, _KOrder4d
+from .transforms import (
+    AllToAll,
+    Conv1dForward,
+    Conv2dForward,
+    ConvTranspose1dForward,
+    ConvTranspose2dForward,
 )
-from .transforms import AllToAll, Conv1dForward, Conv2dForward
 from .transforms import GeneralConnType as GConnType
 from .transforms import Identity, MaskedLinear, OneToOne, Transform
 
 RIGISTER_MASTER_KEY_FORMAT = "{0}.output"
 
 
 def _check_equal(num_in: int, num_out: int) -> int:
@@ -94,15 +93,15 @@
             else:
                 idx = self.dest.timestamp % HwConfig.N_TIMESLOT_MAX
                 synin = self.source.output[idx].copy() if spike is None else spike
         else:
             # Retrieve 0 to the dest neurons if it is not working
             synin = np.zeros_like(self.source.spike, dtype=np.bool_)
 
-        self._synout = self.comm(synin).astype(np.int32)
+        self._synout = self.comm(synin).ravel().astype(np.int32)
         return self._synout
 
     def reset_state(self, *args, **kwargs) -> None:
         # TODO Add other initialization methods in the future.
         self.reset_memory()  # Call reset of `StatusMemory`.
 
     def _set_comm(self, comm: Transform) -> None:
@@ -162,99 +161,172 @@
 
     def __init__(
         self,
         source: Union[NeuDyn, InputProj],
         dest: Neuron,
         kernel: np.ndarray,
         stride: Tuple[int],
-        # padding: Tuple[int],
-        fm_order: _Order2d,
+        padding: Tuple[int],
         order: _KOrder3d,
         name: Optional[str] = None,
     ) -> None:
         super().__init__(source, dest, name)
 
         if kernel.ndim != self._spatial_ndim + 2:
             raise ShapeError(
                 f"convolution kernel dimension must be {self._spatial_ndim + 2}, but got {kernel.ndim}."
             )
 
         if order == "IOL":
-            _kernel = kernel.transpose(1, 0, 2)
+            _kernel = np.swapaxes(kernel, 0, 1)
         else:
             _kernel = kernel.copy()
 
         # O,I,L
         out_channels, in_channels, kernel_l = _kernel.shape
-
         # C,L
-        in_ch, in_l = _fm_ndim1_check(source.shape_out, fm_order)
-        out_ch, out_l = _fm_ndim1_check(dest.shape_out, fm_order)
+        in_ch, in_l = _fm_ndim1_check(source.shape_out, "CL")
+        out_l = (in_l + 2 * padding[0] - kernel_l) // stride[0] + 1
 
         if in_ch != in_channels:
             raise ShapeError(f"input channels mismatch: {in_ch} != {in_channels}.")
 
-        if out_ch != out_channels:
-            raise ShapeError(f"output channels mismatch: {out_ch} != {out_channels}.")
-
-        # If padding is considered, the implementation of convolution unrolling
-        # is extremely complex, so fix it.
-        padding = (0,)
-
-        assert (in_l + 2 * padding[0] - kernel_l) // stride[0] + 1 == out_l
+        if (_output_size := out_channels * out_l) != dest.num_in:
+            raise ShapeError(f"Output size mismatch: {_output_size} != {dest.num_in}.")
 
-        comm = Conv1dForward((in_l,), (out_l,), _kernel, stride, padding, fm_order)
+        comm = Conv1dForward((in_l,), (out_l,), _kernel, stride, padding)
 
         self.comm = comm
 
 
 class Conv2dSyn(FullConnectedSyn):
     _spatial_ndim: ClassVar[int] = 2
 
     def __init__(
         self,
         source: Union[NeuDyn, InputProj],
         dest: Neuron,
         kernel: np.ndarray,
         stride: Tuple[int, int],
-        # padding: Tuple[int, int],
-        fm_order: _Order3d,
+        padding: Tuple[int, int],
         order: _KOrder4d,
         name: Optional[str] = None,
     ) -> None:
         super().__init__(source, dest, name)
 
         if kernel.ndim != self._spatial_ndim + 2:
             raise ShapeError(
                 f"convolution kernel dimension must be {self._spatial_ndim + 2}, but got {kernel.ndim}."
             )
 
         if order == "IOHW":
-            _kernel = kernel.transpose(1, 0, 2, 3)
+            _kernel = np.swapaxes(kernel, 0, 1)
         else:
             _kernel = kernel.copy()
 
         # O,I,H,W
         out_channels, in_channels, kernel_h, kernel_w = _kernel.shape
-
         # C,H,W
-        in_ch, in_h, in_w = _fm_ndim2_check(source.shape_out, fm_order)
-        out_ch, out_h, out_w = _fm_ndim2_check(dest.shape_out, fm_order)
+        in_ch, in_h, in_w = _fm_ndim2_check(source.shape_out, "CHW")
+        out_h = (in_h + 2 * padding[0] - kernel_h) // stride[0] + 1
+        out_w = (in_w + 2 * padding[1] - kernel_w) // stride[1] + 1
 
         if in_ch != in_channels:
             raise ShapeError(f"input channels mismatch: {in_ch} != {in_channels}.")
 
-        if out_ch != out_channels:
-            raise ShapeError(f"output channels mismatch: {out_ch} != {out_channels}.")
+        if (_output_size := out_channels * out_h * out_w) != dest.num_in:
+            raise ShapeError(f"Output size mismatch: {_output_size} != {dest.num_in}.")
+
+        comm = Conv2dForward((in_h, in_w), (out_h, out_w), _kernel, stride, padding)
+
+        self._set_comm(comm)
+
+
+class ConvTranspose1dSyn(FullConnectedSyn):
+    _spatial_ndim: ClassVar[int] = 1
+
+    def __init__(
+        self,
+        source: Union[NeuDyn, InputProj],
+        dest: Neuron,
+        kernel: np.ndarray,
+        stride: Tuple[int],
+        padding: Tuple[int],
+        output_padding: Tuple[int],
+        order: _KOrder3d,
+        name: Optional[str] = None,
+    ) -> None:
+        super().__init__(source, dest, name)
+
+        if kernel.ndim != self._spatial_ndim + 2:
+            raise ShapeError(
+                f"convolution kernel dimension must be {self._spatial_ndim + 2}, but got {kernel.ndim}."
+            )
+
+        if order == "IOL":
+            _kernel = np.swapaxes(kernel, 0, 1)
+        else:
+            _kernel = kernel.copy()
 
-        # If padding is considered, the implementation of convolution unrolling
-        # is extremely complex, so fix it.
-        padding = (0, 0)
+        # O,I,L
+        out_channels, in_channels, kernel_l = _kernel.shape
+        # C,L
+        in_ch, in_l = _fm_ndim1_check(source.shape_out, "CL")
+        out_l = (in_l - 1) * stride[0] - 2 * padding[0] + kernel_l + output_padding[0]
+
+        if in_ch != in_channels:
+            raise ShapeError(f"input channels mismatch: {in_ch} != {in_channels}.")
+
+        if (_output_size := out_channels * out_l) != dest.num_in:
+            raise ShapeError(f"Output size mismatch: {_output_size} != {dest.num_in}.")
+
+        comm = ConvTranspose1dForward(
+            (in_l,), (out_l,), _kernel, stride, padding, output_padding
+        )
+
+        self.comm = comm
+
+
+class ConvTranspose2dSyn(FullConnectedSyn):
+    _spatial_ndim: ClassVar[int] = 2
+
+    def __init__(
+        self,
+        source: Union[NeuDyn, InputProj],
+        dest: Neuron,
+        kernel: np.ndarray,
+        stride: Tuple[int, int],
+        padding: Tuple[int, int],
+        output_padding: Tuple[int, int],
+        order: _KOrder4d,
+        name: Optional[str] = None,
+    ) -> None:
+        super().__init__(source, dest, name)
+
+        if kernel.ndim != self._spatial_ndim + 2:
+            raise ShapeError(
+                f"convolution kernel dimension must be {self._spatial_ndim + 2}, but got {kernel.ndim}."
+            )
+
+        if order == "IOHW":
+            _kernel = np.swapaxes(kernel, 0, 1)
+        else:
+            _kernel = kernel.copy()
+
+        # O,I,H,W
+        out_channels, in_channels, kernel_h, kernel_w = _kernel.shape
+        # C,H,W
+        in_ch, in_h, in_w = _fm_ndim2_check(source.shape_out, "CHW")
+        out_h = (in_h - 1) * stride[0] - 2 * padding[0] + kernel_h + output_padding[0]
+        out_w = (in_w - 1) * stride[1] - 2 * padding[1] + kernel_w + output_padding[1]
+
+        if in_ch != in_channels:
+            raise ShapeError(f"input channels mismatch: {in_ch} != {in_channels}.")
 
-        assert (in_h + 2 * padding[0] - kernel_h) // stride[0] + 1 == out_h
-        assert (in_w + 2 * padding[1] - kernel_w) // stride[1] + 1 == out_w
+        if (_output_size := out_channels * out_h * out_w) != dest.num_in:
+            raise ShapeError(f"Output size mismatch: {_output_size} != {dest.num_in}.")
 
-        comm = Conv2dForward(
-            (in_h, in_w), (out_h, out_w), _kernel, stride, padding, fm_order
+        comm = ConvTranspose2dForward(
+            (in_h, in_w), (out_h, out_w), _kernel, stride, padding, output_padding
         )
 
         self._set_comm(comm)
```

### Comparing `paibox-1.0.0b1/paibox/synapses/transforms.py` & `paibox-1.0.0rc1/paibox/synapses/transforms.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,26 +11,30 @@
 from .conv_utils import (
     Size1Type,
     Size2Type,
     _conv1d_faster,
     _conv1d_unroll,
     _conv2d_faster,
     _conv2d_unroll,
-    _Order2d,
-    _Order3d,
+    _convtranspose1d_faster,
+    _convtranspose1d_unroll,
+    _convtranspose2d_faster,
+    _convtranspose2d_unroll,
 )
 
 __all__ = [
     "GeneralConnType",
     "OneToOne",
     "AllToAll",
     "Identity",
     "MaskedLinear",
     "Conv1dForward",
     "Conv2dForward",
+    "ConvTranspose1dForward",
+    "ConvTranspose2dForward",
 ]
 
 
 MAX_INT1 = np.int8(1)
 MIN_INT1 = np.int8(0)
 MAX_INT2 = np.int8(1)
 MIN_INT2 = np.int8(-2)
@@ -185,17 +189,15 @@
         if self.weights.ndim not in (0, 1):
             raise ShapeError(
                 f"the ndim of weights must be 0 or 1, but got {self.weights.ndim}."
             )
 
     def __call__(self, x: np.ndarray, *args, **kwargs) -> SynOutType:
         # (N,) * (N,) -> (N,)
-        output = x * self.weights.copy()
-
-        return output.astype(np.int32)
+        return x * self.weights.astype(np.int32)
 
     @property
     def connectivity(self):
         return (
             (self.weights * np.eye(self.num, dtype=np.bool_))
             if self.weights.ndim == 0
             else np.diag(self.weights)
@@ -246,15 +248,15 @@
         """
         if self.weights.ndim == 0:
             sum_x = np.sum(x, axis=None, dtype=np.int32)
             # (M,)
             output = np.full((self.conn_size[1],), self.weights * sum_x, dtype=np.int32)
         else:
             # (N,) @ (N, M) -> (M,)
-            output = x @ self.weights.copy().astype(np.int32)
+            output = x @ self.weights.astype(np.int32)
 
         return output
 
     @property
     def connectivity(self):
         return (
             self.weights
@@ -268,98 +270,188 @@
         if not is_shape(weights, conn_size):
             raise ShapeError(f"expected shape is {conn_size}, but got {weights.shape}.")
 
         super().__init__(weights)
 
     def __call__(self, x: np.ndarray, *args, **kwargs) -> SynOutType:
         # (N,) @ (N, M) -> (M,)
-        output = x @ self.weights.copy().astype(np.int32)
-
-        return output.astype(np.int32)
+        return x @ self.weights.astype(np.int32)
 
     @property
     def connectivity(self):
         return self.weights
 
 
 class Conv1dForward(Transform):
     def __init__(
         self,
         in_shape: Size1Type,
         out_shape: Size1Type,
         kernel: np.ndarray,
         stride: Size1Type,
         padding: Size1Type,
-        fm_order: _Order2d,
+        # fm_order: _Order2d,
     ) -> None:
         self.in_shape = in_shape
         self.out_shape = out_shape
         self.stride = stride
         self.padding = padding
-        self.fm_order = fm_order
+        # self.fm_order = fm_order
 
         super().__init__(kernel)
 
     def __call__(self, x: np.ndarray, *args, **kwargs) -> SynOutType:
         cin = self.weights.shape[1]
 
-        if self.fm_order == "LC":
-            # (N,) -> (L, C) -> (C, L)
-            _x = x.reshape(self.in_shape + (cin,)).T
-        else:
-            _x = x.reshape((cin,) + self.in_shape)
+        # if self.fm_order == "LC":
+        #     # (N,) -> (L, C) -> (C, L)
+        #     _x = x.reshape(self.in_shape + (cin,)).T
+        # else:
+        _x = x.reshape((cin,) + self.in_shape)
+
+        return _conv1d_faster(
+            _x, self.out_shape, self.weights, self.stride, self.padding
+        )
+
+    @property
+    def connectivity(self):
+        return _conv1d_unroll(
+            self.in_shape, self.out_shape, self.weights, self.stride, self.padding
+        )
+
+
+class Conv2dForward(Transform):
+    def __init__(
+        self,
+        in_shape: Size2Type,
+        out_shape: Size2Type,
+        kernel: np.ndarray,
+        stride: Size2Type,
+        padding: Size2Type,
+        # fm_order: _Order3d,
+    ) -> None:
+        self.in_shape = in_shape
+        self.out_shape = out_shape
+        self.stride = stride
+        self.padding = padding
+        # self.fm_order = fm_order
+
+        super().__init__(kernel)
+
+    def __call__(self, x: np.ndarray, *args, **kwargs) -> SynOutType:
+        cin = self.weights.shape[1]
+
+        # if self.fm_order == "HWC":
+        #     # (N,) -> (H, W, C) -> (C, H, W)
+        #     _x = x.reshape(self.in_shape + (cin,)).transpose(2, 0, 1)
+        # else:
+        _x = x.reshape((cin,) + self.in_shape)
+
+        return _conv2d_faster(
+            _x, self.out_shape, self.weights, self.stride, self.padding
+        )
+
+    @property
+    def connectivity(self):
+        return _conv2d_unroll(
+            self.in_shape, self.out_shape, self.weights, self.stride, self.padding
+        )
+
 
-        o_conv1d = _conv1d_faster(
+class ConvTranspose1dForward(Transform):
+    def __init__(
+        self,
+        in_shape: Size1Type,
+        out_shape: Size1Type,
+        kernel: np.ndarray,
+        stride: Size1Type,
+        padding: Size1Type,
+        output_padding: Size1Type,
+        # fm_order: _Order2d,
+    ) -> None:
+        self.in_shape = in_shape
+        self.out_shape = out_shape
+        self.stride = stride
+        self.padding = padding
+        self.output_padding = output_padding
+        # self.fm_order = fm_order
+
+        super().__init__(kernel)
+
+    def __call__(self, x: np.ndarray, *args, **kwargs) -> SynOutType:
+        cin = self.weights.shape[1]
+
+        # if self.fm_order == "LC":
+        #     # (N,) -> (L, C) -> (C, L)
+        #     _x = x.reshape(self.in_shape + (cin,)).T
+        # else:
+        _x = x.reshape((cin,) + self.in_shape)
+
+        return _convtranspose1d_faster(
             _x,
             self.out_shape,
             self.weights,
             self.stride,
             self.padding,
+            self.output_padding,
         )
 
-        return o_conv1d.flatten()
-
     @property
     def connectivity(self):
-        return _conv1d_unroll(self.in_shape, self.out_shape, self.weights, self.stride)
+        return _convtranspose1d_unroll(
+            self.in_shape,
+            self.out_shape,
+            self.weights,
+            self.stride,
+            self.padding,
+            self.output_padding,
+        )
 
 
-class Conv2dForward(Transform):
+class ConvTranspose2dForward(Transform):
     def __init__(
         self,
         in_shape: Size2Type,
         out_shape: Size2Type,
         kernel: np.ndarray,
         stride: Size2Type,
         padding: Size2Type,
-        fm_order: _Order3d,
+        output_padding: Size2Type,
+        # fm_order: _Order3d,
     ) -> None:
         self.in_shape = in_shape
         self.out_shape = out_shape
         self.stride = stride
         self.padding = padding
-        self.fm_order = fm_order
+        self.output_padding = output_padding
+        # self.fm_order = fm_order
 
         super().__init__(kernel)
 
     def __call__(self, x: np.ndarray, *args, **kwargs) -> SynOutType:
         cin = self.weights.shape[1]
 
-        if self.fm_order == "HWC":
-            # (N,) -> (H, W, C) -> (C, H, W)
-            _x = x.reshape(self.in_shape + (cin,)).transpose(2, 0, 1)
-        else:
-            _x = x.reshape((cin,) + self.in_shape)
+        # if self.fm_order == "HWC":
+        #     # (N,) -> (H, W, C) -> (C, H, W)
+        #     _x = x.reshape(self.in_shape + (cin,)).transpose(2, 0, 1)
+        # else:
+        _x = x.reshape((cin,) + self.in_shape)
 
-        o_conv2d = _conv2d_faster(
+        return _convtranspose2d_faster(
             _x,
             self.out_shape,
             self.weights,
             self.stride,
             self.padding,
+            self.output_padding,
         )
 
-        return o_conv2d.flatten()
-
     @property
     def connectivity(self):
-        return _conv2d_unroll(self.in_shape, self.out_shape, self.weights, self.stride)
+        return _convtranspose2d_unroll(
+            self.in_shape,
+            self.out_shape,
+            self.weights,
+            self.stride,
+            self.padding,
+            self.output_padding,
+        )
```

### Comparing `paibox-1.0.0b1/paibox/types.py` & `paibox-1.0.0rc1/paibox/types.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/paibox/utils.py` & `paibox-1.0.0rc1/paibox/utils.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0b1/pyproject.toml` & `paibox-1.0.0rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 [tool.poetry]
 name = "paibox"
-version = "1.0.0b1"
-description = "New toolbox of PAICORE 2.0."
+version = "1.0.0rc1"
+description = "Toolchain of PAICORE 2.0."
 authors = ["Ziru Pan <zrpan@stu.pku.edu.cn>"]
-maintainers = ["Ziru Pan <zrpan@stu.pku.edu.cn>"]
+maintainers = [
+    "Hongtu Xia <hongtux@pku.edu.cn>",
+    "Siyuan Gao <siyuan-gao@outlook.com>",
+    "Zhaoyang Hao <hzyang2218@gmail.com>",
+    "Ziru Pan <zrpan@stu.pku.edu.cn>",
+]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/PAICookers/PAIBox"
 homepage = "https://github.com/PAICookers/PAIBox"
 documentation = "https://github.com/PAICookers/PAIBox#readme"
-keywords = ["PAICORE 2.0", "PAIBox", "Toolbox"]
+keywords = ["PAICORE 2.0", "PAIBox", "SNN", "Toolchain"]
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -31,15 +36,15 @@
 # Excludes the experimental code
 exclude = ["paibox/experimental"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^2.0"
 numpy = "^1.24.0"
-paicorelib = "0.0.13"
+paicorelib = "^0.0.13"
 
 [tool.poetry.group.test]
 optional = true
 
 
 [tool.poetry.group.test.dependencies]
 pytest = { version = "^7.4.0", python = "^3.8" }
```

### Comparing `paibox-1.0.0b1/PKG-INFO` & `paibox-1.0.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: paibox
-Version: 1.0.0b1
-Summary: New toolbox of PAICORE 2.0.
+Version: 1.0.0rc1
+Summary: Toolchain of PAICORE 2.0.
 Home-page: https://github.com/PAICookers/PAIBox
 License: GPL-3.0-or-later
-Keywords: PAICORE 2.0,PAIBox,Toolbox
+Keywords: PAICORE 2.0,PAIBox,SNN,Toolchain
 Author: Ziru Pan
 Author-email: zrpan@stu.pku.edu.cn
-Maintainer: Ziru Pan
-Maintainer-email: zrpan@stu.pku.edu.cn
+Maintainer: Hongtu Xia
+Maintainer-email: hongtux@pku.edu.cn
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: numpy (>=1.24.0,<2.0.0)
-Requires-Dist: paicorelib (==0.0.13)
+Requires-Dist: paicorelib (>=0.0.13,<0.0.14)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Project-URL: Documentation, https://github.com/PAICookers/PAIBox#readme
 Project-URL: Repository, https://github.com/PAICookers/PAIBox
 Description-Content-Type: text/markdown
 
 <div align="center">
 
@@ -36,15 +36,15 @@
 
 </div>
 
 <p align="center">
     <a href="https://github.com/PAICookers/PAIBox/blob/master/pyproject.toml">
         <img src="https://img.shields.io/pypi/pyversions/paibox">
     </a>
-    <a href="https://github.com/PAICookers/PAIBox/releases/tag/v1.0.0b1">
+    <a href="https://github.com/PAICookers/PAIBox/releases/tag/v1.0.0rc1">
         <img src="https://img.shields.io/github/v/release/PAICookers/PAIBox?include_prereleases&color=orange">
     </a>
     <a href="https://www.codefactor.io/repository/github/PAICookers/PAIBox">
       <img src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIBox/master?color=red">
     </a>
     <a href="https://results.pre-commit.ci/latest/github/PAICookers/PAIBox/master">
 	   <img src="https://results.pre-commit.ci/badge/github/PAICookers/PAIBox/master.svg" alt="pre-commit.ci status">
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: paibox Version: 1.0.0b1 Summary: New toolbox of
+Metadata-Version: 2.1 Name: paibox Version: 1.0.0rc1 Summary: Toolchain of
 PAICORE 2.0. Home-page: https://github.com/PAICookers/PAIBox License: GPL-3.0-
-or-later Keywords: PAICORE 2.0,PAIBox,Toolbox Author: Ziru Pan Author-email:
-zrpan@stu.pku.edu.cn Maintainer: Ziru Pan Maintainer-email:
-zrpan@stu.pku.edu.cn Requires-Python: >=3.8,<4.0 Classifier: Intended Audience
-:: Science/Research Classifier: License :: OSI Approved :: GNU General Public
+or-later Keywords: PAICORE 2.0,PAIBox,SNN,Toolchain Author: Ziru Pan Author-
+email: zrpan@stu.pku.edu.cn Maintainer: Hongtu Xia Maintainer-email:
+hongtux@pku.edu.cn Requires-Python: >=3.8,<4.0 Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development :: Build Tools Classifier: Topic :: Software Development ::
 Libraries Requires-Dist: numpy (>=1.24.0,<2.0.0) Requires-Dist: paicorelib
-(==0.0.13) Requires-Dist: pydantic (>=2.0,<3.0) Project-URL: Documentation,
-https://github.com/PAICookers/PAIBox#readme Project-URL: Repository, https://
-github.com/PAICookers/PAIBox Description-Content-Type: text/markdown
+(>=0.0.13,<0.0.14) Requires-Dist: pydantic (>=2.0,<3.0) Project-URL:
+Documentation, https://github.com/PAICookers/PAIBox#readme Project-URL:
+Repository, https://github.com/PAICookers/PAIBox Description-Content-Type:
+text/markdown
                                    # PAIBox
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_p_a_i_b_o_x_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
     _v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_?_i_n_c_l_u_d_e___p_r_e_r_e_l_e_a_s_e_s_&_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_f_a_c_t_o_r_/_g_r_a_d_e_/_g_i_t_h_u_b_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_/_m_a_s_t_e_r_?_c_o_l_o_r_=_r_e_d_]_[_p_r_e_-
                                _c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]
 PAIBoxä½¿ç¨æåï¼[Guide-of-PAIBox](docs/Guide-of-PAIBox.md)
 é«æç¼åæµè¯é¡¹ç®æåï¼[Guide-of-Test](docs/Guide-of-Test.md) TODOï¼
```

