# Comparing `tmp/xc3_model_py-0.5.0-cp39-none-win_amd64.whl.zip` & `tmp/xc3_model_py-0.5.1-cp39-cp39-manylinux_2_34_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 2806245 bytes, number of entries: 9
--rw-r--r--  4.6 unx     7784 b- defN 24-Apr-29 15:47 xc3_model_py-0.5.0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-Apr-29 15:47 xc3_model_py-0.5.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     1758 b- defN 24-Apr-29 15:47 xc3_model_py/animation.pyi
--rw-r--r--  4.6 unx     1095 b- defN 24-Apr-29 15:47 xc3_model_py/skinning.pyi
--rw-r--r--  4.6 unx     2111 b- defN 24-Apr-29 15:47 xc3_model_py/vertex.pyi
--rw-r--r--  4.6 unx       27 b- defN 24-Apr-29 15:47 xc3_model_py/__init__.py
--rw-r--r--  4.6 unx     8675 b- defN 24-Apr-29 15:47 xc3_model_py/__init__.pyi
--rwxr-xr-x  4.6 unx  8119808 b- defN 24-Apr-29 15:47 xc3_model_py/xc3_model_py.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      731 b- defN 24-Apr-29 15:47 xc3_model_py-0.5.0.dist-info/RECORD
-9 files, 8142083 bytes uncompressed, 2804993 bytes compressed:  65.6%
+Zip file size: 2828167 bytes, number of entries: 9
+-rw-r--r--  4.6 unx     7650 b- defN 24-Apr-29 16:44 xc3_model_py-0.5.1.dist-info/METADATA
+-rw-r--r--  4.6 unx      106 b- defN 24-Apr-29 16:44 xc3_model_py-0.5.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1689 b- defN 24-Apr-29 16:44 xc3_model_py/animation.pyi
+-rw-r--r--  4.6 unx     1053 b- defN 24-Apr-29 16:44 xc3_model_py/skinning.pyi
+-rw-r--r--  4.6 unx       27 b- defN 24-Apr-29 16:44 xc3_model_py/__init__.py
+-rw-r--r--  4.6 unx     2044 b- defN 24-Apr-29 16:44 xc3_model_py/vertex.pyi
+-rw-r--r--  4.6 unx     8369 b- defN 24-Apr-29 16:44 xc3_model_py/__init__.pyi
+-rwxr-xr-x  4.6 unx  8601904 b- defN 24-Apr-29 16:44 xc3_model_py/xc3_model_py.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  4.6 unx      744 b- defN 24-Apr-29 16:44 xc3_model_py-0.5.1.dist-info/RECORD
+9 files, 8623586 bytes uncompressed, 2826891 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
-Filename: xc3_model_py-0.5.0.dist-info/METADATA
+Filename: xc3_model_py-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: xc3_model_py-0.5.0.dist-info/WHEEL
+Filename: xc3_model_py-0.5.1.dist-info/WHEEL
 Comment: 
 
 Filename: xc3_model_py/animation.pyi
 Comment: 
 
 Filename: xc3_model_py/skinning.pyi
 Comment: 
 
-Filename: xc3_model_py/vertex.pyi
+Filename: xc3_model_py/__init__.py
 Comment: 
 
-Filename: xc3_model_py/__init__.py
+Filename: xc3_model_py/vertex.pyi
 Comment: 
 
 Filename: xc3_model_py/__init__.pyi
 Comment: 
 
-Filename: xc3_model_py/xc3_model_py.cp39-win_amd64.pyd
+Filename: xc3_model_py/xc3_model_py.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: xc3_model_py-0.5.0.dist-info/RECORD
+Filename: xc3_model_py-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xc3_model_py/animation.pyi

 * *Ordering differences only*

```diff
@@ -1,69 +1,69 @@
-from typing import Optional, ClassVar, Tuple
-import numpy
-
-from xc3_model_py import Skeleton
-
-
-class Animation:
-    name: str
-    space_mode: SpaceMode
-    play_mode: PlayMode
-    blend_mode: BlendMode
-    frames_per_second: float
-    frame_count: int
-    tracks: list[Track]
-
-    def current_frame(self, current_time_seconds: float) -> float: ...
-
-    def skinning_transforms(self, skeleton: Skeleton,
-                            frame: float) -> numpy.ndarray: ...
-
-    def model_space_transforms(
-        self, skeleton: Skeleton, frame: float) -> numpy.ndarray: ...
-
-    def local_space_transforms(
-        self, skeleton: Skeleton, frame: float) -> numpy.ndarray: ...
-
-
-class Track:
-    def sample_translation(
-        self, frame: float) -> Optional[Tuple[float, float, float]]: ...
-
-    def sample_rotation(
-        self, frame: float) -> Optional[Tuple[float, float, float]]: ...
-
-    def sample_scale(
-        self, frame: float) -> Optional[Tuple[float, float, float]]: ...
-
-    def sample_transform(self, frame: float) -> Optional[numpy.ndarray]: ...
-
-    def bone_index(self) -> Optional[int]: ...
-
-    def bone_hash(self) -> Optional[int]: ...
-
-    def bone_name(self) -> Optional[str]: ...
-
-
-class KeyFrame:
-    x_coeffs: Tuple[float, float, float, float]
-    y_coeffs: Tuple[float, float, float, float]
-    z_coeffs: Tuple[float, float, float, float]
-    w_coeffs: Tuple[float, float, float, float]
-
-
-class SpaceMode:
-    Local: ClassVar[SpaceMode]
-    Model: ClassVar[SpaceMode]
-
-
-class PlayMode:
-    Loop: ClassVar[PlayMode]
-    Single: ClassVar[PlayMode]
-
-
-class BlendMode:
-    Blend: ClassVar[BlendMode]
-    Add: ClassVar[BlendMode]
-
-
-def murmur3(name: str) -> int: ...
+from typing import Optional, ClassVar, Tuple
+import numpy
+
+from xc3_model_py import Skeleton
+
+
+class Animation:
+    name: str
+    space_mode: SpaceMode
+    play_mode: PlayMode
+    blend_mode: BlendMode
+    frames_per_second: float
+    frame_count: int
+    tracks: list[Track]
+
+    def current_frame(self, current_time_seconds: float) -> float: ...
+
+    def skinning_transforms(self, skeleton: Skeleton,
+                            frame: float) -> numpy.ndarray: ...
+
+    def model_space_transforms(
+        self, skeleton: Skeleton, frame: float) -> numpy.ndarray: ...
+
+    def local_space_transforms(
+        self, skeleton: Skeleton, frame: float) -> numpy.ndarray: ...
+
+
+class Track:
+    def sample_translation(
+        self, frame: float) -> Optional[Tuple[float, float, float]]: ...
+
+    def sample_rotation(
+        self, frame: float) -> Optional[Tuple[float, float, float]]: ...
+
+    def sample_scale(
+        self, frame: float) -> Optional[Tuple[float, float, float]]: ...
+
+    def sample_transform(self, frame: float) -> Optional[numpy.ndarray]: ...
+
+    def bone_index(self) -> Optional[int]: ...
+
+    def bone_hash(self) -> Optional[int]: ...
+
+    def bone_name(self) -> Optional[str]: ...
+
+
+class KeyFrame:
+    x_coeffs: Tuple[float, float, float, float]
+    y_coeffs: Tuple[float, float, float, float]
+    z_coeffs: Tuple[float, float, float, float]
+    w_coeffs: Tuple[float, float, float, float]
+
+
+class SpaceMode:
+    Local: ClassVar[SpaceMode]
+    Model: ClassVar[SpaceMode]
+
+
+class PlayMode:
+    Loop: ClassVar[PlayMode]
+    Single: ClassVar[PlayMode]
+
+
+class BlendMode:
+    Blend: ClassVar[BlendMode]
+    Add: ClassVar[BlendMode]
+
+
+def murmur3(name: str) -> int: ...
```

## xc3_model_py/skinning.pyi

 * *Ordering differences only*

```diff
@@ -1,42 +1,42 @@
-from typing import Optional, ClassVar, Tuple
-import numpy
-
-from xc3_model_py import RenderPassType
-
-
-class Weights:
-    weight_buffers: list[SkinWeights]
-
-    def __init__(self, weight_buffers: list[SkinWeights]) -> None: ...
-
-    def weight_buffer(self, flags2: int) -> Optional[SkinWeights]: ...
-
-    def weights_start_index(self, flags2: int, lod: int,
-                            unk_type: RenderPassType) -> int: ...
-
-
-class SkinWeights:
-    bone_indices: numpy.ndarray
-    weights: numpy.ndarray
-    bone_names: list[str]
-
-    def __init__(self, bone_indices: numpy.ndarray,
-                 weights: numpy.ndarray, bone_names: list[str]) -> None: ...
-
-    def to_influences(
-        self, weight_indices: numpy.ndarray) -> list[Influence]: ...
-
-
-class Influence:
-    bone_name: str
-    weights: list[VertexWeight]
-
-    def __init__(self, bone_name: str,
-                 weights: list[VertexWeight]) -> None: ...
-
-
-class VertexWeight:
-    vertex_index: int
-    weight: float
-
-    def __init__(self, vertex_index: int, weight: float) -> None: ...
+from typing import Optional, ClassVar, Tuple
+import numpy
+
+from xc3_model_py import RenderPassType
+
+
+class Weights:
+    weight_buffers: list[SkinWeights]
+
+    def __init__(self, weight_buffers: list[SkinWeights]) -> None: ...
+
+    def weight_buffer(self, flags2: int) -> Optional[SkinWeights]: ...
+
+    def weights_start_index(self, flags2: int, lod: int,
+                            unk_type: RenderPassType) -> int: ...
+
+
+class SkinWeights:
+    bone_indices: numpy.ndarray
+    weights: numpy.ndarray
+    bone_names: list[str]
+
+    def __init__(self, bone_indices: numpy.ndarray,
+                 weights: numpy.ndarray, bone_names: list[str]) -> None: ...
+
+    def to_influences(
+        self, weight_indices: numpy.ndarray) -> list[Influence]: ...
+
+
+class Influence:
+    bone_name: str
+    weights: list[VertexWeight]
+
+    def __init__(self, bone_name: str,
+                 weights: list[VertexWeight]) -> None: ...
+
+
+class VertexWeight:
+    vertex_index: int
+    weight: float
+
+    def __init__(self, vertex_index: int, weight: float) -> None: ...
```

## xc3_model_py/vertex.pyi

 * *Ordering differences only*

```diff
@@ -1,67 +1,67 @@
-from typing import Optional, ClassVar
-import numpy
-
-from xc3_model_py.skinning import Weights
-
-
-class ModelBuffers:
-    vertex_buffers: list[VertexBuffer]
-    index_buffers: list[IndexBuffer]
-    weights: Optional[Weights]
-
-    def __init__(self, vertex_buffers: list[VertexBuffer],
-                 index_buffers: list[IndexBuffer], weights: Optional[Weights]) -> None: ...
-
-
-class VertexBuffer:
-    attributes: list[AttributeData]
-    morph_targets: list[MorphTarget]
-    outline_buffer_index: Optional[int]
-
-    def __init__(self, attributes: list[AttributeData], morph_targets: list[MorphTarget],
-                 outline_buffer_index: Optional[int]) -> None: ...
-
-
-class AttributeData:
-    attribute_type: AttributeType
-    data: numpy.ndarray
-
-    def __init__(self, attribute_type: AttributeType,
-                 data: numpy.ndarray) -> None: ...
-
-
-class AttributeType:
-    Position: ClassVar[AttributeType]
-    Normal: ClassVar[AttributeType]
-    Tangent: ClassVar[AttributeType]
-    TexCoord0: ClassVar[AttributeType]
-    TexCoord1: ClassVar[AttributeType]
-    TexCoord2: ClassVar[AttributeType]
-    TexCoord3: ClassVar[AttributeType]
-    TexCoord4: ClassVar[AttributeType]
-    TexCoord5: ClassVar[AttributeType]
-    TexCoord6: ClassVar[AttributeType]
-    TexCoord7: ClassVar[AttributeType]
-    TexCoord8: ClassVar[AttributeType]
-    VertexColor: ClassVar[AttributeType]
-    Blend: ClassVar[AttributeType]
-    WeightIndex: ClassVar[AttributeType]
-    SkinWeights: ClassVar[AttributeType]
-    BoneIndices: ClassVar[AttributeType]
-
-
-class MorphTarget:
-    morph_controller_index: int
-    position_deltas: numpy.ndarray
-    normal_deltas: numpy.ndarray
-    tangent_deltas: numpy.ndarray
-    vertex_indices: numpy.ndarray
-
-    def __init__(self, morph_controller_index: int, position_deltas: numpy.ndarray,
-                 normal_deltas: numpy.ndarray, tangent_deltas: numpy.ndarray, vertex_indices: numpy.ndarray) -> None: ...
-
-
-class IndexBuffer:
-    indices: numpy.ndarray
-
-    def __init__(self, indices: numpy.ndarray) -> None: ...
+from typing import Optional, ClassVar
+import numpy
+
+from xc3_model_py.skinning import Weights
+
+
+class ModelBuffers:
+    vertex_buffers: list[VertexBuffer]
+    index_buffers: list[IndexBuffer]
+    weights: Optional[Weights]
+
+    def __init__(self, vertex_buffers: list[VertexBuffer],
+                 index_buffers: list[IndexBuffer], weights: Optional[Weights]) -> None: ...
+
+
+class VertexBuffer:
+    attributes: list[AttributeData]
+    morph_targets: list[MorphTarget]
+    outline_buffer_index: Optional[int]
+
+    def __init__(self, attributes: list[AttributeData], morph_targets: list[MorphTarget],
+                 outline_buffer_index: Optional[int]) -> None: ...
+
+
+class AttributeData:
+    attribute_type: AttributeType
+    data: numpy.ndarray
+
+    def __init__(self, attribute_type: AttributeType,
+                 data: numpy.ndarray) -> None: ...
+
+
+class AttributeType:
+    Position: ClassVar[AttributeType]
+    Normal: ClassVar[AttributeType]
+    Tangent: ClassVar[AttributeType]
+    TexCoord0: ClassVar[AttributeType]
+    TexCoord1: ClassVar[AttributeType]
+    TexCoord2: ClassVar[AttributeType]
+    TexCoord3: ClassVar[AttributeType]
+    TexCoord4: ClassVar[AttributeType]
+    TexCoord5: ClassVar[AttributeType]
+    TexCoord6: ClassVar[AttributeType]
+    TexCoord7: ClassVar[AttributeType]
+    TexCoord8: ClassVar[AttributeType]
+    VertexColor: ClassVar[AttributeType]
+    Blend: ClassVar[AttributeType]
+    WeightIndex: ClassVar[AttributeType]
+    SkinWeights: ClassVar[AttributeType]
+    BoneIndices: ClassVar[AttributeType]
+
+
+class MorphTarget:
+    morph_controller_index: int
+    position_deltas: numpy.ndarray
+    normal_deltas: numpy.ndarray
+    tangent_deltas: numpy.ndarray
+    vertex_indices: numpy.ndarray
+
+    def __init__(self, morph_controller_index: int, position_deltas: numpy.ndarray,
+                 normal_deltas: numpy.ndarray, tangent_deltas: numpy.ndarray, vertex_indices: numpy.ndarray) -> None: ...
+
+
+class IndexBuffer:
+    indices: numpy.ndarray
+
+    def __init__(self, indices: numpy.ndarray) -> None: ...
```

## xc3_model_py/__init__.pyi

 * *Ordering differences only*

```diff
@@ -1,306 +1,306 @@
-from typing import Optional, ClassVar, Tuple
-import numpy
-
-from . import animation
-from . import skinning
-from . import vertex
-
-
-def load_model(wimdo_path: str, database_path: Optional[str]) -> ModelRoot: ...
-
-
-def load_model_legacy(camdo_path) -> ModelRoot: ...
-
-
-def load_map(wismhd: str, database_path: Optional[str]) -> list[MapRoot]: ...
-
-
-def load_animations(anim_path: str) -> list[animation.Animation]: ...
-
-
-class Xc3ModelError(Exception):
-    pass
-
-
-class ModelRoot:
-    models: Models
-    buffers: vertex.ModelBuffers
-    image_textures: list[ImageTexture]
-    skeleton: Optional[Skeleton]
-
-    def __init__(self, models: Models, buffers: vertex.ModelBuffers,
-                 image_textures: list[ImageTexture], skeleton: Optional[Skeleton]) -> None: ...
-
-    def decode_images_rgbaf32(self) -> list[numpy.ndarray]: ...
-
-    def save_images_rgba8(self, folder: str, prefix: str,
-                          ext: str, flip_vertical: bool) -> list[str]: ...
-
-    def to_mxmd_model(self, mxmd: Mxmd, msrd: Msrd) -> Tuple[Mxmd, Msrd]: ...
-
-
-class MapRoot:
-    groups: list[ModelGroup]
-    image_textures: list[ImageTexture]
-
-    def __init__(self, groups: list[ModelGroup],
-                 image_textures: list[ImageTexture]) -> None: ...
-
-    def decode_images_rgbaf32(self) -> list[numpy.ndarray]: ...
-
-    def save_images_rgba8(self, folder: str, prefix: str,
-                          ext: str, flip_vertical: bool) -> list[str]: ...
-
-
-class ModelGroup:
-    models: list[Models]
-    buffers: list[vertex.ModelBuffers]
-
-    def __init__(self, models: list[Models],
-                 buffers: list[vertex.ModelBuffers]) -> None: ...
-
-
-class Models:
-    models: list[Model]
-    materials: list[Material]
-    samplers: list[Sampler]
-    base_lod_indices: Optional[list[int]]
-    morph_controller_names: list[str]
-    animation_morph_names: list[str]
-    max_xyz: list[float]
-    min_xyz: list[float]
-
-    def __init__(self, models: list[Model], materials: list[Material], samplers: list[Sampler], max_xyz: list[float], min_xyz: list[float],
-                 morph_controller_names: list[str], animation_morph_names: list[str], base_lod_indices: Optional[list[int]]) -> None: ...
-
-
-class Model:
-    meshes: list[Mesh]
-    instances: numpy.ndarray
-    model_buffers_index: int
-    max_xyz: list[float]
-    min_xyz: list[float]
-    bounding_radius: float
-
-    def __init__(self, meshes: list[Mesh], instances: numpy.ndarray, model_buffers_index: int,
-                 max_xyz: list[float], min_xyz: list[float], bounding_radius: float) -> None: ...
-
-
-class Mesh:
-    vertex_buffer_index: int
-    index_buffer_index: int
-    material_index: int
-    lod: int
-    flags1: int
-    flags2: int
-
-    def __init__(self, vertex_buffer_index: int, index_buffer_index: int,
-                 material_index: int, lod: int, flags1: int, flags2: int) -> None: ...
-
-
-class Skeleton:
-    bones: list[Bone]
-
-    def __init__(self, bones: list[Bone]) -> None: ...
-
-    def model_space_transforms(self) -> numpy.ndarray: ...
-
-
-class Bone:
-    name: str
-    transform: numpy.ndarray
-    parent_index: Optional[int]
-
-    def __init__(self, name: str, transform: numpy.ndarray,
-                 parent_index: Optional[int]) -> None: ...
-
-
-class Material:
-    name: str
-    textures: list[Texture]
-    alpha_test: Optional[TextureAlphaTest]
-    shader: Optional[Shader]
-    pass_type: RenderPassType
-
-    def __init__(self, name: str, textures: list[Texture], pass_type: RenderPassType,
-                 alpha_test: Optional[TextureAlphaTest], shader: Optional[Shader], ) -> None: ...
-
-    def output_assignments(
-        self, textures: list[ImageTexture]) -> OutputAssignments: ...
-
-
-class RenderPassType:
-    Unk0: ClassVar[RenderPassType]
-    Unk1: ClassVar[RenderPassType]
-    Unk6: ClassVar[RenderPassType]
-    Unk7: ClassVar[RenderPassType]
-    Unk9: ClassVar[RenderPassType]
-
-
-class TextureAlphaTest:
-    texture_index: int
-    channel_index: int
-    ref_value: float
-
-    def __init__(self, texture_index: int, channel_index: int,
-                 ref_value: float) -> None: ...
-
-
-class MaterialParameters:
-    mat_color: list[float]
-    alpha_test_ref: float
-    tex_matrix: Optional[list[float]]
-    work_float4: Optional[list[float]]
-    work_color: Optional[list[float]]
-
-    def __init__(self, mat_color: list[float], alpha_test_ref: float, tex_matrix: Optional[list[float]],
-                 work_float4: Optional[list[float]], work_color: Optional[list[float]]) -> None: ...
-
-
-class Shader:
-    pass
-
-
-class Texture:
-    image_texture_index: int
-    sampler_index: int
-
-    def __init__(self, image_texture_index: int,
-                 sampler_index: int) -> None: ...
-
-
-class ImageTexture:
-    name: Optional[str]
-    usage: Optional[TextureUsage]
-    width: int
-    height: int
-    depth: int
-    view_dimension: ViewDimension
-    image_format: ImageFormat
-    mipmap_count: int
-    image_data: bytes
-
-    def __init__(self, width: int,  height: int,  depth: int, view_dimension: ViewDimension,  image_format: ImageFormat,
-                 mipmap_count: int,  image_data: bytes, name: Optional[str], usage: Optional[TextureUsage]) -> None: ...
-
-
-class TextureUsage:
-    Unk0: ClassVar[TextureUsage]
-    Temp: ClassVar[TextureUsage]
-    Unk6: ClassVar[TextureUsage]
-    Nrm: ClassVar[TextureUsage]
-    Unk13: ClassVar[TextureUsage]
-    WavePlus: ClassVar[TextureUsage]
-    Col: ClassVar[TextureUsage]
-    Unk8: ClassVar[TextureUsage]
-    Alp: ClassVar[TextureUsage]
-    Unk: ClassVar[TextureUsage]
-    Alp2: ClassVar[TextureUsage]
-    Col2: ClassVar[TextureUsage]
-    Unk11: ClassVar[TextureUsage]
-    Unk9: ClassVar[TextureUsage]
-    Alp3: ClassVar[TextureUsage]
-    Nrm2: ClassVar[TextureUsage]
-    Col3: ClassVar[TextureUsage]
-    Unk3: ClassVar[TextureUsage]
-    Unk2: ClassVar[TextureUsage]
-    Unk20: ClassVar[TextureUsage]
-    Unk17: ClassVar[TextureUsage]
-    F01: ClassVar[TextureUsage]
-    Unk4: ClassVar[TextureUsage]
-    Unk7: ClassVar[TextureUsage]
-    Unk15: ClassVar[TextureUsage]
-    Temp2: ClassVar[TextureUsage]
-    Unk14: ClassVar[TextureUsage]
-    Col4: ClassVar[TextureUsage]
-    Alp4: ClassVar[TextureUsage]
-    Unk12: ClassVar[TextureUsage]
-    Unk18: ClassVar[TextureUsage]
-    Unk19: ClassVar[TextureUsage]
-    Unk5: ClassVar[TextureUsage]
-    Unk10: ClassVar[TextureUsage]
-    VolTex: ClassVar[TextureUsage]
-    Unk1: ClassVar[TextureUsage]
-
-
-class ViewDimension:
-    D2: ClassVar[ViewDimension]
-    D3: ClassVar[ViewDimension]
-    Cube: ClassVar[ViewDimension]
-
-
-class ImageFormat:
-    R8Unorm: ClassVar[ImageFormat]
-    R8G8B8A8Unorm: ClassVar[ImageFormat]
-    R4G4B4A4Unorm: ClassVar[ImageFormat]
-    R16G16B16A16Float: ClassVar[ImageFormat]
-    BC1Unorm: ClassVar[ImageFormat]
-    BC2Unorm: ClassVar[ImageFormat]
-    BC3Unorm: ClassVar[ImageFormat]
-    BC4Unorm: ClassVar[ImageFormat]
-    BC5Unorm: ClassVar[ImageFormat]
-    BC56UFloat: ClassVar[ImageFormat]
-    BC7Unorm: ClassVar[ImageFormat]
-    B8G8R8A8Unorm: ClassVar[ImageFormat]
-
-
-class Sampler:
-    address_mode_u: AddressMode
-    address_mode_v: AddressMode
-    address_mode_w: AddressMode
-    min_filter: FilterMode
-    mag_filter: FilterMode
-    mip_filter: FilterMode
-    mipmaps: bool
-
-    def __init__(self, address_mode_u: AddressMode, address_mode_v: AddressMode, address_mode_w: AddressMode,
-                 min_filter: FilterMode, mag_filter: FilterMode, mip_filter: FilterMode, mipmaps: bool) -> None: ...
-
-
-class AddressMode:
-    ClampToEdge: ClassVar[AddressMode]
-    Repeat: ClassVar[AddressMode]
-    MirrorRepeat: ClassVar[AddressMode]
-
-
-class FilterMode:
-    Nearest: ClassVar[FilterMode]
-    Linear: ClassVar[FilterMode]
-
-
-class OutputAssignments:
-    assignments: list[OutputAssignment]
-
-
-class OutputAssignment:
-    x: Optional[ChannelAssignment]
-    y: Optional[ChannelAssignment]
-    z: Optional[ChannelAssignment]
-    w: Optional[ChannelAssignment]
-
-
-class ChannelAssignment:
-    def texture(self) -> Optional[ChannelAssignmentTexture]: ...
-
-    def value(self) -> Optional[float]: ...
-
-
-class ChannelAssignmentTexture:
-    name: str
-    channel_index: int
-    texcoord_name: Optional[str]
-    texcoord_scale: Optional[Tuple[float, float]]
-
-
-class Mxmd:
-    @staticmethod
-    def from_file(path: str) -> Mxmd: ...
-
-    def save(self, path: str): ...
-
-
-class Msrd:
-    @staticmethod
-    def from_file(path: str) -> Msrd: ...
-
-    def save(self, path: str): ...
+from typing import Optional, ClassVar, Tuple
+import numpy
+
+from . import animation
+from . import skinning
+from . import vertex
+
+
+def load_model(wimdo_path: str, database_path: Optional[str]) -> ModelRoot: ...
+
+
+def load_model_legacy(camdo_path) -> ModelRoot: ...
+
+
+def load_map(wismhd: str, database_path: Optional[str]) -> list[MapRoot]: ...
+
+
+def load_animations(anim_path: str) -> list[animation.Animation]: ...
+
+
+class Xc3ModelError(Exception):
+    pass
+
+
+class ModelRoot:
+    models: Models
+    buffers: vertex.ModelBuffers
+    image_textures: list[ImageTexture]
+    skeleton: Optional[Skeleton]
+
+    def __init__(self, models: Models, buffers: vertex.ModelBuffers,
+                 image_textures: list[ImageTexture], skeleton: Optional[Skeleton]) -> None: ...
+
+    def decode_images_rgbaf32(self) -> list[numpy.ndarray]: ...
+
+    def save_images_rgba8(self, folder: str, prefix: str,
+                          ext: str, flip_vertical: bool) -> list[str]: ...
+
+    def to_mxmd_model(self, mxmd: Mxmd, msrd: Msrd) -> Tuple[Mxmd, Msrd]: ...
+
+
+class MapRoot:
+    groups: list[ModelGroup]
+    image_textures: list[ImageTexture]
+
+    def __init__(self, groups: list[ModelGroup],
+                 image_textures: list[ImageTexture]) -> None: ...
+
+    def decode_images_rgbaf32(self) -> list[numpy.ndarray]: ...
+
+    def save_images_rgba8(self, folder: str, prefix: str,
+                          ext: str, flip_vertical: bool) -> list[str]: ...
+
+
+class ModelGroup:
+    models: list[Models]
+    buffers: list[vertex.ModelBuffers]
+
+    def __init__(self, models: list[Models],
+                 buffers: list[vertex.ModelBuffers]) -> None: ...
+
+
+class Models:
+    models: list[Model]
+    materials: list[Material]
+    samplers: list[Sampler]
+    base_lod_indices: Optional[list[int]]
+    morph_controller_names: list[str]
+    animation_morph_names: list[str]
+    max_xyz: list[float]
+    min_xyz: list[float]
+
+    def __init__(self, models: list[Model], materials: list[Material], samplers: list[Sampler], max_xyz: list[float], min_xyz: list[float],
+                 morph_controller_names: list[str], animation_morph_names: list[str], base_lod_indices: Optional[list[int]]) -> None: ...
+
+
+class Model:
+    meshes: list[Mesh]
+    instances: numpy.ndarray
+    model_buffers_index: int
+    max_xyz: list[float]
+    min_xyz: list[float]
+    bounding_radius: float
+
+    def __init__(self, meshes: list[Mesh], instances: numpy.ndarray, model_buffers_index: int,
+                 max_xyz: list[float], min_xyz: list[float], bounding_radius: float) -> None: ...
+
+
+class Mesh:
+    vertex_buffer_index: int
+    index_buffer_index: int
+    material_index: int
+    lod: int
+    flags1: int
+    flags2: int
+
+    def __init__(self, vertex_buffer_index: int, index_buffer_index: int,
+                 material_index: int, lod: int, flags1: int, flags2: int) -> None: ...
+
+
+class Skeleton:
+    bones: list[Bone]
+
+    def __init__(self, bones: list[Bone]) -> None: ...
+
+    def model_space_transforms(self) -> numpy.ndarray: ...
+
+
+class Bone:
+    name: str
+    transform: numpy.ndarray
+    parent_index: Optional[int]
+
+    def __init__(self, name: str, transform: numpy.ndarray,
+                 parent_index: Optional[int]) -> None: ...
+
+
+class Material:
+    name: str
+    textures: list[Texture]
+    alpha_test: Optional[TextureAlphaTest]
+    shader: Optional[Shader]
+    pass_type: RenderPassType
+
+    def __init__(self, name: str, textures: list[Texture], pass_type: RenderPassType,
+                 alpha_test: Optional[TextureAlphaTest], shader: Optional[Shader], ) -> None: ...
+
+    def output_assignments(
+        self, textures: list[ImageTexture]) -> OutputAssignments: ...
+
+
+class RenderPassType:
+    Unk0: ClassVar[RenderPassType]
+    Unk1: ClassVar[RenderPassType]
+    Unk6: ClassVar[RenderPassType]
+    Unk7: ClassVar[RenderPassType]
+    Unk9: ClassVar[RenderPassType]
+
+
+class TextureAlphaTest:
+    texture_index: int
+    channel_index: int
+    ref_value: float
+
+    def __init__(self, texture_index: int, channel_index: int,
+                 ref_value: float) -> None: ...
+
+
+class MaterialParameters:
+    mat_color: list[float]
+    alpha_test_ref: float
+    tex_matrix: Optional[list[float]]
+    work_float4: Optional[list[float]]
+    work_color: Optional[list[float]]
+
+    def __init__(self, mat_color: list[float], alpha_test_ref: float, tex_matrix: Optional[list[float]],
+                 work_float4: Optional[list[float]], work_color: Optional[list[float]]) -> None: ...
+
+
+class Shader:
+    pass
+
+
+class Texture:
+    image_texture_index: int
+    sampler_index: int
+
+    def __init__(self, image_texture_index: int,
+                 sampler_index: int) -> None: ...
+
+
+class ImageTexture:
+    name: Optional[str]
+    usage: Optional[TextureUsage]
+    width: int
+    height: int
+    depth: int
+    view_dimension: ViewDimension
+    image_format: ImageFormat
+    mipmap_count: int
+    image_data: bytes
+
+    def __init__(self, width: int,  height: int,  depth: int, view_dimension: ViewDimension,  image_format: ImageFormat,
+                 mipmap_count: int,  image_data: bytes, name: Optional[str], usage: Optional[TextureUsage]) -> None: ...
+
+
+class TextureUsage:
+    Unk0: ClassVar[TextureUsage]
+    Temp: ClassVar[TextureUsage]
+    Unk6: ClassVar[TextureUsage]
+    Nrm: ClassVar[TextureUsage]
+    Unk13: ClassVar[TextureUsage]
+    WavePlus: ClassVar[TextureUsage]
+    Col: ClassVar[TextureUsage]
+    Unk8: ClassVar[TextureUsage]
+    Alp: ClassVar[TextureUsage]
+    Unk: ClassVar[TextureUsage]
+    Alp2: ClassVar[TextureUsage]
+    Col2: ClassVar[TextureUsage]
+    Unk11: ClassVar[TextureUsage]
+    Unk9: ClassVar[TextureUsage]
+    Alp3: ClassVar[TextureUsage]
+    Nrm2: ClassVar[TextureUsage]
+    Col3: ClassVar[TextureUsage]
+    Unk3: ClassVar[TextureUsage]
+    Unk2: ClassVar[TextureUsage]
+    Unk20: ClassVar[TextureUsage]
+    Unk17: ClassVar[TextureUsage]
+    F01: ClassVar[TextureUsage]
+    Unk4: ClassVar[TextureUsage]
+    Unk7: ClassVar[TextureUsage]
+    Unk15: ClassVar[TextureUsage]
+    Temp2: ClassVar[TextureUsage]
+    Unk14: ClassVar[TextureUsage]
+    Col4: ClassVar[TextureUsage]
+    Alp4: ClassVar[TextureUsage]
+    Unk12: ClassVar[TextureUsage]
+    Unk18: ClassVar[TextureUsage]
+    Unk19: ClassVar[TextureUsage]
+    Unk5: ClassVar[TextureUsage]
+    Unk10: ClassVar[TextureUsage]
+    VolTex: ClassVar[TextureUsage]
+    Unk1: ClassVar[TextureUsage]
+
+
+class ViewDimension:
+    D2: ClassVar[ViewDimension]
+    D3: ClassVar[ViewDimension]
+    Cube: ClassVar[ViewDimension]
+
+
+class ImageFormat:
+    R8Unorm: ClassVar[ImageFormat]
+    R8G8B8A8Unorm: ClassVar[ImageFormat]
+    R4G4B4A4Unorm: ClassVar[ImageFormat]
+    R16G16B16A16Float: ClassVar[ImageFormat]
+    BC1Unorm: ClassVar[ImageFormat]
+    BC2Unorm: ClassVar[ImageFormat]
+    BC3Unorm: ClassVar[ImageFormat]
+    BC4Unorm: ClassVar[ImageFormat]
+    BC5Unorm: ClassVar[ImageFormat]
+    BC56UFloat: ClassVar[ImageFormat]
+    BC7Unorm: ClassVar[ImageFormat]
+    B8G8R8A8Unorm: ClassVar[ImageFormat]
+
+
+class Sampler:
+    address_mode_u: AddressMode
+    address_mode_v: AddressMode
+    address_mode_w: AddressMode
+    min_filter: FilterMode
+    mag_filter: FilterMode
+    mip_filter: FilterMode
+    mipmaps: bool
+
+    def __init__(self, address_mode_u: AddressMode, address_mode_v: AddressMode, address_mode_w: AddressMode,
+                 min_filter: FilterMode, mag_filter: FilterMode, mip_filter: FilterMode, mipmaps: bool) -> None: ...
+
+
+class AddressMode:
+    ClampToEdge: ClassVar[AddressMode]
+    Repeat: ClassVar[AddressMode]
+    MirrorRepeat: ClassVar[AddressMode]
+
+
+class FilterMode:
+    Nearest: ClassVar[FilterMode]
+    Linear: ClassVar[FilterMode]
+
+
+class OutputAssignments:
+    assignments: list[OutputAssignment]
+
+
+class OutputAssignment:
+    x: Optional[ChannelAssignment]
+    y: Optional[ChannelAssignment]
+    z: Optional[ChannelAssignment]
+    w: Optional[ChannelAssignment]
+
+
+class ChannelAssignment:
+    def texture(self) -> Optional[ChannelAssignmentTexture]: ...
+
+    def value(self) -> Optional[float]: ...
+
+
+class ChannelAssignmentTexture:
+    name: str
+    channel_index: int
+    texcoord_name: Optional[str]
+    texcoord_scale: Optional[Tuple[float, float]]
+
+
+class Mxmd:
+    @staticmethod
+    def from_file(path: str) -> Mxmd: ...
+
+    def save(self, path: str): ...
+
+
+class Msrd:
+    @staticmethod
+    def from_file(path: str) -> Msrd: ...
+
+    def save(self, path: str): ...
```

## Comparing `xc3_model_py-0.5.0.dist-info/METADATA` & `xc3_model_py-0.5.1.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,141 +1,141 @@
 Metadata-Version: 2.3
 Name: xc3_model_py
-Version: 0.5.0
+Version: 0.5.1
 Author: ScanMountGoat
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
-# xc3_model_py [![PyPI](https://img.shields.io/pypi/v/xc3_model_py)](https://pypi.org/project/xc3_model_py/)
-Python bindings to [xc3_model](https://github.com/ScanMountGoat/xc3_lib) for high level and efficient data access to model files for Xenoblade 1 DE, Xenoblade 2, and Xenoblade 3.
-
-## Installation
-The package can be installed for Python version 3.9, 3.10, 3.11, or 3.12 using pip on newer versions of Windows, Linux, or MacOS. The prebuilt wheels (.whl files) are included only for situations where pip might not be available such as for plugin development for applications. The wheels are zip archives and can be extracted to obtain the compiled .pyd or .so file. xc3_model_py requires the `numpy` package for transforms and vertex data.
-
-Installing: `pip install xc3_model_py`  
-Updating: `pip install xc3_model_py --upgrade`
-
-## Introduction
-Parsing and processing happens in optimized Rust code when calling `xc3_model_py.load_map` or `xc3_model_py.load_model`. All characters, models, and maps are converted to the same scene hierarchy representation. This avoids needing to add any special handling for maps vs characters. Pregenerated shader JSON databases are available from [xc3_lib](https://github.com/ScanMountGoat/xc3_lib/releases). For more advanced usage, see [xenoblade_blender](https://github.com/ScanMountGoat/xenoblade_blender).
-
-```python
-import xc3_model_py
-
-# Get a list of MapRoot.
-roots = xc3_model_py.load_map("xenoblade3_dump/map/ma59a.wismhd", database_path="xc3.json")
-for root in roots:
-    for group in root.groups:
-        for models in group.models:
-            for material in models.materials:
-                print(material.name)
-                # The shader contains assignment information when specifying a JSON database.
-
-            for model in models.models:
-                buffers = group.buffers[model.model_buffers_index]
-
-                # prints (num_instances, 4, 4)
-                print(len(model.instances.shape))
-```
-
-```python
-# This returns only a single ModelRoot.
-root = xc3_model_py.load_model("xenoblade3_dump/chr/chr/01012013.wimdo", database_path="xc3.json")
-for material in root.models.materials:
-    print(material.name)
-
-for model in root.models.models:
-    # prints (1, 4, 4)
-    print(len(model.instances.shape))
-
-    # Access vertex and index data for this model.
-    buffers = root.buffers
-    for buffer in buffers.vertex_buffers:
-        for attribute in buffer.attributes:
-            print(attribute.attribute_type, attribute.data.shape)
-
-    # Access vertex skinning data for each mesh.
-    for mesh in model.meshes:
-        vertex_buffer = buffers.vertex_buffers[mesh.vertex_buffer_index]
-
-        if buffers.weights is not None:
-            # Calculate the index offset based on the weight group for this mesh.
-            pass_type = root.models.materials[mesh.material_index].pass_type
-            start_index = buffers.weights.weights_start_index(mesh.flags2, mesh.lod, pass_type)
-
-            weight_buffer = buffers.weights.weight_buffer(mesh.flags2)
-            if weight_buffer is not None:
-                # Get vertex skinning attributes.
-                for attribute in vertex_buffer.attributes:
-                    if attribute.attribute_type == xc3_model_py.vertex.AttributeType.WeightIndex:
-                        # Find the actual per vertex skinning information.
-                        weight_indices = attribute.data[:, 0] + start_index
-                        skin_weights = weight_buffer.weights[weight_indices]
-                        # Note that these indices index into a different bone list than the skeleton.
-                        bone_indices = weight_buffer.bone_indices[weight_indices, 0]
-                        bone_name = weight_buffer.bone_names[bone_indices[0]]
-```
-
-Certain types like matrices and vertex atribute data are stored using `numpy.ndarray`. All transformation matrices are column-major to match the Rust code in xc3_model. This greatly reduces conversion overhead and allows for more optimized Python code. xc3_model_py requires the numpy package to be installed. Blender already provides the numpy package, enabling the use of functions like `foreach_get` and `foreach_set` for efficient property access.
-
-```python
-# blender
-blender_mesh.vertices.add(positions_array.shape[0])
-blender_mesh.vertices.foreach_set('co', positions_array.reshape(-1))
-```
-
-Animations can be loaded from a file all at once. The track type is currently opaque, meaning that implementation details are not exposed. The values can be sampled at the desired frame using the appropriate methods.
-
-```python
-import xc3_model_py
-
-path = "xenoblade3_dump/chr/ch/ch01027000_event.mot"
-animations = xc3_model_py.load_animations(path)
-
-for animation in animations:
-    print(animation.name, animation.space_mode, animation.play_mode, animation.blend_mode)
-    print(f'frames: {animation.frame_count}, tracks: {len(animation.tracks)}')
-
-    track = animation.tracks[0]
-
-    # Each track references a bone in one of three ways.
-    bone_index = track.bone_index()
-    bone_hash = track.bone_hash()
-    bone_name = track.bone_name()
-    if bone_index is not None:
-        pass
-    elif bone_hash is not None:
-        # Use xc3_model_py.murmur3(bone_name) for hashing the skeleton bones.
-        pass
-    elif bone_name is not None:
-        pass
-
-    # Sample the transform for a given track at each frame.
-    # This essentially "bakes" the keyframes of the animation.
-    for frame in range(animation.frame_count:)
-        print(track.sample_scale(frame))
-        print(track.sample_rotation(frame))
-        print(track.sample_translation(frame))
-    print()
-```
-
-xc3_model_py enables Rust log output by default to use with Python's `logging` module.
-Logging can be disabled entirely if not needed using `logging.disable()`.
-
-```python
-import logging
-
-# Configure log messages to include more information.
-FORMAT = '%(levelname)s %(name)s %(filename)s:%(lineno)d %(message)s'
-logging.basicConfig(format=FORMAT, level=logging.INFO)
-```
-
-## Documentation
-See the [pyi stub file](https://github.com/ScanMountGoat/xc3_model_py/blob/main/xc3_model_py/__init__.pyi) for complete function and type information. This also enables autocomplete in supported editors like the Python extension for VSCode. The Python API attempts to match the Rust functions and types in xc3_model as closely as possible. 
-
-## Installation
-The compiled extension module can be imported just like any other Python file. On Windows, rename `xc3_model_py.dll` to `xc3_model_py.pyd`. If importing `xc3_model_py` fails, make sure the import path is specified correctly and the current Python version matches the version used when building. For installing in the current Python environment, install [maturin](https://github.com/PyO3/maturin) and use `maturin develop --release`.
-
-## Building
-Build the project with `cargo build --release`. This will compile a native python module for the current Python interpreter. For use with Blender, make sure to build for the Python version used by Blender. This can be achieved by activating a virtual environment with the appropriate Python version or setting the Python interpeter using the `PYO3_PYTHON` environment variable. See the [PyO3 guide](https://pyo3.rs) for details.
-
-## Limitations
-Some types from `xc3_model_py` are opaque wrappers around the underlying Rust types and cannot be constructed in any way from Python. Some of these limitations should hopefully be resolved in the future.
+# xc3_model_py [![PyPI](https://img.shields.io/pypi/v/xc3_model_py)](https://pypi.org/project/xc3_model_py/)
+Python bindings to [xc3_model](https://github.com/ScanMountGoat/xc3_lib) for high level and efficient data access to model files for Xenoblade 1 DE, Xenoblade 2, and Xenoblade 3.
+
+## Installation
+The package can be installed for Python version 3.9, 3.10, 3.11, or 3.12 using pip on newer versions of Windows, Linux, or MacOS. The prebuilt wheels (.whl files) are included only for situations where pip might not be available such as for plugin development for applications. The wheels are zip archives and can be extracted to obtain the compiled .pyd or .so file. xc3_model_py requires the `numpy` package for transforms and vertex data.
+
+Installing: `pip install xc3_model_py`  
+Updating: `pip install xc3_model_py --upgrade`
+
+## Introduction
+Parsing and processing happens in optimized Rust code when calling `xc3_model_py.load_map` or `xc3_model_py.load_model`. All characters, models, and maps are converted to the same scene hierarchy representation. This avoids needing to add any special handling for maps vs characters. Pregenerated shader JSON databases are available from [xc3_lib](https://github.com/ScanMountGoat/xc3_lib/releases). For more advanced usage, see [xenoblade_blender](https://github.com/ScanMountGoat/xenoblade_blender).
+
+```python
+import xc3_model_py
+
+# Get a list of MapRoot.
+roots = xc3_model_py.load_map("xenoblade3_dump/map/ma59a.wismhd", database_path="xc3.json")
+for root in roots:
+    for group in root.groups:
+        for models in group.models:
+            for material in models.materials:
+                print(material.name)
+                # The shader contains assignment information when specifying a JSON database.
+
+            for model in models.models:
+                buffers = group.buffers[model.model_buffers_index]
+
+                # prints (num_instances, 4, 4)
+                print(len(model.instances.shape))
+```
+
+```python
+# This returns only a single ModelRoot.
+root = xc3_model_py.load_model("xenoblade3_dump/chr/chr/01012013.wimdo", database_path="xc3.json")
+for material in root.models.materials:
+    print(material.name)
+
+for model in root.models.models:
+    # prints (1, 4, 4)
+    print(len(model.instances.shape))
+
+    # Access vertex and index data for this model.
+    buffers = root.buffers
+    for buffer in buffers.vertex_buffers:
+        for attribute in buffer.attributes:
+            print(attribute.attribute_type, attribute.data.shape)
+
+    # Access vertex skinning data for each mesh.
+    for mesh in model.meshes:
+        vertex_buffer = buffers.vertex_buffers[mesh.vertex_buffer_index]
+
+        if buffers.weights is not None:
+            # Calculate the index offset based on the weight group for this mesh.
+            pass_type = root.models.materials[mesh.material_index].pass_type
+            start_index = buffers.weights.weights_start_index(mesh.flags2, mesh.lod, pass_type)
+
+            weight_buffer = buffers.weights.weight_buffer(mesh.flags2)
+            if weight_buffer is not None:
+                # Get vertex skinning attributes.
+                for attribute in vertex_buffer.attributes:
+                    if attribute.attribute_type == xc3_model_py.vertex.AttributeType.WeightIndex:
+                        # Find the actual per vertex skinning information.
+                        weight_indices = attribute.data[:, 0] + start_index
+                        skin_weights = weight_buffer.weights[weight_indices]
+                        # Note that these indices index into a different bone list than the skeleton.
+                        bone_indices = weight_buffer.bone_indices[weight_indices, 0]
+                        bone_name = weight_buffer.bone_names[bone_indices[0]]
+```
+
+Certain types like matrices and vertex atribute data are stored using `numpy.ndarray`. All transformation matrices are column-major to match the Rust code in xc3_model. This greatly reduces conversion overhead and allows for more optimized Python code. xc3_model_py requires the numpy package to be installed. Blender already provides the numpy package, enabling the use of functions like `foreach_get` and `foreach_set` for efficient property access.
+
+```python
+# blender
+blender_mesh.vertices.add(positions_array.shape[0])
+blender_mesh.vertices.foreach_set('co', positions_array.reshape(-1))
+```
+
+Animations can be loaded from a file all at once. The track type is currently opaque, meaning that implementation details are not exposed. The values can be sampled at the desired frame using the appropriate methods.
+
+```python
+import xc3_model_py
+
+path = "xenoblade3_dump/chr/ch/ch01027000_event.mot"
+animations = xc3_model_py.load_animations(path)
+
+for animation in animations:
+    print(animation.name, animation.space_mode, animation.play_mode, animation.blend_mode)
+    print(f'frames: {animation.frame_count}, tracks: {len(animation.tracks)}')
+
+    track = animation.tracks[0]
+
+    # Each track references a bone in one of three ways.
+    bone_index = track.bone_index()
+    bone_hash = track.bone_hash()
+    bone_name = track.bone_name()
+    if bone_index is not None:
+        pass
+    elif bone_hash is not None:
+        # Use xc3_model_py.murmur3(bone_name) for hashing the skeleton bones.
+        pass
+    elif bone_name is not None:
+        pass
+
+    # Sample the transform for a given track at each frame.
+    # This essentially "bakes" the keyframes of the animation.
+    for frame in range(animation.frame_count:)
+        print(track.sample_scale(frame))
+        print(track.sample_rotation(frame))
+        print(track.sample_translation(frame))
+    print()
+```
+
+xc3_model_py enables Rust log output by default to use with Python's `logging` module.
+Logging can be disabled entirely if not needed using `logging.disable()`.
+
+```python
+import logging
+
+# Configure log messages to include more information.
+FORMAT = '%(levelname)s %(name)s %(filename)s:%(lineno)d %(message)s'
+logging.basicConfig(format=FORMAT, level=logging.INFO)
+```
+
+## Documentation
+See the [pyi stub file](https://github.com/ScanMountGoat/xc3_model_py/blob/main/xc3_model_py/__init__.pyi) for complete function and type information. This also enables autocomplete in supported editors like the Python extension for VSCode. The Python API attempts to match the Rust functions and types in xc3_model as closely as possible. 
+
+## Installation
+The compiled extension module can be imported just like any other Python file. On Windows, rename `xc3_model_py.dll` to `xc3_model_py.pyd`. If importing `xc3_model_py` fails, make sure the import path is specified correctly and the current Python version matches the version used when building. For installing in the current Python environment, install [maturin](https://github.com/PyO3/maturin) and use `maturin develop --release`.
+
+## Building
+Build the project with `cargo build --release`. This will compile a native python module for the current Python interpreter. For use with Blender, make sure to build for the Python version used by Blender. This can be achieved by activating a virtual environment with the appropriate Python version or setting the Python interpeter using the `PYO3_PYTHON` environment variable. See the [PyO3 guide](https://pyo3.rs) for details.
+
+## Limitations
+Some types from `xc3_model_py` are opaque wrappers around the underlying Rust types and cannot be constructed in any way from Python. Some of these limitations should hopefully be resolved in the future.
```

