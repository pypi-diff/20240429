# Comparing `tmp/rten-convert-0.6.0.tar.gz` & `tmp/rten_convert-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rten-convert-0.6.0.tar", last modified: Sun Mar 31 20:48:38 2024, max compression
+gzip compressed data, was "rten_convert-0.8.0.tar", last modified: Mon Apr 29 20:59:56 2024, max compression
```

## Comparing `rten-convert-0.6.0.tar` & `rten_convert-0.8.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-03-31 20:48:38.930542 rten-convert-0.6.0/
--rw-r--r--   0 robert     (501) staff       (20)     1070 2024-03-27 13:23:26.000000 rten-convert-0.6.0/LICENSE
--rw-r--r--   0 robert     (501) staff       (20)     1212 2024-03-31 20:48:38.929710 rten-convert-0.6.0/PKG-INFO
--rw-r--r--   0 robert     (501) staff       (20)      780 2024-03-27 13:23:26.000000 rten-convert-0.6.0/README.md
--rw-r--r--   0 robert     (501) staff       (20)      533 2024-03-31 20:45:39.000000 rten-convert-0.6.0/pyproject.toml
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-03-31 20:48:38.921471 rten-convert-0.6.0/rten_convert/
--rw-r--r--   0 robert     (501) staff       (20)        0 2024-03-29 09:30:42.000000 rten-convert-0.6.0/rten_convert/__init__.py
--rw-r--r--   0 robert     (501) staff       (20)    44525 2024-03-31 19:32:35.000000 rten-convert-0.6.0/rten_convert/converter.py
--rw-r--r--   0 robert     (501) staff       (20)   165300 2024-03-31 19:32:35.000000 rten-convert-0.6.0/rten_convert/schema_generated.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-03-31 20:48:38.928835 rten-convert-0.6.0/rten_convert.egg-info/
--rw-r--r--   0 robert     (501) staff       (20)     1212 2024-03-31 20:48:38.000000 rten-convert-0.6.0/rten_convert.egg-info/PKG-INFO
--rw-r--r--   0 robert     (501) staff       (20)      334 2024-03-31 20:48:38.000000 rten-convert-0.6.0/rten_convert.egg-info/SOURCES.txt
--rw-r--r--   0 robert     (501) staff       (20)        1 2024-03-31 20:48:38.000000 rten-convert-0.6.0/rten_convert.egg-info/dependency_links.txt
--rw-r--r--   0 robert     (501) staff       (20)       61 2024-03-31 20:48:38.000000 rten-convert-0.6.0/rten_convert.egg-info/entry_points.txt
--rw-r--r--   0 robert     (501) staff       (20)       23 2024-03-31 20:48:38.000000 rten-convert-0.6.0/rten_convert.egg-info/requires.txt
--rw-r--r--   0 robert     (501) staff       (20)       13 2024-03-31 20:48:38.000000 rten-convert-0.6.0/rten_convert.egg-info/top_level.txt
--rw-r--r--   0 robert     (501) staff       (20)       38 2024-03-31 20:48:38.930763 rten-convert-0.6.0/setup.cfg
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-29 20:59:56.489125 rten_convert-0.8.0/
+-rw-r--r--   0 robert     (501) staff       (20)     1070 2024-04-29 18:40:42.000000 rten_convert-0.8.0/LICENSE
+-rw-r--r--   0 robert     (501) staff       (20)     1212 2024-04-29 20:59:56.488448 rten_convert-0.8.0/PKG-INFO
+-rw-r--r--   0 robert     (501) staff       (20)      780 2024-04-29 18:40:42.000000 rten_convert-0.8.0/README.md
+-rw-r--r--   0 robert     (501) staff       (20)      533 2024-04-29 20:59:17.000000 rten_convert-0.8.0/pyproject.toml
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-29 20:59:56.481554 rten_convert-0.8.0/rten_convert/
+-rw-r--r--   0 robert     (501) staff       (20)        0 2024-04-29 18:40:42.000000 rten_convert-0.8.0/rten_convert/__init__.py
+-rw-r--r--   0 robert     (501) staff       (20)    44649 2024-04-29 20:43:46.000000 rten_convert-0.8.0/rten_convert/converter.py
+-rw-r--r--   0 robert     (501) staff       (20)   167524 2024-04-29 20:43:46.000000 rten_convert-0.8.0/rten_convert/schema_generated.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-29 20:59:56.487898 rten_convert-0.8.0/rten_convert.egg-info/
+-rw-r--r--   0 robert     (501) staff       (20)     1212 2024-04-29 20:59:56.000000 rten_convert-0.8.0/rten_convert.egg-info/PKG-INFO
+-rw-r--r--   0 robert     (501) staff       (20)      334 2024-04-29 20:59:56.000000 rten_convert-0.8.0/rten_convert.egg-info/SOURCES.txt
+-rw-r--r--   0 robert     (501) staff       (20)        1 2024-04-29 20:59:56.000000 rten_convert-0.8.0/rten_convert.egg-info/dependency_links.txt
+-rw-r--r--   0 robert     (501) staff       (20)       61 2024-04-29 20:59:56.000000 rten_convert-0.8.0/rten_convert.egg-info/entry_points.txt
+-rw-r--r--   0 robert     (501) staff       (20)       23 2024-04-29 20:59:56.000000 rten_convert-0.8.0/rten_convert.egg-info/requires.txt
+-rw-r--r--   0 robert     (501) staff       (20)       13 2024-04-29 20:59:56.000000 rten_convert-0.8.0/rten_convert.egg-info/top_level.txt
+-rw-r--r--   0 robert     (501) staff       (20)       38 2024-04-29 20:59:56.489299 rten_convert-0.8.0/setup.cfg
```

### Comparing `rten-convert-0.6.0/LICENSE` & `rten_convert-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rten-convert-0.6.0/PKG-INFO` & `rten_convert-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rten-convert
-Version: 0.6.0
+Version: 0.8.0
 Summary: Convert ONNX models to .rten format
 Project-URL: Homepage, https://github.com/robertknight/rten
 Project-URL: Issues, https://github.com/robertknight/rten/issues
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rten-convert-0.6.0/README.md` & `rten_convert-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `rten-convert-0.6.0/pyproject.toml` & `rten_convert-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "rten-convert"
 description = "Convert ONNX models to .rten format"
 requires-python = ">=3.10"
-version = "0.6.0"
+version = "0.8.0"
 dependencies = ["flatbuffers", "onnx", "numpy"]
 readme = "README.md"
 classifiers = [
   "License :: OSI Approved :: MIT License",
 ]
 
 [project.scripts]
```

### Comparing `rten-convert-0.6.0/rten_convert/converter.py` & `rten_convert-0.8.0/rten_convert/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -699,14 +699,18 @@
             op_reader.check_attr("output_padding", "ints", [0, 0, 0, 0])
             op_reader.check_attr("pads", "ints", [0, 0, 0, 0])
 
         case "CumSum":
             op_reader.check_attr("exclusive", "int", 0)
             op_reader.check_attr("reverse", "int", 0)
 
+        case "Elu":
+            attrs = sg.EluAttrsT()
+            attrs.alpha = op_reader.get_attr("alpha", "float", 1.0)
+
         case "Flatten":
             attrs = sg.FlattenAttrsT()
             attrs.axis = op_reader.get_attr("axis", "int", 1)
 
         case "Gather" | "GatherElements":
             attrs = sg.GatherAttrsT()
             attrs.axis = op_reader.get_attr("axis", "int", 0)
```

### Comparing `rten-convert-0.6.0/rten_convert/schema_generated.py` & `rten_convert-0.8.0/rten_convert/schema_generated.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     ScatterND = 89
     NonMaxSuppression = 90
     Sign = 91
     GatherElements = 92
     LayerNormalization = 93
     ReduceSumSquare = 94
     RandomUniform = 95
+    Elu = 96
 
 
 class RNNDirection(object):
     Forward = 0
     Reverse = 1
     Bidirectional = 2
 
@@ -168,14 +169,15 @@
     TopKAttrs = 25
     HardSigmoidAttrs = 26
     TriluAttrs = 27
     ScatterNDAttrs = 28
     NonMaxSuppressionAttrs = 29
     LayerNormalizationAttrs = 30
     RandomUniformAttrs = 31
+    EluAttrs = 32
 
 def OperatorAttrsCreator(unionType, table):
     from flatbuffers.table import Table
     if not isinstance(table, Table):
         return None
     if unionType == OperatorAttrs().ArgMaxAttrs:
         return ArgMaxAttrsT.InitFromBuf(table.Bytes, table.Pos)
@@ -235,14 +237,16 @@
         return ScatterNDAttrsT.InitFromBuf(table.Bytes, table.Pos)
     if unionType == OperatorAttrs().NonMaxSuppressionAttrs:
         return NonMaxSuppressionAttrsT.InitFromBuf(table.Bytes, table.Pos)
     if unionType == OperatorAttrs().LayerNormalizationAttrs:
         return LayerNormalizationAttrsT.InitFromBuf(table.Bytes, table.Pos)
     if unionType == OperatorAttrs().RandomUniformAttrs:
         return RandomUniformAttrsT.InitFromBuf(table.Bytes, table.Pos)
+    if unionType == OperatorAttrs().EluAttrs:
+        return EluAttrsT.InitFromBuf(table.Bytes, table.Pos)
     return None
 
 
 class Scalar(object):
     NONE = 0
     IntScalar = 1
     FloatScalar = 2
@@ -1490,14 +1494,91 @@
         ConvTransposeAttrsStart(builder)
         if self.strides is not None:
             ConvTransposeAttrsAddStrides(builder, strides)
         convTransposeAttrs = ConvTransposeAttrsEnd(builder)
         return convTransposeAttrs
 
 
+class EluAttrs(object):
+    __slots__ = ['_tab']
+
+    @classmethod
+    def GetRootAs(cls, buf, offset=0):
+        n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, offset)
+        x = EluAttrs()
+        x.Init(buf, n + offset)
+        return x
+
+    @classmethod
+    def GetRootAsEluAttrs(cls, buf, offset=0):
+        """This method is deprecated. Please switch to GetRootAs."""
+        return cls.GetRootAs(buf, offset)
+    @classmethod
+    def EluAttrsBufferHasIdentifier(cls, buf, offset, size_prefixed=False):
+        return flatbuffers.util.BufferHasIdentifier(buf, offset, b"\x52\x54\x45\x4E", size_prefixed=size_prefixed)
+
+    # EluAttrs
+    def Init(self, buf, pos):
+        self._tab = flatbuffers.table.Table(buf, pos)
+
+    # EluAttrs
+    def Alpha(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(4))
+        if o != 0:
+            return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
+        return 0.0
+
+def EluAttrsStart(builder):
+    builder.StartObject(1)
+
+def EluAttrsAddAlpha(builder, alpha):
+    builder.PrependFloat32Slot(0, alpha, 0.0)
+
+def EluAttrsEnd(builder):
+    return builder.EndObject()
+
+
+
+class EluAttrsT(object):
+
+    # EluAttrsT
+    def __init__(self):
+        self.alpha = 0.0  # type: float
+
+    @classmethod
+    def InitFromBuf(cls, buf, pos):
+        eluAttrs = EluAttrs()
+        eluAttrs.Init(buf, pos)
+        return cls.InitFromObj(eluAttrs)
+
+    @classmethod
+    def InitFromPackedBuf(cls, buf, pos=0):
+        n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, pos)
+        return cls.InitFromBuf(buf, pos+n)
+
+    @classmethod
+    def InitFromObj(cls, eluAttrs):
+        x = EluAttrsT()
+        x._UnPack(eluAttrs)
+        return x
+
+    # EluAttrsT
+    def _UnPack(self, eluAttrs):
+        if eluAttrs is None:
+            return
+        self.alpha = eluAttrs.Alpha()
+
+    # EluAttrsT
+    def Pack(self, builder):
+        EluAttrsStart(builder)
+        EluAttrsAddAlpha(builder, self.alpha)
+        eluAttrs = EluAttrsEnd(builder)
+        return eluAttrs
+
+
 class FlattenAttrs(object):
     __slots__ = ['_tab']
 
     @classmethod
     def GetRootAs(cls, buf, offset=0):
         n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, offset)
         x = FlattenAttrs()
@@ -3904,15 +3985,15 @@
 
 class OperatorNodeT(object):
 
     # OperatorNodeT
     def __init__(self):
         self.type = 0  # type: int
         self.attrsType = 0  # type: int
-        self.attrs = None  # type: Union[None, ArgMaxAttrsT, AveragePoolAttrsT, BatchNormalizationAttrsT, CastAttrsT, ConcatAttrsT, ConstantOfShapeAttrsT, ConvAttrsT, ConvTransposeAttrsT, FlattenAttrsT, GatherAttrsT, GemmAttrsT, GRUAttrsT, LeakyReluAttrsT, LSTMAttrsT, MaxPoolAttrsT, ReduceMeanAttrsT, ReshapeAttrsT, ResizeAttrsT, SplitAttrsT, SoftmaxAttrsT, TransposeAttrsT, ModAttrsT, ScatterElementsAttrsT, OneHotAttrsT, TopKAttrsT, HardSigmoidAttrsT, TriluAttrsT, ScatterNDAttrsT, NonMaxSuppressionAttrsT, LayerNormalizationAttrsT, RandomUniformAttrsT]
+        self.attrs = None  # type: Union[None, ArgMaxAttrsT, AveragePoolAttrsT, BatchNormalizationAttrsT, CastAttrsT, ConcatAttrsT, ConstantOfShapeAttrsT, ConvAttrsT, ConvTransposeAttrsT, FlattenAttrsT, GatherAttrsT, GemmAttrsT, GRUAttrsT, LeakyReluAttrsT, LSTMAttrsT, MaxPoolAttrsT, ReduceMeanAttrsT, ReshapeAttrsT, ResizeAttrsT, SplitAttrsT, SoftmaxAttrsT, TransposeAttrsT, ModAttrsT, ScatterElementsAttrsT, OneHotAttrsT, TopKAttrsT, HardSigmoidAttrsT, TriluAttrsT, ScatterNDAttrsT, NonMaxSuppressionAttrsT, LayerNormalizationAttrsT, RandomUniformAttrsT, EluAttrsT]
         self.inputs = None  # type: List[int]
         self.outputs = None  # type: List[int]
 
     @classmethod
     def InitFromBuf(cls, buf, pos):
         operatorNode = OperatorNode()
         operatorNode.Init(buf, pos)
```

### Comparing `rten-convert-0.6.0/rten_convert.egg-info/PKG-INFO` & `rten_convert-0.8.0/rten_convert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rten-convert
-Version: 0.6.0
+Version: 0.8.0
 Summary: Convert ONNX models to .rten format
 Project-URL: Homepage, https://github.com/robertknight/rten
 Project-URL: Issues, https://github.com/robertknight/rten/issues
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

