# Comparing `tmp/xc3_model_py-0.4.0-cp39-none-win_amd64.whl.zip` & `tmp/xc3_model_py-0.5.0-cp39-cp39-manylinux_2_34_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,11 @@
-Zip file size: 2109850 bytes, number of entries: 6
--rw-r--r--  4.6 unx     8266 b- defN 24-Mar-15 16:28 xc3_model_py-0.4.0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-Mar-15 16:28 xc3_model_py-0.4.0.dist-info/WHEEL
--rw-r--r--  4.6 unx       27 b- defN 24-Mar-15 16:28 xc3_model_py/__init__.py
--rw-r--r--  4.6 unx     6606 b- defN 24-Mar-15 16:28 xc3_model_py/__init__.pyi
--rwxr-xr-x  4.6 unx  5929472 b- defN 24-Mar-15 16:28 xc3_model_py/xc3_model_py.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      486 b- defN 24-Mar-15 16:28 xc3_model_py-0.4.0.dist-info/RECORD
-6 files, 5944951 bytes uncompressed, 2108974 bytes compressed:  64.5%
+Zip file size: 2825427 bytes, number of entries: 9
+-rw-r--r--  4.6 unx     7650 b- defN 24-Apr-29 15:45 xc3_model_py-0.5.0.dist-info/METADATA
+-rw-r--r--  4.6 unx      106 b- defN 24-Apr-29 15:45 xc3_model_py-0.5.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1689 b- defN 24-Apr-29 15:45 xc3_model_py/animation.pyi
+-rw-r--r--  4.6 unx     1053 b- defN 24-Apr-29 15:45 xc3_model_py/skinning.pyi
+-rw-r--r--  4.6 unx       27 b- defN 24-Apr-29 15:45 xc3_model_py/__init__.py
+-rw-r--r--  4.6 unx     2044 b- defN 24-Apr-29 15:45 xc3_model_py/vertex.pyi
+-rw-r--r--  4.6 unx     8369 b- defN 24-Apr-29 15:45 xc3_model_py/__init__.pyi
+-rwxr-xr-x  4.6 unx  8605896 b- defN 24-Apr-29 15:45 xc3_model_py/xc3_model_py.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  4.6 unx      744 b- defN 24-Apr-29 15:45 xc3_model_py-0.5.0.dist-info/RECORD
+9 files, 8627578 bytes uncompressed, 2824151 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -1,19 +1,28 @@
-Filename: xc3_model_py-0.4.0.dist-info/METADATA
+Filename: xc3_model_py-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: xc3_model_py-0.4.0.dist-info/WHEEL
+Filename: xc3_model_py-0.5.0.dist-info/WHEEL
+Comment: 
+
+Filename: xc3_model_py/animation.pyi
+Comment: 
+
+Filename: xc3_model_py/skinning.pyi
 Comment: 
 
 Filename: xc3_model_py/__init__.py
 Comment: 
 
+Filename: xc3_model_py/vertex.pyi
+Comment: 
+
 Filename: xc3_model_py/__init__.pyi
 Comment: 
 
-Filename: xc3_model_py/xc3_model_py.cp39-win_amd64.pyd
+Filename: xc3_model_py/xc3_model_py.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: xc3_model_py-0.4.0.dist-info/RECORD
+Filename: xc3_model_py-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xc3_model_py/__init__.pyi

```diff
@@ -1,299 +1,306 @@
-from typing import Optional, ClassVar, Tuple
-import numpy
-
-
-def load_model(wimdo_path: str, database_path: Optional[str]) -> ModelRoot: ...
-
-
-def load_map(wismhd: str, database_path: Optional[str]) -> list[ModelRoot]: ...
-
-
-def load_animations(anim_path: str) -> list[Animation]: ...
-
-
-def murmur3(name: str) -> int: ...
-
-
-class Xc3ModelError(Exception):
-    pass
-
-
-class ModelRoot:
-    groups: list[ModelGroup]
-    image_textures: list[ImageTexture]
-    skeleton: Optional[Skeleton]
-
-
-class ModelGroup:
-    models: list[Models]
-    buffers: list[ModelBuffers]
-
-
-class ModelBuffers:
-    vertex_buffers: list[VertexBuffer]
-    index_buffers: list[IndexBuffer]
-    weights: Optional[Weights]
-
-
-class Weights:
-    skin_weights: SkinWeights
-
-    def weights_start_index(self, skin_flags: int,
-                            lod: int, unk_type: RenderPassType) -> int: ...
-
-
-class SkinWeights:
-    bone_indices: numpy.ndarray
-    weights: numpy.ndarray
-    bone_names: list[str]
-
-
-class Models:
-    models: list[Model]
-    materials: list[Material]
-    samplers: list[Sampler]
-    base_lod_indices: Optional[list[int]]
-
-
-class Model:
-    meshes: list[Mesh]
-    instances: numpy.ndarray
-    model_buffers_index: int
-
-
-class Mesh:
-    vertex_buffer_index: int
-    index_buffer_index: int
-    material_index: int
-    lod: int
-    skin_flags: int
-
-
-class Skeleton:
-    bones: list[Bone]
-
-
-class Bone:
-    name: str
-    transform: numpy.ndarray
-    parent_index: Optional[int]
-
-
-class Material:
-    name: str
-    textures: list[Texture]
-    alpha_test: Optional[TextureAlphaTest]
-    shader: Optional[Shader]
-    pass_type: RenderPassType
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
-
-class MaterialParameters:
-    mat_color: list[float]
-    alpha_test_ref: float
-    tex_matrix: Optional[list[float]]
-    work_float4: Optional[list[float]]
-    work_color: Optional[list[float]]
-
-
-class Shader:
-    pass
-
-
-class Texture:
-    image_texture_index: int
-
-
-class VertexBuffer:
-    attributes: list[AttributeData]
-    influences: list[Influence]
-
-
-class AttributeData:
-    attribute_type: AttributeType
-    data: numpy.ndarray
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
-    position_deltas: numpy.ndarray
-    normal_deltas: numpy.ndarray
-    tangent_deltas: numpy.ndarray
-
-
-class Influence:
-    bone_name: str
-    weights: list[SkinWeight]
-
-
-class SkinWeight:
-    vertex_index: int
-    weight: float
-
-
-class IndexBuffer:
-    indices: numpy.ndarray
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
-
-class TextureUsage:
-    pass
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
-    mipmaps: bool
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
-    texcoord_scale: Optional[Tuple[float, float]]
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
-
-class Track:
-    def sample_translation(
-        self, frame: float) -> Tuple[float, float, float]: ...
-
-    def sample_rotation(self, frame: float) -> Tuple[float, float, float]: ...
-
-    def sample_scale(self, frame: float) -> Tuple[float, float, float]: ...
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

